# Comparing `tmp/powerbot_client-2.8.0.tar.gz` & `tmp/powerbot_client-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerbot_client-2.8.0.tar", last modified: Fri Sep  9 11:38:29 2022, max compression
+gzip compressed data, was "powerbot_client-2.9.1.tar", last modified: Tue Dec 20 10:44:50 2022, max compression
```

## Comparing `powerbot_client-2.8.0.tar` & `powerbot_client-2.9.1.tar`

### file list

```diff
@@ -1,142 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:38:29.937506 powerbot_client-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-09-09 11:38:29.937506 powerbot_client-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:38:29.921506 powerbot_client-2.8.0/powerbot_client/
--rwxr-xr-x   0 runner    (1001) docker     (121)    13480 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:38:29.925506 powerbot_client-2.8.0/powerbot_client/api/
--rwxr-xr-x   0 runner    (1001) docker     (121)      948 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    86133 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/algorithms_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    46420 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/authentication_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15372 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/capacities_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   100930 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/contract_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    32533 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/logs_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    72460 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/market_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15497 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/messages_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    69468 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/orders_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    48713 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/portfolios_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    32497 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/report_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17925 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/settings_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    34496 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/signals_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11735 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/subscriptions_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    48709 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/tenants_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    49663 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api/trades_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    32616 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/api_client.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    21995 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10013 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:38:29.937506 powerbot_client-2.8.0/powerbot_client/models/
--rwxr-xr-x   0 runner    (1001) docker     (121)    12119 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8064 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/aggressor_indicator.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9025 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_command.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14442 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_details.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15725 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_event.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9456 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_heartbeat.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16688 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_instance.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8115 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_instance_change.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11362 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_instance_event.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12345 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_instance_parameters.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14481 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8074 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/algo_status.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9183 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/api_key.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17917 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/api_key_details.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10431 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/api_key_portfolio_update.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8242 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/api_key_type.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10508 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/atc_status.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16187 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/audit_log_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13745 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/available_portfolio.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8745 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/bulk_contract_statistics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15591 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/bulk_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10896 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/bulk_signal_response.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16574 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/capacity.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10133 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/capacity_changes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11798 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/cash_limit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9569 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/changed_credentials.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    36447 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/contract.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15184 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/contract_changed_event.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    24454 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/contract_history_item.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17137 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/contract_item.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11354 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/contract_reference.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12033 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/contract_statistics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8058 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/contract_type.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9605 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/credentials.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16083 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/delivery_area.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10716 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/delivery_area_state.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8819 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/error_response.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8201 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/exchange.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10758 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/exchange_cash_limit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8102 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/execution_instruction.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10420 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/initialization.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8090 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/instance_heartbeat_status.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    28067 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/internal_trade.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10421 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/ip_allowlist_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11311 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/limit_violation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13506 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/log_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10124 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/log_entry_added.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8976 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/market_mode.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18741 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/market_options.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8117 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/market_state.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    29678 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/market_status.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10396 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/market_status_changed_event.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15719 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/message.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16171 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/new_api_key.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    21139 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/new_internal_trade.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12737 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/new_portfolio.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10874 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/new_tenant.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12972 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/notification.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8112 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/on_missing_heartbeat.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8543 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_action.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13120 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_book.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18578 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_book_changed_event.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19025 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_book_changes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14593 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_book_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15447 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_books.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    36762 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8149 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_execution_restriction.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    26866 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_modify.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10926 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_modify_item.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8028 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_side.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8083 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_state.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8118 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/order_type.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13053 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/orders.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10972 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/otr_limit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    30144 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/own_order.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13122 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/own_order_changed_event.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10112 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/own_order_changes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10975 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/own_trade_changes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12470 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/portfolio.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16632 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/portfolio_changes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    32777 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/portfolio_information.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8074 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/portfolio_type.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14465 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/position_limit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11643 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/product_information.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16609 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/public_trade.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10169 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/public_trade_changes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12187 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/report.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    24580 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/report_element.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11875 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/risk_management_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11322 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/risk_settings_and_portfolio_information.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8084 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/severity.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18452 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/signal.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10849 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/signal_changes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11661 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/subscription_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9750 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/tenant.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8104 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/text_matching_mode.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    40088 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/trade.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16340 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/trade_changed_event.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8179 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/trade_state.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9796 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/trading_area.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12777 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/update_algo_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11593 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/update_status.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8652 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/updated_api_key.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8779 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/updated_portfolio.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8749 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/updated_tenant.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8086 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/models/validity_restriction.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17545 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/powerbot_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:38:29.921506 powerbot_client-2.8.0/powerbot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-09-09 11:38:29.000000 powerbot_client-2.8.0/powerbot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-09-09 11:38:29.000000 powerbot_client-2.8.0/powerbot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 11:38:29.000000 powerbot_client-2.8.0/powerbot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-09 11:38:29.000000 powerbot_client-2.8.0/powerbot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-09 11:38:29.000000 powerbot_client-2.8.0/powerbot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 11:38:29.000000 powerbot_client-2.8.0/powerbot_client.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-09 11:38:29.937506 powerbot_client-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-09 11:38:18.000000 powerbot_client-2.8.0/setup_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:44:50.639509 powerbot_client-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2022-12-20 10:44:50.639509 powerbot_client-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:44:50.623509 powerbot_client-2.9.1/powerbot_client/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13743 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:44:50.627509 powerbot_client-2.9.1/powerbot_client/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    89175 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/algorithms_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46454 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/authentication_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15773 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/capacities_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   104450 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/contract_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32533 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/logs_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    73463 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/market_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15497 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/messages_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70905 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/orders_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48713 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/portfolios_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32497 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/report_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26651 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/schema_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17925 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/settings_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46692 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/signals_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11735 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/subscriptions_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48709 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/tenants_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49663 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api/trades_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32680 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/api_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21989 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10013 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:44:50.639509 powerbot_client-2.9.1/powerbot_client/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12329 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8064 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/aggressor_indicator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9025 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16789 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_details.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15725 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9456 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_heartbeat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17479 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_instance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8115 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_instance_change.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11362 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_instance_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12345 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_instance_parameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16812 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8074 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/algo_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9183 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/api_key.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17890 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/api_key_details.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10431 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/api_key_portfolio_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8311 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/api_key_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10508 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/atc_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16187 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/audit_log_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8766 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/bulk_contract_statistics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16818 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/bulk_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10896 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/bulk_signal_response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16574 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/capacity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10133 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/capacity_changes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11798 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/cash_limit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9569 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/changed_credentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36425 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/contract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15184 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/contract_changed_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24396 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/contract_history_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17137 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/contract_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11354 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/contract_reference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12033 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/contract_statistics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8058 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/contract_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9605 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/credentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16083 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/delivery_area.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10716 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/delivery_area_state.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8819 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/error_response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8201 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/exchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10758 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/exchange_cash_limit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8102 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/execution_instruction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10420 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/initialization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8090 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/instance_heartbeat_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28067 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/internal_trade.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10421 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/ip_allowlist_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11311 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/limit_violation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13506 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/log_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10124 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/log_entry_added.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8976 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/market_mode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21236 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/market_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8117 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/market_state.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29940 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/market_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10396 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/market_status_changed_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15719 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/message.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16171 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/new_api_key.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21139 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/new_internal_trade.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12737 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/new_portfolio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10874 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/new_tenant.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12972 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/notification.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8112 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/on_missing_heartbeat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8567 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13120 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_book.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18578 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_book_changed_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19025 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_book_changes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14593 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_book_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12253 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_book_group.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15447 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_books.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36762 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8149 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_execution_restriction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26866 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_modify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10926 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_modify_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8028 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_side.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8083 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_state.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8118 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/order_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13764 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10972 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/otr_limit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30899 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/own_order.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13122 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/own_order_changed_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10112 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/own_order_changes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10975 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/own_trade_changes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13328 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/portfolio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16632 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/portfolio_changes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33039 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/portfolio_information.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8074 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/portfolio_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14465 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/position_limit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11643 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/product_information.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16609 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/public_trade.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10169 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/public_trade_changes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26627 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/related_contract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12187 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/report.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24580 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/report_element.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11875 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/risk_management_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11322 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/risk_settings_and_portfolio_information.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8084 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/severity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19277 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/signal_changes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11661 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/subscription_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9750 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/tenant.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/text_matching_mode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40088 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/trade.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16340 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/trade_changed_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8179 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/trade_state.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9796 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/trading_area.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15156 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/update_algo_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11593 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/update_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8652 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/updated_api_key.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8779 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/updated_portfolio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8749 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/updated_tenant.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14297 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/validation_schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8081 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/validation_schema_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8086 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/models/validity_restriction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17545 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/powerbot_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:44:50.623509 powerbot_client-2.9.1/powerbot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2022-12-20 10:44:50.000000 powerbot_client-2.9.1/powerbot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2022-12-20 10:44:50.000000 powerbot_client-2.9.1/powerbot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 10:44:50.000000 powerbot_client-2.9.1/powerbot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-20 10:44:50.000000 powerbot_client-2.9.1/powerbot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-20 10:44:50.000000 powerbot_client-2.9.1/powerbot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 10:44:50.000000 powerbot_client-2.9.1/powerbot_client.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 10:44:50.639509 powerbot_client-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2022-12-20 10:44:34.000000 powerbot_client-2.9.1/setup_sync.py
```

### Comparing `powerbot_client-2.8.0/README.md` & `powerbot_client-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `powerbot_client-2.8.0/powerbot_client/__init__.py` & `powerbot_client-2.9.1/powerbot_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 # flake8: noqa
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.8.0"
+__version__ = "2.9.1"
 
 # import apis into sdk package
 from powerbot_client.api.algorithms_api import AlgorithmsApi
 from powerbot_client.api.authentication_api import AuthenticationApi
 from powerbot_client.api.capacities_api import CapacitiesApi
 from powerbot_client.api.contract_api import ContractApi
 from powerbot_client.api.logs_api import LogsApi
 from powerbot_client.api.market_api import MarketApi
 from powerbot_client.api.messages_api import MessagesApi
 from powerbot_client.api.orders_api import OrdersApi
 from powerbot_client.api.portfolios_api import PortfoliosApi
 from powerbot_client.api.report_api import ReportApi
+from powerbot_client.api.schema_api import SchemaApi
 from powerbot_client.api.settings_api import SettingsApi
 from powerbot_client.api.signals_api import SignalsApi
 from powerbot_client.api.subscriptions_api import SubscriptionsApi
 from powerbot_client.api.tenants_api import TenantsApi
 from powerbot_client.api.trades_api import TradesApi
 
 # import ApiClient
@@ -57,15 +58,14 @@
 from powerbot_client.models.algo_status import AlgoStatus
 from powerbot_client.models.api_key import ApiKey
 from powerbot_client.models.api_key_details import ApiKeyDetails
 from powerbot_client.models.api_key_portfolio_update import ApiKeyPortfolioUpdate
 from powerbot_client.models.api_key_type import ApiKeyType
 from powerbot_client.models.atc_status import AtcStatus
 from powerbot_client.models.audit_log_entry import AuditLogEntry
-from powerbot_client.models.available_portfolio import AvailablePortfolio
 from powerbot_client.models.bulk_contract_statistics import BulkContractStatistics
 from powerbot_client.models.bulk_signal import BulkSignal
 from powerbot_client.models.bulk_signal_response import BulkSignalResponse
 from powerbot_client.models.capacity import Capacity
 from powerbot_client.models.capacity_changes import CapacityChanges
 from powerbot_client.models.cash_limit import CashLimit
 from powerbot_client.models.changed_credentials import ChangedCredentials
@@ -103,14 +103,15 @@
 from powerbot_client.models.notification import Notification
 from powerbot_client.models.on_missing_heartbeat import OnMissingHeartbeat
 from powerbot_client.models.order_action import OrderAction
 from powerbot_client.models.order_book import OrderBook
 from powerbot_client.models.order_book_changed_event import OrderBookChangedEvent
 from powerbot_client.models.order_book_changes import OrderBookChanges
 from powerbot_client.models.order_book_entry import OrderBookEntry
+from powerbot_client.models.order_book_group import OrderBookGroup
 from powerbot_client.models.order_books import OrderBooks
 from powerbot_client.models.order_entry import OrderEntry
 from powerbot_client.models.order_execution_restriction import OrderExecutionRestriction
 from powerbot_client.models.order_modify import OrderModify
 from powerbot_client.models.order_modify_item import OrderModifyItem
 from powerbot_client.models.order_side import OrderSide
 from powerbot_client.models.order_state import OrderState
@@ -125,14 +126,15 @@
 from powerbot_client.models.portfolio_changes import PortfolioChanges
 from powerbot_client.models.portfolio_information import PortfolioInformation
 from powerbot_client.models.portfolio_type import PortfolioType
 from powerbot_client.models.position_limit import PositionLimit
 from powerbot_client.models.product_information import ProductInformation
 from powerbot_client.models.public_trade import PublicTrade
 from powerbot_client.models.public_trade_changes import PublicTradeChanges
+from powerbot_client.models.related_contract import RelatedContract
 from powerbot_client.models.report import Report
 from powerbot_client.models.report_element import ReportElement
 from powerbot_client.models.risk_management_settings import RiskManagementSettings
 from powerbot_client.models.risk_settings_and_portfolio_information import RiskSettingsAndPortfolioInformation
 from powerbot_client.models.severity import Severity
 from powerbot_client.models.signal import Signal
 from powerbot_client.models.signal_changes import SignalChanges
@@ -144,9 +146,11 @@
 from powerbot_client.models.trade_state import TradeState
 from powerbot_client.models.trading_area import TradingArea
 from powerbot_client.models.update_algo_setup import UpdateAlgoSetup
 from powerbot_client.models.update_status import UpdateStatus
 from powerbot_client.models.updated_api_key import UpdatedApiKey
 from powerbot_client.models.updated_portfolio import UpdatedPortfolio
 from powerbot_client.models.updated_tenant import UpdatedTenant
+from powerbot_client.models.validation_schema import ValidationSchema
+from powerbot_client.models.validation_schema_type import ValidationSchemaType
 from powerbot_client.models.validity_restriction import ValidityRestriction
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/__init__.py` & `powerbot_client-2.9.1/powerbot_client/api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 from powerbot_client.api.contract_api import ContractApi
 from powerbot_client.api.logs_api import LogsApi
 from powerbot_client.api.market_api import MarketApi
 from powerbot_client.api.messages_api import MessagesApi
 from powerbot_client.api.orders_api import OrdersApi
 from powerbot_client.api.portfolios_api import PortfoliosApi
 from powerbot_client.api.report_api import ReportApi
+from powerbot_client.api.schema_api import SchemaApi
 from powerbot_client.api.settings_api import SettingsApi
 from powerbot_client.api.signals_api import SignalsApi
 from powerbot_client.api.subscriptions_api import SubscriptionsApi
 from powerbot_client.api.tenants_api import TenantsApi
 from powerbot_client.api.trades_api import TradesApi
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/algorithms_api.py` & `powerbot_client-2.9.1/powerbot_client/api/algorithms_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -1020,26 +1020,28 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def new_instance(self, algorithm_id, start_parameters, **kwargs):  # noqa: E501
+    def new_instance(self, algorithm_id, bypass_validation, start_parameters, **kwargs):  # noqa: E501
         """Add algorithm instance  # noqa: E501
 
         An instance is used to run an algorithm and pass parameters to it. Only the master-API-key and tenant-master-API-keys are allowed to create algorithm-instances. An instance is always bound to a tenant and a list of portfolios.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.new_instance(algorithm_id, start_parameters, async_req=True)
+        >>> thread = api.new_instance(algorithm_id, bypass_validation, start_parameters, async_req=True)
         >>> result = thread.get()
 
         :param algorithm_id: (required)
         :type algorithm_id: str
+        :param bypass_validation: When set to true, the specified parameters will not be validated against the json schema of the algorithm. (required)
+        :type bypass_validation: bool
         :param start_parameters: (required)
         :type start_parameters: AlgoInstanceParameters
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1050,28 +1052,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: AlgoInstance
         """
         kwargs['_return_http_data_only'] = True
-        return self.new_instance_with_http_info(algorithm_id, start_parameters, **kwargs)  # noqa: E501
+        return self.new_instance_with_http_info(algorithm_id, bypass_validation, start_parameters, **kwargs)  # noqa: E501
 
-    def new_instance_with_http_info(self, algorithm_id, start_parameters, **kwargs):  # noqa: E501
+    def new_instance_with_http_info(self, algorithm_id, bypass_validation, start_parameters, **kwargs):  # noqa: E501
         """Add algorithm instance  # noqa: E501
 
         An instance is used to run an algorithm and pass parameters to it. Only the master-API-key and tenant-master-API-keys are allowed to create algorithm-instances. An instance is always bound to a tenant and a list of portfolios.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.new_instance_with_http_info(algorithm_id, start_parameters, async_req=True)
+        >>> thread = api.new_instance_with_http_info(algorithm_id, bypass_validation, start_parameters, async_req=True)
         >>> result = thread.get()
 
         :param algorithm_id: (required)
         :type algorithm_id: str
+        :param bypass_validation: When set to true, the specified parameters will not be validated against the json schema of the algorithm. (required)
+        :type bypass_validation: bool
         :param start_parameters: (required)
         :type start_parameters: AlgoInstanceParameters
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1094,14 +1098,15 @@
         :rtype: tuple(AlgoInstance, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'algorithm_id',
+            'bypass_validation',
             'start_parameters'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1119,25 +1124,30 @@
                     " to method new_instance" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'algorithm_id' is set
         if self.api_client.client_side_validation and local_var_params.get('algorithm_id') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `algorithm_id` when calling `new_instance`")  # noqa: E501
+        # verify the required parameter 'bypass_validation' is set
+        if self.api_client.client_side_validation and local_var_params.get('bypass_validation') is None:  # noqa: E501
+            raise ApiValueError("Missing the required parameter `bypass_validation` when calling `new_instance`")  # noqa: E501
         # verify the required parameter 'start_parameters' is set
         if self.api_client.client_side_validation and local_var_params.get('start_parameters') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `start_parameters` when calling `new_instance`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'algorithm_id' in local_var_params:
             path_params['algorithm_id'] = local_var_params['algorithm_id']  # noqa: E501
 
         query_params = []
+        if local_var_params.get('bypass_validation') is not None:  # noqa: E501
+            query_params.append(('bypass_validation', local_var_params['bypass_validation']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1175,28 +1185,30 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def submit_command(self, algorithm_id, instance_id, command, **kwargs):  # noqa: E501
+    def submit_command(self, algorithm_id, instance_id, bypass_validation, command, **kwargs):  # noqa: E501
         """Start/Stop algorithm instance  # noqa: E501
 
         This request controls the algorithm instance. Use standard-API-keys to start/stop algorithm instances. The key needs access to ALL portfolios specified in the instance. Master-API-keys and tenant-master-API-keys can also start/stop algorithm instances, however this should only be used in exceptional cases.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.submit_command(algorithm_id, instance_id, command, async_req=True)
+        >>> thread = api.submit_command(algorithm_id, instance_id, bypass_validation, command, async_req=True)
         >>> result = thread.get()
 
         :param algorithm_id: (required)
         :type algorithm_id: str
         :param instance_id: (required)
         :type instance_id: str
+        :param bypass_validation: When set to true, the specified parameters will not be validated against the json schema of the algorithm. (required)
+        :type bypass_validation: bool
         :param command: (required)
         :type command: AlgoCommand
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1207,30 +1219,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: AlgoInstance
         """
         kwargs['_return_http_data_only'] = True
-        return self.submit_command_with_http_info(algorithm_id, instance_id, command, **kwargs)  # noqa: E501
+        return self.submit_command_with_http_info(algorithm_id, instance_id, bypass_validation, command, **kwargs)  # noqa: E501
 
-    def submit_command_with_http_info(self, algorithm_id, instance_id, command, **kwargs):  # noqa: E501
+    def submit_command_with_http_info(self, algorithm_id, instance_id, bypass_validation, command, **kwargs):  # noqa: E501
         """Start/Stop algorithm instance  # noqa: E501
 
         This request controls the algorithm instance. Use standard-API-keys to start/stop algorithm instances. The key needs access to ALL portfolios specified in the instance. Master-API-keys and tenant-master-API-keys can also start/stop algorithm instances, however this should only be used in exceptional cases.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.submit_command_with_http_info(algorithm_id, instance_id, command, async_req=True)
+        >>> thread = api.submit_command_with_http_info(algorithm_id, instance_id, bypass_validation, command, async_req=True)
         >>> result = thread.get()
 
         :param algorithm_id: (required)
         :type algorithm_id: str
         :param instance_id: (required)
         :type instance_id: str
+        :param bypass_validation: When set to true, the specified parameters will not be validated against the json schema of the algorithm. (required)
+        :type bypass_validation: bool
         :param command: (required)
         :type command: AlgoCommand
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1254,14 +1268,15 @@
         """
 
         local_var_params = locals()
 
         all_params = [
             'algorithm_id',
             'instance_id',
+            'bypass_validation',
             'command'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1282,27 +1297,32 @@
         del local_var_params['kwargs']
         # verify the required parameter 'algorithm_id' is set
         if self.api_client.client_side_validation and local_var_params.get('algorithm_id') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `algorithm_id` when calling `submit_command`")  # noqa: E501
         # verify the required parameter 'instance_id' is set
         if self.api_client.client_side_validation and local_var_params.get('instance_id') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `instance_id` when calling `submit_command`")  # noqa: E501
+        # verify the required parameter 'bypass_validation' is set
+        if self.api_client.client_side_validation and local_var_params.get('bypass_validation') is None:  # noqa: E501
+            raise ApiValueError("Missing the required parameter `bypass_validation` when calling `submit_command`")  # noqa: E501
         # verify the required parameter 'command' is set
         if self.api_client.client_side_validation and local_var_params.get('command') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `command` when calling `submit_command`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'algorithm_id' in local_var_params:
             path_params['algorithm_id'] = local_var_params['algorithm_id']  # noqa: E501
         if 'instance_id' in local_var_params:
             path_params['instance_id'] = local_var_params['instance_id']  # noqa: E501
 
         query_params = []
+        if local_var_params.get('bypass_validation') is not None:  # noqa: E501
+            query_params.append(('bypass_validation', local_var_params['bypass_validation']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1503,28 +1523,30 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def update_algo_parameters(self, algorithm_id, instance_id, parameters, **kwargs):  # noqa: E501
+    def update_algo_parameters(self, algorithm_id, instance_id, bypass_validation, parameters, **kwargs):  # noqa: E501
         """Update algorithm instance  # noqa: E501
 
         Note that parameter changes will only be accepted if the algorithm is in \"IDLE\" state. - Master-API-keys can update all instances. - Tenant-Master-API-keys can only update instances where the key has access to ALL portfolios specified in the instance. - Standard-API-keys can only update instances where the key has access to ALL portfolios specified in the instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_algo_parameters(algorithm_id, instance_id, parameters, async_req=True)
+        >>> thread = api.update_algo_parameters(algorithm_id, instance_id, bypass_validation, parameters, async_req=True)
         >>> result = thread.get()
 
         :param algorithm_id: (required)
         :type algorithm_id: str
         :param instance_id: (required)
         :type instance_id: str
+        :param bypass_validation: When set to true, the specified parameters will not be validated against the json schema of the algorithm. (required)
+        :type bypass_validation: bool
         :param parameters: (required)
         :type parameters: object
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1535,30 +1557,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: AlgoInstance
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_algo_parameters_with_http_info(algorithm_id, instance_id, parameters, **kwargs)  # noqa: E501
+        return self.update_algo_parameters_with_http_info(algorithm_id, instance_id, bypass_validation, parameters, **kwargs)  # noqa: E501
 
-    def update_algo_parameters_with_http_info(self, algorithm_id, instance_id, parameters, **kwargs):  # noqa: E501
+    def update_algo_parameters_with_http_info(self, algorithm_id, instance_id, bypass_validation, parameters, **kwargs):  # noqa: E501
         """Update algorithm instance  # noqa: E501
 
         Note that parameter changes will only be accepted if the algorithm is in \"IDLE\" state. - Master-API-keys can update all instances. - Tenant-Master-API-keys can only update instances where the key has access to ALL portfolios specified in the instance. - Standard-API-keys can only update instances where the key has access to ALL portfolios specified in the instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_algo_parameters_with_http_info(algorithm_id, instance_id, parameters, async_req=True)
+        >>> thread = api.update_algo_parameters_with_http_info(algorithm_id, instance_id, bypass_validation, parameters, async_req=True)
         >>> result = thread.get()
 
         :param algorithm_id: (required)
         :type algorithm_id: str
         :param instance_id: (required)
         :type instance_id: str
+        :param bypass_validation: When set to true, the specified parameters will not be validated against the json schema of the algorithm. (required)
+        :type bypass_validation: bool
         :param parameters: (required)
         :type parameters: object
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1582,14 +1606,15 @@
         """
 
         local_var_params = locals()
 
         all_params = [
             'algorithm_id',
             'instance_id',
+            'bypass_validation',
             'parameters'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1610,27 +1635,32 @@
         del local_var_params['kwargs']
         # verify the required parameter 'algorithm_id' is set
         if self.api_client.client_side_validation and local_var_params.get('algorithm_id') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `algorithm_id` when calling `update_algo_parameters`")  # noqa: E501
         # verify the required parameter 'instance_id' is set
         if self.api_client.client_side_validation and local_var_params.get('instance_id') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `instance_id` when calling `update_algo_parameters`")  # noqa: E501
+        # verify the required parameter 'bypass_validation' is set
+        if self.api_client.client_side_validation and local_var_params.get('bypass_validation') is None:  # noqa: E501
+            raise ApiValueError("Missing the required parameter `bypass_validation` when calling `update_algo_parameters`")  # noqa: E501
         # verify the required parameter 'parameters' is set
         if self.api_client.client_side_validation and local_var_params.get('parameters') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `parameters` when calling `update_algo_parameters`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'algorithm_id' in local_var_params:
             path_params['algorithm_id'] = local_var_params['algorithm_id']  # noqa: E501
         if 'instance_id' in local_var_params:
             path_params['instance_id'] = local_var_params['instance_id']  # noqa: E501
 
         query_params = []
+        if local_var_params.get('bypass_validation') is not None:  # noqa: E501
+            query_params.append(('bypass_validation', local_var_params['bypass_validation']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/authentication_api.py` & `powerbot_client-2.9.1/powerbot_client/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -166,14 +166,15 @@
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
         auth_settings = ['api_key_security']  # noqa: E501
 
         response_types_map = {
             200: "ApiKey",
+            409: "ErrorResponse",
         }
 
         return self.api_client.call_api(
             '/api-keys', 'POST',
             path_params,
             query_params,
             header_params,
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/capacities_api.py` & `powerbot_client-2.9.1/powerbot_client/api/capacities_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -149,14 +149,17 @@
         # verify the required parameter 'delivery_from' is set
         if self.api_client.client_side_validation and local_var_params.get('delivery_from') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `delivery_from` when calling `get_capacities`")  # noqa: E501
         # verify the required parameter 'delivery_to' is set
         if self.api_client.client_side_validation and local_var_params.get('delivery_to') is None:  # noqa: E501
             raise ApiValueError("Missing the required parameter `delivery_to` when calling `get_capacities`")  # noqa: E501
 
+        if self.api_client.client_side_validation and ('delivery_area' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['delivery_area']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `delivery_area` when calling `get_capacities`, number of items must be greater than or equal to `1`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if local_var_params.get('delivery_area') is not None:  # noqa: E501
             query_params.append(('delivery_area', local_var_params['delivery_area']))  # noqa: E501
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/contract_api.py` & `powerbot_client-2.9.1/powerbot_client/api/contract_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -36,15 +36,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def calculate_bulk_statistics(self, contract_duration_minutes, delivery_area, delivery_from, delivery_to, **kwargs):  # noqa: E501
         """Get contract statistics in bulk  # noqa: E501
 
-        Calculates the average price and volume of public trades executed for a given delivery interval for reference price and index calculation. Allows you to filter for public trades executed within a certain time period and to restrict the calculation to a given amount of last traded quantity. Please note that this functionality is only available for active or recently active contracts, that cross border trades are taken into account if either the buy or sell leg of the trade is in the specified delivery area(s) and that the quantity of a trade is only counted once.  # noqa: E501
+        Calculates the average price and volume of public trades executed for a given delivery interval for reference price and index calculation. Allows you to filter for public trades executed within a certain time period to restrict the calculation to a given amount of last traded quantity. Per default, only active or recently active contracts with be included in the calculation. Historic contracts matching the given delivery period can be included with setting the respective toggle. Please note that delivery_start and delivery_end have to be within 24 hours. Cross border trades are taken into account if either the buy or sell leg of the trade is in the specified delivery area(s). The quantity of only one of those trades will be taken into account, if a trades matches.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.calculate_bulk_statistics(contract_duration_minutes, delivery_area, delivery_from, delivery_to, async_req=True)
         >>> result = thread.get()
 
         :param contract_duration_minutes: the duration of the contracts to calculate statistics for (required)
@@ -57,14 +57,16 @@
         :type delivery_to: datetime
         :param execution_from_offset_minutes: only consider trades that happened after or at (delivery start - n minutes)
         :type execution_from_offset_minutes: int
         :param execution_to_offset_minutes: only consider trades that happened before (delivery start - n minutes)
         :type execution_to_offset_minutes: int
         :param limit_to_last_mw:
         :type limit_to_last_mw: float
+        :param include_historic_data: If this option is enabled, statistics will also be calculated for expired contracts that match the given delivery period.
+        :type include_historic_data: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -78,15 +80,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.calculate_bulk_statistics_with_http_info(contract_duration_minutes, delivery_area, delivery_from, delivery_to, **kwargs)  # noqa: E501
 
     def calculate_bulk_statistics_with_http_info(self, contract_duration_minutes, delivery_area, delivery_from, delivery_to, **kwargs):  # noqa: E501
         """Get contract statistics in bulk  # noqa: E501
 
-        Calculates the average price and volume of public trades executed for a given delivery interval for reference price and index calculation. Allows you to filter for public trades executed within a certain time period and to restrict the calculation to a given amount of last traded quantity. Please note that this functionality is only available for active or recently active contracts, that cross border trades are taken into account if either the buy or sell leg of the trade is in the specified delivery area(s) and that the quantity of a trade is only counted once.  # noqa: E501
+        Calculates the average price and volume of public trades executed for a given delivery interval for reference price and index calculation. Allows you to filter for public trades executed within a certain time period to restrict the calculation to a given amount of last traded quantity. Per default, only active or recently active contracts with be included in the calculation. Historic contracts matching the given delivery period can be included with setting the respective toggle. Please note that delivery_start and delivery_end have to be within 24 hours. Cross border trades are taken into account if either the buy or sell leg of the trade is in the specified delivery area(s). The quantity of only one of those trades will be taken into account, if a trades matches.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.calculate_bulk_statistics_with_http_info(contract_duration_minutes, delivery_area, delivery_from, delivery_to, async_req=True)
         >>> result = thread.get()
 
         :param contract_duration_minutes: the duration of the contracts to calculate statistics for (required)
@@ -99,14 +101,16 @@
         :type delivery_to: datetime
         :param execution_from_offset_minutes: only consider trades that happened after or at (delivery start - n minutes)
         :type execution_from_offset_minutes: int
         :param execution_to_offset_minutes: only consider trades that happened before (delivery start - n minutes)
         :type execution_to_offset_minutes: int
         :param limit_to_last_mw:
         :type limit_to_last_mw: float
+        :param include_historic_data: If this option is enabled, statistics will also be calculated for expired contracts that match the given delivery period.
+        :type include_historic_data: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -132,15 +136,16 @@
         all_params = [
             'contract_duration_minutes',
             'delivery_area',
             'delivery_from',
             'delivery_to',
             'execution_from_offset_minutes',
             'execution_to_offset_minutes',
-            'limit_to_last_mw'
+            'limit_to_last_mw',
+            'include_historic_data'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -191,14 +196,16 @@
             query_params.append(('delivery_to', local_var_params['delivery_to']))  # noqa: E501
         if local_var_params.get('execution_from_offset_minutes') is not None:  # noqa: E501
             query_params.append(('execution_from_offset_minutes', local_var_params['execution_from_offset_minutes']))  # noqa: E501
         if local_var_params.get('execution_to_offset_minutes') is not None:  # noqa: E501
             query_params.append(('execution_to_offset_minutes', local_var_params['execution_to_offset_minutes']))  # noqa: E501
         if local_var_params.get('limit_to_last_mw') is not None:  # noqa: E501
             query_params.append(('limit_to_last_mw', local_var_params['limit_to_last_mw']))  # noqa: E501
+        if local_var_params.get('include_historic_data') is not None:  # noqa: E501
+            query_params.append(('includeHistoricData', local_var_params['include_historic_data']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -229,15 +236,15 @@
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def calculate_statistics(self, delivery_area, delivery_start, delivery_end, **kwargs):  # noqa: E501
         """Get contract statistics  # noqa: E501
 
-        Calculates the average price and volume of public trades executed for a given delivery interval for reference price and index calculation. Allows you to filter for public trades executed within a certain time period and to restrict the calculation to a given amount of last traded quantity. Please note that this functionality is only available for active or recently active contracts, that cross border trades are taken into account if either the buy or sell leg of the trade is in the specified delivery area(s) and that the quantity of a trade is only counted once.  # noqa: E501
+        Calculates the average price and volume of public trades executed for a given delivery interval for reference price and index calculation. Allows you to filter for public trades executed within a certain time period to restrict the calculation to a given amount of last traded quantity. Per default, only active or recently active contracts with be included in the calculation. Historic contracts matching the given delivery period can be included with setting the respective toggle. Please note that delivery_start and delivery_end have to be within 24 hours. Cross border trades are taken into account if either the buy or sell leg of the trade is in the specified delivery area(s). The quantity of only one of those trades will be taken into account, if a trades matches.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.calculate_statistics(delivery_area, delivery_start, delivery_end, async_req=True)
         >>> result = thread.get()
 
         :param delivery_area: (required)
@@ -248,14 +255,16 @@
         :type delivery_end: datetime
         :param execution_from:
         :type execution_from: datetime
         :param execution_to:
         :type execution_to: datetime
         :param limit_to_last_mw:
         :type limit_to_last_mw: float
+        :param include_historic_data: If this option is enabled, statistics will also be calculated for expired contracts that match the given delivery period.
+        :type include_historic_data: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -269,15 +278,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.calculate_statistics_with_http_info(delivery_area, delivery_start, delivery_end, **kwargs)  # noqa: E501
 
     def calculate_statistics_with_http_info(self, delivery_area, delivery_start, delivery_end, **kwargs):  # noqa: E501
         """Get contract statistics  # noqa: E501
 
-        Calculates the average price and volume of public trades executed for a given delivery interval for reference price and index calculation. Allows you to filter for public trades executed within a certain time period and to restrict the calculation to a given amount of last traded quantity. Please note that this functionality is only available for active or recently active contracts, that cross border trades are taken into account if either the buy or sell leg of the trade is in the specified delivery area(s) and that the quantity of a trade is only counted once.  # noqa: E501
+        Calculates the average price and volume of public trades executed for a given delivery interval for reference price and index calculation. Allows you to filter for public trades executed within a certain time period to restrict the calculation to a given amount of last traded quantity. Per default, only active or recently active contracts with be included in the calculation. Historic contracts matching the given delivery period can be included with setting the respective toggle. Please note that delivery_start and delivery_end have to be within 24 hours. Cross border trades are taken into account if either the buy or sell leg of the trade is in the specified delivery area(s). The quantity of only one of those trades will be taken into account, if a trades matches.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.calculate_statistics_with_http_info(delivery_area, delivery_start, delivery_end, async_req=True)
         >>> result = thread.get()
 
         :param delivery_area: (required)
@@ -288,14 +297,16 @@
         :type delivery_end: datetime
         :param execution_from:
         :type execution_from: datetime
         :param execution_to:
         :type execution_to: datetime
         :param limit_to_last_mw:
         :type limit_to_last_mw: float
+        :param include_historic_data: If this option is enabled, statistics will also be calculated for expired contracts that match the given delivery period.
+        :type include_historic_data: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -320,15 +331,16 @@
 
         all_params = [
             'delivery_area',
             'delivery_start',
             'delivery_end',
             'execution_from',
             'execution_to',
-            'limit_to_last_mw'
+            'limit_to_last_mw',
+            'include_historic_data'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -370,14 +382,16 @@
             query_params.append(('delivery_end', local_var_params['delivery_end']))  # noqa: E501
         if local_var_params.get('execution_from') is not None:  # noqa: E501
             query_params.append(('execution_from', local_var_params['execution_from']))  # noqa: E501
         if local_var_params.get('execution_to') is not None:  # noqa: E501
             query_params.append(('execution_to', local_var_params['execution_to']))  # noqa: E501
         if local_var_params.get('limit_to_last_mw') is not None:  # noqa: E501
             query_params.append(('limit_to_last_mw', local_var_params['limit_to_last_mw']))  # noqa: E501
+        if local_var_params.get('include_historic_data') is not None:  # noqa: E501
+            query_params.append(('includeHistoricData', local_var_params['include_historic_data']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -408,27 +422,31 @@
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def find_contracts(self, **kwargs):  # noqa: E501
         """Find contracts  # noqa: E501
 
-        This method allows you to find active or historical contracts based on their delivery_start and delivery_end time (UTC) and lets you determine their contract_id.  # noqa: E501
+        This method allows you to find active or historical contracts based on their exact delivery_start and delivery_end time (UTC) and lets you determine their contract_id. Using delivery_from and delivery_to, the contracts can be further limited to a given timespan.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.find_contracts(async_req=True)
         >>> result = thread.get()
 
         :param contract_id:
         :type contract_id: list[str]
-        :param delivery_start:
+        :param delivery_start: Limit the contracts to those with the given delivery start date.
         :type delivery_start: datetime
-        :param delivery_end:
+        :param delivery_end: Limit the contracts to those with the given delivery end date.
         :type delivery_end: datetime
+        :param delivery_from: Limits the contracts to those with a delivery start date >= delivery_from.
+        :type delivery_from: datetime
+        :param delivery_to: Limits the contracts to those with a delivery end date <= delivery_to.
+        :type delivery_to: datetime
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -442,27 +460,31 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.find_contracts_with_http_info(**kwargs)  # noqa: E501
 
     def find_contracts_with_http_info(self, **kwargs):  # noqa: E501
         """Find contracts  # noqa: E501
 
-        This method allows you to find active or historical contracts based on their delivery_start and delivery_end time (UTC) and lets you determine their contract_id.  # noqa: E501
+        This method allows you to find active or historical contracts based on their exact delivery_start and delivery_end time (UTC) and lets you determine their contract_id. Using delivery_from and delivery_to, the contracts can be further limited to a given timespan.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.find_contracts_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param contract_id:
         :type contract_id: list[str]
-        :param delivery_start:
+        :param delivery_start: Limit the contracts to those with the given delivery start date.
         :type delivery_start: datetime
-        :param delivery_end:
+        :param delivery_end: Limit the contracts to those with the given delivery end date.
         :type delivery_end: datetime
+        :param delivery_from: Limits the contracts to those with a delivery start date >= delivery_from.
+        :type delivery_from: datetime
+        :param delivery_to: Limits the contracts to those with a delivery end date <= delivery_to.
+        :type delivery_to: datetime
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -484,15 +506,17 @@
         """
 
         local_var_params = locals()
 
         all_params = [
             'contract_id',
             'delivery_start',
-            'delivery_end'
+            'delivery_end',
+            'delivery_from',
+            'delivery_to'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -519,14 +543,18 @@
         if local_var_params.get('contract_id') is not None:  # noqa: E501
             query_params.append(('contract_id', local_var_params['contract_id']))  # noqa: E501
             collection_formats['contract_id'] = 'csv'  # noqa: E501
         if local_var_params.get('delivery_start') is not None:  # noqa: E501
             query_params.append(('delivery_start', local_var_params['delivery_start']))  # noqa: E501
         if local_var_params.get('delivery_end') is not None:  # noqa: E501
             query_params.append(('delivery_end', local_var_params['delivery_end']))  # noqa: E501
+        if local_var_params.get('delivery_from') is not None:  # noqa: E501
+            query_params.append(('delivery_from', local_var_params['delivery_from']))  # noqa: E501
+        if local_var_params.get('delivery_to') is not None:  # noqa: E501
+            query_params.append(('delivery_to', local_var_params['delivery_to']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1115,15 +1143,15 @@
         :type delivery_within: datetime
         :param past_hours: The number of hours to look into the past in the orderbook. If this parameter is set, historic closed contracts are contained in the orderbook as well. Can't be used in conjunction with delivery_from.
         :type past_hours: int
         :param delivery_area: The EIC code of the delivery area of the orderbook
         :type delivery_area: str
         :param delivery_from: Limits the orderbook to those contracts with a delivery start date >= delivery_from. When used in conjunction with past_hours, has to be after the time defined by past_hours (delivery_from > now - past_hours).
         :type delivery_from: datetime
-        :param delivery_to: Limits the orderbook to those contracts with a delivery end date <= delivery_to
+        :param delivery_to: Limits the orderbook to those contracts with a delivery end date <= delivery_to.
         :type delivery_to: datetime
         :param with_order_details: If set to true, the returned orderbook will contain all current bids and asks of each contract (full orderbook depth). *Heads up* We generally recommend to request the full orderbook depth on a per contract basis when orderbook-changed notifications are received via websocket. If you need the full orderbook depth for all contracts at once more frequently, please consider using full orderbook snapshots via websocket.
         :type with_order_details: bool
         :param contract_type: **PDC**: (default) the order book only includes predefined contracts, i.e. the normal contracts generated by the backend  UDC: the order book only includes block products, which were created as the result of a block order submitted by a member  ALL: the order book contains both, PDC and UDC contracts
         :type contract_type: ContractType
         :param with_portfolio_information: If set to true, the portfolio_information is included in the response. Set to false to optimize caching.
         :type with_portfolio_information: bool
@@ -1181,15 +1209,15 @@
         :type delivery_within: datetime
         :param past_hours: The number of hours to look into the past in the orderbook. If this parameter is set, historic closed contracts are contained in the orderbook as well. Can't be used in conjunction with delivery_from.
         :type past_hours: int
         :param delivery_area: The EIC code of the delivery area of the orderbook
         :type delivery_area: str
         :param delivery_from: Limits the orderbook to those contracts with a delivery start date >= delivery_from. When used in conjunction with past_hours, has to be after the time defined by past_hours (delivery_from > now - past_hours).
         :type delivery_from: datetime
-        :param delivery_to: Limits the orderbook to those contracts with a delivery end date <= delivery_to
+        :param delivery_to: Limits the orderbook to those contracts with a delivery end date <= delivery_to.
         :type delivery_to: datetime
         :param with_order_details: If set to true, the returned orderbook will contain all current bids and asks of each contract (full orderbook depth). *Heads up* We generally recommend to request the full orderbook depth on a per contract basis when orderbook-changed notifications are received via websocket. If you need the full orderbook depth for all contracts at once more frequently, please consider using full orderbook snapshots via websocket.
         :type with_order_details: bool
         :param contract_type: **PDC**: (default) the order book only includes predefined contracts, i.e. the normal contracts generated by the backend  UDC: the order book only includes block products, which were created as the result of a block order submitted by a member  ALL: the order book contains both, PDC and UDC contracts
         :type contract_type: ContractType
         :param with_portfolio_information: If set to true, the portfolio_information is included in the response. Set to false to optimize caching.
         :type with_portfolio_information: bool
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/logs_api.py` & `powerbot_client-2.9.1/powerbot_client/api/logs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/market_api.py` & `powerbot_client-2.9.1/powerbot_client/api/market_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -885,14 +885,16 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.login(credentials, async_req=True)
         >>> result = thread.get()
 
         :param credentials: (required)
         :type credentials: Credentials
+        :param force: This parameter is only relevant for M7 based exchanges. It will disconnect anyone already connected with the specified account.
+        :type force: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -915,14 +917,16 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.login_with_http_info(credentials, async_req=True)
         >>> result = thread.get()
 
         :param credentials: (required)
         :type credentials: Credentials
+        :param force: This parameter is only relevant for M7 based exchanges. It will disconnect anyone already connected with the specified account.
+        :type force: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -942,15 +946,16 @@
                  returns the request thread.
         :rtype: tuple(MarketStatus, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'credentials'
+            'credentials',
+            'force'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -973,14 +978,16 @@
             raise ApiValueError("Missing the required parameter `credentials` when calling `login`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if local_var_params.get('force') is not None:  # noqa: E501
+            query_params.append(('force', local_var_params['force']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1028,14 +1035,16 @@
         Allows you to log the server out of the exchange. This needs to be done only on very rare occasions and can only be done by the master-API-key. **Heads up!** This function is NOT for you logging out of this server but to log out of the exchange.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.logout(async_req=True)
         >>> result = thread.get()
 
+        :param delete_orders: If this parameter is set to true, all orders will be deleted on logout. 
+        :type delete_orders: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -1056,14 +1065,16 @@
         Allows you to log the server out of the exchange. This needs to be done only on very rare occasions and can only be done by the master-API-key. **Heads up!** This function is NOT for you logging out of this server but to log out of the exchange.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.logout_with_http_info(async_req=True)
         >>> result = thread.get()
 
+        :param delete_orders: If this parameter is set to true, all orders will be deleted on logout. 
+        :type delete_orders: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1083,14 +1094,15 @@
                  returns the request thread.
         :rtype: tuple(MarketStatus, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
+            'delete_orders'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1110,14 +1122,16 @@
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if local_var_params.get('delete_orders') is not None:  # noqa: E501
+            query_params.append(('delete_orders', local_var_params['delete_orders']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/messages_api.py` & `powerbot_client-2.9.1/powerbot_client/api/messages_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/orders_api.py` & `powerbot_client-2.9.1/powerbot_client/api/orders_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -55,14 +55,16 @@
         :type internal_trading: bool
         :param fail_on_limit_violations: If set to true, a single limit violation will prevent sending all orders to the exchange. If set to false, orders for contracts which cause a violation wont be sent, orders which do not cause a violation will be sent to the exchange. If not set, true is taken as default value.  Please note that this only covers limit violations on limits defined by the system. Violating limits defined at exchange level on one order will not prevent correct orders from being sent to the exchange. In this case, this parameter does not have any effect. 
         :type fail_on_limit_violations: bool
         :param ignore_otr: If set to true, all configured OTR-limits will be ignored the order is send to the exchange without OTR-validation.
         :type ignore_otr: bool
         :param ignore_order_action_quota: The behavior on this parameter is depending on the current exchange. * M7: If set to true, the exchange otm limit can be bypassed, as long as the current load is under L2. * Nordpool: If set to true, default exchange throttling mechanism is bypassed by PowerBot. Nordpool may still reject the request.
         :type ignore_order_action_quota: bool
+        :param include_errors: If this parameter is set to true, the response will contain orders that failed to be processed by the exchange, along with successfully placed orders. If set to false, only an error will be returned if any order fails.  Please note that this parameter only effects the response and has no effect on how orders are treaded by PowerBot or the exchange. 
+        :type include_errors: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -95,14 +97,16 @@
         :type internal_trading: bool
         :param fail_on_limit_violations: If set to true, a single limit violation will prevent sending all orders to the exchange. If set to false, orders for contracts which cause a violation wont be sent, orders which do not cause a violation will be sent to the exchange. If not set, true is taken as default value.  Please note that this only covers limit violations on limits defined by the system. Violating limits defined at exchange level on one order will not prevent correct orders from being sent to the exchange. In this case, this parameter does not have any effect. 
         :type fail_on_limit_violations: bool
         :param ignore_otr: If set to true, all configured OTR-limits will be ignored the order is send to the exchange without OTR-validation.
         :type ignore_otr: bool
         :param ignore_order_action_quota: The behavior on this parameter is depending on the current exchange. * M7: If set to true, the exchange otm limit can be bypassed, as long as the current load is under L2. * Nordpool: If set to true, default exchange throttling mechanism is bypassed by PowerBot. Nordpool may still reject the request.
         :type ignore_order_action_quota: bool
+        :param include_errors: If this parameter is set to true, the response will contain orders that failed to be processed by the exchange, along with successfully placed orders. If set to false, only an error will be returned if any order fails.  Please note that this parameter only effects the response and has no effect on how orders are treaded by PowerBot or the exchange. 
+        :type include_errors: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -127,15 +131,16 @@
 
         all_params = [
             'order',
             'exec_instruction',
             'internal_trading',
             'fail_on_limit_violations',
             'ignore_otr',
-            'ignore_order_action_quota'
+            'ignore_order_action_quota',
+            'include_errors'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -168,14 +173,16 @@
             query_params.append(('internal_trading', local_var_params['internal_trading']))  # noqa: E501
         if local_var_params.get('fail_on_limit_violations') is not None:  # noqa: E501
             query_params.append(('fail_on_limit_violations', local_var_params['fail_on_limit_violations']))  # noqa: E501
         if local_var_params.get('ignore_otr') is not None:  # noqa: E501
             query_params.append(('ignore_otr', local_var_params['ignore_otr']))  # noqa: E501
         if local_var_params.get('ignore_order_action_quota') is not None:  # noqa: E501
             query_params.append(('ignore_order_action_quota', local_var_params['ignore_order_action_quota']))  # noqa: E501
+        if local_var_params.get('include_errors') is not None:  # noqa: E501
+            query_params.append(('include_errors', local_var_params['include_errors']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -213,25 +220,25 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def delete_orders(self, **kwargs):  # noqa: E501
+    def delete_orders(self, portfolio_id, **kwargs):  # noqa: E501
         """Delete all orders  # noqa: E501
 
         Allows you to delete all orders of a portfolio  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_orders(async_req=True)
+        >>> thread = api.delete_orders(portfolio_id, async_req=True)
         >>> result = thread.get()
 
-        :param portfolio_id:
+        :param portfolio_id: (required)
         :type portfolio_id: list[str]
         :param delivery_areas:
         :type delivery_areas: list[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -243,27 +250,27 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: list[OwnOrder]
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_orders_with_http_info(**kwargs)  # noqa: E501
+        return self.delete_orders_with_http_info(portfolio_id, **kwargs)  # noqa: E501
 
-    def delete_orders_with_http_info(self, **kwargs):  # noqa: E501
+    def delete_orders_with_http_info(self, portfolio_id, **kwargs):  # noqa: E501
         """Delete all orders  # noqa: E501
 
         Allows you to delete all orders of a portfolio  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_orders_with_http_info(async_req=True)
+        >>> thread = api.delete_orders_with_http_info(portfolio_id, async_req=True)
         >>> result = thread.get()
 
-        :param portfolio_id:
+        :param portfolio_id: (required)
         :type portfolio_id: list[str]
         :param delivery_areas:
         :type delivery_areas: list[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
@@ -309,14 +316,17 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method delete_orders" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'portfolio_id' is set
+        if self.api_client.client_side_validation and local_var_params.get('portfolio_id') is None:  # noqa: E501
+            raise ApiValueError("Missing the required parameter `portfolio_id` when calling `delete_orders`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if local_var_params.get('portfolio_id') is not None:  # noqa: E501
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/portfolios_api.py` & `powerbot_client-2.9.1/powerbot_client/api/portfolios_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/report_api.py` & `powerbot_client-2.9.1/powerbot_client/api/report_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/settings_api.py` & `powerbot_client-2.9.1/powerbot_client/api/settings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/signals_api.py` & `powerbot_client-2.9.1/powerbot_client/api/schema_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -21,88 +21,68 @@
 from powerbot_client.api_client import ApiClient
 from powerbot_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class SignalsApi(object):
+class SchemaApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def delete_signals(self, source, delivery_start, delivery_end, **kwargs):  # noqa: E501
-        """Delete signals  # noqa: E501
+    def add_schema(self, validation_schema, **kwargs):  # noqa: E501
+        """Add schema  # noqa: E501
 
-        Allows you to delete signals. By setting the optional delivery_areas and/or portfolio_ids parameters, you can delete signals for selected cases only. Without specifying these parameters, the signal is removed completely. **Heads up** The \"source\" of a signal containing position_long and position_short is always \"POSITION\".  # noqa: E501
+        Create a new schema.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_signals(source, delivery_start, delivery_end, async_req=True)
+        >>> thread = api.add_schema(validation_schema, async_req=True)
         >>> result = thread.get()
 
-        :param source: (required)
-        :type source: str
-        :param delivery_start: (required)
-        :type delivery_start: datetime
-        :param delivery_end: (required)
-        :type delivery_end: datetime
-        :param delivery_areas:
-        :type delivery_areas: list[str]
-        :param portfolio_id:
-        :type portfolio_id: list[str]
-        :param exact: only delete signals matching `delivery_start` and `delivery_end` exactly
-        :type exact: bool
+        :param validation_schema: (required)
+        :type validation_schema: ValidationSchema
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: ValidationSchema
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_signals_with_http_info(source, delivery_start, delivery_end, **kwargs)  # noqa: E501
+        return self.add_schema_with_http_info(validation_schema, **kwargs)  # noqa: E501
 
-    def delete_signals_with_http_info(self, source, delivery_start, delivery_end, **kwargs):  # noqa: E501
-        """Delete signals  # noqa: E501
+    def add_schema_with_http_info(self, validation_schema, **kwargs):  # noqa: E501
+        """Add schema  # noqa: E501
 
-        Allows you to delete signals. By setting the optional delivery_areas and/or portfolio_ids parameters, you can delete signals for selected cases only. Without specifying these parameters, the signal is removed completely. **Heads up** The \"source\" of a signal containing position_long and position_short is always \"POSITION\".  # noqa: E501
+        Create a new schema.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_signals_with_http_info(source, delivery_start, delivery_end, async_req=True)
+        >>> thread = api.add_schema_with_http_info(validation_schema, async_req=True)
         >>> result = thread.get()
 
-        :param source: (required)
-        :type source: str
-        :param delivery_start: (required)
-        :type delivery_start: datetime
-        :param delivery_end: (required)
-        :type delivery_end: datetime
-        :param delivery_areas:
-        :type delivery_areas: list[str]
-        :param portfolio_id:
-        :type portfolio_id: list[str]
-        :param exact: only delete signals matching `delivery_start` and `delivery_end` exactly
-        :type exact: bool
+        :param validation_schema: (required)
+        :type validation_schema: ValidationSchema
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -116,26 +96,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(ValidationSchema, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'source',
-            'delivery_start',
-            'delivery_end',
-            'delivery_areas',
-            'portfolio_id',
-            'exact'
+            'validation_schema'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -145,65 +120,57 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_signals" % key
+                    " to method add_schema" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'source' is set
-        if self.api_client.client_side_validation and local_var_params.get('source') is None:  # noqa: E501
-            raise ApiValueError("Missing the required parameter `source` when calling `delete_signals`")  # noqa: E501
-        # verify the required parameter 'delivery_start' is set
-        if self.api_client.client_side_validation and local_var_params.get('delivery_start') is None:  # noqa: E501
-            raise ApiValueError("Missing the required parameter `delivery_start` when calling `delete_signals`")  # noqa: E501
-        # verify the required parameter 'delivery_end' is set
-        if self.api_client.client_side_validation and local_var_params.get('delivery_end') is None:  # noqa: E501
-            raise ApiValueError("Missing the required parameter `delivery_end` when calling `delete_signals`")  # noqa: E501
+        # verify the required parameter 'validation_schema' is set
+        if self.api_client.client_side_validation and local_var_params.get('validation_schema') is None:  # noqa: E501
+            raise ApiValueError("Missing the required parameter `validation_schema` when calling `add_schema`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'source' in local_var_params:
-            path_params['source'] = local_var_params['source']  # noqa: E501
-        if 'delivery_start' in local_var_params:
-            path_params['delivery_start'] = local_var_params['delivery_start']  # noqa: E501
-        if 'delivery_end' in local_var_params:
-            path_params['delivery_end'] = local_var_params['delivery_end']  # noqa: E501
 
         query_params = []
-        if local_var_params.get('delivery_areas') is not None:  # noqa: E501
-            query_params.append(('delivery_areas', local_var_params['delivery_areas']))  # noqa: E501
-            collection_formats['delivery_areas'] = 'csv'  # noqa: E501
-        if local_var_params.get('portfolio_id') is not None:  # noqa: E501
-            query_params.append(('portfolio_id', local_var_params['portfolio_id']))  # noqa: E501
-            collection_formats['portfolio_id'] = 'csv'  # noqa: E501
-        if local_var_params.get('exact') is not None:  # noqa: E501
-            query_params.append(('exact', local_var_params['exact']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'validation_schema' in local_var_params:
+            body_params = local_var_params['validation_schema']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # HTTP header `Content-Type`
+        content_types_list = local_var_params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json'],
+                'PUT', body_params))  # noqa: E501
+        if content_types_list:
+                header_params['Content-Type'] = content_types_list
+
         # Authentication setting
         auth_settings = ['api_key_security']  # noqa: E501
 
-        response_types_map = {}
+        response_types_map = {
+            200: "ValidationSchema",
+        }
 
         return self.api_client.call_api(
-            '/signals/{source}/{delivery_start}/{delivery_end}', 'DELETE',
+            '/schema', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -211,92 +178,64 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def get_signals(self, **kwargs):  # noqa: E501
-        """List signals  # noqa: E501
+    def delete_schema(self, type, name, version, **kwargs):  # noqa: E501
+        """Delete schema  # noqa: E501
 
-        Allows you to retrieve signals you have previously sent to the system.  # noqa: E501
+        Deletes the schema matching the given name, type and version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_signals(async_req=True)
+        >>> thread = api.delete_schema(type, name, version, async_req=True)
         >>> result = thread.get()
 
-        :param portfolio_id:
-        :type portfolio_id: list[str]
-        :param offset: Offset when loading a list of items
-        :type offset: int
-        :param limit: Limits the number of loaded items
-        :type limit: int
-        :param received_from: from timestamp is 'inclusive' (i.e. >=), use UTC timezone
-        :type received_from: datetime
-        :param received_to: to timestamp is 'exclusive' (i.e. <), use UTC timezone
-        :type received_to: datetime
-        :param delivery_area: filter by delivery area
-        :type delivery_area: str
-        :param delivery_start: filter by delivery_start, use UTC timezone
-        :type delivery_start: datetime
-        :param delivery_end: filter by delivery_end, use UTC timezone
-        :type delivery_end: datetime
-        :param delivery_from: limit signals to those that have a delivery start greater or equal to the given value
-        :type delivery_from: datetime
-        :param delivery_to: limit signals to those that have a delivery end less than or equal to the given value
-        :type delivery_to: datetime
+        :param type: (required)
+        :type type: ValidationSchemaType
+        :param name: (required)
+        :type name: str
+        :param version: (required)
+        :type version: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: list[Signal]
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_signals_with_http_info(**kwargs)  # noqa: E501
+        return self.delete_schema_with_http_info(type, name, version, **kwargs)  # noqa: E501
 
-    def get_signals_with_http_info(self, **kwargs):  # noqa: E501
-        """List signals  # noqa: E501
+    def delete_schema_with_http_info(self, type, name, version, **kwargs):  # noqa: E501
+        """Delete schema  # noqa: E501
 
-        Allows you to retrieve signals you have previously sent to the system.  # noqa: E501
+        Deletes the schema matching the given name, type and version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_signals_with_http_info(async_req=True)
+        >>> thread = api.delete_schema_with_http_info(type, name, version, async_req=True)
         >>> result = thread.get()
 
-        :param portfolio_id:
-        :type portfolio_id: list[str]
-        :param offset: Offset when loading a list of items
-        :type offset: int
-        :param limit: Limits the number of loaded items
-        :type limit: int
-        :param received_from: from timestamp is 'inclusive' (i.e. >=), use UTC timezone
-        :type received_from: datetime
-        :param received_to: to timestamp is 'exclusive' (i.e. <), use UTC timezone
-        :type received_to: datetime
-        :param delivery_area: filter by delivery area
-        :type delivery_area: str
-        :param delivery_start: filter by delivery_start, use UTC timezone
-        :type delivery_start: datetime
-        :param delivery_end: filter by delivery_end, use UTC timezone
-        :type delivery_end: datetime
-        :param delivery_from: limit signals to those that have a delivery start greater or equal to the given value
-        :type delivery_from: datetime
-        :param delivery_to: limit signals to those that have a delivery end less than or equal to the given value
-        :type delivery_to: datetime
+        :param type: (required)
+        :type type: ValidationSchemaType
+        :param name: (required)
+        :type name: str
+        :param version: (required)
+        :type version: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -310,30 +249,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(list[Signal], status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         local_var_params = locals()
 
         all_params = [
-            'portfolio_id',
-            'offset',
-            'limit',
-            'received_from',
-            'received_to',
-            'delivery_area',
-            'delivery_start',
-            'delivery_end',
-            'delivery_from',
-            'delivery_to'
+            'type',
+            'name',
+            'version'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -343,71 +275,57 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_signals" % key
+                    " to method delete_schema" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'type' is set
+        if self.api_client.client_side_validation and local_var_params.get('type') is None:  # noqa: E501
+            raise ApiValueError("Missing the required parameter `type` when calling `delete_schema`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if self.api_client.client_side_validation and local_var_params.get('name') is None:  # noqa: E501
+            raise ApiValueError("Missing the required parameter `name` when calling `delete_schema`")  # noqa: E501
+        # verify the required parameter 'version' is set
+        if self.api_client.client_side_validation and local_var_params.get('version') is None:  # noqa: E501
+            raise ApiValueError("Missing the required parameter `version` when calling `delete_schema`")  # noqa: E501
 
-        if self.api_client.client_side_validation and 'offset' in local_var_params and local_var_params['offset'] < 0:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `offset` when calling `get_signals`, must be a value greater than or equal to `0`")  # noqa: E501
-        if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] > 500:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `limit` when calling `get_signals`, must be a value less than or equal to `500`")  # noqa: E501
-        if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] < 0:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `limit` when calling `get_signals`, must be a value greater than or equal to `0`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
+        if 'type' in local_var_params:
+            path_params['type'] = local_var_params['type']  # noqa: E501
+        if 'name' in local_var_params:
+            path_params['name'] = local_var_params['name']  # noqa: E501
+        if 'version' in local_var_params:
+            path_params['version'] = local_var_params['version']  # noqa: E501
 
         query_params = []
-        if local_var_params.get('portfolio_id') is not None:  # noqa: E501
-            query_params.append(('portfolio_id', local_var_params['portfolio_id']))  # noqa: E501
-            collection_formats['portfolio_id'] = 'csv'  # noqa: E501
-        if local_var_params.get('offset') is not None:  # noqa: E501
-            query_params.append(('offset', local_var_params['offset']))  # noqa: E501
-        if local_var_params.get('limit') is not None:  # noqa: E501
-            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
-        if local_var_params.get('received_from') is not None:  # noqa: E501
-            query_params.append(('received_from', local_var_params['received_from']))  # noqa: E501
-        if local_var_params.get('received_to') is not None:  # noqa: E501
-            query_params.append(('received_to', local_var_params['received_to']))  # noqa: E501
-        if local_var_params.get('delivery_area') is not None:  # noqa: E501
-            query_params.append(('delivery_area', local_var_params['delivery_area']))  # noqa: E501
-        if local_var_params.get('delivery_start') is not None:  # noqa: E501
-            query_params.append(('delivery_start', local_var_params['delivery_start']))  # noqa: E501
-        if local_var_params.get('delivery_end') is not None:  # noqa: E501
-            query_params.append(('delivery_end', local_var_params['delivery_end']))  # noqa: E501
-        if local_var_params.get('delivery_from') is not None:  # noqa: E501
-            query_params.append(('delivery_from', local_var_params['delivery_from']))  # noqa: E501
-        if local_var_params.get('delivery_to') is not None:  # noqa: E501
-            query_params.append(('delivery_to', local_var_params['delivery_to']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['api_key_security']  # noqa: E501
 
-        response_types_map = {
-            200: "list[Signal]",
-        }
+        response_types_map = {}
 
         return self.api_client.call_api(
-            '/signals', 'GET',
+            '/schema/{type}/{name}/{version}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -415,56 +333,72 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def update_signals(self, value, **kwargs):  # noqa: E501
-        """Add signals  # noqa: E501
+    def get_schemas(self, **kwargs):  # noqa: E501
+        """List schemas  # noqa: E501
 
-        Allows you to send trading signals to the system, e.g. positions, fundamental data, weather data or outputs of an optimization software. This data is then aligned to contracts at the market and delivered with the orderbook. This way, trading signals are automatically archived for ex-post analysis and algorithms do not need to import data themselves. In addition, signals are displayed in the dashboard.  This methods can receive a collection of signals at once and each signal has a freely defined source (e.g. ETRM_system).  Note that it is not possible to post signals for a defined contract. All contracts which have the specified \"delivery_start\" and \"delivery_end\" field will receive the signal (e.g. XBID and local contracts), limited to the specified delivery areas and portfolios.  A signal can contain EITHER a position_long and position_short (the MWs to be traded, both need to be equal or greater than zero) OR a freely defined JSON object containing key/value pairs, but not both at once.  **Heads up** The \"source\" of a signal containing position_long and position_short will always be \"POSITION\", no matter what is defined in the request body.  * \"position_long\" indicates the surplus in MW that should or can be sold at the market (equal or greater than zero)  * \"position_short\" indicates the deficiency in MW that should or can be bought at the market (equal or greater than zero)  * \"value\" should contain the freely defined JSON object with key/value pairs. Please be aware that a signal-key for each contract is unique and data is overwritten, if sent from multiple sources.  # noqa: E501
+        Retrieves all schemas matching the provided filter criteria.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_signals(value, async_req=True)
+        >>> thread = api.get_schemas(async_req=True)
         >>> result = thread.get()
 
-        :param value: Signals payload (required)
-        :type value: list[BulkSignal]
+        :param offset: Offset when loading a list of items
+        :type offset: int
+        :param limit: Limits the number of loaded items
+        :type limit: int
+        :param type:
+        :type type: ValidationSchemaType
+        :param name:
+        :type name: str
+        :param version:
+        :type version: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: list[BulkSignalResponse]
+        :rtype: list[ValidationSchema]
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_signals_with_http_info(value, **kwargs)  # noqa: E501
+        return self.get_schemas_with_http_info(**kwargs)  # noqa: E501
 
-    def update_signals_with_http_info(self, value, **kwargs):  # noqa: E501
-        """Add signals  # noqa: E501
+    def get_schemas_with_http_info(self, **kwargs):  # noqa: E501
+        """List schemas  # noqa: E501
 
-        Allows you to send trading signals to the system, e.g. positions, fundamental data, weather data or outputs of an optimization software. This data is then aligned to contracts at the market and delivered with the orderbook. This way, trading signals are automatically archived for ex-post analysis and algorithms do not need to import data themselves. In addition, signals are displayed in the dashboard.  This methods can receive a collection of signals at once and each signal has a freely defined source (e.g. ETRM_system).  Note that it is not possible to post signals for a defined contract. All contracts which have the specified \"delivery_start\" and \"delivery_end\" field will receive the signal (e.g. XBID and local contracts), limited to the specified delivery areas and portfolios.  A signal can contain EITHER a position_long and position_short (the MWs to be traded, both need to be equal or greater than zero) OR a freely defined JSON object containing key/value pairs, but not both at once.  **Heads up** The \"source\" of a signal containing position_long and position_short will always be \"POSITION\", no matter what is defined in the request body.  * \"position_long\" indicates the surplus in MW that should or can be sold at the market (equal or greater than zero)  * \"position_short\" indicates the deficiency in MW that should or can be bought at the market (equal or greater than zero)  * \"value\" should contain the freely defined JSON object with key/value pairs. Please be aware that a signal-key for each contract is unique and data is overwritten, if sent from multiple sources.  # noqa: E501
+        Retrieves all schemas matching the provided filter criteria.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_signals_with_http_info(value, async_req=True)
+        >>> thread = api.get_schemas_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param value: Signals payload (required)
-        :type value: list[BulkSignal]
+        :param offset: Offset when loading a list of items
+        :type offset: int
+        :param limit: Limits the number of loaded items
+        :type limit: int
+        :param type:
+        :type type: ValidationSchemaType
+        :param name:
+        :type name: str
+        :param version:
+        :type version: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -478,21 +412,25 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(list[BulkSignalResponse], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(list[ValidationSchema], status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'value'
+            'offset',
+            'limit',
+            'type',
+            'name',
+            'version'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -502,57 +440,60 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_signals" % key
+                    " to method get_schemas" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'value' is set
-        if self.api_client.client_side_validation and local_var_params.get('value') is None:  # noqa: E501
-            raise ApiValueError("Missing the required parameter `value` when calling `update_signals`")  # noqa: E501
 
+        if self.api_client.client_side_validation and 'offset' in local_var_params and local_var_params['offset'] < 0:  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `offset` when calling `get_schemas`, must be a value greater than or equal to `0`")  # noqa: E501
+        if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] > 500:  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `limit` when calling `get_schemas`, must be a value less than or equal to `500`")  # noqa: E501
+        if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] < 0:  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `limit` when calling `get_schemas`, must be a value greater than or equal to `0`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if local_var_params.get('offset') is not None:  # noqa: E501
+            query_params.append(('offset', local_var_params['offset']))  # noqa: E501
+        if local_var_params.get('limit') is not None:  # noqa: E501
+            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
+        if local_var_params.get('type') is not None:  # noqa: E501
+            query_params.append(('type', local_var_params['type']))  # noqa: E501
+        if local_var_params.get('name') is not None:  # noqa: E501
+            query_params.append(('name', local_var_params['name']))  # noqa: E501
+        if local_var_params.get('version') is not None:  # noqa: E501
+            query_params.append(('version', local_var_params['version']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'value' in local_var_params:
-            body_params = local_var_params['value']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        content_types_list = local_var_params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json'],
-                'POST', body_params))  # noqa: E501
-        if content_types_list:
-                header_params['Content-Type'] = content_types_list
-
         # Authentication setting
         auth_settings = ['api_key_security']  # noqa: E501
 
         response_types_map = {
-            200: "list[BulkSignalResponse]",
+            200: "list[ValidationSchema]",
         }
 
         return self.api_client.call_api(
-            '/signals', 'POST',
+            '/schema', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/subscriptions_api.py` & `powerbot_client-2.9.1/powerbot_client/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/tenants_api.py` & `powerbot_client-2.9.1/powerbot_client/api/tenants_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api/trades_api.py` & `powerbot_client-2.9.1/powerbot_client/api/trades_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `powerbot_client-2.8.0/powerbot_client/api_client.py` & `powerbot_client-2.9.1/powerbot_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.8.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.9.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -298,16 +298,16 @@
 
         if type(klass) == str:
             if klass.startswith('list['):
                 sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
                 return [self.__deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
-            if klass.startswith('dict('):
-                sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
+            if klass.startswith('dict['):
+                sub_kls = re.match(r'dict\[([^,]*), (.*)\]', klass).group(2)
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in six.iteritems(data)}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
@@ -688,14 +688,15 @@
                 klass.openapi_types is not None and
                 isinstance(data, (list, dict))):
             for attr, attr_type in six.iteritems(klass.openapi_types):
                 if klass.attribute_map[attr] in data:
                     value = data[klass.attribute_map[attr]]
                     kwargs[attr] = self.__deserialize(value, attr_type)
 
