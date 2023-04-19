# Comparing `tmp/yookassa_async-0.1.2.tar.gz` & `tmp/yookassa_async-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yookassa_async-0.1.2.tar", max compression
+gzip compressed data, was "yookassa_async-0.1.3.tar", max compression
```

## Comparing `yookassa_async-0.1.2.tar` & `yookassa_async-0.1.3.tar`

### file list

```diff
@@ -1,155 +1,155 @@
--rw-r--r--   0        0        0     1101 2023-04-18 22:47:40.640643 yookassa_async-0.1.2/LICENSE
--rw-r--r--   0        0        0      535 2023-04-19 02:23:34.248623 yookassa_async-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6337 2023-04-18 22:57:38.445440 yookassa_async-0.1.2/README.md
--rw-r--r--   0        0        0      481 2023-04-18 22:55:43.289005 yookassa_async-0.1.2/yookassa_async/yookassa/__init__.py
--rw-r--r--   0        0        0     5188 2023-04-18 22:47:40.649618 yookassa_async-0.1.2/yookassa_async/yookassa/client.py
--rw-r--r--   0        0        0     2620 2023-04-18 22:47:40.649618 yookassa_async-0.1.2/yookassa_async/yookassa/configuration.py
--rw-r--r--   0        0        0     1915 2023-04-18 22:47:40.650617 yookassa_async-0.1.2/yookassa_async/yookassa/deal.py
--rw-r--r--   0        0        0       90 2023-04-18 22:47:40.651614 yookassa_async-0.1.2/yookassa_async/yookassa/domain/__init__.py
--rw-r--r--   0        0        0      873 2023-04-18 22:47:40.651614 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/__init__.py
--rw-r--r--   0        0        0     1529 2023-04-18 22:47:40.652611 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/base_object.py
--rw-r--r--   0        0        0      571 2023-04-18 22:47:40.652611 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/confirmation_type.py
--rw-r--r--   0        0        0      404 2023-04-18 22:47:40.653608 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/context.py
--rw-r--r--   0        0        0      353 2023-04-18 22:47:40.653608 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/data_context.py
--rw-r--r--   0        0        0      596 2023-04-18 22:47:40.654633 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/http_verb.py
--rw-r--r--   0        0        0     1502 2023-04-18 22:47:40.655600 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/payment_method_type.py
--rw-r--r--   0        0        0      582 2023-04-18 22:47:40.655600 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/receipt_type.py
--rw-r--r--   0        0        0      400 2023-04-18 22:47:40.655600 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/request_object.py
--rw-r--r--   0        0        0      302 2023-04-18 22:47:40.656600 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/response_object.py
--rw-r--r--   0        0        0      726 2023-04-18 22:47:40.656600 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/security_helper.py
--rw-r--r--   0        0        0     1132 2023-04-18 22:47:40.656600 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/type_factory.py
--rw-r--r--   0        0        0     4158 2023-04-18 22:47:40.657596 yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/user_agent.py
--rw-r--r--   0        0        0      688 2023-04-18 22:47:40.658594 yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/__init__.py
--rw-r--r--   0        0        0       67 2023-04-18 22:47:40.658594 yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/api_error.py
--rw-r--r--   0        0        0      131 2023-04-18 22:47:40.658594 yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/authorize_error.py
--rw-r--r--   0        0        0      143 2023-04-18 22:47:40.659591 yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/bad_request_error.py
--rw-r--r--   0        0        0      144 2023-04-18 22:47:40.659591 yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/forbidden_error.py
--rw-r--r--   0        0        0      141 2023-04-18 22:47:40.660590 yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/not_found_error.py
--rw-r--r--   0        0        0      151 2023-04-18 22:47:40.661587 yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/response_processing_error.py
--rw-r--r--   0        0        0      148 2023-04-18 22:47:40.661587 yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/too_many_request_error.py
--rw-r--r--   0        0        0      145 2023-04-18 22:47:40.662583 yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/unauthorized_error.py
--rw-r--r--   0        0        0     1149 2023-04-18 22:47:40.662583 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/__init__.py
--rw-r--r--   0        0        0     4347 2023-04-18 22:47:40.662583 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/airline.py
--rw-r--r--   0        0        0      702 2023-04-18 22:47:40.663579 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/amount.py
--rw-r--r--   0        0        0     1343 2023-04-18 22:47:40.663579 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/authorization_details.py
--rw-r--r--   0        0        0     1938 2023-04-18 22:47:40.663579 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/cancellation_details.py
--rw-r--r--   0        0        0        0 2023-04-18 22:47:40.664577 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/__init__.py
--rw-r--r--   0        0        0      336 2023-04-18 22:47:40.665574 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/confirmation.py
--rw-r--r--   0        0        0     2563 2023-04-18 22:47:40.665574 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/confirmation_class_map.py
--rw-r--r--   0        0        0      324 2023-04-18 22:47:40.666585 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/confirmation_factory.py
--rw-r--r--   0        0        0        0 2023-04-18 22:47:40.667571 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/__init__.py
--rw-r--r--   0        0        0      563 2023-04-18 22:47:40.667571 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_embedded.py
--rw-r--r--   0        0        0      565 2023-04-18 22:47:40.668568 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_external.py
--rw-r--r--   0        0        0      949 2023-04-18 22:47:40.669567 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py
--rw-r--r--   0        0        0      535 2023-04-18 22:47:40.669567 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_qr.py
--rw-r--r--   0        0        0     1089 2023-04-18 22:47:40.670590 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_redirect.py
--rw-r--r--   0        0        0      393 2023-04-18 22:47:40.671562 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_request.py
--rw-r--r--   0        0        0        0 2023-04-18 22:47:40.672557 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/__init__.py
--rw-r--r--   0        0        0      928 2023-04-18 22:47:40.673553 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_embedded.py
--rw-r--r--   0        0        0      535 2023-04-18 22:47:40.673553 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_external.py
--rw-r--r--   0        0        0      817 2023-04-18 22:47:40.674552 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py
--rw-r--r--   0        0        0      891 2023-04-18 22:47:40.674552 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_qr.py
--rw-r--r--   0        0        0     1295 2023-04-18 22:47:40.675548 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_redirect.py
--rw-r--r--   0        0        0      229 2023-04-18 22:47:40.676550 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/currency.py
--rw-r--r--   0        0        0     3948 2023-04-18 22:47:40.676550 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/deal.py
--rw-r--r--   0        0        0        0 2023-04-18 22:47:40.677544 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/__init__.py
--rw-r--r--   0        0        0      543 2023-04-18 22:55:43.291001 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/card_type.py
--rw-r--r--   0        0        0      887 2023-04-18 22:47:40.678540 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/payment_data.py
--rw-r--r--   0        0        0     6905 2023-04-18 22:47:40.678540 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/payment_data_class_map.py
--rw-r--r--   0        0        0      378 2023-04-18 22:47:40.679538 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/payment_data_factory.py
--rw-r--r--   0        0        0        0 2023-04-18 22:47:40.680536 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/__init__.py
--rw-r--r--   0        0        0     1979 2023-04-18 22:47:40.681533 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/credit_card.py
--rw-r--r--   0        0        0      633 2023-04-18 22:47:40.681533 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_alfabank.py
--rw-r--r--   0        0        0      675 2023-04-18 22:47:40.682529 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_applepay.py
--rw-r--r--   0        0        0     2452 2023-04-18 22:47:40.682529 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
--rw-r--r--   0        0        0      931 2023-04-18 22:47:40.683549 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
--rw-r--r--   0        0        0      791 2023-04-18 22:47:40.684525 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_cash.py
--rw-r--r--   0        0        0     1000 2023-04-18 22:47:40.686519 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
--rw-r--r--   0        0        0      472 2023-04-18 22:47:40.686519 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_installments.py
--rw-r--r--   0        0        0      829 2023-04-18 22:47:40.687533 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
--rw-r--r--   0        0        0      791 2023-04-18 22:47:40.687533 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_qiwi.py
--rw-r--r--   0        0        0      807 2023-04-18 22:47:40.687533 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
--rw-r--r--   0        0        0      438 2023-04-18 22:47:40.688514 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_sbp.py
--rw-r--r--   0        0        0      472 2023-04-18 22:47:40.688514 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
--rw-r--r--   0        0        0      458 2023-04-18 22:47:40.689511 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_webmoney.py
--rw-r--r--   0        0        0      556 2023-04-18 22:47:40.689511 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_wechat.py
--rw-r--r--   0        0        0      472 2023-04-18 22:47:40.689511 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
--rw-r--r--   0        0        0        0 2023-04-18 22:47:40.690510 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/__init__.py
--rw-r--r--   0        0        0     3685 2023-04-18 22:55:43.291999 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/credit_card.py
--rw-r--r--   0        0        0      649 2023-04-18 22:47:40.691507 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_alfabank.py
--rw-r--r--   0        0        0      474 2023-04-18 22:47:40.691507 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_applepay.py
--rw-r--r--   0        0        0     3541 2023-04-18 22:47:40.691507 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py
--rw-r--r--   0        0        0      948 2023-04-18 22:47:40.692503 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_bank_card.py
--rw-r--r--   0        0        0      807 2023-04-18 22:47:40.692503 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_cash.py
--rw-r--r--   0        0        0      482 2023-04-18 22:47:40.693503 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_google_pay.py
--rw-r--r--   0        0        0      488 2023-04-18 22:47:40.693503 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_installments.py
--rw-r--r--   0        0        0      845 2023-04-18 22:47:40.693503 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py
--rw-r--r--   0        0        0      454 2023-04-18 22:47:40.694499 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_psb.py
--rw-r--r--   0        0        0      807 2023-04-18 22:47:40.694499 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_qiwi.py
--rw-r--r--   0        0        0      842 2023-04-18 22:55:43.292997 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_sberbank.py
--rw-r--r--   0        0        0      454 2023-04-18 22:47:40.694499 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_sbp.py
--rw-r--r--   0        0        0      488 2023-04-18 22:47:40.695496 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_tinkoff_bank.py
--rw-r--r--   0        0        0      474 2023-04-18 22:47:40.695496 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_webmoney.py
--rw-r--r--   0        0        0      572 2023-04-18 22:47:40.695496 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_wechat.py
--rw-r--r--   0        0        0      488 2023-04-18 22:47:40.696494 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_yoomoney_wallet.py
--rw-r--r--   0        0        0      216 2023-04-18 22:47:40.696494 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout.py
--rw-r--r--   0        0        0        0 2023-04-18 22:47:40.696494 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/__init__.py
--rw-r--r--   0        0        0      345 2023-04-18 22:47:40.697491 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/payout_destination.py
--rw-r--r--   0        0        0     1433 2023-04-18 22:47:40.697491 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/payout_destination_class_map.py
--rw-r--r--   0        0        0      407 2023-04-18 22:47:40.697491 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/payout_destination_factory.py
--rw-r--r--   0        0        0        0 2023-04-18 22:47:40.698488 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/request/__init__.py
--rw-r--r--   0        0        0      465 2023-04-18 22:47:40.698488 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/request/credit_card.py
--rw-r--r--   0        0        0      968 2023-04-18 22:47:40.698488 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py
--rw-r--r--   0        0        0      732 2023-04-18 22:47:40.699485 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py
--rw-r--r--   0        0        0        0 2023-04-18 22:47:40.700481 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/response/__init__.py
--rw-r--r--   0        0        0     2263 2023-04-18 22:47:40.700481 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/response/credit_card.py
--rw-r--r--   0        0        0      968 2023-04-18 22:47:40.701478 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py
--rw-r--r--   0        0        0      732 2023-04-18 22:47:40.701478 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py
--rw-r--r--   0        0        0     2417 2023-04-18 22:47:40.702476 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/receipt.py
--rw-r--r--   0        0        0     1108 2023-04-18 22:47:40.702476 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/receipt_customer.py
--rw-r--r--   0        0        0     3673 2023-04-18 22:47:40.703473 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/receipt_item.py
--rw-r--r--   0        0        0      732 2023-04-18 22:47:40.703473 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/receipt_item_supplier.py
--rw-r--r--   0        0        0      586 2023-04-18 22:47:40.703473 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/recipient.py
--rw-r--r--   0        0        0     1307 2023-04-18 22:47:40.704471 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/refund_source.py
--rw-r--r--   0        0        0     2878 2023-04-18 22:47:40.704471 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/requestor.py
--rw-r--r--   0        0        0     1173 2023-04-18 22:47:40.704471 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/settlement.py
--rw-r--r--   0        0        0     2169 2023-04-18 22:55:43.293993 yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/transfer.py
--rw-r--r--   0        0        0      228 2023-04-18 22:47:40.705467 yookassa_async-0.1.2/yookassa_async/yookassa/domain/notification/__init__.py
--rw-r--r--   0        0        0     4114 2023-04-18 22:47:40.705467 yookassa_async-0.1.2/yookassa_async/yookassa/domain/notification/webhook_notification.py
--rw-r--r--   0        0        0      488 2023-04-18 22:47:40.706465 yookassa_async-0.1.2/yookassa_async/yookassa/domain/notification/webhook_notification_types.py
--rw-r--r--   0        0        0     1138 2023-04-18 22:47:40.706465 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/__init__.py
--rw-r--r--   0        0        0      776 2023-04-18 22:47:40.706465 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/capture_payment_builder.py
--rw-r--r--   0        0        0     2717 2023-04-18 22:47:40.707462 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/capture_payment_request.py
--rw-r--r--   0        0        0     1671 2023-04-18 22:47:40.707462 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/deal_request.py
--rw-r--r--   0        0        0      635 2023-04-18 22:47:40.707462 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/deal_request_builder.py
--rw-r--r--   0        0        0     9889 2023-04-18 22:47:40.708459 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/payment_request.py
--rw-r--r--   0        0        0     1956 2023-04-18 22:47:40.708459 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/payment_request_builder.py
--rw-r--r--   0        0        0     3767 2023-04-18 22:47:40.709456 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/payout_request.py
--rw-r--r--   0        0        0      871 2023-04-18 22:47:40.709456 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/payout_request_builder.py
--rw-r--r--   0        0        0     3526 2023-04-18 22:47:40.709456 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/receipt_item_request.py
--rw-r--r--   0        0        0     5800 2023-04-18 22:47:40.710454 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/receipt_request.py
--rw-r--r--   0        0        0     1170 2023-04-18 22:47:40.710454 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/receipt_request_builder.py
--rw-r--r--   0        0        0     3622 2023-04-18 22:47:40.710454 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/refund_request.py
--rw-r--r--   0        0        0      848 2023-04-18 22:47:40.711451 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/refund_request_builder.py
--rw-r--r--   0        0        0      534 2023-04-18 22:47:40.711451 yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/webhook_request.py
--rw-r--r--   0        0        0     1002 2023-04-18 22:47:40.712449 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/__init__.py
--rw-r--r--   0        0        0      871 2023-04-18 22:47:40.712449 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/deal_list_response.py
--rw-r--r--   0        0        0     2178 2023-04-18 22:47:40.712449 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/deal_response.py
--rw-r--r--   0        0        0      883 2023-04-18 22:47:40.713446 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/payment_list_response.py
--rw-r--r--   0        0        0     5572 2023-04-18 22:47:40.713446 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/payment_response.py
--rw-r--r--   0        0        0     2453 2023-04-18 22:47:40.714443 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/payout_response.py
--rw-r--r--   0        0        0     2136 2023-04-18 22:47:40.714443 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/receipt_item_response.py
--rw-r--r--   0        0        0      883 2023-04-18 22:47:40.714443 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/receipt_list_response.py
--rw-r--r--   0        0        0     3740 2023-04-18 22:47:40.715440 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/receipt_response.py
--rw-r--r--   0        0        0      877 2023-04-18 22:47:40.715964 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/refund_list_response.py
--rw-r--r--   0        0        0     2247 2023-04-18 22:47:40.716471 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/refund_response.py
--rw-r--r--   0        0        0     2167 2023-04-18 22:55:43.295017 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/transfer_response.py
--rw-r--r--   0        0        0     1124 2023-04-18 22:55:43.295987 yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/webhook_response.py
--rw-r--r--   0        0        0     3788 2023-04-18 22:47:40.717474 yookassa_async-0.1.2/yookassa_async/yookassa/payment.py
--rw-r--r--   0        0        0     1694 2023-04-18 22:47:40.718471 yookassa_async-0.1.2/yookassa_async/yookassa/payout.py
--rw-r--r--   0        0        0     2058 2023-04-18 22:47:40.719469 yookassa_async-0.1.2/yookassa_async/yookassa/receipt.py
--rw-r--r--   0        0        0     2015 2023-04-18 22:47:40.719469 yookassa_async-0.1.2/yookassa_async/yookassa/refund.py
--rw-r--r--   0        0        0      707 2023-04-18 22:47:40.719469 yookassa_async-0.1.2/yookassa_async/yookassa/settings.py
--rw-r--r--   0        0        0     2094 2023-04-18 22:47:40.720466 yookassa_async-0.1.2/yookassa_async/yookassa/webhook.py
--rw-r--r--   0        0        0     7737 1970-01-01 00:00:00.000000 yookassa_async-0.1.2/setup.py
--rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 yookassa_async-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-04-18 22:47:40.640643 yookassa_async-0.1.3/LICENSE
+-rw-r--r--   0        0        0      520 2023-04-19 02:25:37.806478 yookassa_async-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6337 2023-04-18 22:57:38.445440 yookassa_async-0.1.3/README.md
+-rw-r--r--   0        0        0      481 2023-04-18 22:55:43.289005 yookassa_async-0.1.3/yookassa/__init__.py
+-rw-r--r--   0        0        0     5188 2023-04-18 22:47:40.649618 yookassa_async-0.1.3/yookassa/client.py
+-rw-r--r--   0        0        0     2620 2023-04-18 22:47:40.649618 yookassa_async-0.1.3/yookassa/configuration.py
+-rw-r--r--   0        0        0     1915 2023-04-18 22:47:40.650617 yookassa_async-0.1.3/yookassa/deal.py
+-rw-r--r--   0        0        0       90 2023-04-18 22:47:40.651614 yookassa_async-0.1.3/yookassa/domain/__init__.py
+-rw-r--r--   0        0        0      873 2023-04-18 22:47:40.651614 yookassa_async-0.1.3/yookassa/domain/common/__init__.py
+-rw-r--r--   0        0        0     1529 2023-04-18 22:47:40.652611 yookassa_async-0.1.3/yookassa/domain/common/base_object.py
+-rw-r--r--   0        0        0      571 2023-04-18 22:47:40.652611 yookassa_async-0.1.3/yookassa/domain/common/confirmation_type.py
+-rw-r--r--   0        0        0      404 2023-04-18 22:47:40.653608 yookassa_async-0.1.3/yookassa/domain/common/context.py
+-rw-r--r--   0        0        0      353 2023-04-18 22:47:40.653608 yookassa_async-0.1.3/yookassa/domain/common/data_context.py
+-rw-r--r--   0        0        0      596 2023-04-18 22:47:40.654633 yookassa_async-0.1.3/yookassa/domain/common/http_verb.py
+-rw-r--r--   0        0        0     1502 2023-04-18 22:47:40.655600 yookassa_async-0.1.3/yookassa/domain/common/payment_method_type.py
+-rw-r--r--   0        0        0      582 2023-04-18 22:47:40.655600 yookassa_async-0.1.3/yookassa/domain/common/receipt_type.py
+-rw-r--r--   0        0        0      400 2023-04-18 22:47:40.655600 yookassa_async-0.1.3/yookassa/domain/common/request_object.py
+-rw-r--r--   0        0        0      302 2023-04-18 22:47:40.656600 yookassa_async-0.1.3/yookassa/domain/common/response_object.py
+-rw-r--r--   0        0        0      726 2023-04-18 22:47:40.656600 yookassa_async-0.1.3/yookassa/domain/common/security_helper.py
+-rw-r--r--   0        0        0     1132 2023-04-18 22:47:40.656600 yookassa_async-0.1.3/yookassa/domain/common/type_factory.py
+-rw-r--r--   0        0        0     4158 2023-04-18 22:47:40.657596 yookassa_async-0.1.3/yookassa/domain/common/user_agent.py
+-rw-r--r--   0        0        0      688 2023-04-18 22:47:40.658594 yookassa_async-0.1.3/yookassa/domain/exceptions/__init__.py
+-rw-r--r--   0        0        0       67 2023-04-18 22:47:40.658594 yookassa_async-0.1.3/yookassa/domain/exceptions/api_error.py
+-rw-r--r--   0        0        0      131 2023-04-18 22:47:40.658594 yookassa_async-0.1.3/yookassa/domain/exceptions/authorize_error.py
+-rw-r--r--   0        0        0      143 2023-04-18 22:47:40.659591 yookassa_async-0.1.3/yookassa/domain/exceptions/bad_request_error.py
+-rw-r--r--   0        0        0      144 2023-04-18 22:47:40.659591 yookassa_async-0.1.3/yookassa/domain/exceptions/forbidden_error.py
+-rw-r--r--   0        0        0      141 2023-04-18 22:47:40.660590 yookassa_async-0.1.3/yookassa/domain/exceptions/not_found_error.py
+-rw-r--r--   0        0        0      151 2023-04-18 22:47:40.661587 yookassa_async-0.1.3/yookassa/domain/exceptions/response_processing_error.py
+-rw-r--r--   0        0        0      148 2023-04-18 22:47:40.661587 yookassa_async-0.1.3/yookassa/domain/exceptions/too_many_request_error.py
+-rw-r--r--   0        0        0      145 2023-04-18 22:47:40.662583 yookassa_async-0.1.3/yookassa/domain/exceptions/unauthorized_error.py
+-rw-r--r--   0        0        0     1149 2023-04-18 22:47:40.662583 yookassa_async-0.1.3/yookassa/domain/models/__init__.py
+-rw-r--r--   0        0        0     4347 2023-04-18 22:47:40.662583 yookassa_async-0.1.3/yookassa/domain/models/airline.py
+-rw-r--r--   0        0        0      702 2023-04-18 22:47:40.663579 yookassa_async-0.1.3/yookassa/domain/models/amount.py
+-rw-r--r--   0        0        0     1343 2023-04-18 22:47:40.663579 yookassa_async-0.1.3/yookassa/domain/models/authorization_details.py
+-rw-r--r--   0        0        0     1938 2023-04-18 22:47:40.663579 yookassa_async-0.1.3/yookassa/domain/models/cancellation_details.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:47:40.664577 yookassa_async-0.1.3/yookassa/domain/models/confirmation/__init__.py
+-rw-r--r--   0        0        0      336 2023-04-18 22:47:40.665574 yookassa_async-0.1.3/yookassa/domain/models/confirmation/confirmation.py
+-rw-r--r--   0        0        0     2563 2023-04-18 22:47:40.665574 yookassa_async-0.1.3/yookassa/domain/models/confirmation/confirmation_class_map.py
+-rw-r--r--   0        0        0      324 2023-04-18 22:47:40.666585 yookassa_async-0.1.3/yookassa/domain/models/confirmation/confirmation_factory.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:47:40.667571 yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/__init__.py
+-rw-r--r--   0        0        0      563 2023-04-18 22:47:40.667571 yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_embedded.py
+-rw-r--r--   0        0        0      565 2023-04-18 22:47:40.668568 yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_external.py
+-rw-r--r--   0        0        0      949 2023-04-18 22:47:40.669567 yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py
+-rw-r--r--   0        0        0      535 2023-04-18 22:47:40.669567 yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_qr.py
+-rw-r--r--   0        0        0     1089 2023-04-18 22:47:40.670590 yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_redirect.py
+-rw-r--r--   0        0        0      393 2023-04-18 22:47:40.671562 yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_request.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:47:40.672557 yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/__init__.py
+-rw-r--r--   0        0        0      928 2023-04-18 22:47:40.673553 yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_embedded.py
+-rw-r--r--   0        0        0      535 2023-04-18 22:47:40.673553 yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_external.py
+-rw-r--r--   0        0        0      817 2023-04-18 22:47:40.674552 yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py
+-rw-r--r--   0        0        0      891 2023-04-18 22:47:40.674552 yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_qr.py
+-rw-r--r--   0        0        0     1295 2023-04-18 22:47:40.675548 yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_redirect.py
+-rw-r--r--   0        0        0      229 2023-04-18 22:47:40.676550 yookassa_async-0.1.3/yookassa/domain/models/currency.py
+-rw-r--r--   0        0        0     3948 2023-04-18 22:47:40.676550 yookassa_async-0.1.3/yookassa/domain/models/deal.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:47:40.677544 yookassa_async-0.1.3/yookassa/domain/models/payment_data/__init__.py
+-rw-r--r--   0        0        0      543 2023-04-18 22:55:43.291001 yookassa_async-0.1.3/yookassa/domain/models/payment_data/card_type.py
+-rw-r--r--   0        0        0      887 2023-04-18 22:47:40.678540 yookassa_async-0.1.3/yookassa/domain/models/payment_data/payment_data.py
+-rw-r--r--   0        0        0     6905 2023-04-18 22:47:40.678540 yookassa_async-0.1.3/yookassa/domain/models/payment_data/payment_data_class_map.py
+-rw-r--r--   0        0        0      378 2023-04-18 22:47:40.679538 yookassa_async-0.1.3/yookassa/domain/models/payment_data/payment_data_factory.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:47:40.680536 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/__init__.py
+-rw-r--r--   0        0        0     1979 2023-04-18 22:47:40.681533 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/credit_card.py
+-rw-r--r--   0        0        0      633 2023-04-18 22:47:40.681533 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_alfabank.py
+-rw-r--r--   0        0        0      675 2023-04-18 22:47:40.682529 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_applepay.py
+-rw-r--r--   0        0        0     2452 2023-04-18 22:47:40.682529 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
+-rw-r--r--   0        0        0      931 2023-04-18 22:47:40.683549 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
+-rw-r--r--   0        0        0      791 2023-04-18 22:47:40.684525 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_cash.py
+-rw-r--r--   0        0        0     1000 2023-04-18 22:47:40.686519 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
+-rw-r--r--   0        0        0      472 2023-04-18 22:47:40.686519 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_installments.py
+-rw-r--r--   0        0        0      829 2023-04-18 22:47:40.687533 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
+-rw-r--r--   0        0        0      791 2023-04-18 22:47:40.687533 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_qiwi.py
+-rw-r--r--   0        0        0      807 2023-04-18 22:47:40.687533 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
+-rw-r--r--   0        0        0      438 2023-04-18 22:47:40.688514 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_sbp.py
+-rw-r--r--   0        0        0      472 2023-04-18 22:47:40.688514 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
+-rw-r--r--   0        0        0      458 2023-04-18 22:47:40.689511 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_webmoney.py
+-rw-r--r--   0        0        0      556 2023-04-18 22:47:40.689511 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_wechat.py
+-rw-r--r--   0        0        0      472 2023-04-18 22:47:40.689511 yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:47:40.690510 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/__init__.py
+-rw-r--r--   0        0        0     3685 2023-04-18 22:55:43.291999 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/credit_card.py
+-rw-r--r--   0        0        0      649 2023-04-18 22:47:40.691507 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_alfabank.py
+-rw-r--r--   0        0        0      474 2023-04-18 22:47:40.691507 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_applepay.py
+-rw-r--r--   0        0        0     3541 2023-04-18 22:47:40.691507 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py
+-rw-r--r--   0        0        0      948 2023-04-18 22:47:40.692503 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_bank_card.py
+-rw-r--r--   0        0        0      807 2023-04-18 22:47:40.692503 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_cash.py
+-rw-r--r--   0        0        0      482 2023-04-18 22:47:40.693503 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_google_pay.py
+-rw-r--r--   0        0        0      488 2023-04-18 22:47:40.693503 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_installments.py
+-rw-r--r--   0        0        0      845 2023-04-18 22:47:40.693503 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py
+-rw-r--r--   0        0        0      454 2023-04-18 22:47:40.694499 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_psb.py
+-rw-r--r--   0        0        0      807 2023-04-18 22:47:40.694499 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_qiwi.py
+-rw-r--r--   0        0        0      842 2023-04-18 22:55:43.292997 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_sberbank.py
+-rw-r--r--   0        0        0      454 2023-04-18 22:47:40.694499 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_sbp.py
+-rw-r--r--   0        0        0      488 2023-04-18 22:47:40.695496 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_tinkoff_bank.py
+-rw-r--r--   0        0        0      474 2023-04-18 22:47:40.695496 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_webmoney.py
+-rw-r--r--   0        0        0      572 2023-04-18 22:47:40.695496 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_wechat.py
+-rw-r--r--   0        0        0      488 2023-04-18 22:47:40.696494 yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_yoomoney_wallet.py
+-rw-r--r--   0        0        0      216 2023-04-18 22:47:40.696494 yookassa_async-0.1.3/yookassa/domain/models/payout.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:47:40.696494 yookassa_async-0.1.3/yookassa/domain/models/payout_data/__init__.py
+-rw-r--r--   0        0        0      345 2023-04-18 22:47:40.697491 yookassa_async-0.1.3/yookassa/domain/models/payout_data/payout_destination.py
+-rw-r--r--   0        0        0     1433 2023-04-18 22:47:40.697491 yookassa_async-0.1.3/yookassa/domain/models/payout_data/payout_destination_class_map.py
+-rw-r--r--   0        0        0      407 2023-04-18 22:47:40.697491 yookassa_async-0.1.3/yookassa/domain/models/payout_data/payout_destination_factory.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:47:40.698488 yookassa_async-0.1.3/yookassa/domain/models/payout_data/request/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-18 22:47:40.698488 yookassa_async-0.1.3/yookassa/domain/models/payout_data/request/credit_card.py
+-rw-r--r--   0        0        0      968 2023-04-18 22:47:40.698488 yookassa_async-0.1.3/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py
+-rw-r--r--   0        0        0      732 2023-04-18 22:47:40.699485 yookassa_async-0.1.3/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:47:40.700481 yookassa_async-0.1.3/yookassa/domain/models/payout_data/response/__init__.py
+-rw-r--r--   0        0        0     2263 2023-04-18 22:47:40.700481 yookassa_async-0.1.3/yookassa/domain/models/payout_data/response/credit_card.py
+-rw-r--r--   0        0        0      968 2023-04-18 22:47:40.701478 yookassa_async-0.1.3/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py
+-rw-r--r--   0        0        0      732 2023-04-18 22:47:40.701478 yookassa_async-0.1.3/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py
+-rw-r--r--   0        0        0     2417 2023-04-18 22:47:40.702476 yookassa_async-0.1.3/yookassa/domain/models/receipt.py
+-rw-r--r--   0        0        0     1108 2023-04-18 22:47:40.702476 yookassa_async-0.1.3/yookassa/domain/models/receipt_customer.py
+-rw-r--r--   0        0        0     3673 2023-04-18 22:47:40.703473 yookassa_async-0.1.3/yookassa/domain/models/receipt_item.py
+-rw-r--r--   0        0        0      732 2023-04-18 22:47:40.703473 yookassa_async-0.1.3/yookassa/domain/models/receipt_item_supplier.py
+-rw-r--r--   0        0        0      586 2023-04-18 22:47:40.703473 yookassa_async-0.1.3/yookassa/domain/models/recipient.py
+-rw-r--r--   0        0        0     1307 2023-04-18 22:47:40.704471 yookassa_async-0.1.3/yookassa/domain/models/refund_source.py
+-rw-r--r--   0        0        0     2878 2023-04-18 22:47:40.704471 yookassa_async-0.1.3/yookassa/domain/models/requestor.py
+-rw-r--r--   0        0        0     1173 2023-04-18 22:47:40.704471 yookassa_async-0.1.3/yookassa/domain/models/settlement.py
+-rw-r--r--   0        0        0     2169 2023-04-18 22:55:43.293993 yookassa_async-0.1.3/yookassa/domain/models/transfer.py
+-rw-r--r--   0        0        0      228 2023-04-18 22:47:40.705467 yookassa_async-0.1.3/yookassa/domain/notification/__init__.py
+-rw-r--r--   0        0        0     4114 2023-04-18 22:47:40.705467 yookassa_async-0.1.3/yookassa/domain/notification/webhook_notification.py
+-rw-r--r--   0        0        0      488 2023-04-18 22:47:40.706465 yookassa_async-0.1.3/yookassa/domain/notification/webhook_notification_types.py
+-rw-r--r--   0        0        0     1138 2023-04-18 22:47:40.706465 yookassa_async-0.1.3/yookassa/domain/request/__init__.py
+-rw-r--r--   0        0        0      776 2023-04-18 22:47:40.706465 yookassa_async-0.1.3/yookassa/domain/request/capture_payment_builder.py
+-rw-r--r--   0        0        0     2717 2023-04-18 22:47:40.707462 yookassa_async-0.1.3/yookassa/domain/request/capture_payment_request.py
+-rw-r--r--   0        0        0     1671 2023-04-18 22:47:40.707462 yookassa_async-0.1.3/yookassa/domain/request/deal_request.py
+-rw-r--r--   0        0        0      635 2023-04-18 22:47:40.707462 yookassa_async-0.1.3/yookassa/domain/request/deal_request_builder.py
+-rw-r--r--   0        0        0     9889 2023-04-18 22:47:40.708459 yookassa_async-0.1.3/yookassa/domain/request/payment_request.py
+-rw-r--r--   0        0        0     1956 2023-04-18 22:47:40.708459 yookassa_async-0.1.3/yookassa/domain/request/payment_request_builder.py
+-rw-r--r--   0        0        0     3767 2023-04-18 22:47:40.709456 yookassa_async-0.1.3/yookassa/domain/request/payout_request.py
+-rw-r--r--   0        0        0      871 2023-04-18 22:47:40.709456 yookassa_async-0.1.3/yookassa/domain/request/payout_request_builder.py
+-rw-r--r--   0        0        0     3526 2023-04-18 22:47:40.709456 yookassa_async-0.1.3/yookassa/domain/request/receipt_item_request.py
+-rw-r--r--   0        0        0     5800 2023-04-18 22:47:40.710454 yookassa_async-0.1.3/yookassa/domain/request/receipt_request.py
+-rw-r--r--   0        0        0     1170 2023-04-18 22:47:40.710454 yookassa_async-0.1.3/yookassa/domain/request/receipt_request_builder.py
+-rw-r--r--   0        0        0     3622 2023-04-18 22:47:40.710454 yookassa_async-0.1.3/yookassa/domain/request/refund_request.py
+-rw-r--r--   0        0        0      848 2023-04-18 22:47:40.711451 yookassa_async-0.1.3/yookassa/domain/request/refund_request_builder.py
+-rw-r--r--   0        0        0      534 2023-04-18 22:47:40.711451 yookassa_async-0.1.3/yookassa/domain/request/webhook_request.py
+-rw-r--r--   0        0        0     1002 2023-04-18 22:47:40.712449 yookassa_async-0.1.3/yookassa/domain/response/__init__.py
+-rw-r--r--   0        0        0      871 2023-04-18 22:47:40.712449 yookassa_async-0.1.3/yookassa/domain/response/deal_list_response.py
+-rw-r--r--   0        0        0     2178 2023-04-18 22:47:40.712449 yookassa_async-0.1.3/yookassa/domain/response/deal_response.py
+-rw-r--r--   0        0        0      883 2023-04-18 22:47:40.713446 yookassa_async-0.1.3/yookassa/domain/response/payment_list_response.py
+-rw-r--r--   0        0        0     5572 2023-04-18 22:47:40.713446 yookassa_async-0.1.3/yookassa/domain/response/payment_response.py
+-rw-r--r--   0        0        0     2453 2023-04-18 22:47:40.714443 yookassa_async-0.1.3/yookassa/domain/response/payout_response.py
+-rw-r--r--   0        0        0     2136 2023-04-18 22:47:40.714443 yookassa_async-0.1.3/yookassa/domain/response/receipt_item_response.py
+-rw-r--r--   0        0        0      883 2023-04-18 22:47:40.714443 yookassa_async-0.1.3/yookassa/domain/response/receipt_list_response.py
+-rw-r--r--   0        0        0     3740 2023-04-18 22:47:40.715440 yookassa_async-0.1.3/yookassa/domain/response/receipt_response.py
+-rw-r--r--   0        0        0      877 2023-04-18 22:47:40.715964 yookassa_async-0.1.3/yookassa/domain/response/refund_list_response.py
+-rw-r--r--   0        0        0     2247 2023-04-18 22:47:40.716471 yookassa_async-0.1.3/yookassa/domain/response/refund_response.py
+-rw-r--r--   0        0        0     2167 2023-04-18 22:55:43.295017 yookassa_async-0.1.3/yookassa/domain/response/transfer_response.py
+-rw-r--r--   0        0        0     1124 2023-04-18 22:55:43.295987 yookassa_async-0.1.3/yookassa/domain/response/webhook_response.py
+-rw-r--r--   0        0        0     3788 2023-04-18 22:47:40.717474 yookassa_async-0.1.3/yookassa/payment.py
+-rw-r--r--   0        0        0     1694 2023-04-18 22:47:40.718471 yookassa_async-0.1.3/yookassa/payout.py
+-rw-r--r--   0        0        0     2058 2023-04-18 22:47:40.719469 yookassa_async-0.1.3/yookassa/receipt.py
+-rw-r--r--   0        0        0     2015 2023-04-18 22:47:40.719469 yookassa_async-0.1.3/yookassa/refund.py
+-rw-r--r--   0        0        0      707 2023-04-18 22:47:40.719469 yookassa_async-0.1.3/yookassa/settings.py
+-rw-r--r--   0        0        0     2094 2023-04-18 22:47:40.720466 yookassa_async-0.1.3/yookassa/webhook.py
+-rw-r--r--   0        0        0     7737 1970-01-01 00:00:00.000000 yookassa_async-0.1.3/setup.py
+-rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 yookassa_async-0.1.3/PKG-INFO
```

### Comparing `yookassa_async-0.1.2/LICENSE` & `yookassa_async-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/pyproject.toml` & `yookassa_async-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "yookassa-async"
-version = "0.1.2"
+version = "0.1.3"
 description = "Based on work of https://github.com/tonchik-tm and main yookassa package"
 authors = ["Илья Снимщиков <igsnimschikov@edu.hse.ru>"]
 readme = "README.md"