+        kwargs["local_vars_configuration"] = self.configuration
         instance = klass(**kwargs)
 
         if has_discriminator:
             klass_name = instance.get_real_child_model(data)
             if klass_name:
                 instance = self.__deserialize(data, klass_name)
         return instance
```

### Comparing `powerbot_client-2.8.0/powerbot_client/configuration.py` & `powerbot_client-2.9.1/powerbot_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -113,15 +113,15 @@
                  disabled_client_side_validations="",
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ):
         """Constructor
         """
-        self._base_path = "https://playground.powerbot-trading.com/v2/api" if host is None else host
+        self._base_path = "https://playground.powerbot-trading.com/api" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -406,26 +406,26 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.8.0\n"\
-               "SDK Package Version: 2.8.0".\
+               "Version of the API: 2.9.1\n"\
+               "SDK Package Version: 2.9.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://playground.powerbot-trading.com/v2/api",
+                'url': "https://playground.powerbot-trading.com/api",
                 'description': "No description provided",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `powerbot_client-2.8.0/powerbot_client/exceptions.py` & `powerbot_client-2.9.1/powerbot_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/__init__.py` & `powerbot_client-2.9.1/powerbot_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -28,15 +28,14 @@
 from powerbot_client.models.algo_status import AlgoStatus
 from powerbot_client.models.api_key import ApiKey
 from powerbot_client.models.api_key_details import ApiKeyDetails
 from powerbot_client.models.api_key_portfolio_update import ApiKeyPortfolioUpdate
 from powerbot_client.models.api_key_type import ApiKeyType
 from powerbot_client.models.atc_status import AtcStatus
 from powerbot_client.models.audit_log_entry import AuditLogEntry
-from powerbot_client.models.available_portfolio import AvailablePortfolio
 from powerbot_client.models.bulk_contract_statistics import BulkContractStatistics
 from powerbot_client.models.bulk_signal import BulkSignal
 from powerbot_client.models.bulk_signal_response import BulkSignalResponse
 from powerbot_client.models.capacity import Capacity
 from powerbot_client.models.capacity_changes import CapacityChanges
 from powerbot_client.models.cash_limit import CashLimit
 from powerbot_client.models.changed_credentials import ChangedCredentials
@@ -74,14 +73,15 @@
 from powerbot_client.models.notification import Notification
 from powerbot_client.models.on_missing_heartbeat import OnMissingHeartbeat
 from powerbot_client.models.order_action import OrderAction
 from powerbot_client.models.order_book import OrderBook
 from powerbot_client.models.order_book_changed_event import OrderBookChangedEvent
 from powerbot_client.models.order_book_changes import OrderBookChanges
 from powerbot_client.models.order_book_entry import OrderBookEntry
+from powerbot_client.models.order_book_group import OrderBookGroup
 from powerbot_client.models.order_books import OrderBooks
 from powerbot_client.models.order_entry import OrderEntry
 from powerbot_client.models.order_execution_restriction import OrderExecutionRestriction
 from powerbot_client.models.order_modify import OrderModify
 from powerbot_client.models.order_modify_item import OrderModifyItem
 from powerbot_client.models.order_side import OrderSide
 from powerbot_client.models.order_state import OrderState
@@ -96,14 +96,15 @@
 from powerbot_client.models.portfolio_changes import PortfolioChanges
 from powerbot_client.models.portfolio_information import PortfolioInformation
 from powerbot_client.models.portfolio_type import PortfolioType
 from powerbot_client.models.position_limit import PositionLimit
 from powerbot_client.models.product_information import ProductInformation
 from powerbot_client.models.public_trade import PublicTrade
 from powerbot_client.models.public_trade_changes import PublicTradeChanges
+from powerbot_client.models.related_contract import RelatedContract
 from powerbot_client.models.report import Report
 from powerbot_client.models.report_element import ReportElement
 from powerbot_client.models.risk_management_settings import RiskManagementSettings
 from powerbot_client.models.risk_settings_and_portfolio_information import RiskSettingsAndPortfolioInformation
 from powerbot_client.models.severity import Severity
 from powerbot_client.models.signal import Signal
 from powerbot_client.models.signal_changes import SignalChanges
@@ -115,8 +116,10 @@
 from powerbot_client.models.trade_state import TradeState
 from powerbot_client.models.trading_area import TradingArea
 from powerbot_client.models.update_algo_setup import UpdateAlgoSetup
 from powerbot_client.models.update_status import UpdateStatus
 from powerbot_client.models.updated_api_key import UpdatedApiKey
 from powerbot_client.models.updated_portfolio import UpdatedPortfolio
 from powerbot_client.models.updated_tenant import UpdatedTenant
+from powerbot_client.models.validation_schema import ValidationSchema
+from powerbot_client.models.validation_schema_type import ValidationSchemaType
 from powerbot_client.models.validity_restriction import ValidityRestriction
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/aggressor_indicator.py` & `powerbot_client-2.9.1/powerbot_client/models/aggressor_indicator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_command.py` & `powerbot_client-2.9.1/powerbot_client/models/algo_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_details.py` & `powerbot_client-2.9.1/powerbot_client/models/algo_details.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -39,40 +39,46 @@
     openapi_types = {
         'algo_id': 'str',
         'algo_name': 'str',
         'algo_description': 'str',
         'require_heartbeat_every_seconds': 'int',
         'on_missing_heartbeat': 'OnMissingHeartbeat',
         'image': 'str',
-        'instances': 'list[AlgoInstance]'
+        'instances': 'list[AlgoInstance]',
+        'parameter_schema_name': 'str',
+        'parameter_schema_version': 'str'
     }
 
     attribute_map = {
         'algo_id': 'algo_id',
         'algo_name': 'algo_name',
         'algo_description': 'algo_description',
         'require_heartbeat_every_seconds': 'require_heartbeat_every_seconds',
         'on_missing_heartbeat': 'on_missing_heartbeat',
         'image': 'image',
-        'instances': 'instances'
+        'instances': 'instances',
+        'parameter_schema_name': 'parameter_schema_name',
+        'parameter_schema_version': 'parameter_schema_version'
     }
 
-    def __init__(self, algo_id=None, algo_name=None, algo_description=None, require_heartbeat_every_seconds=None, on_missing_heartbeat=None, image=None, instances=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, algo_id=None, algo_name=None, algo_description=None, require_heartbeat_every_seconds=None, on_missing_heartbeat=None, image=None, instances=None, parameter_schema_name=None, parameter_schema_version=None, local_vars_configuration=None):  # noqa: E501
         """AlgoDetails - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._algo_id = None
         self._algo_name = None
         self._algo_description = None
         self._require_heartbeat_every_seconds = None
         self._on_missing_heartbeat = None
         self._image = None
         self._instances = None
+        self._parameter_schema_name = None
+        self._parameter_schema_version = None
         self.discriminator = None
 
         if algo_id is not None:
             self.algo_id = algo_id
         if algo_name is not None:
             self.algo_name = algo_name
         if algo_description is not None:
@@ -81,14 +87,18 @@
             self.require_heartbeat_every_seconds = require_heartbeat_every_seconds
         if on_missing_heartbeat is not None:
             self.on_missing_heartbeat = on_missing_heartbeat
         if image is not None:
             self.image = image
         if instances is not None:
             self.instances = instances
+        if parameter_schema_name is not None:
+            self.parameter_schema_name = parameter_schema_name
+        if parameter_schema_version is not None:
+            self.parameter_schema_version = parameter_schema_version
 
     @property
     def algo_id(self):
         """Gets the algo_id of this AlgoDetails.  # noqa: E501
 
         The id of the algorithm  # noqa: E501
 
@@ -241,14 +251,60 @@
 
         :param instances: The instances of this AlgoDetails.  # noqa: E501
         :type instances: list[AlgoInstance]
         """
 
         self._instances = instances
 
+    @property
+    def parameter_schema_name(self):
+        """Gets the parameter_schema_name of this AlgoDetails.  # noqa: E501
+
+        The JSON schema name for the payload of object parameters required by the algo.  # noqa: E501
+
+        :return: The parameter_schema_name of this AlgoDetails.  # noqa: E501
+        :rtype: str
+        """
+        return self._parameter_schema_name
+
+    @parameter_schema_name.setter
+    def parameter_schema_name(self, parameter_schema_name):
+        """Sets the parameter_schema_name of this AlgoDetails.
+
+        The JSON schema name for the payload of object parameters required by the algo.  # noqa: E501
+
+        :param parameter_schema_name: The parameter_schema_name of this AlgoDetails.  # noqa: E501
+        :type parameter_schema_name: str
+        """
+
+        self._parameter_schema_name = parameter_schema_name
+
+    @property
+    def parameter_schema_version(self):
+        """Gets the parameter_schema_version of this AlgoDetails.  # noqa: E501
+
+        The JSON schema version for the payload of object parameters required by the algo.  # noqa: E501
+
+        :return: The parameter_schema_version of this AlgoDetails.  # noqa: E501
+        :rtype: str
+        """
+        return self._parameter_schema_version
+
+    @parameter_schema_version.setter
+    def parameter_schema_version(self, parameter_schema_version):
+        """Sets the parameter_schema_version of this AlgoDetails.
+
+        The JSON schema version for the payload of object parameters required by the algo.  # noqa: E501
+
+        :param parameter_schema_version: The parameter_schema_version of this AlgoDetails.  # noqa: E501
+        :type parameter_schema_version: str
+        """
+
+        self._parameter_schema_version = parameter_schema_version
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_event.py` & `powerbot_client-2.9.1/powerbot_client/models/algo_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_heartbeat.py` & `powerbot_client-2.9.1/powerbot_client/models/algo_heartbeat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_instance.py` & `powerbot_client-2.9.1/powerbot_client/models/algo_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,59 +35,64 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'instance_id': 'str',
         'exchange': 'str',
+        'tenant_id': 'str',
         'portfolio_ids': 'list[str]',
         'parameters': 'object',
         'status': 'AlgoStatus',
         'started_at': 'datetime',
         'stopped_at': 'datetime',
         'stop_status_text': 'str',
         'last_heartbeat_at': 'datetime',
         'heartbeat': 'AlgoHeartbeat'
     }
 
     attribute_map = {
         'instance_id': 'instance_id',
         'exchange': 'exchange',
+        'tenant_id': 'tenant_id',
         'portfolio_ids': 'portfolio_ids',
         'parameters': 'parameters',
         'status': 'status',
         'started_at': 'started_at',
         'stopped_at': 'stopped_at',
         'stop_status_text': 'stop_status_text',
         'last_heartbeat_at': 'last_heartbeat_at',
         'heartbeat': 'heartbeat'
     }
 
-    def __init__(self, instance_id=None, exchange=None, portfolio_ids=None, parameters=None, status=None, started_at=None, stopped_at=None, stop_status_text=None, last_heartbeat_at=None, heartbeat=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, instance_id=None, exchange=None, tenant_id=None, portfolio_ids=None, parameters=None, status=None, started_at=None, stopped_at=None, stop_status_text=None, last_heartbeat_at=None, heartbeat=None, local_vars_configuration=None):  # noqa: E501
         """AlgoInstance - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._instance_id = None
         self._exchange = None
+        self._tenant_id = None
         self._portfolio_ids = None
         self._parameters = None
         self._status = None
         self._started_at = None
         self._stopped_at = None
         self._stop_status_text = None
         self._last_heartbeat_at = None
         self._heartbeat = None
         self.discriminator = None
 
         if instance_id is not None:
             self.instance_id = instance_id
         if exchange is not None:
             self.exchange = exchange
+        if tenant_id is not None:
+            self.tenant_id = tenant_id
         if portfolio_ids is not None:
             self.portfolio_ids = portfolio_ids
         if parameters is not None:
             self.parameters = parameters
         if status is not None:
             self.status = status
         if started_at is not None:
@@ -144,14 +149,37 @@
         :param exchange: The exchange of this AlgoInstance.  # noqa: E501
         :type exchange: str
         """
 
         self._exchange = exchange
 
     @property
+    def tenant_id(self):
+        """Gets the tenant_id of this AlgoInstance.  # noqa: E501
+
+        The tenant for this instance.  # noqa: E501
+
+        :return: The tenant_id of this AlgoInstance.  # noqa: E501
+        :rtype: str
+        """
+        return self._tenant_id
+
+    @tenant_id.setter
+    def tenant_id(self, tenant_id):
+        """Sets the tenant_id of this AlgoInstance.
+
+        The tenant for this instance.  # noqa: E501
+
+        :param tenant_id: The tenant_id of this AlgoInstance.  # noqa: E501
+        :type tenant_id: str
+        """
+
+        self._tenant_id = tenant_id
+
+    @property
     def portfolio_ids(self):
         """Gets the portfolio_ids of this AlgoInstance.  # noqa: E501
 
         The configured portfolios for this instance.  # noqa: E501
 
         :return: The portfolio_ids of this AlgoInstance.  # noqa: E501
         :rtype: list[str]
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_instance_change.py` & `powerbot_client-2.9.1/powerbot_client/models/algo_instance_change.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_instance_event.py` & `powerbot_client-2.9.1/powerbot_client/models/algo_instance_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_instance_parameters.py` & `powerbot_client-2.9.1/powerbot_client/models/algo_instance_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_setup.py` & `powerbot_client-2.9.1/powerbot_client/models/update_algo_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,218 +18,237 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from powerbot_client.configuration import Configuration
 
 
-class AlgoSetup(object):
+class UpdateAlgoSetup(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'str',
         'name': 'str',
         'description': 'str',
         'require_heartbeat_every_seconds': 'int',
         'on_missing_heartbeat': 'OnMissingHeartbeat',
-        'image': 'str'
+        'image': 'str',
+        'parameter_schema_name': 'str',
+        'parameter_schema_version': 'str'
     }
 
     attribute_map = {
-        'id': 'id',
         'name': 'name',
         'description': 'description',
         'require_heartbeat_every_seconds': 'require_heartbeat_every_seconds',
         'on_missing_heartbeat': 'on_missing_heartbeat',
-        'image': 'image'
+        'image': 'image',
+        'parameter_schema_name': 'parameter_schema_name',
+        'parameter_schema_version': 'parameter_schema_version'
     }
 
-    def __init__(self, id=None, name=None, description=None, require_heartbeat_every_seconds=None, on_missing_heartbeat=None, image=None, local_vars_configuration=None):  # noqa: E501
-        """AlgoSetup - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name=None, description=None, require_heartbeat_every_seconds=None, on_missing_heartbeat=None, image=None, parameter_schema_name=None, parameter_schema_version=None, local_vars_configuration=None):  # noqa: E501
+        """UpdateAlgoSetup - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
         self._name = None
         self._description = None
         self._require_heartbeat_every_seconds = None
         self._on_missing_heartbeat = None
         self._image = None
+        self._parameter_schema_name = None
+        self._parameter_schema_version = None
         self.discriminator = None
 
-        self.id = id
         if name is not None:
             self.name = name
         if description is not None:
             self.description = description
-        self.require_heartbeat_every_seconds = require_heartbeat_every_seconds
-        self.on_missing_heartbeat = on_missing_heartbeat
+        if require_heartbeat_every_seconds is not None:
+            self.require_heartbeat_every_seconds = require_heartbeat_every_seconds
+        if on_missing_heartbeat is not None:
+            self.on_missing_heartbeat = on_missing_heartbeat
         if image is not None:
             self.image = image
-
-    @property
-    def id(self):
-        """Gets the id of this AlgoSetup.  # noqa: E501
-
-        A unique id of the algorithm  # noqa: E501
-
-        :return: The id of this AlgoSetup.  # noqa: E501
-        :rtype: str
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this AlgoSetup.
-
-        A unique id of the algorithm  # noqa: E501
-
-        :param id: The id of this AlgoSetup.  # noqa: E501
-        :type id: str
-        """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and not re.search(r'[a-zA-Z0-9._-]+', id)):  # noqa: E501
-            raise ValueError(r"Invalid value for `id`, must be a follow pattern or equal to `/[a-zA-Z0-9._-]+/`")  # noqa: E501
-
-        self._id = id
+        if parameter_schema_name is not None:
+            self.parameter_schema_name = parameter_schema_name
+        if parameter_schema_version is not None:
+            self.parameter_schema_version = parameter_schema_version
 
     @property
     def name(self):
-        """Gets the name of this AlgoSetup.  # noqa: E501
+        """Gets the name of this UpdateAlgoSetup.  # noqa: E501
 
         The name of the algorithm  # noqa: E501
 
-        :return: The name of this AlgoSetup.  # noqa: E501
+        :return: The name of this UpdateAlgoSetup.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this AlgoSetup.
+        """Sets the name of this UpdateAlgoSetup.
 
         The name of the algorithm  # noqa: E501
 
-        :param name: The name of this AlgoSetup.  # noqa: E501
+        :param name: The name of this UpdateAlgoSetup.  # noqa: E501
         :type name: str
         """
 
         self._name = name
 
     @property
     def description(self):
-        """Gets the description of this AlgoSetup.  # noqa: E501
+        """Gets the description of this UpdateAlgoSetup.  # noqa: E501
 
         A short description of the algorithm  # noqa: E501
 
-        :return: The description of this AlgoSetup.  # noqa: E501
+        :return: The description of this UpdateAlgoSetup.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this AlgoSetup.
+        """Sets the description of this UpdateAlgoSetup.
 
         A short description of the algorithm  # noqa: E501
 
-        :param description: The description of this AlgoSetup.  # noqa: E501
+        :param description: The description of this UpdateAlgoSetup.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
     @property
     def require_heartbeat_every_seconds(self):
-        """Gets the require_heartbeat_every_seconds of this AlgoSetup.  # noqa: E501
+        """Gets the require_heartbeat_every_seconds of this UpdateAlgoSetup.  # noqa: E501
 
-        Specifies how often the algorithm requires a heartbeat via POST/.../heartbeat. Floating point values will be rounded to the nearest integer.  # noqa: E501
+        Specifies how often the algorithm requires a heartbeat via POST/.../heartbeat. Must be > 0  # noqa: E501
 
-        :return: The require_heartbeat_every_seconds of this AlgoSetup.  # noqa: E501
+        :return: The require_heartbeat_every_seconds of this UpdateAlgoSetup.  # noqa: E501
         :rtype: int
         """
         return self._require_heartbeat_every_seconds
 
     @require_heartbeat_every_seconds.setter
     def require_heartbeat_every_seconds(self, require_heartbeat_every_seconds):
-        """Sets the require_heartbeat_every_seconds of this AlgoSetup.
+        """Sets the require_heartbeat_every_seconds of this UpdateAlgoSetup.
 
-        Specifies how often the algorithm requires a heartbeat via POST/.../heartbeat. Floating point values will be rounded to the nearest integer.  # noqa: E501
+        Specifies how often the algorithm requires a heartbeat via POST/.../heartbeat. Must be > 0  # noqa: E501
 
-        :param require_heartbeat_every_seconds: The require_heartbeat_every_seconds of this AlgoSetup.  # noqa: E501
+        :param require_heartbeat_every_seconds: The require_heartbeat_every_seconds of this UpdateAlgoSetup.  # noqa: E501
         :type require_heartbeat_every_seconds: int
         """
-        if self.local_vars_configuration.client_side_validation and require_heartbeat_every_seconds is None:  # noqa: E501
-            raise ValueError("Invalid value for `require_heartbeat_every_seconds`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                require_heartbeat_every_seconds is not None and require_heartbeat_every_seconds < 1):  # noqa: E501
-            raise ValueError("Invalid value for `require_heartbeat_every_seconds`, must be a value greater than or equal to `1`")  # noqa: E501
 
         self._require_heartbeat_every_seconds = require_heartbeat_every_seconds
 
     @property
     def on_missing_heartbeat(self):
-        """Gets the on_missing_heartbeat of this AlgoSetup.  # noqa: E501
+        """Gets the on_missing_heartbeat of this UpdateAlgoSetup.  # noqa: E501
 
 
-        :return: The on_missing_heartbeat of this AlgoSetup.  # noqa: E501
+        :return: The on_missing_heartbeat of this UpdateAlgoSetup.  # noqa: E501
         :rtype: OnMissingHeartbeat
         """
         return self._on_missing_heartbeat
 
     @on_missing_heartbeat.setter
     def on_missing_heartbeat(self, on_missing_heartbeat):
-        """Sets the on_missing_heartbeat of this AlgoSetup.
+        """Sets the on_missing_heartbeat of this UpdateAlgoSetup.
 
 
-        :param on_missing_heartbeat: The on_missing_heartbeat of this AlgoSetup.  # noqa: E501
+        :param on_missing_heartbeat: The on_missing_heartbeat of this UpdateAlgoSetup.  # noqa: E501
         :type on_missing_heartbeat: OnMissingHeartbeat
         """
-        if self.local_vars_configuration.client_side_validation and on_missing_heartbeat is None:  # noqa: E501
-            raise ValueError("Invalid value for `on_missing_heartbeat`, must not be `None`")  # noqa: E501
 
         self._on_missing_heartbeat = on_missing_heartbeat
 
     @property
     def image(self):
-        """Gets the image of this AlgoSetup.  # noqa: E501
+        """Gets the image of this UpdateAlgoSetup.  # noqa: E501
 
         The image of the algorithm, this can be any valid docker image name with a tag. The tag can not be \"latest\" to avoid accidental upgrades.  # noqa: E501
 
-        :return: The image of this AlgoSetup.  # noqa: E501
+        :return: The image of this UpdateAlgoSetup.  # noqa: E501
         :rtype: str
         """
         return self._image
 
     @image.setter
     def image(self, image):
-        """Sets the image of this AlgoSetup.
+        """Sets the image of this UpdateAlgoSetup.
 
         The image of the algorithm, this can be any valid docker image name with a tag. The tag can not be \"latest\" to avoid accidental upgrades.  # noqa: E501
 
-        :param image: The image of this AlgoSetup.  # noqa: E501
+        :param image: The image of this UpdateAlgoSetup.  # noqa: E501
         :type image: str
         """
 
         self._image = image
 
+    @property
+    def parameter_schema_name(self):
+        """Gets the parameter_schema_name of this UpdateAlgoSetup.  # noqa: E501
+
+        The JSON schema name for the payload of object parameters required by the algo.  # noqa: E501
+
+        :return: The parameter_schema_name of this UpdateAlgoSetup.  # noqa: E501
+        :rtype: str
+        """
+        return self._parameter_schema_name
+
+    @parameter_schema_name.setter
+    def parameter_schema_name(self, parameter_schema_name):
+        """Sets the parameter_schema_name of this UpdateAlgoSetup.
+
+        The JSON schema name for the payload of object parameters required by the algo.  # noqa: E501
+
+        :param parameter_schema_name: The parameter_schema_name of this UpdateAlgoSetup.  # noqa: E501
+        :type parameter_schema_name: str
+        """
+
+        self._parameter_schema_name = parameter_schema_name
+
+    @property
+    def parameter_schema_version(self):
+        """Gets the parameter_schema_version of this UpdateAlgoSetup.  # noqa: E501
+
+        The JSON schema version for the payload of object parameters required by the algo.  # noqa: E501
+
+        :return: The parameter_schema_version of this UpdateAlgoSetup.  # noqa: E501
+        :rtype: str
+        """
+        return self._parameter_schema_version
+
+    @parameter_schema_version.setter
+    def parameter_schema_version(self, parameter_schema_version):
+        """Sets the parameter_schema_version of this UpdateAlgoSetup.
+
+        The JSON schema version for the payload of object parameters required by the algo.  # noqa: E501
+
+        :param parameter_schema_version: The parameter_schema_version of this UpdateAlgoSetup.  # noqa: E501
+        :type parameter_schema_version: str
+        """
+
+        self._parameter_schema_version = parameter_schema_version
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -264,18 +283,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AlgoSetup):
+        if not isinstance(other, UpdateAlgoSetup):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AlgoSetup):
+        if not isinstance(other, UpdateAlgoSetup):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/algo_status.py` & `powerbot_client-2.9.1/powerbot_client/models/algo_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/api_key.py` & `powerbot_client-2.9.1/powerbot_client/models/api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/api_key_details.py` & `powerbot_client-2.9.1/powerbot_client/models/api_key_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -39,15 +39,15 @@
     openapi_types = {
         'name': 'str',
         'description': 'str',
         'type': 'ApiKeyType',
         'tenant_id': 'str',
         'tenant_name': 'str',
         'inherit_tenant_portfolios': 'bool',
-        'portfolios': 'list[AvailablePortfolio]',
+        'portfolios': 'list[Portfolio]',
         'tenant_risk_settings': 'RiskManagementSettings',
         'can_read': 'bool',
         'can_trade': 'bool',
         'can_signal': 'bool'
     }
 
     attribute_map = {
@@ -238,25 +238,25 @@
 
     @property
     def portfolios(self):
         """Gets the portfolios of this ApiKeyDetails.  # noqa: E501
 
 
         :return: The portfolios of this ApiKeyDetails.  # noqa: E501
-        :rtype: list[AvailablePortfolio]
+        :rtype: list[Portfolio]
         """
         return self._portfolios
 
     @portfolios.setter
     def portfolios(self, portfolios):
         """Sets the portfolios of this ApiKeyDetails.
 
 
         :param portfolios: The portfolios of this ApiKeyDetails.  # noqa: E501
-        :type portfolios: list[AvailablePortfolio]
+        :type portfolios: list[Portfolio]
         """
 
         self._portfolios = portfolios
 
     @property
     def tenant_risk_settings(self):
         """Gets the tenant_risk_settings of this ApiKeyDetails.  # noqa: E501
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/api_key_portfolio_update.py` & `powerbot_client-2.9.1/powerbot_client/models/api_key_portfolio_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/api_key_type.py` & `powerbot_client-2.9.1/powerbot_client/models/api_key_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -32,16 +32,17 @@
     """
     allowed enum values
     """
     MASTER_API_KEY = "MASTER_API_KEY"
     STANDARD_API_KEY = "STANDARD_API_KEY"
     TENANT_MASTER_API_KEY = "TENANT_MASTER_API_KEY"
     SCHEDULING_API_KEY = "SCHEDULING_API_KEY"
+    ALGO_MANAGEMENT_KEY = "ALGO_MANAGEMENT_KEY"
 
-    allowable_values = [MASTER_API_KEY, STANDARD_API_KEY, TENANT_MASTER_API_KEY, SCHEDULING_API_KEY]  # noqa: E501
+    allowable_values = [MASTER_API_KEY, STANDARD_API_KEY, TENANT_MASTER_API_KEY, SCHEDULING_API_KEY, ALGO_MANAGEMENT_KEY]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/atc_status.py` & `powerbot_client-2.9.1/powerbot_client/models/atc_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/audit_log_entry.py` & `powerbot_client-2.9.1/powerbot_client/models/audit_log_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/available_portfolio.py` & `powerbot_client-2.9.1/powerbot_client/models/new_portfolio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from powerbot_client.configuration import Configuration
 
 
-class AvailablePortfolio(object):
+class NewPortfolio(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,192 +35,165 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'id': 'str',
         'name': 'str',
-        'tenant_id': 'str',
-        'tenant_name': 'str',
         'type': 'PortfolioType',
+        'tenant_id': 'str',
         'risk_management': 'RiskManagementSettings'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
-        'tenant_id': 'tenant_id',
-        'tenant_name': 'tenant_name',
         'type': 'type',
+        'tenant_id': 'tenant_id',
         'risk_management': 'risk_management'
     }
 
-    def __init__(self, id=None, name=None, tenant_id=None, tenant_name=None, type=None, risk_management=None, local_vars_configuration=None):  # noqa: E501
-        """AvailablePortfolio - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, id=None, name=None, type=None, tenant_id=None, risk_management=None, local_vars_configuration=None):  # noqa: E501
+        """NewPortfolio - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
-        self._tenant_id = None
-        self._tenant_name = None
         self._type = None
+        self._tenant_id = None
         self._risk_management = None
         self.discriminator = None
 
         self.id = id
         self.name = name
+        if type is not None:
+            self.type = type
         self.tenant_id = tenant_id
-        self.tenant_name = tenant_name
-        self.type = type
         self.risk_management = risk_management
 
     @property
     def id(self):
-        """Gets the id of this AvailablePortfolio.  # noqa: E501
+        """Gets the id of this NewPortfolio.  # noqa: E501
 
         A unique id (max 5 alphanumeric characters) of the portfolio  # noqa: E501
 
-        :return: The id of this AvailablePortfolio.  # noqa: E501
+        :return: The id of this NewPortfolio.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this AvailablePortfolio.
+        """Sets the id of this NewPortfolio.
 
         A unique id (max 5 alphanumeric characters) of the portfolio  # noqa: E501
 
-        :param id: The id of this AvailablePortfolio.  # noqa: E501
+        :param id: The id of this NewPortfolio.  # noqa: E501
         :type id: str
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 id is not None and len(id) > 5):
             raise ValueError("Invalid value for `id`, length must be less than or equal to `5`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                id is not None and not re.search(r'[a-zA-Z0-9._-]{1,5}', id)):  # noqa: E501
+            raise ValueError(r"Invalid value for `id`, must be a follow pattern or equal to `/[a-zA-Z0-9._-]{1,5}/`")  # noqa: E501
 
         self._id = id
 
     @property
     def name(self):
-        """Gets the name of this AvailablePortfolio.  # noqa: E501
+        """Gets the name of this NewPortfolio.  # noqa: E501
 
         The name of the portfolio  # noqa: E501
 
-        :return: The name of this AvailablePortfolio.  # noqa: E501
+        :return: The name of this NewPortfolio.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this AvailablePortfolio.
+        """Sets the name of this NewPortfolio.
 
         The name of the portfolio  # noqa: E501
 
-        :param name: The name of this AvailablePortfolio.  # noqa: E501
+        :param name: The name of this NewPortfolio.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def tenant_id(self):
-        """Gets the tenant_id of this AvailablePortfolio.  # noqa: E501
+    def type(self):
+        """Gets the type of this NewPortfolio.  # noqa: E501
 
-        The tenant the portfolio belongs to  # noqa: E501
 
-        :return: The tenant_id of this AvailablePortfolio.  # noqa: E501
-        :rtype: str
+        :return: The type of this NewPortfolio.  # noqa: E501
+        :rtype: PortfolioType
         """
-        return self._tenant_id
+        return self._type
 
-    @tenant_id.setter
-    def tenant_id(self, tenant_id):
-        """Sets the tenant_id of this AvailablePortfolio.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this NewPortfolio.
 
-        The tenant the portfolio belongs to  # noqa: E501
 
-        :param tenant_id: The tenant_id of this AvailablePortfolio.  # noqa: E501
-        :type tenant_id: str
+        :param type: The type of this NewPortfolio.  # noqa: E501
+        :type type: PortfolioType
         """
-        if self.local_vars_configuration.client_side_validation and tenant_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `tenant_id`, must not be `None`")  # noqa: E501
 
-        self._tenant_id = tenant_id
+        self._type = type
 
     @property
-    def tenant_name(self):
-        """Gets the tenant_name of this AvailablePortfolio.  # noqa: E501
+    def tenant_id(self):
+        """Gets the tenant_id of this NewPortfolio.  # noqa: E501
 
-        The name of the tenant  # noqa: E501
+        The tenant the portfolio belongs to  # noqa: E501
 
-        :return: The tenant_name of this AvailablePortfolio.  # noqa: E501
+        :return: The tenant_id of this NewPortfolio.  # noqa: E501
         :rtype: str
         """
-        return self._tenant_name
-
-    @tenant_name.setter
-    def tenant_name(self, tenant_name):
-        """Sets the tenant_name of this AvailablePortfolio.
-
-        The name of the tenant  # noqa: E501
-
-        :param tenant_name: The tenant_name of this AvailablePortfolio.  # noqa: E501
-        :type tenant_name: str
-        """
-        if self.local_vars_configuration.client_side_validation and tenant_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `tenant_name`, must not be `None`")  # noqa: E501
-
-        self._tenant_name = tenant_name
-
-    @property
-    def type(self):
-        """Gets the type of this AvailablePortfolio.  # noqa: E501
-
-
-        :return: The type of this AvailablePortfolio.  # noqa: E501
-        :rtype: PortfolioType
-        """
-        return self._type
+        return self._tenant_id
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this AvailablePortfolio.
+    @tenant_id.setter
+    def tenant_id(self, tenant_id):
+        """Sets the tenant_id of this NewPortfolio.
 
+        The tenant the portfolio belongs to  # noqa: E501
 
-        :param type: The type of this AvailablePortfolio.  # noqa: E501
-        :type type: PortfolioType
+        :param tenant_id: The tenant_id of this NewPortfolio.  # noqa: E501
+        :type tenant_id: str
         """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and tenant_id is None:  # noqa: E501
+            raise ValueError("Invalid value for `tenant_id`, must not be `None`")  # noqa: E501
 
-        self._type = type
+        self._tenant_id = tenant_id
 
     @property
     def risk_management(self):
-        """Gets the risk_management of this AvailablePortfolio.  # noqa: E501
+        """Gets the risk_management of this NewPortfolio.  # noqa: E501
 
 
-        :return: The risk_management of this AvailablePortfolio.  # noqa: E501
+        :return: The risk_management of this NewPortfolio.  # noqa: E501
         :rtype: RiskManagementSettings
         """
         return self._risk_management
 
     @risk_management.setter
     def risk_management(self, risk_management):
-        """Sets the risk_management of this AvailablePortfolio.
+        """Sets the risk_management of this NewPortfolio.
 
 
-        :param risk_management: The risk_management of this AvailablePortfolio.  # noqa: E501
+        :param risk_management: The risk_management of this NewPortfolio.  # noqa: E501
         :type risk_management: RiskManagementSettings
         """
         if self.local_vars_configuration.client_side_validation and risk_management is None:  # noqa: E501
             raise ValueError("Invalid value for `risk_management`, must not be `None`")  # noqa: E501
 
         self._risk_management = risk_management
 
@@ -262,18 +235,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AvailablePortfolio):
+        if not isinstance(other, NewPortfolio):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AvailablePortfolio):
+        if not isinstance(other, NewPortfolio):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/bulk_contract_statistics.py` & `powerbot_client-2.9.1/powerbot_client/models/bulk_contract_statistics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -33,53 +33,53 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'contracts': 'list[ContractStatistics]'
+        'statistics': 'list[ContractStatistics]'
     }
 
     attribute_map = {
-        'contracts': 'contracts'
+        'statistics': 'statistics'
     }
 
-    def __init__(self, contracts=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, statistics=None, local_vars_configuration=None):  # noqa: E501
         """BulkContractStatistics - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._contracts = None
+        self._statistics = None
         self.discriminator = None
 
-        if contracts is not None:
-            self.contracts = contracts
+        if statistics is not None:
+            self.statistics = statistics
 
     @property
-    def contracts(self):
-        """Gets the contracts of this BulkContractStatistics.  # noqa: E501
+    def statistics(self):
+        """Gets the statistics of this BulkContractStatistics.  # noqa: E501
 
 
-        :return: The contracts of this BulkContractStatistics.  # noqa: E501
+        :return: The statistics of this BulkContractStatistics.  # noqa: E501
         :rtype: list[ContractStatistics]
         """
-        return self._contracts
+        return self._statistics
 
-    @contracts.setter
-    def contracts(self, contracts):
-        """Sets the contracts of this BulkContractStatistics.
+    @statistics.setter
+    def statistics(self, statistics):
+        """Sets the statistics of this BulkContractStatistics.
 
 
-        :param contracts: The contracts of this BulkContractStatistics.  # noqa: E501
-        :type contracts: list[ContractStatistics]
+        :param statistics: The statistics of this BulkContractStatistics.  # noqa: E501
+        :type statistics: list[ContractStatistics]
         """
 
-        self._contracts = contracts
+        self._statistics = statistics
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/bulk_signal.py` & `powerbot_client-2.9.1/powerbot_client/models/bulk_signal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -40,41 +40,44 @@
         'source': 'str',
         'delivery_start': 'datetime',
         'delivery_end': 'datetime',
         'delivery_areas': 'list[str]',
         'portfolio_ids': 'list[str]',
         'position_long': 'float',
         'position_short': 'float',
+        'locked': 'bool',
         'value': 'object'
     }
 
     attribute_map = {
         'source': 'source',
         'delivery_start': 'delivery_start',
         'delivery_end': 'delivery_end',
         'delivery_areas': 'delivery_areas',
         'portfolio_ids': 'portfolio_ids',
         'position_long': 'position_long',
         'position_short': 'position_short',
+        'locked': 'locked',
         'value': 'value'
     }
 
-    def __init__(self, source=None, delivery_start=None, delivery_end=None, delivery_areas=None, portfolio_ids=None, position_long=None, position_short=None, value=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, source=None, delivery_start=None, delivery_end=None, delivery_areas=None, portfolio_ids=None, position_long=None, position_short=None, locked=None, value=None, local_vars_configuration=None):  # noqa: E501
         """BulkSignal - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._source = None
         self._delivery_start = None
         self._delivery_end = None
         self._delivery_areas = None
         self._portfolio_ids = None
         self._position_long = None
         self._position_short = None
+        self._locked = None
         self._value = None
         self.discriminator = None
 
         self.source = source
         if delivery_start is not None:
             self.delivery_start = delivery_start
         if delivery_end is not None:
@@ -83,14 +86,16 @@
             self.delivery_areas = delivery_areas
         if portfolio_ids is not None:
             self.portfolio_ids = portfolio_ids
         if position_long is not None:
             self.position_long = position_long
         if position_short is not None:
             self.position_short = position_short
+        if locked is not None:
+            self.locked = locked
         if value is not None:
             self.value = value
 
     @property
     def source(self):
         """Gets the source of this BulkSignal.  # noqa: E501
 
@@ -250,14 +255,37 @@
         :param position_short: The position_short of this BulkSignal.  # noqa: E501
         :type position_short: float
         """
 
         self._position_short = position_short
 
     @property
+    def locked(self):
+        """Gets the locked of this BulkSignal.  # noqa: E501
+
+        Setting this value to true marks this signal as locked. Locked signals can't be modified, unless the `ignore_lock` parameter is set to `true`.  This can be useful if a signal needs to be manually adjusted, and you don't want automated signal posting programs to overwrite it again.  # noqa: E501
+
+        :return: The locked of this BulkSignal.  # noqa: E501
+        :rtype: bool
+        """
+        return self._locked
+
+    @locked.setter
+    def locked(self, locked):
+        """Sets the locked of this BulkSignal.
+
+        Setting this value to true marks this signal as locked. Locked signals can't be modified, unless the `ignore_lock` parameter is set to `true`.  This can be useful if a signal needs to be manually adjusted, and you don't want automated signal posting programs to overwrite it again.  # noqa: E501
+
+        :param locked: The locked of this BulkSignal.  # noqa: E501
+        :type locked: bool
+        """
+
+        self._locked = locked
+
+    @property
     def value(self):
         """Gets the value of this BulkSignal.  # noqa: E501
 
         The custom content of the signal, posted as key/value pairs  # noqa: E501
 
         :return: The value of this BulkSignal.  # noqa: E501
         :rtype: object
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/bulk_signal_response.py` & `powerbot_client-2.9.1/powerbot_client/models/bulk_signal_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/capacity.py` & `powerbot_client-2.9.1/powerbot_client/models/capacity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/capacity_changes.py` & `powerbot_client-2.9.1/powerbot_client/models/capacity_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/cash_limit.py` & `powerbot_client-2.9.1/powerbot_client/models/cash_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/changed_credentials.py` & `powerbot_client-2.9.1/powerbot_client/models/changed_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/contract.py` & `powerbot_client-2.9.1/powerbot_client/models/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -466,95 +466,95 @@
 
         self._delivery_end = delivery_end
 
     @property
     def best_bid_price(self):
         """Gets the best_bid_price of this Contract.  # noqa: E501
 
-        The best bid's price in the orderbook's currency (i.e. EUR)  # noqa: E501
+        The price of the best bid.  # noqa: E501
 
         :return: The best_bid_price of this Contract.  # noqa: E501
         :rtype: float
         """
         return self._best_bid_price
 
     @best_bid_price.setter
     def best_bid_price(self, best_bid_price):
         """Sets the best_bid_price of this Contract.
 
-        The best bid's price in the orderbook's currency (i.e. EUR)  # noqa: E501
+        The price of the best bid.  # noqa: E501
 
         :param best_bid_price: The best_bid_price of this Contract.  # noqa: E501
         :type best_bid_price: float
         """
 
         self._best_bid_price = best_bid_price
 
     @property
     def best_bid_quantity(self):
         """Gets the best_bid_quantity of this Contract.  # noqa: E501
 
-        The best bid's quantity in the orderbook's quantity unit (i.e. MW)  # noqa: E501
+        The quantity of the best bid.  # noqa: E501
 
         :return: The best_bid_quantity of this Contract.  # noqa: E501
         :rtype: float
         """
         return self._best_bid_quantity
 
     @best_bid_quantity.setter
     def best_bid_quantity(self, best_bid_quantity):
         """Sets the best_bid_quantity of this Contract.
 
-        The best bid's quantity in the orderbook's quantity unit (i.e. MW)  # noqa: E501
+        The quantity of the best bid.  # noqa: E501
 
         :param best_bid_quantity: The best_bid_quantity of this Contract.  # noqa: E501
         :type best_bid_quantity: float
         """
 
         self._best_bid_quantity = best_bid_quantity
 
     @property
     def best_ask_price(self):
         """Gets the best_ask_price of this Contract.  # noqa: E501
 
-        The best asks's price in the orderbook's currency (i.e. EUR)  # noqa: E501
+        The price of the best ask.  # noqa: E501
 
         :return: The best_ask_price of this Contract.  # noqa: E501
         :rtype: float
         """
         return self._best_ask_price
 
     @best_ask_price.setter
     def best_ask_price(self, best_ask_price):
         """Sets the best_ask_price of this Contract.
 
-        The best asks's price in the orderbook's currency (i.e. EUR)  # noqa: E501
+        The price of the best ask.  # noqa: E501
 
         :param best_ask_price: The best_ask_price of this Contract.  # noqa: E501
         :type best_ask_price: float
         """
 
         self._best_ask_price = best_ask_price
 
     @property
     def best_ask_quantity(self):
         """Gets the best_ask_quantity of this Contract.  # noqa: E501
 
-        The best asks's quantity in the orderbook's quantity unit (i.e. MW)  # noqa: E501
+        The quantity of the best ask.  # noqa: E501
 
         :return: The best_ask_quantity of this Contract.  # noqa: E501
         :rtype: float
         """
         return self._best_ask_quantity
 
     @best_ask_quantity.setter
     def best_ask_quantity(self, best_ask_quantity):
         """Sets the best_ask_quantity of this Contract.
 
-        The best asks's quantity in the orderbook's quantity unit (i.e. MW)  # noqa: E501
+        The quantity of the best ask.  # noqa: E501
 
         :param best_ask_quantity: The best_ask_quantity of this Contract.  # noqa: E501
         :type best_ask_quantity: float
         """
 
         self._best_ask_quantity = best_ask_quantity
 
@@ -901,26 +901,26 @@
 
         self._trading_end = trading_end
 
     @property
     def order_action_quota(self):
         """Gets the order_action_quota of this Contract.  # noqa: E501
 
-        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  # noqa: E501
+        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  This value is currently only calculated for EPEX based on the following formula:  `max{short_usage/short_l1, long_usage/long_l1}`  # noqa: E501
 
         :return: The order_action_quota of this Contract.  # noqa: E501
         :rtype: float
         """
         return self._order_action_quota
 
     @order_action_quota.setter
     def order_action_quota(self, order_action_quota):
         """Sets the order_action_quota of this Contract.
 
-        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  # noqa: E501
+        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  This value is currently only calculated for EPEX based on the following formula:  `max{short_usage/short_l1, long_usage/long_l1}`  # noqa: E501
 
         :param order_action_quota: The order_action_quota of this Contract.  # noqa: E501
         :type order_action_quota: float
         """
 
         self._order_action_quota = order_action_quota
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/contract_changed_event.py` & `powerbot_client-2.9.1/powerbot_client/models/contract_changed_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/contract_history_item.py` & `powerbot_client-2.9.1/powerbot_client/models/contract_history_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -257,95 +257,95 @@
 
         self._vwap = vwap
 
     @property
     def best_bid_price(self):
         """Gets the best_bid_price of this ContractHistoryItem.  # noqa: E501
 
-        The best bid's price at that time  # noqa: E501
+        The price of the best bid.  # noqa: E501
 
         :return: The best_bid_price of this ContractHistoryItem.  # noqa: E501
         :rtype: float
         """
         return self._best_bid_price
 
     @best_bid_price.setter
     def best_bid_price(self, best_bid_price):
         """Sets the best_bid_price of this ContractHistoryItem.
 
-        The best bid's price at that time  # noqa: E501
+        The price of the best bid.  # noqa: E501
 
         :param best_bid_price: The best_bid_price of this ContractHistoryItem.  # noqa: E501
         :type best_bid_price: float
         """
 
         self._best_bid_price = best_bid_price
 
     @property
     def best_bid_quantity(self):
         """Gets the best_bid_quantity of this ContractHistoryItem.  # noqa: E501
 
-        The best bid's quantity at that time  # noqa: E501
+        The quantity of the best bid.  # noqa: E501
 
         :return: The best_bid_quantity of this ContractHistoryItem.  # noqa: E501
         :rtype: float
         """
         return self._best_bid_quantity
 
     @best_bid_quantity.setter
     def best_bid_quantity(self, best_bid_quantity):
         """Sets the best_bid_quantity of this ContractHistoryItem.
 
-        The best bid's quantity at that time  # noqa: E501
+        The quantity of the best bid.  # noqa: E501
 
         :param best_bid_quantity: The best_bid_quantity of this ContractHistoryItem.  # noqa: E501
         :type best_bid_quantity: float
         """
 
         self._best_bid_quantity = best_bid_quantity
 
     @property
     def best_ask_price(self):
         """Gets the best_ask_price of this ContractHistoryItem.  # noqa: E501
 
-        The best ask's price at that time  # noqa: E501
+        The price of the best ask.  # noqa: E501
 
         :return: The best_ask_price of this ContractHistoryItem.  # noqa: E501
         :rtype: float
         """
         return self._best_ask_price
 
     @best_ask_price.setter
     def best_ask_price(self, best_ask_price):
         """Sets the best_ask_price of this ContractHistoryItem.
 
-        The best ask's price at that time  # noqa: E501
+        The price of the best ask.  # noqa: E501
 
         :param best_ask_price: The best_ask_price of this ContractHistoryItem.  # noqa: E501
         :type best_ask_price: float
         """
 
         self._best_ask_price = best_ask_price
 
     @property
     def best_ask_quantity(self):
         """Gets the best_ask_quantity of this ContractHistoryItem.  # noqa: E501
 
-        The best asks's quantity at that time  # noqa: E501
+        The quantity of the best ask.  # noqa: E501
 
         :return: The best_ask_quantity of this ContractHistoryItem.  # noqa: E501
         :rtype: float
         """
         return self._best_ask_quantity
 
     @best_ask_quantity.setter
     def best_ask_quantity(self, best_ask_quantity):
         """Sets the best_ask_quantity of this ContractHistoryItem.
 
-        The best asks's quantity at that time  # noqa: E501
+        The quantity of the best ask.  # noqa: E501
 
         :param best_ask_quantity: The best_ask_quantity of this ContractHistoryItem.  # noqa: E501
         :type best_ask_quantity: float
         """
 
         self._best_ask_quantity = best_ask_quantity
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/contract_item.py` & `powerbot_client-2.9.1/powerbot_client/models/contract_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/contract_reference.py` & `powerbot_client-2.9.1/powerbot_client/models/contract_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/contract_statistics.py` & `powerbot_client-2.9.1/powerbot_client/models/contract_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/contract_type.py` & `powerbot_client-2.9.1/powerbot_client/models/contract_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/credentials.py` & `powerbot_client-2.9.1/powerbot_client/models/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/delivery_area.py` & `powerbot_client-2.9.1/powerbot_client/models/delivery_area.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/delivery_area_state.py` & `powerbot_client-2.9.1/powerbot_client/models/delivery_area_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/error_response.py` & `powerbot_client-2.9.1/powerbot_client/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/exchange.py` & `powerbot_client-2.9.1/powerbot_client/models/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/exchange_cash_limit.py` & `powerbot_client-2.9.1/powerbot_client/models/exchange_cash_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/execution_instruction.py` & `powerbot_client-2.9.1/powerbot_client/models/execution_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/initialization.py` & `powerbot_client-2.9.1/powerbot_client/models/initialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/instance_heartbeat_status.py` & `powerbot_client-2.9.1/powerbot_client/models/instance_heartbeat_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/internal_trade.py` & `powerbot_client-2.9.1/powerbot_client/models/internal_trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/ip_allowlist_entry.py` & `powerbot_client-2.9.1/powerbot_client/models/ip_allowlist_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/limit_violation.py` & `powerbot_client-2.9.1/powerbot_client/models/limit_violation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/log_entry.py` & `powerbot_client-2.9.1/powerbot_client/models/log_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/log_entry_added.py` & `powerbot_client-2.9.1/powerbot_client/models/log_entry_added.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/market_mode.py` & `powerbot_client-2.9.1/powerbot_client/models/market_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/market_options.py` & `powerbot_client-2.9.1/powerbot_client/models/market_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -38,52 +38,57 @@
     """
     openapi_types = {
         'internal_trading': 'str',
         'internal_trading_cross_area': 'bool',
         'internal_trading_cross_area_lead_time': 'int',
         'internal_trading_include_external_orders': 'bool',
         'default_delivery_area_id': 'str',
-        'restrict_safe_mode': 'bool'
+        'restrict_safe_mode': 'bool',
+        'throttling_user_action': 'str'
     }
 
     attribute_map = {
         'internal_trading': 'internal_trading',
         'internal_trading_cross_area': 'internal_trading_cross_area',
         'internal_trading_cross_area_lead_time': 'internal_trading_cross_area_lead_time',
         'internal_trading_include_external_orders': 'internal_trading_include_external_orders',
         'default_delivery_area_id': 'default_delivery_area_id',
-        'restrict_safe_mode': 'restrict_safe_mode'
+        'restrict_safe_mode': 'restrict_safe_mode',
+        'throttling_user_action': 'throttling_user_action'
     }
 
-    def __init__(self, internal_trading=None, internal_trading_cross_area=None, internal_trading_cross_area_lead_time=None, internal_trading_include_external_orders=None, default_delivery_area_id=None, restrict_safe_mode=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, internal_trading=None, internal_trading_cross_area=None, internal_trading_cross_area_lead_time=None, internal_trading_include_external_orders=None, default_delivery_area_id=None, restrict_safe_mode=None, throttling_user_action=None, local_vars_configuration=None):  # noqa: E501
         """MarketOptions - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._internal_trading = None
         self._internal_trading_cross_area = None
         self._internal_trading_cross_area_lead_time = None
         self._internal_trading_include_external_orders = None
         self._default_delivery_area_id = None
         self._restrict_safe_mode = None
+        self._throttling_user_action = None
         self.discriminator = None
 
         if internal_trading is not None:
             self.internal_trading = internal_trading
         if internal_trading_cross_area is not None:
             self.internal_trading_cross_area = internal_trading_cross_area
         if internal_trading_cross_area_lead_time is not None:
             self.internal_trading_cross_area_lead_time = internal_trading_cross_area_lead_time
         if internal_trading_include_external_orders is not None:
             self.internal_trading_include_external_orders = internal_trading_include_external_orders
         if default_delivery_area_id is not None:
             self.default_delivery_area_id = default_delivery_area_id
         if restrict_safe_mode is not None:
             self.restrict_safe_mode = restrict_safe_mode
+        if throttling_user_action is not None:
+            self.throttling_user_action = throttling_user_action
 
     @property
     def internal_trading(self):
         """Gets the internal_trading of this MarketOptions.  # noqa: E501
 
 
         :return: The internal_trading of this MarketOptions.  # noqa: E501
@@ -222,14 +227,43 @@
 
         :param restrict_safe_mode: The restrict_safe_mode of this MarketOptions.  # noqa: E501
         :type restrict_safe_mode: bool
         """
 
         self._restrict_safe_mode = restrict_safe_mode
 
+    @property
+    def throttling_user_action(self):
+        """Gets the throttling_user_action of this MarketOptions.  # noqa: E501
+
+        This setting is only relevant for EPEX.  The behaviour of the exchange if you get suspended for violating your OMT limit. The default setting is `DO_NOTHING`.  **Warning**: To apply this setting, you will need to log out of the market and reconnect. In production, you will need to do this for both prod1 and prod2.  * `DO_NOTHING`       The exchange will take no further action after suspending you for OMT limit violations. * `HIBERNATE_ORDERS` The exchange will hibernate all user orders after suspending you for OMT limit violations.  # noqa: E501
+
+        :return: The throttling_user_action of this MarketOptions.  # noqa: E501
+        :rtype: str
+        """
+        return self._throttling_user_action
+
+    @throttling_user_action.setter
+    def throttling_user_action(self, throttling_user_action):
+        """Sets the throttling_user_action of this MarketOptions.
+
+        This setting is only relevant for EPEX.  The behaviour of the exchange if you get suspended for violating your OMT limit. The default setting is `DO_NOTHING`.  **Warning**: To apply this setting, you will need to log out of the market and reconnect. In production, you will need to do this for both prod1 and prod2.  * `DO_NOTHING`       The exchange will take no further action after suspending you for OMT limit violations. * `HIBERNATE_ORDERS` The exchange will hibernate all user orders after suspending you for OMT limit violations.  # noqa: E501
+
+        :param throttling_user_action: The throttling_user_action of this MarketOptions.  # noqa: E501
+        :type throttling_user_action: str
+        """
+        allowed_values = ["DO_NOTHING", "HIBERNATE_ORDERS"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and throttling_user_action not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `throttling_user_action` ({0}), must be one of {1}"  # noqa: E501
+                .format(throttling_user_action, allowed_values)
+            )
+
+        self._throttling_user_action = throttling_user_action
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/market_state.py` & `powerbot_client-2.9.1/powerbot_client/models/market_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/market_status.py` & `powerbot_client-2.9.1/powerbot_client/models/market_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -693,26 +693,26 @@
 
         self._mode = mode
 
     @property
     def order_action_quota(self):
         """Gets the order_action_quota of this MarketStatus.  # noqa: E501
 
-        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  # noqa: E501
+        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  This value is currently only calculated for EPEX based on the following formula:  `max{short_usage/short_l1, long_usage/long_l1}`  # noqa: E501
 
         :return: The order_action_quota of this MarketStatus.  # noqa: E501
         :rtype: float
         """
         return self._order_action_quota
 
     @order_action_quota.setter
     def order_action_quota(self, order_action_quota):
         """Sets the order_action_quota of this MarketStatus.
 
-        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  # noqa: E501
+        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  This value is currently only calculated for EPEX based on the following formula:  `max{short_usage/short_l1, long_usage/long_l1}`  # noqa: E501
 
         :param order_action_quota: The order_action_quota of this MarketStatus.  # noqa: E501
         :type order_action_quota: float
         """
 
         self._order_action_quota = order_action_quota
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/market_status_changed_event.py` & `powerbot_client-2.9.1/powerbot_client/models/market_status_changed_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/message.py` & `powerbot_client-2.9.1/powerbot_client/models/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/new_api_key.py` & `powerbot_client-2.9.1/powerbot_client/models/new_api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/new_internal_trade.py` & `powerbot_client-2.9.1/powerbot_client/models/new_internal_trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/new_portfolio.py` & `powerbot_client-2.9.1/powerbot_client/models/portfolio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from powerbot_client.configuration import Configuration
 
 
-class NewPortfolio(object):
+class Portfolio(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -37,167 +37,193 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'id': 'str',
         'name': 'str',
         'type': 'PortfolioType',
         'tenant_id': 'str',
+        'tenant_name': 'str',
         'risk_management': 'RiskManagementSettings'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'type': 'type',
         'tenant_id': 'tenant_id',
+        'tenant_name': 'tenant_name',
         'risk_management': 'risk_management'
     }
 
-    def __init__(self, id=None, name=None, type=None, tenant_id=None, risk_management=None, local_vars_configuration=None):  # noqa: E501
-        """NewPortfolio - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, id=None, name=None, type=None, tenant_id=None, tenant_name=None, risk_management=None, local_vars_configuration=None):  # noqa: E501
+        """Portfolio - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
         self._type = None
         self._tenant_id = None
+        self._tenant_name = None
         self._risk_management = None
         self.discriminator = None
 
         self.id = id
         self.name = name
-        if type is not None:
-            self.type = type
+        self.type = type
         self.tenant_id = tenant_id
-        self.risk_management = risk_management
+        self.tenant_name = tenant_name
+        if risk_management is not None:
+            self.risk_management = risk_management
 
     @property
     def id(self):
-        """Gets the id of this NewPortfolio.  # noqa: E501
+        """Gets the id of this Portfolio.  # noqa: E501
 
         A unique id (max 5 alphanumeric characters) of the portfolio  # noqa: E501
 
-        :return: The id of this NewPortfolio.  # noqa: E501
+        :return: The id of this Portfolio.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this NewPortfolio.
+        """Sets the id of this Portfolio.
 
         A unique id (max 5 alphanumeric characters) of the portfolio  # noqa: E501
 
-        :param id: The id of this NewPortfolio.  # noqa: E501
+        :param id: The id of this Portfolio.  # noqa: E501
         :type id: str
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 id is not None and len(id) > 5):
             raise ValueError("Invalid value for `id`, length must be less than or equal to `5`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and not re.search(r'[a-zA-Z0-9._-]{1,5}', id)):  # noqa: E501
-            raise ValueError(r"Invalid value for `id`, must be a follow pattern or equal to `/[a-zA-Z0-9._-]{1,5}/`")  # noqa: E501
 
         self._id = id
 
     @property
     def name(self):
-        """Gets the name of this NewPortfolio.  # noqa: E501
+        """Gets the name of this Portfolio.  # noqa: E501
 
         The name of the portfolio  # noqa: E501
 
-        :return: The name of this NewPortfolio.  # noqa: E501
+        :return: The name of this Portfolio.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this NewPortfolio.
+        """Sets the name of this Portfolio.
 
         The name of the portfolio  # noqa: E501
 
-        :param name: The name of this NewPortfolio.  # noqa: E501
+        :param name: The name of this Portfolio.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def type(self):
-        """Gets the type of this NewPortfolio.  # noqa: E501
+        """Gets the type of this Portfolio.  # noqa: E501
 
 
-        :return: The type of this NewPortfolio.  # noqa: E501
+        :return: The type of this Portfolio.  # noqa: E501
         :rtype: PortfolioType
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this NewPortfolio.
+        """Sets the type of this Portfolio.
 
 
-        :param type: The type of this NewPortfolio.  # noqa: E501
+        :param type: The type of this Portfolio.  # noqa: E501
         :type type: PortfolioType
         """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
         self._type = type
 
     @property
     def tenant_id(self):
-        """Gets the tenant_id of this NewPortfolio.  # noqa: E501
+        """Gets the tenant_id of this Portfolio.  # noqa: E501
 
         The tenant the portfolio belongs to  # noqa: E501
 
-        :return: The tenant_id of this NewPortfolio.  # noqa: E501
+        :return: The tenant_id of this Portfolio.  # noqa: E501
         :rtype: str
         """
         return self._tenant_id
 
     @tenant_id.setter
     def tenant_id(self, tenant_id):
-        """Sets the tenant_id of this NewPortfolio.
+        """Sets the tenant_id of this Portfolio.
 
         The tenant the portfolio belongs to  # noqa: E501
 
-        :param tenant_id: The tenant_id of this NewPortfolio.  # noqa: E501
+        :param tenant_id: The tenant_id of this Portfolio.  # noqa: E501
         :type tenant_id: str
         """
         if self.local_vars_configuration.client_side_validation and tenant_id is None:  # noqa: E501
             raise ValueError("Invalid value for `tenant_id`, must not be `None`")  # noqa: E501
 
         self._tenant_id = tenant_id
 
     @property
+    def tenant_name(self):
+        """Gets the tenant_name of this Portfolio.  # noqa: E501
+
+        The name of the tenant  # noqa: E501
+
+        :return: The tenant_name of this Portfolio.  # noqa: E501
+        :rtype: str
+        """
+        return self._tenant_name
+
+    @tenant_name.setter
+    def tenant_name(self, tenant_name):
+        """Sets the tenant_name of this Portfolio.
+
+        The name of the tenant  # noqa: E501
+
+        :param tenant_name: The tenant_name of this Portfolio.  # noqa: E501
+        :type tenant_name: str
+        """
+        if self.local_vars_configuration.client_side_validation and tenant_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `tenant_name`, must not be `None`")  # noqa: E501
+
+        self._tenant_name = tenant_name
+
+    @property
     def risk_management(self):
-        """Gets the risk_management of this NewPortfolio.  # noqa: E501
+        """Gets the risk_management of this Portfolio.  # noqa: E501
 
 
-        :return: The risk_management of this NewPortfolio.  # noqa: E501
+        :return: The risk_management of this Portfolio.  # noqa: E501
         :rtype: RiskManagementSettings
         """
         return self._risk_management
 
     @risk_management.setter
     def risk_management(self, risk_management):
-        """Sets the risk_management of this NewPortfolio.
+        """Sets the risk_management of this Portfolio.
 
 
-        :param risk_management: The risk_management of this NewPortfolio.  # noqa: E501
+        :param risk_management: The risk_management of this Portfolio.  # noqa: E501
         :type risk_management: RiskManagementSettings
         """
-        if self.local_vars_configuration.client_side_validation and risk_management is None:  # noqa: E501
-            raise ValueError("Invalid value for `risk_management`, must not be `None`")  # noqa: E501
 
         self._risk_management = risk_management
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -235,18 +261,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NewPortfolio):
+        if not isinstance(other, Portfolio):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, NewPortfolio):
+        if not isinstance(other, Portfolio):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/new_tenant.py` & `powerbot_client-2.9.1/powerbot_client/models/new_tenant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/notification.py` & `powerbot_client-2.9.1/powerbot_client/models/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/on_missing_heartbeat.py` & `powerbot_client-2.9.1/powerbot_client/models/on_missing_heartbeat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_action.py` & `powerbot_client-2.9.1/powerbot_client/models/order_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -51,16 +51,17 @@
     PEXE = "PEXE"
     IADD = "IADD"
     SERR = "SERR"
     SNAV = "SNAV"
     QADD = "QADD"
     AFEX = "AFEX"
     QPEX = "QPEX"
+    RLVI = "RLVI"
 
-    allowable_values = [UADD, UHIB, UMOD, UDEL, UREJ, AADD, AHIB, AMOD, ADEL, AREJ, SADD, SHIB, SMOD, SDEL, SREJ, FEXE, PEXE, IADD, SERR, SNAV, QADD, AFEX, QPEX]  # noqa: E501
+    allowable_values = [UADD, UHIB, UMOD, UDEL, UREJ, AADD, AHIB, AMOD, ADEL, AREJ, SADD, SHIB, SMOD, SDEL, SREJ, FEXE, PEXE, IADD, SERR, SNAV, QADD, AFEX, QPEX, RLVI]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_book.py` & `powerbot_client-2.9.1/powerbot_client/models/order_book.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_book_changed_event.py` & `powerbot_client-2.9.1/powerbot_client/models/order_book_changed_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_book_changes.py` & `powerbot_client-2.9.1/powerbot_client/models/order_book_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_book_entry.py` & `powerbot_client-2.9.1/powerbot_client/models/order_book_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_books.py` & `powerbot_client-2.9.1/powerbot_client/models/order_books.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_entry.py` & `powerbot_client-2.9.1/powerbot_client/models/order_entry.py`

 * *Files identical despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -602,26 +602,26 @@
 
         self._txt = txt
 
     @property
     def ppd(self):
         """Gets the ppd of this OrderEntry.  # noqa: E501
 
-        Peak price delta for Iceberg orders. * The ppd of buy orders must be smaller or equal than zero. * The ppd of sell orders must be greater or equal than zero. If it is omitted the system will assume a value of ?0,00?.  # noqa: E501
+        Peak price delta for Iceberg orders. * The ppd of buy orders must be smaller or equal than zero. * The ppd of sell orders must be greater or equal than zero. If it is omitted the system will assume a value of `0.00`.  # noqa: E501
 
         :return: The ppd of this OrderEntry.  # noqa: E501
         :rtype: float
         """
         return self._ppd
 
     @ppd.setter
     def ppd(self, ppd):
         """Sets the ppd of this OrderEntry.
 
-        Peak price delta for Iceberg orders. * The ppd of buy orders must be smaller or equal than zero. * The ppd of sell orders must be greater or equal than zero. If it is omitted the system will assume a value of ?0,00?.  # noqa: E501
+        Peak price delta for Iceberg orders. * The ppd of buy orders must be smaller or equal than zero. * The ppd of sell orders must be greater or equal than zero. If it is omitted the system will assume a value of `0.00`.  # noqa: E501
 
         :param ppd: The ppd of this OrderEntry.  # noqa: E501
         :type ppd: float
         """
 
         self._ppd = ppd
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_execution_restriction.py` & `powerbot_client-2.9.1/powerbot_client/models/order_execution_restriction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_modify.py` & `powerbot_client-2.9.1/powerbot_client/models/order_modify.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -342,26 +342,26 @@
 
         self._price = price
 
     @property
     def ppd(self):
         """Gets the ppd of this OrderModify.  # noqa: E501
 
-        Set this field if you want to update the Peak price delta for Iceberg orders. * The ppd of buy orders must be smaller or equal than zero. * The ppd of sell orders must be greater or equal than zero. If it is omitted the system will assume a value of ?0,00?.  # noqa: E501
+        Set this field if you want to update the Peak price delta for Iceberg orders. * The ppd of buy orders must be smaller or equal than zero. * The ppd of sell orders must be greater or equal than zero. If it is omitted the system will assume a value of `0.00`.  # noqa: E501
 
         :return: The ppd of this OrderModify.  # noqa: E501
         :rtype: float
         """
         return self._ppd
 
     @ppd.setter
     def ppd(self, ppd):
         """Sets the ppd of this OrderModify.
 
-        Set this field if you want to update the Peak price delta for Iceberg orders. * The ppd of buy orders must be smaller or equal than zero. * The ppd of sell orders must be greater or equal than zero. If it is omitted the system will assume a value of ?0,00?.  # noqa: E501
+        Set this field if you want to update the Peak price delta for Iceberg orders. * The ppd of buy orders must be smaller or equal than zero. * The ppd of sell orders must be greater or equal than zero. If it is omitted the system will assume a value of `0.00`.  # noqa: E501
 
         :param ppd: The ppd of this OrderModify.  # noqa: E501
         :type ppd: float
         """
 
         self._ppd = ppd
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_modify_item.py` & `powerbot_client-2.9.1/powerbot_client/models/order_modify_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_side.py` & `powerbot_client-2.9.1/powerbot_client/models/order_side.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_state.py` & `powerbot_client-2.9.1/powerbot_client/models/order_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/order_type.py` & `powerbot_client-2.9.1/powerbot_client/models/order_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/orders.py` & `powerbot_client-2.9.1/powerbot_client/models/orders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -34,49 +34,54 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'contract_id': 'str',
+        'product': 'str',
         'delivery_area': 'str',
         'sequence_number': 'int',
         'revision_no': 'int',
         'delta': 'bool',
         'bid': 'list[OrderBookEntry]',
         'ask': 'list[OrderBookEntry]'
     }
 
     attribute_map = {
         'contract_id': 'contract_id',
+        'product': 'product',
         'delivery_area': 'delivery_area',
         'sequence_number': 'sequence_number',
         'revision_no': 'revision_no',
         'delta': 'delta',
         'bid': 'bid',
         'ask': 'ask'
     }
 
-    def __init__(self, contract_id=None, delivery_area=None, sequence_number=None, revision_no=None, delta=None, bid=None, ask=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, contract_id=None, product=None, delivery_area=None, sequence_number=None, revision_no=None, delta=None, bid=None, ask=None, local_vars_configuration=None):  # noqa: E501
         """Orders - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._contract_id = None
+        self._product = None
         self._delivery_area = None
         self._sequence_number = None
         self._revision_no = None
         self._delta = None
         self._bid = None
         self._ask = None
         self.discriminator = None
 
         if contract_id is not None:
             self.contract_id = contract_id
+        if product is not None:
+            self.product = product
         if delivery_area is not None:
             self.delivery_area = delivery_area
         if sequence_number is not None:
             self.sequence_number = sequence_number
         if revision_no is not None:
             self.revision_no = revision_no
         if delta is not None:
@@ -104,14 +109,37 @@
         :param contract_id: The contract_id of this Orders.  # noqa: E501
         :type contract_id: str
         """
 
         self._contract_id = contract_id
 
     @property
+    def product(self):
+        """Gets the product of this Orders.  # noqa: E501
+
+        the contract's product  # noqa: E501
+
+        :return: The product of this Orders.  # noqa: E501
+        :rtype: str
+        """
+        return self._product
+
+    @product.setter
+    def product(self, product):
+        """Sets the product of this Orders.
+
+        the contract's product  # noqa: E501
+
+        :param product: The product of this Orders.  # noqa: E501
+        :type product: str
+        """
+
+        self._product = product
+
+    @property
     def delivery_area(self):
         """Gets the delivery_area of this Orders.  # noqa: E501
 
 
         :return: The delivery_area of this Orders.  # noqa: E501
         :rtype: str
         """
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/otr_limit.py` & `powerbot_client-2.9.1/powerbot_client/models/otr_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/own_order.py` & `powerbot_client-2.9.1/powerbot_client/models/own_order.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -58,15 +58,16 @@
         'display_quantity': 'float',
         'peak_price_delta': 'float',
         'action': 'OrderAction',
         'type': 'OrderType',
         'details': 'object',
         'user_code': 'str',
         'pre_arranged': 'bool',