-packages = [{include = "yookassa_async/yookassa"}]
+packages = [{include = "yookassa"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = "^0.24.0"
 requests = "^2.28.2"
 netaddr = "^0.8.0"
 distro = "^1.8.0"
```

### Comparing `yookassa_async-0.1.2/README.md` & `yookassa_async-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/client.py` & `yookassa_async-0.1.3/yookassa/client.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/configuration.py` & `yookassa_async-0.1.3/yookassa/configuration.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/deal.py` & `yookassa_async-0.1.3/yookassa/deal.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/__init__.py` & `yookassa_async-0.1.3/yookassa/domain/common/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/base_object.py` & `yookassa_async-0.1.3/yookassa/domain/common/base_object.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/confirmation_type.py` & `yookassa_async-0.1.3/yookassa/domain/common/confirmation_type.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/http_verb.py` & `yookassa_async-0.1.3/yookassa/domain/common/http_verb.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/payment_method_type.py` & `yookassa_async-0.1.3/yookassa/domain/common/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/receipt_type.py` & `yookassa_async-0.1.3/yookassa/domain/common/receipt_type.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/security_helper.py` & `yookassa_async-0.1.3/yookassa/domain/common/security_helper.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/type_factory.py` & `yookassa_async-0.1.3/yookassa/domain/common/type_factory.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/common/user_agent.py` & `yookassa_async-0.1.3/yookassa/domain/common/user_agent.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/exceptions/__init__.py` & `yookassa_async-0.1.3/yookassa/domain/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/__init__.py` & `yookassa_async-0.1.3/yookassa/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/airline.py` & `yookassa_async-0.1.3/yookassa/domain/models/airline.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/amount.py` & `yookassa_async-0.1.3/yookassa/domain/models/amount.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/authorization_details.py` & `yookassa_async-0.1.3/yookassa/domain/models/authorization_details.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/cancellation_details.py` & `yookassa_async-0.1.3/yookassa/domain/models/cancellation_details.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/confirmation_class_map.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/confirmation_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_embedded.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_embedded.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_external.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_external.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_qr.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_qr.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/request/confirmation_redirect.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/request/confirmation_redirect.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_embedded.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_embedded.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_external.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_external.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_qr.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_qr.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/confirmation/response/confirmation_redirect.py` & `yookassa_async-0.1.3/yookassa/domain/models/confirmation/response/confirmation_redirect.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/deal.py` & `yookassa_async-0.1.3/yookassa/domain/models/deal.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/card_type.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/card_type.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/payment_data.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/payment_data.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/payment_data_class_map.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/payment_data_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/credit_card.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_alfabank.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_alfabank.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_applepay.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_applepay.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_bank_card.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_cash.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_cash.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_google_pay.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_google_pay.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_qiwi.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_qiwi.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_sberbank.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/request/payment_data_wechat.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/request/payment_data_wechat.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/credit_card.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_alfabank.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_alfabank.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_bank_card.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_cash.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_cash.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_qiwi.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_qiwi.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_sberbank.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payment_data/response/payment_data_wechat.py` & `yookassa_async-0.1.3/yookassa/domain/models/payment_data/response/payment_data_wechat.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/payout_destination_class_map.py` & `yookassa_async-0.1.3/yookassa/domain/models/payout_data/payout_destination_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py` & `yookassa_async-0.1.3/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py` & `yookassa_async-0.1.3/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/response/credit_card.py` & `yookassa_async-0.1.3/yookassa/domain/models/payout_data/response/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py` & `yookassa_async-0.1.3/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py` & `yookassa_async-0.1.3/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/receipt.py` & `yookassa_async-0.1.3/yookassa/domain/models/receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/receipt_customer.py` & `yookassa_async-0.1.3/yookassa/domain/models/receipt_customer.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/receipt_item.py` & `yookassa_async-0.1.3/yookassa/domain/models/receipt_item.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/receipt_item_supplier.py` & `yookassa_async-0.1.3/yookassa/domain/models/receipt_item_supplier.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/recipient.py` & `yookassa_async-0.1.3/yookassa/domain/models/recipient.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/refund_source.py` & `yookassa_async-0.1.3/yookassa/domain/models/refund_source.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/requestor.py` & `yookassa_async-0.1.3/yookassa/domain/models/requestor.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/settlement.py` & `yookassa_async-0.1.3/yookassa/domain/models/settlement.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/models/transfer.py` & `yookassa_async-0.1.3/yookassa/domain/models/transfer.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/notification/webhook_notification.py` & `yookassa_async-0.1.3/yookassa/domain/notification/webhook_notification.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/__init__.py` & `yookassa_async-0.1.3/yookassa/domain/request/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/capture_payment_builder.py` & `yookassa_async-0.1.3/yookassa/domain/request/capture_payment_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/capture_payment_request.py` & `yookassa_async-0.1.3/yookassa/domain/request/capture_payment_request.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/deal_request.py` & `yookassa_async-0.1.3/yookassa/domain/request/deal_request.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/deal_request_builder.py` & `yookassa_async-0.1.3/yookassa/domain/request/deal_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/payment_request.py` & `yookassa_async-0.1.3/yookassa/domain/request/payment_request.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/payment_request_builder.py` & `yookassa_async-0.1.3/yookassa/domain/request/payment_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/payout_request.py` & `yookassa_async-0.1.3/yookassa/domain/request/payout_request.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/payout_request_builder.py` & `yookassa_async-0.1.3/yookassa/domain/request/payout_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/receipt_item_request.py` & `yookassa_async-0.1.3/yookassa/domain/request/receipt_item_request.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/receipt_request.py` & `yookassa_async-0.1.3/yookassa/domain/request/receipt_request.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/receipt_request_builder.py` & `yookassa_async-0.1.3/yookassa/domain/request/receipt_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/refund_request.py` & `yookassa_async-0.1.3/yookassa/domain/request/refund_request.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/refund_request_builder.py` & `yookassa_async-0.1.3/yookassa/domain/request/refund_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/request/webhook_request.py` & `yookassa_async-0.1.3/yookassa/domain/request/webhook_request.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/__init__.py` & `yookassa_async-0.1.3/yookassa/domain/response/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/deal_list_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/deal_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/deal_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/deal_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/payment_list_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/payment_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/payment_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/payment_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/payout_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/payout_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/receipt_item_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/receipt_item_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/receipt_list_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/receipt_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/receipt_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/receipt_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/refund_list_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/refund_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/refund_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/refund_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/transfer_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/transfer_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/domain/response/webhook_response.py` & `yookassa_async-0.1.3/yookassa/domain/response/webhook_response.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/payment.py` & `yookassa_async-0.1.3/yookassa/payment.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/payout.py` & `yookassa_async-0.1.3/yookassa/payout.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/receipt.py` & `yookassa_async-0.1.3/yookassa/receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/refund.py` & `yookassa_async-0.1.3/yookassa/refund.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/settings.py` & `yookassa_async-0.1.3/yookassa/settings.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/yookassa_async/yookassa/webhook.py` & `yookassa_async-0.1.3/yookassa/webhook.py`

 * *Files identical despite different names*

### Comparing `yookassa_async-0.1.2/setup.py` & `yookassa_async-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'distro>=1.8.0,<2.0.0',
  'httpx>=0.24.0,<0.25.0',
  'netaddr>=0.8.0,<0.9.0',
  'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'yookassa-async',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Based on work of https://github.com/tonchik-tm and main yookassa package',
     'long_description': "# YooKassa ASync API Python Client Library\n\n[![Build Status](https://travis-ci.org/yoomoney/yookassa-sdk-python.svg?branch=master)](https://travis-ci.org/yoomoney/yookassa-sdk-python)\n[![Latest Stable Version](https://img.shields.io/pypi/v/yookassa.svg)](https://pypi.org/project/yookassa/)\n[![Total Downloads](https://img.shields.io/pypi/dm/yookassa.svg)](https://pypi.org/project/yookassa/)\n[![License](https://img.shields.io/pypi/l/yookassa.svg)](https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python)\n\nRussian | [English](README.en.md)\n\nКлиент для работы с платежами по [API ЮKassa](https://yookassa.ru/developers/api)\nПодходит тем, у кого способ подключения к ЮKassa называется API.\n\nАсинхронная версия.\n\n## Требования\n\n1. Python >=3.7\n2. pip\n\n## Установка\n### C помощью pip\n\n1. Установите pip.\n2. В консоли выполните команду\n```bash\npip install --upgrade yookassa\n```\n\n### С помощью easy_install\n1. Установите easy_install.\n2. В консоли выполните команду\n```bash\neasy_install --upgrade yookassa\n```\n\n### Вручную\n\n1. В консоли выполните команды:\n```bash\nwget https://pypi.python.org/packages/5a/be/5eafdfb14aa6f32107e9feb6514ca1ad3fe56f8e5ee59d20693b32f7e79f/yookassa-1.0.0.tar.gz#md5=46595279b5578fd82a199bfd4cd51db2\ntar zxf yookassa-1.0.0.tar.gz\ncd yookassa-1.0.0\npython setup.py install\n```\n\n## Начало работы\n\n1. Импортируйте модуль\n```python\nimport yookassa\n```\n2. Установите данные для конфигурации\n```python\nfrom yookassa import Configuration\n\nConfiguration.configure('<Идентификатор магазина>', '<Секретный ключ>')\n```\n\nили\n\n```python\nfrom yookassa import Configuration\n\nConfiguration.account_id = '<Идентификатор магазина>'\nConfiguration.secret_key = '<Секретный ключ>'\n```\n\nили через oauth\n\n```python\nfrom yookassa import Configuration\n\nConfiguration.configure_auth_token('<Oauth Token>')\n```\n\nЕсли вы согласны участвовать в развитии SDK, вы можете передать данные о вашем фреймворке, cms или модуле:\n```python\nfrom yookassa import Configuration\nfrom yookassa.domain.common.user_agent import Version\n\nConfiguration.configure('<Идентификатор магазина>', '<Секретный ключ>')\nConfiguration.configure_user_agent(\n    framework=Version('Django', '2.2.3'),\n    cms=Version('Wagtail', '2.6.2'),\n    module=Version('Y.CMS', '0.0.1')\n)\n```\n\n3. Вызовите нужный метод API. [Подробнее в документации к API ЮKassa](https://yookassa.ru/developers/api)\n\n## Примеры использования SDK\n\n#### [Настройки SDK API ЮKassa](./docs/examples/01-configuration.md)\n* [Аутентификация](./docs/examples/01-configuration.md#Аутентификация)\n* [Статистические данные об используемом окружении](./docs/examples/01-configuration.md#Статистические-данные-об-используемом-окружении)\n* [Получение информации о магазине](./docs/examples/01-configuration.md#Получение-информации-о-магазине)\n* [Работа с Webhook](./docs/examples/01-configuration.md#Работа-с-Webhook)\n* [Входящие уведомления](./docs/examples/01-configuration.md#Входящие-уведомления)\n\n#### [Работа с платежами](./docs/examples/02-payments.md)\n* [Запрос на создание платежа](./docs/examples/02-payments.md#Запрос-на-создание-платежа)\n* [Запрос на создание платежа через билдер](./docs/examples/02-payments.md#Запрос-на-создание-платежа-через-билдер)\n* [Запрос на частичное подтверждение платежа](./docs/examples/02-payments.md#Запрос-на-частичное-подтверждение-платежа)\n* [Запрос на отмену незавершенного платежа](./docs/examples/02-payments.md#Запрос-на-отмену-незавершенного-платежа)\n* [Получить информацию о платеже](./docs/examples/02-payments.md#Получить-информацию-о-платеже)\n* [Получить список платежей с фильтрацией](./docs/examples/02-payments.md#Получить-список-платежей-с-фильтрацией)\n\n#### [Работа с возвратами](./docs/examples/03-refunds.md)\n* [Запрос на создание возврата](./docs/examples/03-refunds.md#Запрос-на-создание-возврата)\n* [Запрос на создание возврата через билдер](./docs/examples/03-refunds.md#Запрос-на-создание-возврата-через-билдер)\n* [Получить информацию о возврате](./docs/examples/03-refunds.md#Получить-информацию-о-возврате)\n* [Получить список возвратов с фильтрацией](./docs/examples/03-refunds.md#Получить-список-возвратов-с-фильтрацией)\n\n#### [Работа с чеками](./docs/examples/04-receipts.md)\n* [Запрос на создание чека](./docs/examples/04-receipts.md#Запрос-на-создание-чека)\n* [Запрос на создание чека через билдер](./docs/examples/04-receipts.md#Запрос-на-создание-чека-через-билдер)\n* [Получить информацию о чеке](./docs/examples/04-receipts.md#Получить-информацию-о-чеке)\n* [Получить список чеков с фильтрацией](./docs/examples/04-receipts.md#Получить-список-чеков-с-фильтрацией)\n",
     'author': 'Илья Снимщиков',
     'author_email': 'igsnimschikov@edu.hse.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `yookassa_async-0.1.2/PKG-INFO` & `yookassa_async-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yookassa-async
-Version: 0.1.2
+Version: 0.1.3
 Summary: Based on work of https://github.com/tonchik-tm and main yookassa package
 Author: Илья Снимщиков
 Author-email: igsnimschikov@edu.hse.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