-        'pre_arranged_acct': 'str'
+        'pre_arranged_acct': 'str',
+        'error_message': 'str'
     }
 
     attribute_map = {
         'order_id': 'order_id',
         'revision_no': 'revision_no',
         'api_timestamp': 'api_timestamp',
         'state': 'state',
@@ -87,18 +88,19 @@
         'display_quantity': 'display_quantity',
         'peak_price_delta': 'peak_price_delta',
         'action': 'action',
         'type': 'type',
         'details': 'details',
         'user_code': 'user_code',
         'pre_arranged': 'pre_arranged',
-        'pre_arranged_acct': 'pre_arranged_acct'
+        'pre_arranged_acct': 'pre_arranged_acct',
+        'error_message': 'error_message'
     }
 
-    def __init__(self, order_id=None, revision_no=None, api_timestamp=None, state=None, delivery_area=None, last_change_timestamp=None, buy=None, sell=None, side=None, contracts=None, delivery_start=None, delivery_end=None, cl_ordr_id=None, txt=None, portfolio_id=None, price=None, quantity=None, hidden_quantity=None, display_quantity=None, peak_price_delta=None, action=None, type=None, details=None, user_code=None, pre_arranged=None, pre_arranged_acct=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, order_id=None, revision_no=None, api_timestamp=None, state=None, delivery_area=None, last_change_timestamp=None, buy=None, sell=None, side=None, contracts=None, delivery_start=None, delivery_end=None, cl_ordr_id=None, txt=None, portfolio_id=None, price=None, quantity=None, hidden_quantity=None, display_quantity=None, peak_price_delta=None, action=None, type=None, details=None, user_code=None, pre_arranged=None, pre_arranged_acct=None, error_message=None, local_vars_configuration=None):  # noqa: E501
         """OwnOrder - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._order_id = None
         self._revision_no = None
@@ -122,14 +124,15 @@
         self._peak_price_delta = None
         self._action = None
         self._type = None
         self._details = None
         self._user_code = None
         self._pre_arranged = None
         self._pre_arranged_acct = None
+        self._error_message = None
         self.discriminator = None
 
         if order_id is not None:
             self.order_id = order_id
         if revision_no is not None:
             self.revision_no = revision_no
         if api_timestamp is not None:
@@ -171,14 +174,16 @@
             self.details = details
         if user_code is not None:
             self.user_code = user_code
         if pre_arranged is not None:
             self.pre_arranged = pre_arranged
         if pre_arranged_acct is not None:
             self.pre_arranged_acct = pre_arranged_acct
+        if error_message is not None:
+            self.error_message = error_message
 
     @property
     def order_id(self):
         """Gets the order_id of this OwnOrder.  # noqa: E501
 
         the unique id of the order. **Note** if you modify an order, the id will change!  # noqa: E501
 
@@ -762,14 +767,35 @@
 
         :param pre_arranged_acct: The pre_arranged_acct of this OwnOrder.  # noqa: E501
         :type pre_arranged_acct: str
         """
 
         self._pre_arranged_acct = pre_arranged_acct
 
+    @property
+    def error_message(self):
+        """Gets the error_message of this OwnOrder.  # noqa: E501
+
+
+        :return: The error_message of this OwnOrder.  # noqa: E501
+        :rtype: str
+        """
+        return self._error_message
+
+    @error_message.setter
+    def error_message(self, error_message):
+        """Sets the error_message of this OwnOrder.
+
+
+        :param error_message: The error_message of this OwnOrder.  # noqa: E501
+        :type error_message: str
+        """
+
+        self._error_message = error_message
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/own_order_changed_event.py` & `powerbot_client-2.9.1/powerbot_client/models/own_order_changed_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/own_order_changes.py` & `powerbot_client-2.9.1/powerbot_client/models/own_order_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/own_trade_changes.py` & `powerbot_client-2.9.1/powerbot_client/models/own_trade_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/portfolio.py` & `powerbot_client-2.9.1/powerbot_client/models/validation_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,188 +18,205 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from powerbot_client.configuration import Configuration
 
 
-class Portfolio(object):
+class ValidationSchema(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'str',
+        'type': 'ValidationSchemaType',
         'name': 'str',
-        'type': 'PortfolioType',
-        'tenant_id': 'str',
-        'tenant_name': 'str'
+        'version': 'str',
+        'description': 'str',
+        'parameters': 'object'
     }
 
     attribute_map = {
-        'id': 'id',
-        'name': 'name',
         'type': 'type',
-        'tenant_id': 'tenant_id',
-        'tenant_name': 'tenant_name'
+        'name': 'name',
+        'version': 'version',
+        'description': 'description',
+        'parameters': 'parameters'
     }
 
-    def __init__(self, id=None, name=None, type=None, tenant_id=None, tenant_name=None, local_vars_configuration=None):  # noqa: E501
-        """Portfolio - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, type=None, name=None, version=None, description=None, parameters=None, local_vars_configuration=None):  # noqa: E501
+        """ValidationSchema - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._name = None
         self._type = None
-        self._tenant_id = None
-        self._tenant_name = None
+        self._name = None
+        self._version = None
+        self._description = None
+        self._parameters = None
         self.discriminator = None
 
-        self.id = id
-        self.name = name
         self.type = type
-        self.tenant_id = tenant_id
-        self.tenant_name = tenant_name
+        self.name = name
+        self.version = version
+        if description is not None:
+            self.description = description
+        self.parameters = parameters
 
     @property
-    def id(self):
-        """Gets the id of this Portfolio.  # noqa: E501
+    def type(self):
+        """Gets the type of this ValidationSchema.  # noqa: E501
 
-        A unique id (max 5 alphanumeric characters) of the portfolio  # noqa: E501
 
-        :return: The id of this Portfolio.  # noqa: E501
-        :rtype: str
+        :return: The type of this ValidationSchema.  # noqa: E501
+        :rtype: ValidationSchemaType
         """
-        return self._id
+        return self._type
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this Portfolio.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this ValidationSchema.
 
-        A unique id (max 5 alphanumeric characters) of the portfolio  # noqa: E501
 
-        :param id: The id of this Portfolio.  # noqa: E501
-        :type id: str
+        :param type: The type of this ValidationSchema.  # noqa: E501
+        :type type: ValidationSchemaType
         """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and len(id) > 5):
-            raise ValueError("Invalid value for `id`, length must be less than or equal to `5`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
-        self._id = id
+        self._type = type
 
     @property
     def name(self):
-        """Gets the name of this Portfolio.  # noqa: E501
+        """Gets the name of this ValidationSchema.  # noqa: E501
 
-        The name of the portfolio  # noqa: E501
+        The name of the schema.  # noqa: E501
 
-        :return: The name of this Portfolio.  # noqa: E501
+        :return: The name of this ValidationSchema.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this Portfolio.
+        """Sets the name of this ValidationSchema.
 
-        The name of the portfolio  # noqa: E501
+        The name of the schema.  # noqa: E501
 
-        :param name: The name of this Portfolio.  # noqa: E501
+        :param name: The name of this ValidationSchema.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) > 255):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `255`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and not re.search(r'[a-zA-Z0-9._\-]+', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/[a-zA-Z0-9._\-]+/`")  # noqa: E501
 
         self._name = name
 
     @property
-    def type(self):
-        """Gets the type of this Portfolio.  # noqa: E501
+    def version(self):
+        """Gets the version of this ValidationSchema.  # noqa: E501
 
+        The version of the related algorithm that uses this schema.  # noqa: E501
 
-        :return: The type of this Portfolio.  # noqa: E501
-        :rtype: PortfolioType
+        :return: The version of this ValidationSchema.  # noqa: E501
+        :rtype: str
         """
-        return self._type
+        return self._version
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this Portfolio.
+    @version.setter
+    def version(self, version):
+        """Sets the version of this ValidationSchema.
 
+        The version of the related algorithm that uses this schema.  # noqa: E501
 
-        :param type: The type of this Portfolio.  # noqa: E501
-        :type type: PortfolioType
+        :param version: The version of this ValidationSchema.  # noqa: E501
+        :type version: str
         """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and version is None:  # noqa: E501
+            raise ValueError("Invalid value for `version`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                version is not None and len(version) > 255):
+            raise ValueError("Invalid value for `version`, length must be less than or equal to `255`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                version is not None and len(version) < 1):
+            raise ValueError("Invalid value for `version`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                version is not None and not re.search(r'[a-zA-Z0-9._\-]+', version)):  # noqa: E501
+            raise ValueError(r"Invalid value for `version`, must be a follow pattern or equal to `/[a-zA-Z0-9._\-]+/`")  # noqa: E501
 
-        self._type = type
+        self._version = version
 
     @property
-    def tenant_id(self):
-        """Gets the tenant_id of this Portfolio.  # noqa: E501
+    def description(self):
+        """Gets the description of this ValidationSchema.  # noqa: E501
 
-        The tenant the portfolio belongs to  # noqa: E501
+        A description text detailing information regarding the schema.  # noqa: E501
 
-        :return: The tenant_id of this Portfolio.  # noqa: E501
+        :return: The description of this ValidationSchema.  # noqa: E501
         :rtype: str
         """
-        return self._tenant_id
+        return self._description
 
-    @tenant_id.setter
-    def tenant_id(self, tenant_id):
-        """Sets the tenant_id of this Portfolio.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this ValidationSchema.
 
-        The tenant the portfolio belongs to  # noqa: E501
+        A description text detailing information regarding the schema.  # noqa: E501
 
-        :param tenant_id: The tenant_id of this Portfolio.  # noqa: E501
-        :type tenant_id: str
+        :param description: The description of this ValidationSchema.  # noqa: E501
+        :type description: str
         """
-        if self.local_vars_configuration.client_side_validation and tenant_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `tenant_id`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                description is not None and len(description) > 1024):
+            raise ValueError("Invalid value for `description`, length must be less than or equal to `1024`")  # noqa: E501
 
-        self._tenant_id = tenant_id
+        self._description = description
 
     @property
-    def tenant_name(self):
-        """Gets the tenant_name of this Portfolio.  # noqa: E501
+    def parameters(self):
+        """Gets the parameters of this ValidationSchema.  # noqa: E501
 
-        The name of the tenant  # noqa: E501
+        The contents of the schema  # noqa: E501
 
-        :return: The tenant_name of this Portfolio.  # noqa: E501
-        :rtype: str
+        :return: The parameters of this ValidationSchema.  # noqa: E501
+        :rtype: object
         """
-        return self._tenant_name
+        return self._parameters
 
-    @tenant_name.setter
-    def tenant_name(self, tenant_name):
-        """Sets the tenant_name of this Portfolio.
+    @parameters.setter
+    def parameters(self, parameters):
+        """Sets the parameters of this ValidationSchema.
 
-        The name of the tenant  # noqa: E501
+        The contents of the schema  # noqa: E501
 
-        :param tenant_name: The tenant_name of this Portfolio.  # noqa: E501
-        :type tenant_name: str
+        :param parameters: The parameters of this ValidationSchema.  # noqa: E501
+        :type parameters: object
         """
-        if self.local_vars_configuration.client_side_validation and tenant_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `tenant_name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and parameters is None:  # noqa: E501
+            raise ValueError("Invalid value for `parameters`, must not be `None`")  # noqa: E501
 
-        self._tenant_name = tenant_name
+        self._parameters = parameters
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -235,18 +252,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Portfolio):
+        if not isinstance(other, ValidationSchema):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Portfolio):
+        if not isinstance(other, ValidationSchema):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/portfolio_changes.py` & `powerbot_client-2.9.1/powerbot_client/models/portfolio_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/portfolio_information.py` & `powerbot_client-2.9.1/powerbot_client/models/portfolio_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -530,26 +530,26 @@
 
         self._buy_abs_pos = buy_abs_pos
 
     @property
     def order_action_quota(self):
         """Gets the order_action_quota of this PortfolioInformation.  # noqa: E501
 
-        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  # noqa: E501
+        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  This value is currently only calculated for EPEX based on the following formula:  `max{short_usage/short_l1, long_usage/long_l1}`  # noqa: E501
 
         :return: The order_action_quota of this PortfolioInformation.  # noqa: E501
         :rtype: float
         """
         return self._order_action_quota
 
     @order_action_quota.setter
     def order_action_quota(self, order_action_quota):
         """Sets the order_action_quota of this PortfolioInformation.
 
-        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  # noqa: E501
+        The percentage (0.0 - 1.0) of consumed order entry/modification quota calculated depending on the underlying exchange.  This value is currently only calculated for EPEX based on the following formula:  `max{short_usage/short_l1, long_usage/long_l1}`  # noqa: E501
 
         :param order_action_quota: The order_action_quota of this PortfolioInformation.  # noqa: E501
         :type order_action_quota: float
         """
 
         self._order_action_quota = order_action_quota
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/portfolio_type.py` & `powerbot_client-2.9.1/powerbot_client/models/portfolio_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/position_limit.py` & `powerbot_client-2.9.1/powerbot_client/models/position_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/product_information.py` & `powerbot_client-2.9.1/powerbot_client/models/product_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/public_trade.py` & `powerbot_client-2.9.1/powerbot_client/models/public_trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/public_trade_changes.py` & `powerbot_client-2.9.1/powerbot_client/models/public_trade_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/report.py` & `powerbot_client-2.9.1/powerbot_client/models/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/report_element.py` & `powerbot_client-2.9.1/powerbot_client/models/report_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/risk_management_settings.py` & `powerbot_client-2.9.1/powerbot_client/models/risk_management_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/risk_settings_and_portfolio_information.py` & `powerbot_client-2.9.1/powerbot_client/models/risk_settings_and_portfolio_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/severity.py` & `powerbot_client-2.9.1/powerbot_client/models/severity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/signal.py` & `powerbot_client-2.9.1/powerbot_client/models/signal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -44,14 +44,15 @@
         'delivery_start': 'datetime',
         'delivery_end': 'datetime',
         'delivery_areas': 'list[str]',
         'portfolio_ids': 'list[str]',
         'tenant_id': 'str',
         'position_short': 'float',
         'position_long': 'float',
+        'locked': 'bool',
         'value': 'object'
     }
 
     attribute_map = {
         'id': 'id',
         'source': 'source',
         'received_at': 'received_at',
@@ -59,18 +60,19 @@
         'delivery_start': 'delivery_start',
         'delivery_end': 'delivery_end',
         'delivery_areas': 'delivery_areas',
         'portfolio_ids': 'portfolio_ids',
         'tenant_id': 'tenant_id',
         'position_short': 'position_short',
         'position_long': 'position_long',
+        'locked': 'locked',
         'value': 'value'
     }
 
-    def __init__(self, id=None, source=None, received_at=None, revision=None, delivery_start=None, delivery_end=None, delivery_areas=None, portfolio_ids=None, tenant_id=None, position_short=None, position_long=None, value=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, source=None, received_at=None, revision=None, delivery_start=None, delivery_end=None, delivery_areas=None, portfolio_ids=None, tenant_id=None, position_short=None, position_long=None, locked=None, value=None, local_vars_configuration=None):  # noqa: E501
         """Signal - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._source = None
@@ -79,14 +81,15 @@
         self._delivery_start = None
         self._delivery_end = None
         self._delivery_areas = None
         self._portfolio_ids = None
         self._tenant_id = None
         self._position_short = None
         self._position_long = None
+        self._locked = None
         self._value = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if source is not None:
             self.source = source
@@ -104,14 +107,16 @@
             self.portfolio_ids = portfolio_ids
         if tenant_id is not None:
             self.tenant_id = tenant_id
         if position_short is not None:
             self.position_short = position_short
         if position_long is not None:
             self.position_long = position_long
+        if locked is not None:
+            self.locked = locked
         if value is not None:
             self.value = value
 
     @property
     def id(self):
         """Gets the id of this Signal.  # noqa: E501
 
@@ -359,14 +364,37 @@
         :param position_long: The position_long of this Signal.  # noqa: E501
         :type position_long: float
         """
 
         self._position_long = position_long
 
     @property
+    def locked(self):
+        """Gets the locked of this Signal.  # noqa: E501
+
+        Locked signals can not be modified, unless the `ignore_lock` parameter is set to `true`.  # noqa: E501
+
+        :return: The locked of this Signal.  # noqa: E501
+        :rtype: bool
+        """
+        return self._locked
+
+    @locked.setter
+    def locked(self, locked):
+        """Sets the locked of this Signal.
+
+        Locked signals can not be modified, unless the `ignore_lock` parameter is set to `true`.  # noqa: E501
+
+        :param locked: The locked of this Signal.  # noqa: E501
+        :type locked: bool
+        """
+
+        self._locked = locked
+
+    @property
     def value(self):
         """Gets the value of this Signal.  # noqa: E501
 
         The custom content of the signal, posted as key/value pairs  # noqa: E501
 
         :return: The value of this Signal.  # noqa: E501
         :rtype: object
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/signal_changes.py` & `powerbot_client-2.9.1/powerbot_client/models/signal_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/subscription_endpoint.py` & `powerbot_client-2.9.1/powerbot_client/models/subscription_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/tenant.py` & `powerbot_client-2.9.1/powerbot_client/models/tenant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/text_matching_mode.py` & `powerbot_client-2.9.1/powerbot_client/models/text_matching_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/trade.py` & `powerbot_client-2.9.1/powerbot_client/models/trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/trade_changed_event.py` & `powerbot_client-2.9.1/powerbot_client/models/trade_changed_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/trade_state.py` & `powerbot_client-2.9.1/powerbot_client/models/trade_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/trading_area.py` & `powerbot_client-2.9.1/powerbot_client/models/trading_area.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/update_algo_setup.py` & `powerbot_client-2.9.1/powerbot_client/models/update_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,180 +18,133 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from powerbot_client.configuration import Configuration
 
 
-class UpdateAlgoSetup(object):
+class UpdateStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        'description': 'str',
-        'require_heartbeat_every_seconds': 'int',
-        'on_missing_heartbeat': 'OnMissingHeartbeat',
-        'image': 'str'
+        'order_mod_type': 'str',
+        'incl_pre_arranged': 'bool',
+        'prod_name': 'list[str]'
     }
 
     attribute_map = {
-        'name': 'name',
-        'description': 'description',
-        'require_heartbeat_every_seconds': 'require_heartbeat_every_seconds',
-        'on_missing_heartbeat': 'on_missing_heartbeat',
-        'image': 'image'
+        'order_mod_type': 'orderModType',
+        'incl_pre_arranged': 'inclPreArranged',
+        'prod_name': 'prodName'
     }
 
-    def __init__(self, name=None, description=None, require_heartbeat_every_seconds=None, on_missing_heartbeat=None, image=None, local_vars_configuration=None):  # noqa: E501
-        """UpdateAlgoSetup - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, order_mod_type=None, incl_pre_arranged=False, prod_name=None, local_vars_configuration=None):  # noqa: E501
+        """UpdateStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._description = None
-        self._require_heartbeat_every_seconds = None
-        self._on_missing_heartbeat = None
-        self._image = None
+        self._order_mod_type = None
+        self._incl_pre_arranged = None
+        self._prod_name = None
         self.discriminator = None
 
-        if name is not None:
-            self.name = name
-        if description is not None:
-            self.description = description
-        if require_heartbeat_every_seconds is not None:
-            self.require_heartbeat_every_seconds = require_heartbeat_every_seconds
-        if on_missing_heartbeat is not None:
-            self.on_missing_heartbeat = on_missing_heartbeat
-        if image is not None:
-            self.image = image
+        self.order_mod_type = order_mod_type
+        if incl_pre_arranged is not None:
+            self.incl_pre_arranged = incl_pre_arranged
+        if prod_name is not None:
+            self.prod_name = prod_name
 
     @property
-    def name(self):
-        """Gets the name of this UpdateAlgoSetup.  # noqa: E501
+    def order_mod_type(self):
+        """Gets the order_mod_type of this UpdateStatus.  # noqa: E501
 
-        The name of the algorithm  # noqa: E501
+        * ACTI: Activates the order. Ignored if already active. * DEAC: Deactivates (hibernates) the order. Hibernated orders are removed from the order book but are still available for modification or activation in the own orders list. * DELE: Delete the order  # noqa: E501
 
-        :return: The name of this UpdateAlgoSetup.  # noqa: E501
+        :return: The order_mod_type of this UpdateStatus.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._order_mod_type
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this UpdateAlgoSetup.
+    @order_mod_type.setter
+    def order_mod_type(self, order_mod_type):
+        """Sets the order_mod_type of this UpdateStatus.
+
+        * ACTI: Activates the order. Ignored if already active. * DEAC: Deactivates (hibernates) the order. Hibernated orders are removed from the order book but are still available for modification or activation in the own orders list. * DELE: Delete the order  # noqa: E501
+
+        :param order_mod_type: The order_mod_type of this UpdateStatus.  # noqa: E501
+        :type order_mod_type: str
+        """
+        if self.local_vars_configuration.client_side_validation and order_mod_type is None:  # noqa: E501
+            raise ValueError("Invalid value for `order_mod_type`, must not be `None`")  # noqa: E501
+        allowed_values = ["ACTI", "DEAC", "DELE"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and order_mod_type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `order_mod_type` ({0}), must be one of {1}"  # noqa: E501
+                .format(order_mod_type, allowed_values)
+            )
 
-        The name of the algorithm  # noqa: E501
-
-        :param name: The name of this UpdateAlgoSetup.  # noqa: E501
-        :type name: str
-        """
-
-        self._name = name
+        self._order_mod_type = order_mod_type
 
     @property
-    def description(self):
-        """Gets the description of this UpdateAlgoSetup.  # noqa: E501
+    def incl_pre_arranged(self):
+        """Gets the incl_pre_arranged of this UpdateStatus.  # noqa: E501
 
-        A short description of the algorithm  # noqa: E501
+        Include pre-arranged orders  # noqa: E501
 
-        :return: The description of this UpdateAlgoSetup.  # noqa: E501
-        :rtype: str
+        :return: The incl_pre_arranged of this UpdateStatus.  # noqa: E501
+        :rtype: bool
         """
-        return self._description
+        return self._incl_pre_arranged
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this UpdateAlgoSetup.
+    @incl_pre_arranged.setter
+    def incl_pre_arranged(self, incl_pre_arranged):
+        """Sets the incl_pre_arranged of this UpdateStatus.
 
-        A short description of the algorithm  # noqa: E501
+        Include pre-arranged orders  # noqa: E501
 
-        :param description: The description of this UpdateAlgoSetup.  # noqa: E501
-        :type description: str
+        :param incl_pre_arranged: The incl_pre_arranged of this UpdateStatus.  # noqa: E501
+        :type incl_pre_arranged: bool
         """
 
-        self._description = description
+        self._incl_pre_arranged = incl_pre_arranged
 
     @property
-    def require_heartbeat_every_seconds(self):
-        """Gets the require_heartbeat_every_seconds of this UpdateAlgoSetup.  # noqa: E501
-
-        Specifies how often the algorithm requires a heartbeat via POST/.../heartbeat. Must be > 0  # noqa: E501
-
-        :return: The require_heartbeat_every_seconds of this UpdateAlgoSetup.  # noqa: E501
-        :rtype: int
-        """
-        return self._require_heartbeat_every_seconds
+    def prod_name(self):
+        """Gets the prod_name of this UpdateStatus.  # noqa: E501
 
-    @require_heartbeat_every_seconds.setter
-    def require_heartbeat_every_seconds(self, require_heartbeat_every_seconds):
-        """Sets the require_heartbeat_every_seconds of this UpdateAlgoSetup.
-
-        Specifies how often the algorithm requires a heartbeat via POST/.../heartbeat. Must be > 0  # noqa: E501
-
-        :param require_heartbeat_every_seconds: The require_heartbeat_every_seconds of this UpdateAlgoSetup.  # noqa: E501
-        :type require_heartbeat_every_seconds: int
-        """
-
-        self._require_heartbeat_every_seconds = require_heartbeat_every_seconds
-
-    @property
-    def on_missing_heartbeat(self):
-        """Gets the on_missing_heartbeat of this UpdateAlgoSetup.  # noqa: E501
+        Restrict the request to the given product(s)  # noqa: E501
 
-
-        :return: The on_missing_heartbeat of this UpdateAlgoSetup.  # noqa: E501
-        :rtype: OnMissingHeartbeat
-        """
-        return self._on_missing_heartbeat
-
-    @on_missing_heartbeat.setter
-    def on_missing_heartbeat(self, on_missing_heartbeat):
-        """Sets the on_missing_heartbeat of this UpdateAlgoSetup.
-
-
-        :param on_missing_heartbeat: The on_missing_heartbeat of this UpdateAlgoSetup.  # noqa: E501
-        :type on_missing_heartbeat: OnMissingHeartbeat
-        """
-
-        self._on_missing_heartbeat = on_missing_heartbeat
-
-    @property
-    def image(self):
-        """Gets the image of this UpdateAlgoSetup.  # noqa: E501
-
-        The image of the algorithm, this can be any valid docker image name with a tag. The tag can not be \"latest\" to avoid accidental upgrades.  # noqa: E501
-
-        :return: The image of this UpdateAlgoSetup.  # noqa: E501
-        :rtype: str
+        :return: The prod_name of this UpdateStatus.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._image
+        return self._prod_name
 
-    @image.setter
-    def image(self, image):
-        """Sets the image of this UpdateAlgoSetup.
+    @prod_name.setter
+    def prod_name(self, prod_name):
+        """Sets the prod_name of this UpdateStatus.
 
-        The image of the algorithm, this can be any valid docker image name with a tag. The tag can not be \"latest\" to avoid accidental upgrades.  # noqa: E501
+        Restrict the request to the given product(s)  # noqa: E501
 
-        :param image: The image of this UpdateAlgoSetup.  # noqa: E501
-        :type image: str
+        :param prod_name: The prod_name of this UpdateStatus.  # noqa: E501
+        :type prod_name: list[str]
         """
 
-        self._image = image
+        self._prod_name = prod_name
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -227,18 +180,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UpdateAlgoSetup):
+        if not isinstance(other, UpdateStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, UpdateAlgoSetup):
+        if not isinstance(other, UpdateStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/updated_api_key.py` & `powerbot_client-2.9.1/powerbot_client/models/updated_api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/updated_portfolio.py` & `powerbot_client-2.9.1/powerbot_client/models/updated_portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/updated_tenant.py` & `powerbot_client-2.9.1/powerbot_client/models/updated_tenant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/models/validity_restriction.py` & `powerbot_client-2.9.1/powerbot_client/models/validity_restriction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `powerbot_client-2.8.0/powerbot_client/rest.py` & `powerbot_client-2.9.1/powerbot_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PowerBot - Webservice for algotrading
 
     # TERMS AND CONDITIONS The PowerBot system provides B2B services for trading at intraday power markets. By using the PowerBot service, each user agrees to the terms and conditions of this licence: 1. The user confirms that they are familiar with the exchanges trading system and all relevant rules, is professionally qualified and in possession of a trading license for the relevant exchange. 2. The user will comply with the exchanges market rules (e.g. [EPEX Spot Market Rules](https://www.epexspot.com/en/downloads#rules-fees-processes) or [Nord Pool Market Rules](https://www.nordpoolgroup.com/trading/Rules-and-regulations/)) and will not endanger the exchange system at any time with heavy load from trading algorithms or by other use. 3. The user is aware of OTR (order-to-trade) limits and other limits imposed by the exchange. 4. The user is solely liable for actions resulting from the use of PowerBot.   # INTRODUCTION PowerBot is a web-based software service enabling algorithmic trading on intraday power exchanges such as EPEX, Nord Pool, HUPX, BSP Southpool or TGE. The service is straightforward to integrate in an existing software environment and provides a variety of programming interfaces for development of individual trading algorithms and software tools. Besides enabling fully automated intraday trading, it can be used to create tools for human traders providing relevant information and trading opportunities or can be integrated in existing software tools. For further details see https://www.powerbot-trading.com  ## Knowledge Base In addition to this API guide, please find the documentation at https://docs.powerbot-trading.com - the password will be provided by the PowerBot team. If not, please reach out to us at support@powerbot-trading.com  ## Endpoints The PowerBot service is available at the following REST endpoints:  | Instance                | Base URL for REST Endpoints                                           | |-------------------------|-----------------------------------------------------------------------| | Test (EPEX)             | https://staging.powerbot-trading.com/playground/epex/v2/api           | | Test (Nord Pool)        | https://staging.powerbot-trading.com/playground/nordpool/v2/api       | | Test (HUPX)             | https://staging.powerbot-trading.com/playground/hupx/v2/api           | | Test (BSP Southpool)    | https://staging.powerbot-trading.com/playground/southpool/v2/api      | | Test (TGE)              | https://staging.powerbot-trading.com/playground/tge/v2/api            | | Test (IBEX)             | https://staging.powerbot-trading.com/playground/ibex/v2/api           | | Test (CROPEX)           | https://staging.powerbot-trading.com/playground/cropex/v2/api         | | Staging, Production     | Provided on request                                                   |  Access to endpoints is secured via an API Key, which needs to be passed as an \"api_key\" header in each request.   Notes on API Keys:  * API keys are specific to Test, Staging or Production.  * API keys are generated by the system administrator and need to be requested.  ## How to generate API clients (libraries) This OpenAPI specification can be used to generate API clients (programming libraries) for a wide range of programming languages using tools like [OpenAPI Generator](https://openapi-generator.tech/). A detailed guide can be found in the [knowledge base](https://docs.powerbot-trading.com/articles/getting-started/generating-clients/).  ## PowerBot Python client For Python, a ready-made client is also available on PyPI and can be downloaded locally via:  ```shell   pip install powerbot-client ```  ## Errors The API uses standard HTTP status codes to indicate the success or failure of the API call. The body of the response will be in JSON format as follows:  ``` {   \"message\": \"... an error message ...\" } ```  ## Paging The API uses offset and limit parameters for paged operations. An X-Total-Count header is added to responses to indicate the total number of items in a paged response.  ## Cross-Origin Resource Sharing This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with  [W3C spec](https://www.w3.org/TR/cors/). This allows cross-domain communication from the browser. All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.  ## API Rate Limiting The API limits the number of concurrent calls to 50 - when that limit is reached, the client will receive 503 http status codes (service unavailable) with the following text:  ``` {   \"message\": \"API rate limit exceeded\" } ``` Clients should ensure that they stay within the limit for concurrent API calls.    ## Additional code samples Additional information and code samples demonstrating the use of the API can be found at https://github.com/powerbot-trading.  # noqa: E501
 
-    The version of the OpenAPI document: 2.8.0
+    The version of the OpenAPI document: 2.9.1
     Contact: office@powerbot-trading.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `powerbot_client-2.8.0/powerbot_client.egg-info/SOURCES.txt` & `powerbot_client-2.9.1/powerbot_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 powerbot_client/api/contract_api.py
 powerbot_client/api/logs_api.py
 powerbot_client/api/market_api.py
 powerbot_client/api/messages_api.py
 powerbot_client/api/orders_api.py
 powerbot_client/api/portfolios_api.py
 powerbot_client/api/report_api.py
+powerbot_client/api/schema_api.py
 powerbot_client/api/settings_api.py
 powerbot_client/api/signals_api.py
 powerbot_client/api/subscriptions_api.py
 powerbot_client/api/tenants_api.py
 powerbot_client/api/trades_api.py
 powerbot_client/models/__init__.py
 powerbot_client/models/aggressor_indicator.py
@@ -41,15 +42,14 @@
 powerbot_client/models/algo_status.py
 powerbot_client/models/api_key.py
 powerbot_client/models/api_key_details.py
 powerbot_client/models/api_key_portfolio_update.py
 powerbot_client/models/api_key_type.py
 powerbot_client/models/atc_status.py
 powerbot_client/models/audit_log_entry.py
-powerbot_client/models/available_portfolio.py
 powerbot_client/models/bulk_contract_statistics.py
 powerbot_client/models/bulk_signal.py
 powerbot_client/models/bulk_signal_response.py
 powerbot_client/models/capacity.py
 powerbot_client/models/capacity_changes.py
 powerbot_client/models/cash_limit.py
 powerbot_client/models/changed_credentials.py
@@ -87,14 +87,15 @@
 powerbot_client/models/notification.py
 powerbot_client/models/on_missing_heartbeat.py
 powerbot_client/models/order_action.py
 powerbot_client/models/order_book.py
 powerbot_client/models/order_book_changed_event.py
 powerbot_client/models/order_book_changes.py
 powerbot_client/models/order_book_entry.py
+powerbot_client/models/order_book_group.py
 powerbot_client/models/order_books.py
 powerbot_client/models/order_entry.py
 powerbot_client/models/order_execution_restriction.py
 powerbot_client/models/order_modify.py
 powerbot_client/models/order_modify_item.py
 powerbot_client/models/order_side.py
 powerbot_client/models/order_state.py
@@ -109,14 +110,15 @@
 powerbot_client/models/portfolio_changes.py
 powerbot_client/models/portfolio_information.py
 powerbot_client/models/portfolio_type.py
 powerbot_client/models/position_limit.py
 powerbot_client/models/product_information.py
 powerbot_client/models/public_trade.py
 powerbot_client/models/public_trade_changes.py
+powerbot_client/models/related_contract.py
 powerbot_client/models/report.py
 powerbot_client/models/report_element.py
 powerbot_client/models/risk_management_settings.py
 powerbot_client/models/risk_settings_and_portfolio_information.py
 powerbot_client/models/severity.py
 powerbot_client/models/signal.py
 powerbot_client/models/signal_changes.py
@@ -128,8 +130,10 @@
 powerbot_client/models/trade_state.py
 powerbot_client/models/trading_area.py
 powerbot_client/models/update_algo_setup.py
 powerbot_client/models/update_status.py
 powerbot_client/models/updated_api_key.py
 powerbot_client/models/updated_portfolio.py
 powerbot_client/models/updated_tenant.py
+powerbot_client/models/validation_schema.py
+powerbot_client/models/validation_schema_type.py
 powerbot_client/models/validity_restriction.py
```

