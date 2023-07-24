# Comparing `tmp/mergepythonclient-0.1.0.tar.gz` & `tmp/mergepythonclient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergepythonclient-0.1.0.tar", max compression
+gzip compressed data, was "mergepythonclient-0.1.1.tar", max compression
```

## Comparing `mergepythonclient-0.1.0.tar` & `mergepythonclient-0.1.1.tar`

### file list

```diff
@@ -1,1114 +1,1114 @@
--rw-r--r--   0        0        0     3274 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     4158 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/README.md
--rw-r--r--   0        0        0      535 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      249 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/__init__.py
--rw-r--r--   0        0        0     2459 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/client.py
--rw-r--r--   0        0        0      519 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/core/api_error.py
--rw-r--r--   0        0        0     1101 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      201 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/environment.py
--rw-r--r--   0        0        0        0 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/py.typed
--rw-r--r--   0        0        0      178 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/__init__.py
--rw-r--r--   0        0        0    12630 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/__init__.py
--rw-r--r--   0        0        0    12026 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/client.py
--rw-r--r--   0        0        0     1410 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2394 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2634 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/accounts/__init__.py
--rw-r--r--   0        0        0    18106 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/addresses/__init__.py
--rw-r--r--   0        0        0     4472 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/addresses/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/attachments/__init__.py
--rw-r--r--   0        0        0    14525 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2472 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/balance_sheets/__init__.py
--rw-r--r--   0        0        0    10863 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/balance_sheets/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/cash_flow_statements/__init__.py
--rw-r--r--   0        0        0    10991 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/cash_flow_statements/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/company_info/__init__.py
--rw-r--r--   0        0        0    10522 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/company_info/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/contacts/__init__.py
--rw-r--r--   0        0        0    17812 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/contacts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/credit_notes/__init__.py
--rw-r--r--   0        0        0    14782 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/credit_notes/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2137 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/expenses/__init__.py
--rw-r--r--   0        0        0    16471 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/expenses/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3050 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2819 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/income_statements/__init__.py
--rw-r--r--   0        0        0    10937 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/income_statements/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/invoices/__init__.py
--rw-r--r--   0        0        0    20058 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/invoices/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/issues/__init__.py
--rw-r--r--   0        0        0    10522 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/items/__init__.py
--rw-r--r--   0        0        0    13083 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/items/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/journal_entries/__init__.py
--rw-r--r--   0        0        0    16787 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/journal_entries/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8898 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10663 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7356 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/payments/__init__.py
--rw-r--r--   0        0        0    17271 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/payments/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/phone_numbers/__init__.py
--rw-r--r--   0        0        0     3281 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/phone_numbers/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/purchase_orders/__init__.py
--rw-r--r--   0        0        0    19114 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/purchase_orders/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2829 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8228 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3372 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/tax_rates/__init__.py
--rw-r--r--   0        0        0    10743 2023-07-21 19:21:23.772705 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/tax_rates/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/tracking_categories/__init__.py
--rw-r--r--   0        0        0    13333 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/tracking_categories/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/transactions/__init__.py
--rw-r--r--   0        0        0    12010 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/transactions/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/vendor_credits/__init__.py
--rw-r--r--   0        0        0    12034 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/vendor_credits/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5199 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    17717 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/__init__.py
--rw-r--r--   0        0        0    17393 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account.py
--rw-r--r--   0        0        0      195 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_classification.py
--rw-r--r--   0        0        0      171 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_currency.py
--rw-r--r--   0        0        0     1483 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_integration.py
--rw-r--r--   0        0        0    16986 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_request.py
--rw-r--r--   0        0        0      202 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_request_classification.py
--rw-r--r--   0        0        0      178 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_request_currency.py
--rw-r--r--   0        0        0      192 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_request_status.py
--rw-r--r--   0        0        0     1105 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_response.py
--rw-r--r--   0        0        0      185 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_status.py
--rw-r--r--   0        0        0      758 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_status_enum.py
--rw-r--r--   0        0        0      845 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_token.py
--rw-r--r--   0        0        0     1935 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_attachment.py
--rw-r--r--   0        0        0     1462 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_attachment_request.py
--rw-r--r--   0        0        0     1158 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_attachment_response.py
--rw-r--r--   0        0        0     1344 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_phone_number.py
--rw-r--r--   0        0        0     1346 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_phone_number_request.py
--rw-r--r--   0        0        0      819 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py
--rw-r--r--   0        0        0      831 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      835 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      847 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    11090 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/address.py
--rw-r--r--   0        0        0      167 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/address_country.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/address_type.py
--rw-r--r--   0        0        0      555 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/address_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/available_actions.py
--rw-r--r--   0        0        0    16903 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/balance_sheet.py
--rw-r--r--   0        0        0      176 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/balance_sheet_currency.py
--rw-r--r--   0        0        0    17216 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/cash_flow_statement.py
--rw-r--r--   0        0        0      181 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/cash_flow_statement_currency.py
--rw-r--r--   0        0        0     1391 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/category_enum.py
--rw-r--r--   0        0        0      560 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/category_type_enum.py
--rw-r--r--   0        0        0     1103 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/classification_enum.py
--rw-r--r--   0        0        0      997 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0    16863 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/company_info.py
--rw-r--r--   0        0        0      175 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/company_info_currency.py
--rw-r--r--   0        0        0      827 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/company_info_list_request_expand.py
--rw-r--r--   0        0        0      843 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py
--rw-r--r--   0        0        0     2324 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/condition_type_enum.py
--rw-r--r--   0        0        0     3027 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/contact.py
--rw-r--r--   0        0        0     2478 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/contact_request.py
--rw-r--r--   0        0        0      182 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/contact_request_status.py
--rw-r--r--   0        0        0     1105 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/contact_response.py
--rw-r--r--   0        0        0      175 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/contact_status.py
--rw-r--r--   0        0        0     1675 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/contacts_list_request_expand.py
--rw-r--r--   0        0        0     1707 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py
--rw-r--r--   0        0        0    35178 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/country_enum.py
--rw-r--r--   0        0        0    17747 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_note.py
--rw-r--r--   0        0        0      174 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_note_currency.py
--rw-r--r--   0        0        0     2275 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_note_line_item.py
--rw-r--r--   0        0        0      198 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_note_status.py
--rw-r--r--   0        0        0      784 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_note_status_enum.py
--rw-r--r--   0        0        0     1859 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_list_request_expand.py
--rw-r--r--   0        0        0      731 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py
--rw-r--r--   0        0        0      743 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1891 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py
--rw-r--r--   0        0        0      747 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      759 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    47961 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/currency_enum.py
--rw-r--r--   0        0        0      870 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/debug_model_log_summary.py
--rw-r--r--   0        0        0      522 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-21 19:21:23.776703 mergepythonclient-0.1.0/src/merge/resources/accounting/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/error_validation_problem.py
--rw-r--r--   0        0        0    16980 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense.py
--rw-r--r--   0        0        0      171 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_currency.py
--rw-r--r--   0        0        0     2074 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_line.py
--rw-r--r--   0        0        0     2076 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_line_request.py
--rw-r--r--   0        0        0    16445 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_request.py
--rw-r--r--   0        0        0      178 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_request_currency.py
--rw-r--r--   0        0        0     1105 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_response.py
--rw-r--r--   0        0        0     3715 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/expenses_list_request_expand.py
--rw-r--r--   0        0        0     3779 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py
--rw-r--r--   0        0        0    17240 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/income_statement.py
--rw-r--r--   0        0        0      179 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/income_statement_currency.py
--rw-r--r--   0        0        0    18003 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice.py
--rw-r--r--   0        0        0      171 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_currency.py
--rw-r--r--   0        0        0    16460 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_line_item.py
--rw-r--r--   0        0        0      179 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_line_item_currency.py
--rw-r--r--   0        0        0    16389 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_line_item_request.py
--rw-r--r--   0        0        0      186 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_line_item_request_currency.py
--rw-r--r--   0        0        0    17620 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_request.py
--rw-r--r--   0        0        0      178 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_request_currency.py
--rw-r--r--   0        0        0      184 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_request_type.py
--rw-r--r--   0        0        0     1105 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_response.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_type.py
--rw-r--r--   0        0        0      709 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_type_enum.py
--rw-r--r--   0        0        0     8275 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoices_list_request_expand.py
--rw-r--r--   0        0        0      622 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoices_list_request_type.py
--rw-r--r--   0        0        0     8403 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py
--rw-r--r--   0        0        0     1323 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/issues_list_request_status.py
--rw-r--r--   0        0        0     2624 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/item.py
--rw-r--r--   0        0        0      172 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/item_status.py
--rw-r--r--   0        0        0     1791 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/items_list_request_expand.py
--rw-r--r--   0        0        0     1823 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/items_retrieve_request_expand.py
--rw-r--r--   0        0        0     3771 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entries_list_request_expand.py
--rw-r--r--   0        0        0     3835 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py
--rw-r--r--   0        0        0    17164 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry.py
--rw-r--r--   0        0        0      176 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry_currency.py
--rw-r--r--   0        0        0      197 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry_posting_status.py
--rw-r--r--   0        0        0    16526 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry_request.py
--rw-r--r--   0        0        0      183 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry_request_currency.py
--rw-r--r--   0        0        0      204 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry_request_posting_status.py
--rw-r--r--   0        0        0     1126 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry_response.py
--rw-r--r--   0        0        0     1790 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_line.py
--rw-r--r--   0        0        0     1792 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_line_request.py
--rw-r--r--   0        0        0      835 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_account_list.py
--rw-r--r--   0        0        0      941 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py
--rw-r--r--   0        0        0      909 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_balance_sheet_list.py
--rw-r--r--   0        0        0      930 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py
--rw-r--r--   0        0        0      905 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_company_info_list.py
--rw-r--r--   0        0        0      921 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_contact_list.py
--rw-r--r--   0        0        0      901 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_credit_note_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_expense_list.py
--rw-r--r--   0        0        0      921 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_income_statement_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_invoice_list.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_issue_list.py
--rw-r--r--   0        0        0      876 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_item_list.py
--rw-r--r--   0        0        0      909 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_journal_entry_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_payment_list.py
--rw-r--r--   0        0        0      913 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_purchase_order_list.py
--rw-r--r--   0        0        0      901 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      889 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_tax_rate_list.py
--rw-r--r--   0        0        0      925 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_tracking_category_list.py
--rw-r--r--   0        0        0      904 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_transaction_list.py
--rw-r--r--   0        0        0      909 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_vendor_credit_list.py
--rw-r--r--   0        0        0    16832 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/payment.py
--rw-r--r--   0        0        0      171 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/payment_currency.py
--rw-r--r--   0        0        0    16241 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/payment_request.py
--rw-r--r--   0        0        0      178 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/payment_request_currency.py
--rw-r--r--   0        0        0     1105 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/payment_response.py
--rw-r--r--   0        0        0     3715 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/payments_list_request_expand.py
--rw-r--r--   0        0        0     3779 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/payments_retrieve_request_expand.py
--rw-r--r--   0        0        0      554 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/posting_status_enum.py
--rw-r--r--   0        0        0    17816 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_currency.py
--rw-r--r--   0        0        0    16830 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_line_item.py
--rw-r--r--   0        0        0      185 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_line_item_currency.py
--rw-r--r--   0        0        0    16854 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_line_item_request.py
--rw-r--r--   0        0        0      192 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_line_item_request_currency.py
--rw-r--r--   0        0        0    17041 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_request.py
--rw-r--r--   0        0        0      184 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_request_currency.py
--rw-r--r--   0        0        0      217 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_request_status.py
--rw-r--r--   0        0        0     1130 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_response.py
--rw-r--r--   0        0        0      210 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_status.py
--rw-r--r--   0        0        0     1154 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_status_enum.py
--rw-r--r--   0        0        0     9043 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py
--rw-r--r--   0        0        0     9171 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/remote_response.py
--rw-r--r--   0        0        0     1649 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/report_item.py
--rw-r--r--   0        0        0      723 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0      542 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/status_7_d_1_enum.py
--rw-r--r--   0        0        0     1411 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     2002 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/tax_rate.py
--rw-r--r--   0        0        0     2481 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/tracking_category.py
--rw-r--r--   0        0        0      197 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/tracking_category_category_type.py
--rw-r--r--   0        0        0      184 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/tracking_category_status.py
--rw-r--r--   0        0        0    17229 2023-07-21 19:21:23.780702 mergepythonclient-0.1.0/src/merge/resources/accounting/types/transaction.py
--rw-r--r--   0        0        0      175 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/transaction_currency.py
--rw-r--r--   0        0        0    16685 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/transaction_line_item.py
--rw-r--r--   0        0        0      183 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/transaction_line_item_currency.py
--rw-r--r--   0        0        0     3899 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/transactions_list_request_expand.py
--rw-r--r--   0        0        0     3963 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py
--rw-r--r--   0        0        0      762 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/validation_problem_source.py
--rw-r--r--   0        0        0    16901 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/vendor_credit.py
--rw-r--r--   0        0        0      176 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/vendor_credit_currency.py
--rw-r--r--   0        0        0     1999 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/vendor_credit_line.py
--rw-r--r--   0        0        0     3675 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py
--rw-r--r--   0        0        0     3739 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py
--rw-r--r--   0        0        0      915 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/accounting/types/webhook_receiver.py
--rw-r--r--   0        0        0     9656 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/__init__.py
--rw-r--r--   0        0        0    10018 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/client.py
--rw-r--r--   0        0        0     1144 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2416 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2656 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/activities/__init__.py
--rw-r--r--   0        0        0    18450 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/activities/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/applications/__init__.py
--rw-r--r--   0        0        0    22753 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/applications/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/attachments/__init__.py
--rw-r--r--   0        0        0    18326 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2494 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/candidates/__init__.py
--rw-r--r--   0        0        0    25052 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/candidates/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2159 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/departments/__init__.py
--rw-r--r--   0        0        0     9128 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/departments/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/eeocs/__init__.py
--rw-r--r--   0        0        0    13425 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/eeocs/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3072 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2841 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/interviews/__init__.py
--rw-r--r--   0        0        0    19472 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/interviews/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/issues/__init__.py
--rw-r--r--   0        0        0    10566 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/job_interview_stages/__init__.py
--rw-r--r--   0        0        0    10955 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/job_interview_stages/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/jobs/__init__.py
--rw-r--r--   0        0        0    14939 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/jobs/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8920 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10685 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/offers/__init__.py
--rw-r--r--   0        0        0    13609 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/offers/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/offices/__init__.py
--rw-r--r--   0        0        0     9042 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/offices/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7378 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2851 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/reject_reasons/__init__.py
--rw-r--r--   0        0        0     9178 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/reject_reasons/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/scorecards/__init__.py
--rw-r--r--   0        0        0    14473 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/scorecards/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8294 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3394 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/tags/__init__.py
--rw-r--r--   0        0        0     6731 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/users/__init__.py
--rw-r--r--   0        0        0    11995 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5243 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    13447 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/__init__.py
--rw-r--r--   0        0        0     1240 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/access_role_enum.py
--rw-r--r--   0        0        0     1483 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/account_token.py
--rw-r--r--   0        0        0      857 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activities_list_request_remote_fields.py
--rw-r--r--   0        0        0      869 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      873 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      885 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     2705 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activity.py
--rw-r--r--   0        0        0      189 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_activity_type.py
--rw-r--r--   0        0        0     2155 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_request.py
--rw-r--r--   0        0        0      196 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_request_activity_type.py
--rw-r--r--   0        0        0      187 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_request_visibility.py
--rw-r--r--   0        0        0     1109 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_response.py
--rw-r--r--   0        0        0      705 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_visibility.py
--rw-r--r--   0        0        0     2473 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/application.py
--rw-r--r--   0        0        0     2269 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/application_request.py
--rw-r--r--   0        0        0     1121 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/application_response.py
--rw-r--r--   0        0        0     8243 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/applications_list_request_expand.py
--rw-r--r--   0        0        0     8371 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/applications_retrieve_request_expand.py
--rw-r--r--   0        0        0     2146 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment.py
--rw-r--r--   0        0        0      199 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment_attachment_type.py
--rw-r--r--   0        0        0     1820 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment_request.py
--rw-r--r--   0        0        0      206 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment_request_attachment_type.py
--rw-r--r--   0        0        0     1117 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment_response.py
--rw-r--r--   0        0        0      985 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/available_actions.py
--rw-r--r--   0        0        0     3471 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/candidate.py
--rw-r--r--   0        0        0     3061 2023-07-21 19:21:23.784700 mergepythonclient-0.1.0/src/merge/resources/ats/types/candidate_request.py
--rw-r--r--   0        0        0     1113 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/candidate_response.py
--rw-r--r--   0        0        0      833 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/candidates_list_request_expand.py
--rw-r--r--   0        0        0      849 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
--rw-r--r--   0        0        0     1391 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/condition_type_enum.py
--rw-r--r--   0        0        0      870 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     1698 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/department.py
--rw-r--r--   0        0        0     1337 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/disability_status_enum.py
--rw-r--r--   0        0        0     4088 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/eeoc.py
--rw-r--r--   0        0        0      201 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/eeoc_disability_status.py
--rw-r--r--   0        0        0      160 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/eeoc_gender.py
--rw-r--r--   0        0        0      152 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/eeoc_race.py
--rw-r--r--   0        0        0      189 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/eeoc_veteran_status.py
--rw-r--r--   0        0        0     3803 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
--rw-r--r--   0        0        0     3851 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     3867 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     3915 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1529 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/email_address.py
--rw-r--r--   0        0        0      210 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/email_address_email_address_type.py
--rw-r--r--   0        0        0     1553 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/email_address_request.py
--rw-r--r--   0        0        0      217 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/email_address_request_email_address_type.py
--rw-r--r--   0        0        0      742 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/email_address_type_enum.py
--rw-r--r--   0        0        0      522 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/error_validation_problem.py
--rw-r--r--   0        0        0     1160 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/gender_enum.py
--rw-r--r--   0        0        0     4187 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/interviews_list_request_expand.py
--rw-r--r--   0        0        0     4251 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
--rw-r--r--   0        0        0     1323 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/issues_list_request_status.py
--rw-r--r--   0        0        0     3428 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/job.py
--rw-r--r--   0        0        0     2387 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/job_interview_stage.py
--rw-r--r--   0        0        0      169 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/job_status.py
--rw-r--r--   0        0        0     1045 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/job_status_enum.py
--rw-r--r--   0        0        0     3771 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/jobs_list_request_expand.py
--rw-r--r--   0        0        0      956 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/jobs_list_request_status.py
--rw-r--r--   0        0        0     3835 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0     2786 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/offer.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/offer_status.py
--rw-r--r--   0        0        0     1832 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/offer_status_enum.py
--rw-r--r--   0        0        0      767 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/offers_list_request_expand.py
--rw-r--r--   0        0        0      783 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/offers_retrieve_request_expand.py
--rw-r--r--   0        0        0     1817 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/office.py
--rw-r--r--   0        0        0      993 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/operator_schema.py
--rw-r--r--   0        0        0     1180 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/overall_recommendation_enum.py
--rw-r--r--   0        0        0      959 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      892 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_activity_list.py
--rw-r--r--   0        0        0      904 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_application_list.py
--rw-r--r--   0        0        0      900 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      896 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_candidate_list.py
--rw-r--r--   0        0        0      921 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      900 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_department_list.py
--rw-r--r--   0        0        0      876 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_eeoc_list.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_issue_list.py
--rw-r--r--   0        0        0      930 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
--rw-r--r--   0        0        0      872 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_job_list.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_offer_list.py
--rw-r--r--   0        0        0      884 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_office_list.py
--rw-r--r--   0        0        0      909 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_reject_reason_list.py
--rw-r--r--   0        0        0      901 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_remote_user_list.py
--rw-r--r--   0        0        0      933 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
--rw-r--r--   0        0        0      896 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_scorecard_list.py
--rw-r--r--   0        0        0      901 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_tag_list.py
--rw-r--r--   0        0        0     3068 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/patched_candidate_request.py
--rw-r--r--   0        0        0     1624 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/phone_number.py
--rw-r--r--   0        0        0      205 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/phone_number_phone_number_type.py
--rw-r--r--   0        0        0     1648 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/phone_number_request.py
--rw-r--r--   0        0        0      212 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
--rw-r--r--   0        0        0     1039 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/phone_number_type_enum.py
--rw-r--r--   0        0        0     2326 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/race_enum.py
--rw-r--r--   0        0        0      814 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/reason_enum.py
--rw-r--r--   0        0        0     1775 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/reject_reason.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_response_response_type.py
--rw-r--r--   0        0        0     2562 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_user.py
--rw-r--r--   0        0        0      183 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_user_access_role.py
--rw-r--r--   0        0        0      723 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/response_type_enum.py
--rw-r--r--   0        0        0     3187 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview.py
--rw-r--r--   0        0        0     2464 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview_request.py
--rw-r--r--   0        0        0      237 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview_request_status.py
--rw-r--r--   0        0        0     1150 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview_response.py
--rw-r--r--   0        0        0      230 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview_status.py
--rw-r--r--   0        0        0      893 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview_status_enum.py
--rw-r--r--   0        0        0     2692 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scorecard.py
--rw-r--r--   0        0        0      226 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scorecard_overall_recommendation.py
--rw-r--r--   0        0        0     1731 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scorecards_list_request_expand.py
--rw-r--r--   0        0        0     1763 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
--rw-r--r--   0        0        0      695 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1623 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/tag.py
--rw-r--r--   0        0        0     1659 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/url.py
--rw-r--r--   0        0        0     1683 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/url_request.py
--rw-r--r--   0        0        0      171 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/url_request_url_type.py
--rw-r--r--   0        0        0     1451 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/url_type_enum.py
--rw-r--r--   0        0        0      164 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/url_url_type.py
--rw-r--r--   0        0        0      762 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/validation_problem_source.py
--rw-r--r--   0        0        0     1467 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/veteran_status_enum.py
--rw-r--r--   0        0        0      760 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/visibility_enum.py
--rw-r--r--   0        0        0      915 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/ats/types/webhook_receiver.py
--rw-r--r--   0        0        0     9538 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/crm/__init__.py
--rw-r--r--   0        0        0     9931 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/crm/client.py
--rw-r--r--   0        0        0     1144 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/crm/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/crm/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2394 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/crm/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/crm/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2634 2023-07-21 19:21:23.788699 mergepythonclient-0.1.0/src/merge/resources/crm/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/accounts/__init__.py
--rw-r--r--   0        0        0    25839 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/association_types/__init__.py
--rw-r--r--   0        0        0    17150 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/association_types/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/associations/__init__.py
--rw-r--r--   0        0        0    12433 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/associations/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2472 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/contacts/__init__.py
--rw-r--r--   0        0        0    28151 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/contacts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/custom_object_classes/__init__.py
--rw-r--r--   0        0        0    13261 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/custom_object_classes/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/custom_objects/__init__.py
--rw-r--r--   0        0        0    22340 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/custom_objects/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2137 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/engagement_types/__init__.py
--rw-r--r--   0        0        0    14939 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/engagement_types/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/engagements/__init__.py
--rw-r--r--   0        0        0    25713 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/engagements/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3050 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2819 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/issues/__init__.py
--rw-r--r--   0        0        0    10522 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/leads/__init__.py
--rw-r--r--   0        0        0    22008 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/leads/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8898 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10663 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/notes/__init__.py
--rw-r--r--   0        0        0    22286 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/notes/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/opportunities/__init__.py
--rw-r--r--   0        0        0    30390 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/opportunities/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7356 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2829 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8228 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/stages/__init__.py
--rw-r--r--   0        0        0    14713 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/stages/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3372 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/tasks/__init__.py
--rw-r--r--   0        0        0    25263 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/tasks/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/users/__init__.py
--rw-r--r--   0        0        0    17118 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5199 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    13264 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/__init__.py
--rw-r--r--   0        0        0     2708 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/account.py
--rw-r--r--   0        0        0     1483 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/account_integration.py
--rw-r--r--   0        0        0     1916 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/account_request.py
--rw-r--r--   0        0        0      845 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/account_token.py
--rw-r--r--   0        0        0      719 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/activity_type_enum.py
--rw-r--r--   0        0        0    10978 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/address.py
--rw-r--r--   0        0        0      184 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/address_address_type.py
--rw-r--r--   0        0        0      167 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/address_country.py
--rw-r--r--   0        0        0    11024 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/address_request.py
--rw-r--r--   0        0        0      191 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/address_request_address_type.py
--rw-r--r--   0        0        0      174 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/address_request_country.py
--rw-r--r--   0        0        0      555 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/address_type_enum.py
--rw-r--r--   0        0        0     1226 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/association.py
--rw-r--r--   0        0        0      955 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/association_sub_type.py
--rw-r--r--   0        0        0     1663 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/association_type.py
--rw-r--r--   0        0        0      191 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/association_type_cardinality.py
--rw-r--r--   0        0        0     1335 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/association_type_request_request.py
--rw-r--r--   0        0        0     1245 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/available_actions.py
--rw-r--r--   0        0        0     1033 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/cardinality_enum.py
--rw-r--r--   0        0        0     1391 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/condition_type_enum.py
--rw-r--r--   0        0        0     2324 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/contact.py
--rw-r--r--   0        0        0     1944 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/contact_request.py
--rw-r--r--   0        0        0    35178 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/country_enum.py
--rw-r--r--   0        0        0     1108 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/crm_account_response.py
--rw-r--r--   0        0        0     1141 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/crm_association_type_response.py
--rw-r--r--   0        0        0     1108 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/crm_contact_response.py
--rw-r--r--   0        0        0     1129 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/crm_custom_object_response.py
--rw-r--r--   0        0        0     1399 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/custom_object.py
--rw-r--r--   0        0        0     1520 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/custom_object_class.py
--rw-r--r--   0        0        0      782 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/custom_object_request.py
--rw-r--r--   0        0        0      870 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/debug_model_log_summary.py
--rw-r--r--   0        0        0      549 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/direction_enum.py
--rw-r--r--   0        0        0     1317 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/email_address.py
--rw-r--r--   0        0        0     1319 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/email_address_request.py
--rw-r--r--   0        0        0      522 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/encoding_enum.py
--rw-r--r--   0        0        0     2645 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement.py
--rw-r--r--   0        0        0      178 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement_direction.py
--rw-r--r--   0        0        0     2216 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement_request.py
--rw-r--r--   0        0        0      185 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement_request_direction.py
--rw-r--r--   0        0        0     1117 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement_response.py
--rw-r--r--   0        0        0     1866 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement_type.py
--rw-r--r--   0        0        0      195 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement_type_activity_type.py
--rw-r--r--   0        0        0     3563 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/engagements_list_request_expand.py
--rw-r--r--   0        0        0     3627 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/engagements_retrieve_request_expand.py
--rw-r--r--   0        0        0      913 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/error_validation_problem.py
--rw-r--r--   0        0        0     1193 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/field_format_enum.py
--rw-r--r--   0        0        0     1179 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/field_type_enum.py
--rw-r--r--   0        0        0      999 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/ignore_common_model_request.py
--rw-r--r--   0        0        0     1323 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-21 19:21:23.792697 mergepythonclient-0.1.0/src/merge/resources/crm/types/issues_list_request_status.py
--rw-r--r--   0        0        0     1186 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/item_format_enum.py
--rw-r--r--   0        0        0      964 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/item_schema.py
--rw-r--r--   0        0        0     1172 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/item_type_enum.py
--rw-r--r--   0        0        0     2863 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/lead.py
--rw-r--r--   0        0        0     2369 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/lead_request.py
--rw-r--r--   0        0        0     1093 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/lead_response.py
--rw-r--r--   0        0        0     1851 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/leads_list_request_expand.py
--rw-r--r--   0        0        0     1883 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/leads_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0     2150 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/note.py
--rw-r--r--   0        0        0     1590 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/note_request.py
--rw-r--r--   0        0        0     1093 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/note_response.py
--rw-r--r--   0        0        0     3267 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/notes_list_request_expand.py
--rw-r--r--   0        0        0     3331 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/notes_retrieve_request_expand.py
--rw-r--r--   0        0        0      925 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/object_class_description_request.py
--rw-r--r--   0        0        0      993 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/operator_schema.py
--rw-r--r--   0        0        0     1475 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunities_list_request_expand.py
--rw-r--r--   0        0        0      665 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunities_list_request_status.py
--rw-r--r--   0        0        0     1507 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py
--rw-r--r--   0        0        0     2685 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity.py
--rw-r--r--   0        0        0     2243 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity_request.py
--rw-r--r--   0        0        0      208 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity_request_status.py
--rw-r--r--   0        0        0     1121 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity_response.py
--rw-r--r--   0        0        0      201 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity_status.py
--rw-r--r--   0        0        0      704 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity_status_enum.py
--rw-r--r--   0        0        0      893 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/origin_type_enum.py
--rw-r--r--   0        0        0      959 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_account_list.py
--rw-r--r--   0        0        0      904 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_association_list.py
--rw-r--r--   0        0        0      921 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_association_type_list.py
--rw-r--r--   0        0        0      921 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_contact_list.py
--rw-r--r--   0        0        0      930 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_custom_object_class_list.py
--rw-r--r--   0        0        0      909 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_custom_object_list.py
--rw-r--r--   0        0        0      900 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_engagement_list.py
--rw-r--r--   0        0        0      917 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_engagement_type_list.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_issue_list.py
--rw-r--r--   0        0        0      876 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_lead_list.py
--rw-r--r--   0        0        0      876 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_note_list.py
--rw-r--r--   0        0        0      904 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_opportunity_list.py
--rw-r--r--   0        0        0      926 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_remote_field_class_list.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_stage_list.py
--rw-r--r--   0        0        0      901 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_task_list.py
--rw-r--r--   0        0        0      876 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_user_list.py
--rw-r--r--   0        0        0     1923 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_account_request.py
--rw-r--r--   0        0        0     1951 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_contact_request.py
--rw-r--r--   0        0        0     2245 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_engagement_request.py
--rw-r--r--   0        0        0      192 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_engagement_request_direction.py
--rw-r--r--   0        0        0     2272 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_opportunity_request.py
--rw-r--r--   0        0        0      215 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_opportunity_request_status.py
--rw-r--r--   0        0        0     2029 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_task_request.py
--rw-r--r--   0        0        0      187 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_task_request_status.py
--rw-r--r--   0        0        0     1307 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/phone_number.py
--rw-r--r--   0        0        0     1309 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/phone_number_request.py
--rw-r--r--   0        0        0      814 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_data.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field.py
--rw-r--r--   0        0        0     1284 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_class.py
--rw-r--r--   0        0        0     1722 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py
--rw-r--r--   0        0        0      213 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_format.py
--rw-r--r--   0        0        0      205 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_type.py
--rw-r--r--   0        0        0      911 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py
--rw-r--r--   0        0        0      825 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_request.py
--rw-r--r--   0        0        0      986 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_response.py
--rw-r--r--   0        0        0      723 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1694 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/stage.py
--rw-r--r--   0        0        0     1411 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     2429 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/task.py
--rw-r--r--   0        0        0     2000 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/task_request.py
--rw-r--r--   0        0        0      180 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/task_request_status.py
--rw-r--r--   0        0        0     1093 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/task_response.py
--rw-r--r--   0        0        0      173 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/task_status.py
--rw-r--r--   0        0        0      517 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/task_status_enum.py
--rw-r--r--   0        0        0     1531 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/tasks_list_request_expand.py
--rw-r--r--   0        0        0     1563 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/tasks_retrieve_request_expand.py
--rw-r--r--   0        0        0     1894 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/user.py
--rw-r--r--   0        0        0      762 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/crm/types/webhook_receiver.py
--rw-r--r--   0        0        0    10290 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/__init__.py
--rw-r--r--   0        0        0     9511 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/client.py
--rw-r--r--   0        0        0     1106 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2418 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2658 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2496 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/bank_info/__init__.py
--rw-r--r--   0        0        0    15339 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/bank_info/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/benefits/__init__.py
--rw-r--r--   0        0        0    10821 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/benefits/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/companies/__init__.py
--rw-r--r--   0        0        0     9072 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/companies/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2161 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
--rw-r--r--   0        0        0    13612 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/employee_payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/employees/__init__.py
--rw-r--r--   0        0        0    30137 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/employees/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/employments/__init__.py
--rw-r--r--   0        0        0    14343 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/employments/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3074 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2843 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/groups/__init__.py
--rw-r--r--   0        0        0    11861 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/issues/__init__.py
--rw-r--r--   0        0        0    10570 2023-07-21 19:21:23.796695 mergepythonclient-0.1.0/src/merge/resources/hris/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8922 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10687 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/locations/__init__.py
--rw-r--r--   0        0        0    11629 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/locations/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7380 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/pay_groups/__init__.py
--rw-r--r--   0        0        0     9094 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/pay_groups/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/payroll_runs/__init__.py
--rw-r--r--   0        0        0    15544 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2853 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8300 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3396 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/teams/__init__.py
--rw-r--r--   0        0        0    10785 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/time_off/__init__.py
--rw-r--r--   0        0        0    22208 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/time_off/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/time_off_balances/__init__.py
--rw-r--r--   0        0        0    15538 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/time_off_balances/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5247 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    14549 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/account_token.py
--rw-r--r--   0        0        0      555 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/account_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/available_actions.py
--rw-r--r--   0        0        0     2399 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/bank_info.py
--rw-r--r--   0        0        0      185 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/bank_info_account_type.py
--rw-r--r--   0        0        0      529 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/bank_info_list_request_account_type.py
--rw-r--r--   0        0        0      728 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/bank_info_list_request_order_by.py
--rw-r--r--   0        0        0     2342 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/benefit.py
--rw-r--r--   0        0        0     1391 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     1962 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/company.py
--rw-r--r--   0        0        0     2324 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/condition_type_enum.py
--rw-r--r--   0        0        0    35178 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/country_enum.py
--rw-r--r--   0        0        0      870 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     2140 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/deduction.py
--rw-r--r--   0        0        0     2143 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/earning.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/earning_type.py
--rw-r--r--   0        0        0      949 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/earning_type_enum.py
--rw-r--r--   0        0        0     6788 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee.py
--rw-r--r--   0        0        0      205 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_employment_status.py
--rw-r--r--   0        0        0      176 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_ethnicity.py
--rw-r--r--   0        0        0      164 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_gender.py
--rw-r--r--   0        0        0      193 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_marital_status.py
--rw-r--r--   0        0        0     2796 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_payroll_run.py
--rw-r--r--   0        0        0      829 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
--rw-r--r--   0        0        0      845 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
--rw-r--r--   0        0        0     6252 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_request.py
--rw-r--r--   0        0        0      212 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_request_employment_status.py
--rw-r--r--   0        0        0      183 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_request_ethnicity.py
--rw-r--r--   0        0        0      171 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_request_gender.py
--rw-r--r--   0        0        0      200 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_request_marital_status.py
--rw-r--r--   0        0        0     1109 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_response.py
--rw-r--r--   0        0        0      739 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_list_request_employment_status.py
--rw-r--r--   0        0        0    80247 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_list_request_expand.py
--rw-r--r--   0        0        0     4067 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_list_request_remote_fields.py
--rw-r--r--   0        0        0     4115 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
--rw-r--r--   0        0        0    81343 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_retrieve_request_expand.py
--rw-r--r--   0        0        0     4131 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4179 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    18682 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employment.py
--rw-r--r--   0        0        0      199 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employment_employment_type.py
--rw-r--r--   0        0        0      183 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employment_flsa_status.py
--rw-r--r--   0        0        0      187 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employment_pay_currency.py
--rw-r--r--   0        0        0      191 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employment_pay_frequency.py
--rw-r--r--   0        0        0      179 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employment_pay_period.py
--rw-r--r--   0        0        0      770 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employment_status_enum.py
--rw-r--r--   0        0        0     1166 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employment_type_enum.py
--rw-r--r--   0        0        0      777 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_list_request_expand.py
--rw-r--r--   0        0        0      707 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_list_request_order_by.py
--rw-r--r--   0        0        0     4219 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_list_request_remote_fields.py
--rw-r--r--   0        0        0     4267 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      793 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_retrieve_request_expand.py
--rw-r--r--   0        0        0     4283 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4331 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      522 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/error_validation_problem.py
--rw-r--r--   0        0        0     2511 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/ethnicity_enum.py
--rw-r--r--   0        0        0      986 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/flsa_status_enum.py
--rw-r--r--   0        0        0     1146 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/gender_enum.py
--rw-r--r--   0        0        0     2225 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/group.py
--rw-r--r--   0        0        0      169 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/group_type.py
--rw-r--r--   0        0        0     1136 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/group_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/ignore_common_model_request_reason.py
--rw-r--r--   0        0        0     1323 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/issues_list_request_status.py
--rw-r--r--   0        0        0      835 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0    11870 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/location.py
--rw-r--r--   0        0        0      168 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/location_country.py
--rw-r--r--   0        0        0      189 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/location_location_type.py
--rw-r--r--   0        0        0      509 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/location_type_enum.py
--rw-r--r--   0        0        0     1685 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/marital_status_enum.py
--rw-r--r--   0        0        0     1037 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-21 19:21:23.800694 mergepythonclient-0.1.0/src/merge/resources/hris/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      893 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_bank_info_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_benefit_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_company_list.py
--rw-r--r--   0        0        0      921 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      892 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_employee_list.py
--rw-r--r--   0        0        0      934 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
--rw-r--r--   0        0        0      900 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_employment_list.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_group_list.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_issue_list.py
--rw-r--r--   0        0        0      892 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_location_list.py
--rw-r--r--   0        0        0      893 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_pay_group_list.py
--rw-r--r--   0        0        0      901 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_payroll_run_list.py
--rw-r--r--   0        0        0      901 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_team_list.py
--rw-r--r--   0        0        0      918 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_time_off_balance_list.py
--rw-r--r--   0        0        0      889 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_time_off_list.py
--rw-r--r--   0        0        0    48882 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/pay_currency_enum.py
--rw-r--r--   0        0        0     1940 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/pay_frequency_enum.py
--rw-r--r--   0        0        0     1754 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/pay_group.py
--rw-r--r--   0        0        0     1798 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/pay_period_enum.py
--rw-r--r--   0        0        0     2811 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_run.py
--rw-r--r--   0        0        0      175 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_run_run_state.py
--rw-r--r--   0        0        0      171 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_run_run_type.py
--rw-r--r--   0        0        0      801 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
--rw-r--r--   0        0        0     1104 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
--rw-r--r--   0        0        0      813 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      817 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      829 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1305 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/policy_type_enum.py
--rw-r--r--   0        0        0      814 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/remote_response_response_type.py
--rw-r--r--   0        0        0      723 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/request_format_enum.py
--rw-r--r--   0        0        0     1312 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/request_type_enum.py
--rw-r--r--   0        0        0      562 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/response_type_enum.py
--rw-r--r--   0        0        0     1032 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/run_state_enum.py
--rw-r--r--   0        0        0     1173 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/run_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1975 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/tax.py
--rw-r--r--   0        0        0     1953 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/team.py
--rw-r--r--   0        0        0     3481 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off.py
--rw-r--r--   0        0        0     2517 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_balance.py
--rw-r--r--   0        0        0      187 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_balance_policy_type.py
--rw-r--r--   0        0        0     1272 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
--rw-r--r--   0        0        0      751 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_expand.py
--rw-r--r--   0        0        0     1595 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
--rw-r--r--   0        0        0     1223 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_request_type.py
--rw-r--r--   0        0        0     1619 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1029 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_status.py
--rw-r--r--   0        0        0     3199 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_request.py
--rw-r--r--   0        0        0      191 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_request_request_type.py
--rw-r--r--   0        0        0      193 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_request_status.py
--rw-r--r--   0        0        0      184 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_request_type.py
--rw-r--r--   0        0        0      166 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_request_units.py
--rw-r--r--   0        0        0     1106 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_response.py
--rw-r--r--   0        0        0      767 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
--rw-r--r--   0        0        0     1627 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1651 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      186 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_status.py
--rw-r--r--   0        0        0     1146 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_status_enum.py
--rw-r--r--   0        0        0      159 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_units.py
--rw-r--r--   0        0        0      495 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/units_enum.py
--rw-r--r--   0        0        0      762 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/hris/types/webhook_receiver.py
--rw-r--r--   0        0        0     7030 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/__init__.py
--rw-r--r--   0        0        0     8338 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/client.py
--rw-r--r--   0        0        0      946 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2394 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2634 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/accounts/__init__.py
--rw-r--r--   0        0        0     9020 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/attachments/__init__.py
--rw-r--r--   0        0        0    17085 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2472 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/collections/__init__.py
--rw-r--r--   0        0        0    19110 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/collections/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/comments/__init__.py
--rw-r--r--   0        0        0    15411 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/comments/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/contacts/__init__.py
--rw-r--r--   0        0        0    10333 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/contacts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2137 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3050 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2819 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/issues/__init__.py
--rw-r--r--   0        0        0    10522 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8898 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10663 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7356 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/projects/__init__.py
--rw-r--r--   0        0        0    13470 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/projects/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2829 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8228 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3372 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/tags/__init__.py
--rw-r--r--   0        0        0     8930 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/teams/__init__.py
--rw-r--r--   0        0        0     8952 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/tickets/__init__.py
--rw-r--r--   0        0        0    41949 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/tickets/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/users/__init__.py
--rw-r--r--   0        0        0    10782 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5199 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0     9623 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/__init__.py
--rw-r--r--   0        0        0      743 2023-07-21 19:21:23.804692 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/access_level_enum.py
--rw-r--r--   0        0        0     1879 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account.py
--rw-r--r--   0        0        0     1483 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_token.py
--rw-r--r--   0        0        0     2201 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/attachment.py
--rw-r--r--   0        0        0     1716 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/attachment_request.py
--rw-r--r--   0        0        0     1245 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/available_actions.py
--rw-r--r--   0        0        0     1391 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/category_enum.py
--rw-r--r--   0        0        0     2535 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collection.py
--rw-r--r--   0        0        0      187 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collection_access_level.py
--rw-r--r--   0        0        0      199 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collection_collection_type.py
--rw-r--r--   0        0        0      536 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collection_type_enum.py
--rw-r--r--   0        0        0      527 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collections_list_request_collection_type.py
--rw-r--r--   0        0        0      727 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collections_users_list_request_expand.py
--rw-r--r--   0        0        0     2161 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comment.py
--rw-r--r--   0        0        0     1693 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comment_request.py
--rw-r--r--   0        0        0     1105 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comment_response.py
--rw-r--r--   0        0        0     1435 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comments_list_request_expand.py
--rw-r--r--   0        0        0     1467 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py
--rw-r--r--   0        0        0      997 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/condition_type_enum.py
--rw-r--r--   0        0        0     2024 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/contact.py
--rw-r--r--   0        0        0      870 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/debug_model_log_summary.py
--rw-r--r--   0        0        0      522 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/error_validation_problem.py
--rw-r--r--   0        0        0     1193 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/field_format_enum.py
--rw-r--r--   0        0        0     1179 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/field_type_enum.py
--rw-r--r--   0        0        0     1323 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/issues_list_request_status.py
--rw-r--r--   0        0        0     1186 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/item_format_enum.py
--rw-r--r--   0        0        0      964 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/item_schema.py
--rw-r--r--   0        0        0     1172 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/item_type_enum.py
--rw-r--r--   0        0        0      835 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_account_list.py
--rw-r--r--   0        0        0      900 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      900 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_collection_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_comment_list.py
--rw-r--r--   0        0        0      921 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_contact_list.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_issue_list.py
--rw-r--r--   0        0        0      888 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_project_list.py
--rw-r--r--   0        0        0      926 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py
--rw-r--r--   0        0        0      901 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_tag_list.py
--rw-r--r--   0        0        0      876 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_team_list.py
--rw-r--r--   0        0        0      884 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_ticket_list.py
--rw-r--r--   0        0        0      876 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_user_list.py
--rw-r--r--   0        0        0     3241 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/patched_ticket_request.py
--rw-r--r--   0        0        0      184 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/patched_ticket_request_priority.py
--rw-r--r--   0        0        0      195 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/patched_ticket_request_status.py
--rw-r--r--   0        0        0      843 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/priority_enum.py
--rw-r--r--   0        0        0     1704 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/project.py
--rw-r--r--   0        0        0      715 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/projects_users_list_request_expand.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_data.py
--rw-r--r--   0        0        0      880 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_field.py
--rw-r--r--   0        0        0     1284 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_field_class.py
--rw-r--r--   0        0        0      825 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_field_request.py
--rw-r--r--   0        0        0      986 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_response.py
--rw-r--r--   0        0        0      723 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1559 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tag.py
--rw-r--r--   0        0        0     1705 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/team.py
--rw-r--r--   0        0        0     3778 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket.py
--rw-r--r--   0        0        0      170 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_priority.py
--rw-r--r--   0        0        0     3258 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_request.py
--rw-r--r--   0        0        0      177 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_request_priority.py
--rw-r--r--   0        0        0      188 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_request_status.py
--rw-r--r--   0        0        0     1101 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_response.py
--rw-r--r--   0        0        0      181 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_status.py
--rw-r--r--   0        0        0      926 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_status_enum.py
--rw-r--r--   0        0        0     1126 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticketing_attachment_response.py
--rw-r--r--   0        0        0      743 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py
--rw-r--r--   0        0        0    37875 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_expand.py
--rw-r--r--   0        0        0      810 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_priority.py
--rw-r--r--   0        0        0     1635 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py
--rw-r--r--   0        0        0     1659 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      845 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_status.py
--rw-r--r--   0        0        0    38387 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py
--rw-r--r--   0        0        0     1667 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1691 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1949 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/user.py
--rw-r--r--   0        0        0      683 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/users_list_request_expand.py
--rw-r--r--   0        0        0      699 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/users_retrieve_request_expand.py
--rw-r--r--   0        0        0      762 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-21 19:21:23.808691 mergepythonclient-0.1.0/src/merge/resources/ticketing/types/webhook_receiver.py
--rw-r--r--   0        0        0     4947 1970-01-01 00:00:00.000000 mergepythonclient-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3274 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     4897 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/README.md
+-rw-r--r--   0        0        0      535 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/client.py
+-rw-r--r--   0        0        0      519 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/api_error.py
+-rw-r--r--   0        0        0     1113 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      201 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/environment.py
+-rw-r--r--   0        0        0        0 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/py.typed
+-rw-r--r--   0        0        0      178 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/__init__.py
+-rw-r--r--   0        0        0    12630 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/__init__.py
+-rw-r--r--   0        0        0    12026 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/client.py
+-rw-r--r--   0        0        0     1410 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2394 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2634 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    18106 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/addresses/__init__.py
+-rw-r--r--   0        0        0     4472 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/addresses/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    14525 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2472 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/balance_sheets/__init__.py
+-rw-r--r--   0        0        0    10863 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/balance_sheets/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/cash_flow_statements/__init__.py
+-rw-r--r--   0        0        0    10991 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/cash_flow_statements/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/company_info/__init__.py
+-rw-r--r--   0        0        0    10522 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/company_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/contacts/__init__.py
+-rw-r--r--   0        0        0    17812 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/contacts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/credit_notes/__init__.py
+-rw-r--r--   0        0        0    14782 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/credit_notes/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2137 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/expenses/__init__.py
+-rw-r--r--   0        0        0    16471 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/expenses/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3050 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2819 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/income_statements/__init__.py
+-rw-r--r--   0        0        0    10937 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/income_statements/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/invoices/__init__.py
+-rw-r--r--   0        0        0    20058 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/invoices/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10522 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/items/__init__.py
+-rw-r--r--   0        0        0    13083 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/items/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/journal_entries/__init__.py
+-rw-r--r--   0        0        0    16787 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/journal_entries/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8898 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10663 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7356 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/payments/__init__.py
+-rw-r--r--   0        0        0    17271 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/payments/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/phone_numbers/__init__.py
+-rw-r--r--   0        0        0     3281 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/phone_numbers/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/purchase_orders/__init__.py
+-rw-r--r--   0        0        0    19114 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/purchase_orders/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2829 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8228 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3372 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tax_rates/__init__.py
+-rw-r--r--   0        0        0    10743 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tax_rates/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tracking_categories/__init__.py
+-rw-r--r--   0        0        0    13333 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tracking_categories/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    12010 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/transactions/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/vendor_credits/__init__.py
+-rw-r--r--   0        0        0    12034 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/vendor_credits/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5199 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    17717 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/__init__.py
+-rw-r--r--   0        0        0    17393 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account.py
+-rw-r--r--   0        0        0      195 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_classification.py
+-rw-r--r--   0        0        0      171 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_currency.py
+-rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_integration.py
+-rw-r--r--   0        0        0    16986 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request.py
+-rw-r--r--   0        0        0      202 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request_classification.py
+-rw-r--r--   0        0        0      178 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request_currency.py
+-rw-r--r--   0        0        0      192 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request_status.py
+-rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_response.py
+-rw-r--r--   0        0        0      185 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_status.py
+-rw-r--r--   0        0        0      758 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_status_enum.py
+-rw-r--r--   0        0        0      845 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_token.py
+-rw-r--r--   0        0        0     1935 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment.py
+-rw-r--r--   0        0        0     1462 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment_request.py
+-rw-r--r--   0        0        0     1158 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment_response.py
+-rw-r--r--   0        0        0     1344 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_phone_number.py
+-rw-r--r--   0        0        0     1346 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_phone_number_request.py
+-rw-r--r--   0        0        0      819 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py
+-rw-r--r--   0        0        0      831 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      835 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      847 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    11090 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/address.py
+-rw-r--r--   0        0        0      167 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/address_country.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/address_type.py
+-rw-r--r--   0        0        0      555 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/address_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/available_actions.py
+-rw-r--r--   0        0        0    16903 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/balance_sheet.py
+-rw-r--r--   0        0        0      176 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/balance_sheet_currency.py
+-rw-r--r--   0        0        0    17216 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/cash_flow_statement.py
+-rw-r--r--   0        0        0      181 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/cash_flow_statement_currency.py
+-rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/category_enum.py
+-rw-r--r--   0        0        0      560 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/category_type_enum.py
+-rw-r--r--   0        0        0     1103 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/classification_enum.py
+-rw-r--r--   0        0        0      997 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0    16863 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info.py
+-rw-r--r--   0        0        0      175 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_currency.py
+-rw-r--r--   0        0        0      827 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_list_request_expand.py
+-rw-r--r--   0        0        0      843 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_type_enum.py
+-rw-r--r--   0        0        0     3027 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact.py
+-rw-r--r--   0        0        0     2478 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_request.py
+-rw-r--r--   0        0        0      182 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_request_status.py
+-rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_response.py
+-rw-r--r--   0        0        0      175 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_status.py
+-rw-r--r--   0        0        0     1675 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contacts_list_request_expand.py
+-rw-r--r--   0        0        0     1707 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py
+-rw-r--r--   0        0        0    35178 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/country_enum.py
+-rw-r--r--   0        0        0    17747 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note.py
+-rw-r--r--   0        0        0      174 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_currency.py
+-rw-r--r--   0        0        0     2275 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_line_item.py
+-rw-r--r--   0        0        0      198 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_status.py
+-rw-r--r--   0        0        0      784 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_status_enum.py
+-rw-r--r--   0        0        0     1859 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_expand.py
+-rw-r--r--   0        0        0      731 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py
+-rw-r--r--   0        0        0      743 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1891 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py
+-rw-r--r--   0        0        0      747 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      759 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    47961 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/currency_enum.py
+-rw-r--r--   0        0        0      870 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0      522 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/error_validation_problem.py
+-rw-r--r--   0        0        0    16980 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense.py
+-rw-r--r--   0        0        0      171 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_currency.py
+-rw-r--r--   0        0        0     2074 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_line.py
+-rw-r--r--   0        0        0     2076 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_line_request.py
+-rw-r--r--   0        0        0    16445 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_request.py
+-rw-r--r--   0        0        0      178 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_request_currency.py
+-rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_response.py
+-rw-r--r--   0        0        0     3715 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expenses_list_request_expand.py
+-rw-r--r--   0        0        0     3779 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py
+-rw-r--r--   0        0        0    17240 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/income_statement.py
+-rw-r--r--   0        0        0      179 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/income_statement_currency.py
+-rw-r--r--   0        0        0    18003 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice.py
+-rw-r--r--   0        0        0      171 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_currency.py
+-rw-r--r--   0        0        0    16460 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item.py
+-rw-r--r--   0        0        0      179 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item_currency.py
+-rw-r--r--   0        0        0    16389 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0      186 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item_request_currency.py
+-rw-r--r--   0        0        0    17620 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_request.py
+-rw-r--r--   0        0        0      178 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_request_currency.py
+-rw-r--r--   0        0        0      184 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_request_type.py
+-rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_response.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_type.py
+-rw-r--r--   0        0        0      709 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_type_enum.py
+-rw-r--r--   0        0        0     8275 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_list_request_expand.py
+-rw-r--r--   0        0        0      622 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_list_request_type.py
+-rw-r--r--   0        0        0     8403 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     2624 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/item.py
+-rw-r--r--   0        0        0      172 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/item_status.py
+-rw-r--r--   0        0        0     1791 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/items_list_request_expand.py
+-rw-r--r--   0        0        0     1823 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/items_retrieve_request_expand.py
+-rw-r--r--   0        0        0     3771 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entries_list_request_expand.py
+-rw-r--r--   0        0        0     3835 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py
+-rw-r--r--   0        0        0    17164 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry.py
+-rw-r--r--   0        0        0      176 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_currency.py
+-rw-r--r--   0        0        0      197 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_posting_status.py
+-rw-r--r--   0        0        0    16526 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_request.py
+-rw-r--r--   0        0        0      183 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_request_currency.py
+-rw-r--r--   0        0        0      204 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_request_posting_status.py
+-rw-r--r--   0        0        0     1126 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_response.py
+-rw-r--r--   0        0        0     1790 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_line.py
+-rw-r--r--   0        0        0     1792 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_line_request.py
+-rw-r--r--   0        0        0      835 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_account_list.py
+-rw-r--r--   0        0        0      941 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py
+-rw-r--r--   0        0        0      909 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_balance_sheet_list.py
+-rw-r--r--   0        0        0      930 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py
+-rw-r--r--   0        0        0      905 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_company_info_list.py
+-rw-r--r--   0        0        0      921 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_contact_list.py
+-rw-r--r--   0        0        0      901 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_credit_note_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_expense_list.py
+-rw-r--r--   0        0        0      921 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_income_statement_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_invoice_list.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      876 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_item_list.py
+-rw-r--r--   0        0        0      909 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_journal_entry_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_payment_list.py
+-rw-r--r--   0        0        0      913 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_purchase_order_list.py
+-rw-r--r--   0        0        0      901 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      889 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_tax_rate_list.py
+-rw-r--r--   0        0        0      925 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_tracking_category_list.py
+-rw-r--r--   0        0        0      904 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_transaction_list.py
+-rw-r--r--   0        0        0      909 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_vendor_credit_list.py
+-rw-r--r--   0        0        0    16832 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment.py
+-rw-r--r--   0        0        0      171 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_currency.py
+-rw-r--r--   0        0        0    16241 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_request.py
+-rw-r--r--   0        0        0      178 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_request_currency.py
+-rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_response.py
+-rw-r--r--   0        0        0     3715 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payments_list_request_expand.py
+-rw-r--r--   0        0        0     3779 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payments_retrieve_request_expand.py
+-rw-r--r--   0        0        0      554 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/posting_status_enum.py
+-rw-r--r--   0        0        0    17816 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_currency.py
+-rw-r--r--   0        0        0    16830 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item.py
+-rw-r--r--   0        0        0      185 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item_currency.py
+-rw-r--r--   0        0        0    16854 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item_request.py
+-rw-r--r--   0        0        0      192 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item_request_currency.py
+-rw-r--r--   0        0        0    17041 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_request.py
+-rw-r--r--   0        0        0      184 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_request_currency.py
+-rw-r--r--   0        0        0      217 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_request_status.py
+-rw-r--r--   0        0        0     1130 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_response.py
+-rw-r--r--   0        0        0      210 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_status.py
+-rw-r--r--   0        0        0     1154 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_status_enum.py
+-rw-r--r--   0        0        0     9043 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py
+-rw-r--r--   0        0        0     9171 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_response.py
+-rw-r--r--   0        0        0     1649 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/report_item.py
+-rw-r--r--   0        0        0      723 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0      542 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/status_7_d_1_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     2002 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/tax_rate.py
+-rw-r--r--   0        0        0     2481 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/tracking_category.py
+-rw-r--r--   0        0        0      197 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/tracking_category_category_type.py
+-rw-r--r--   0        0        0      184 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/tracking_category_status.py
+-rw-r--r--   0        0        0    17229 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction.py
+-rw-r--r--   0        0        0      175 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction_currency.py
+-rw-r--r--   0        0        0    16685 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction_line_item.py
+-rw-r--r--   0        0        0      183 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction_line_item_currency.py
+-rw-r--r--   0        0        0     3899 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transactions_list_request_expand.py
+-rw-r--r--   0        0        0     3963 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py
+-rw-r--r--   0        0        0      762 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/validation_problem_source.py
+-rw-r--r--   0        0        0    16901 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit.py
+-rw-r--r--   0        0        0      176 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit_currency.py
+-rw-r--r--   0        0        0     1999 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit_line.py
+-rw-r--r--   0        0        0     3675 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py
+-rw-r--r--   0        0        0     3739 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py
+-rw-r--r--   0        0        0      915 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/webhook_receiver.py
+-rw-r--r--   0        0        0     9656 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/__init__.py
+-rw-r--r--   0        0        0    10018 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/client.py
+-rw-r--r--   0        0        0     1144 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2416 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2656 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/activities/__init__.py
+-rw-r--r--   0        0        0    18450 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/activities/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/applications/__init__.py
+-rw-r--r--   0        0        0    22753 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/applications/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    18326 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/candidates/__init__.py
+-rw-r--r--   0        0        0    25052 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/candidates/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2159 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/departments/__init__.py
+-rw-r--r--   0        0        0     9128 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/departments/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/eeocs/__init__.py
+-rw-r--r--   0        0        0    13425 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/eeocs/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3072 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2841 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/interviews/__init__.py
+-rw-r--r--   0        0        0    19472 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/interviews/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10566 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/job_interview_stages/__init__.py
+-rw-r--r--   0        0        0    10955 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/job_interview_stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/jobs/__init__.py
+-rw-r--r--   0        0        0    14939 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/jobs/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8920 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10685 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/offers/__init__.py
+-rw-r--r--   0        0        0    13609 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/offers/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/offices/__init__.py
+-rw-r--r--   0        0        0     9042 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/offices/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7378 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2851 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/reject_reasons/__init__.py
+-rw-r--r--   0        0        0     9178 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/reject_reasons/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/scorecards/__init__.py
+-rw-r--r--   0        0        0    14473 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/scorecards/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8294 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3394 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/tags/__init__.py
+-rw-r--r--   0        0        0     6731 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/users/__init__.py
+-rw-r--r--   0        0        0    11995 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5243 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    13447 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/__init__.py
+-rw-r--r--   0        0        0     1240 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/access_role_enum.py
+-rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_token.py
+-rw-r--r--   0        0        0      857 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_list_request_remote_fields.py
+-rw-r--r--   0        0        0      869 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      873 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      885 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     2705 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity.py
+-rw-r--r--   0        0        0      189 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_activity_type.py
+-rw-r--r--   0        0        0     2155 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_request.py
+-rw-r--r--   0        0        0      196 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_request_activity_type.py
+-rw-r--r--   0        0        0      187 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_request_visibility.py
+-rw-r--r--   0        0        0     1109 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_response.py
+-rw-r--r--   0        0        0      705 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_visibility.py
+-rw-r--r--   0        0        0     2473 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/application.py
+-rw-r--r--   0        0        0     2269 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/application_request.py
+-rw-r--r--   0        0        0     1121 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/application_response.py
+-rw-r--r--   0        0        0     8243 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/applications_list_request_expand.py
+-rw-r--r--   0        0        0     8371 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/applications_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2146 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment.py
+-rw-r--r--   0        0        0      199 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_attachment_type.py
+-rw-r--r--   0        0        0     1820 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_request.py
+-rw-r--r--   0        0        0      206 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_request_attachment_type.py
+-rw-r--r--   0        0        0     1117 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_response.py
+-rw-r--r--   0        0        0      985 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/available_actions.py
+-rw-r--r--   0        0        0     3471 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate.py
+-rw-r--r--   0        0        0     3061 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate_request.py
+-rw-r--r--   0        0        0     1113 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate_response.py
+-rw-r--r--   0        0        0      833 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidates_list_request_expand.py
+-rw-r--r--   0        0        0      849 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_type_enum.py
+-rw-r--r--   0        0        0      870 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     1698 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/department.py
+-rw-r--r--   0        0        0     1337 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/disability_status_enum.py
+-rw-r--r--   0        0        0     4088 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc.py
+-rw-r--r--   0        0        0      201 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc_disability_status.py
+-rw-r--r--   0        0        0      160 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc_gender.py
+-rw-r--r--   0        0        0      152 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc_race.py
+-rw-r--r--   0        0        0      189 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc_veteran_status.py
+-rw-r--r--   0        0        0     3803 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     3851 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     3867 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     3915 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1529 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address.py
+-rw-r--r--   0        0        0      210 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_email_address_type.py
+-rw-r--r--   0        0        0     1553 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_request.py
+-rw-r--r--   0        0        0      217 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_request_email_address_type.py
+-rw-r--r--   0        0        0      742 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_type_enum.py
+-rw-r--r--   0        0        0      522 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1160 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/gender_enum.py
+-rw-r--r--   0        0        0     4187 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/interviews_list_request_expand.py
+-rw-r--r--   0        0        0     4251 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     3428 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/job.py
+-rw-r--r--   0        0        0     2387 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/job_interview_stage.py
+-rw-r--r--   0        0        0      169 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/job_status.py
+-rw-r--r--   0        0        0     1045 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/job_status_enum.py
+-rw-r--r--   0        0        0     3771 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_list_request_expand.py
+-rw-r--r--   0        0        0      956 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_list_request_status.py
+-rw-r--r--   0        0        0     3835 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0     2786 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offer.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offer_status.py
+-rw-r--r--   0        0        0     1832 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offer_status_enum.py
+-rw-r--r--   0        0        0      767 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offers_list_request_expand.py
+-rw-r--r--   0        0        0      783 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offers_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1817 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/office.py
+-rw-r--r--   0        0        0      993 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/operator_schema.py
+-rw-r--r--   0        0        0     1180 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/overall_recommendation_enum.py
+-rw-r--r--   0        0        0      959 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      892 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_activity_list.py
+-rw-r--r--   0        0        0      904 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_application_list.py
+-rw-r--r--   0        0        0      900 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      896 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_candidate_list.py
+-rw-r--r--   0        0        0      921 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      900 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_department_list.py
+-rw-r--r--   0        0        0      876 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_eeoc_list.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      930 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
+-rw-r--r--   0        0        0      872 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_job_list.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_offer_list.py
+-rw-r--r--   0        0        0      884 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_office_list.py
+-rw-r--r--   0        0        0      909 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_reject_reason_list.py
+-rw-r--r--   0        0        0      901 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_remote_user_list.py
+-rw-r--r--   0        0        0      933 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
+-rw-r--r--   0        0        0      896 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_scorecard_list.py
+-rw-r--r--   0        0        0      901 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_tag_list.py
+-rw-r--r--   0        0        0     3068 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/patched_candidate_request.py
+-rw-r--r--   0        0        0     1624 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number.py
+-rw-r--r--   0        0        0      205 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_phone_number_type.py
+-rw-r--r--   0        0        0     1648 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_request.py
+-rw-r--r--   0        0        0      212 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
+-rw-r--r--   0        0        0     1039 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_type_enum.py
+-rw-r--r--   0        0        0     2326 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/race_enum.py
+-rw-r--r--   0        0        0      814 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/reason_enum.py
+-rw-r--r--   0        0        0     1775 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/reject_reason.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_response_response_type.py
+-rw-r--r--   0        0        0     2562 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_user.py
+-rw-r--r--   0        0        0      183 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_user_access_role.py
+-rw-r--r--   0        0        0      723 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/response_type_enum.py
+-rw-r--r--   0        0        0     3187 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview.py
+-rw-r--r--   0        0        0     2464 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_request.py
+-rw-r--r--   0        0        0      237 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_request_status.py
+-rw-r--r--   0        0        0     1150 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_response.py
+-rw-r--r--   0        0        0      230 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_status.py
+-rw-r--r--   0        0        0      893 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_status_enum.py
+-rw-r--r--   0        0        0     2692 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecard.py
+-rw-r--r--   0        0        0      226 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecard_overall_recommendation.py
+-rw-r--r--   0        0        0     1731 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecards_list_request_expand.py
+-rw-r--r--   0        0        0     1763 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
+-rw-r--r--   0        0        0      695 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1623 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/tag.py
+-rw-r--r--   0        0        0     1659 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url.py
+-rw-r--r--   0        0        0     1683 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url_request.py
+-rw-r--r--   0        0        0      171 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url_request_url_type.py
+-rw-r--r--   0        0        0     1451 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url_type_enum.py
+-rw-r--r--   0        0        0      164 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url_url_type.py
+-rw-r--r--   0        0        0      762 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/validation_problem_source.py
+-rw-r--r--   0        0        0     1467 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/veteran_status_enum.py
+-rw-r--r--   0        0        0      760 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/visibility_enum.py
+-rw-r--r--   0        0        0      915 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/webhook_receiver.py
+-rw-r--r--   0        0        0     9538 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/__init__.py
+-rw-r--r--   0        0        0     9931 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/client.py
+-rw-r--r--   0        0        0     1144 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2394 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2634 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    25839 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/association_types/__init__.py
+-rw-r--r--   0        0        0    17150 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/association_types/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/associations/__init__.py
+-rw-r--r--   0        0        0    12433 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/associations/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2472 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/contacts/__init__.py
+-rw-r--r--   0        0        0    28151 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/contacts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_object_classes/__init__.py
+-rw-r--r--   0        0        0    13261 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_object_classes/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_objects/__init__.py
+-rw-r--r--   0        0        0    22340 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_objects/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2137 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagement_types/__init__.py
+-rw-r--r--   0        0        0    14939 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagement_types/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagements/__init__.py
+-rw-r--r--   0        0        0    25713 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagements/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3050 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2819 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10522 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/leads/__init__.py
+-rw-r--r--   0        0        0    22008 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/leads/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8898 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10663 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/notes/__init__.py
+-rw-r--r--   0        0        0    22286 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/notes/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/opportunities/__init__.py
+-rw-r--r--   0        0        0    30390 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/opportunities/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7356 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2829 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8228 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/stages/__init__.py
+-rw-r--r--   0        0        0    14713 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3372 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/tasks/__init__.py
+-rw-r--r--   0        0        0    25263 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/tasks/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/users/__init__.py
+-rw-r--r--   0        0        0    17118 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5199 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    13264 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/__init__.py
+-rw-r--r--   0        0        0     2708 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account.py
+-rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_integration.py
+-rw-r--r--   0        0        0     1916 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_request.py
+-rw-r--r--   0        0        0      845 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_token.py
+-rw-r--r--   0        0        0      719 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/activity_type_enum.py
+-rw-r--r--   0        0        0    10978 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address.py
+-rw-r--r--   0        0        0      184 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_address_type.py
+-rw-r--r--   0        0        0      167 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_country.py
+-rw-r--r--   0        0        0    11024 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_request.py
+-rw-r--r--   0        0        0      191 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_request_address_type.py
+-rw-r--r--   0        0        0      174 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_request_country.py
+-rw-r--r--   0        0        0      555 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_type_enum.py
+-rw-r--r--   0        0        0     1226 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association.py
+-rw-r--r--   0        0        0      955 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association_sub_type.py
+-rw-r--r--   0        0        0     1663 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type.py
+-rw-r--r--   0        0        0      191 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type_cardinality.py
+-rw-r--r--   0        0        0     1335 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type_request_request.py
+-rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/available_actions.py
+-rw-r--r--   0        0        0     1033 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/cardinality_enum.py
+-rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_type_enum.py
+-rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/contact.py
+-rw-r--r--   0        0        0     1944 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/contact_request.py
+-rw-r--r--   0        0        0    35178 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/country_enum.py
+-rw-r--r--   0        0        0     1108 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_account_response.py
+-rw-r--r--   0        0        0     1141 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_association_type_response.py
+-rw-r--r--   0        0        0     1108 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_contact_response.py
+-rw-r--r--   0        0        0     1129 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_custom_object_response.py
+-rw-r--r--   0        0        0     1399 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object.py
+-rw-r--r--   0        0        0     1520 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object_class.py
+-rw-r--r--   0        0        0      782 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object_request.py
+-rw-r--r--   0        0        0      870 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0      549 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/direction_enum.py
+-rw-r--r--   0        0        0     1317 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/email_address.py
+-rw-r--r--   0        0        0     1319 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/email_address_request.py
+-rw-r--r--   0        0        0      522 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/encoding_enum.py
+-rw-r--r--   0        0        0     2645 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement.py
+-rw-r--r--   0        0        0      178 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_direction.py
+-rw-r--r--   0        0        0     2216 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_request.py
+-rw-r--r--   0        0        0      185 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_request_direction.py
+-rw-r--r--   0        0        0     1117 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_response.py
+-rw-r--r--   0        0        0     1866 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_type.py
+-rw-r--r--   0        0        0      195 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_type_activity_type.py
+-rw-r--r--   0        0        0     3563 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagements_list_request_expand.py
+-rw-r--r--   0        0        0     3627 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagements_retrieve_request_expand.py
+-rw-r--r--   0        0        0      913 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1193 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/field_format_enum.py
+-rw-r--r--   0        0        0     1179 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/field_type_enum.py
+-rw-r--r--   0        0        0      999 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/ignore_common_model_request.py
+-rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     1186 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/item_format_enum.py
+-rw-r--r--   0        0        0      964 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/item_schema.py
+-rw-r--r--   0        0        0     1172 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/item_type_enum.py
+-rw-r--r--   0        0        0     2863 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/lead.py
+-rw-r--r--   0        0        0     2369 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/lead_request.py
+-rw-r--r--   0        0        0     1093 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/lead_response.py
+-rw-r--r--   0        0        0     1851 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/leads_list_request_expand.py
+-rw-r--r--   0        0        0     1883 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/leads_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0     2150 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/note.py
+-rw-r--r--   0        0        0     1590 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/note_request.py
+-rw-r--r--   0        0        0     1093 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/note_response.py
+-rw-r--r--   0        0        0     3267 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/notes_list_request_expand.py
+-rw-r--r--   0        0        0     3331 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/notes_retrieve_request_expand.py
+-rw-r--r--   0        0        0      925 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/object_class_description_request.py
+-rw-r--r--   0        0        0      993 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/operator_schema.py
+-rw-r--r--   0        0        0     1475 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_list_request_expand.py
+-rw-r--r--   0        0        0      665 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_list_request_status.py
+-rw-r--r--   0        0        0     1507 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2685 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity.py
+-rw-r--r--   0        0        0     2243 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_request.py
+-rw-r--r--   0        0        0      208 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_request_status.py
+-rw-r--r--   0        0        0     1121 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_response.py
+-rw-r--r--   0        0        0      201 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_status.py
+-rw-r--r--   0        0        0      704 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_status_enum.py
+-rw-r--r--   0        0        0      893 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/origin_type_enum.py
+-rw-r--r--   0        0        0      959 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_account_list.py
+-rw-r--r--   0        0        0      904 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_association_list.py
+-rw-r--r--   0        0        0      921 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_association_type_list.py
+-rw-r--r--   0        0        0      921 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_contact_list.py
+-rw-r--r--   0        0        0      930 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_custom_object_class_list.py
+-rw-r--r--   0        0        0      909 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_custom_object_list.py
+-rw-r--r--   0        0        0      900 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_engagement_list.py
+-rw-r--r--   0        0        0      917 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_engagement_type_list.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      876 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_lead_list.py
+-rw-r--r--   0        0        0      876 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_note_list.py
+-rw-r--r--   0        0        0      904 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_opportunity_list.py
+-rw-r--r--   0        0        0      926 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_remote_field_class_list.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_stage_list.py
+-rw-r--r--   0        0        0      901 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_task_list.py
+-rw-r--r--   0        0        0      876 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_user_list.py
+-rw-r--r--   0        0        0     1923 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_account_request.py
+-rw-r--r--   0        0        0     1951 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_contact_request.py
+-rw-r--r--   0        0        0     2245 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_engagement_request.py
+-rw-r--r--   0        0        0      192 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_engagement_request_direction.py
+-rw-r--r--   0        0        0     2272 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_opportunity_request.py
+-rw-r--r--   0        0        0      215 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_opportunity_request_status.py
+-rw-r--r--   0        0        0     2029 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_task_request.py
+-rw-r--r--   0        0        0      187 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_task_request_status.py
+-rw-r--r--   0        0        0     1307 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/phone_number.py
+-rw-r--r--   0        0        0     1309 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/phone_number_request.py
+-rw-r--r--   0        0        0      814 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_data.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field.py
+-rw-r--r--   0        0        0     1284 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class.py
+-rw-r--r--   0        0        0     1722 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py
+-rw-r--r--   0        0        0      213 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_format.py
+-rw-r--r--   0        0        0      205 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_type.py
+-rw-r--r--   0        0        0      911 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py
+-rw-r--r--   0        0        0      825 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_request.py
+-rw-r--r--   0        0        0      986 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_response.py
+-rw-r--r--   0        0        0      723 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1694 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/stage.py
+-rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     2429 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task.py
+-rw-r--r--   0        0        0     2000 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_request.py
+-rw-r--r--   0        0        0      180 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_request_status.py
+-rw-r--r--   0        0        0     1093 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_response.py
+-rw-r--r--   0        0        0      173 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_status.py
+-rw-r--r--   0        0        0      517 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_status_enum.py
+-rw-r--r--   0        0        0     1531 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/tasks_list_request_expand.py
+-rw-r--r--   0        0        0     1563 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/tasks_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1894 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/user.py
+-rw-r--r--   0        0        0      762 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/webhook_receiver.py
+-rw-r--r--   0        0        0    10290 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/__init__.py
+-rw-r--r--   0        0        0     9511 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/client.py
+-rw-r--r--   0        0        0     1106 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2418 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2658 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2496 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/bank_info/__init__.py
+-rw-r--r--   0        0        0    15339 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/bank_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/benefits/__init__.py
+-rw-r--r--   0        0        0    10821 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/benefits/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/companies/__init__.py
+-rw-r--r--   0        0        0     9072 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/companies/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2161 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
+-rw-r--r--   0        0        0    13612 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employee_payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employees/__init__.py
+-rw-r--r--   0        0        0    30137 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employees/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employments/__init__.py
+-rw-r--r--   0        0        0    14343 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employments/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3074 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2843 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/groups/__init__.py
+-rw-r--r--   0        0        0    11861 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10570 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8922 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10687 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/locations/__init__.py
+-rw-r--r--   0        0        0    11629 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/locations/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7380 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/pay_groups/__init__.py
+-rw-r--r--   0        0        0     9094 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/pay_groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/payroll_runs/__init__.py
+-rw-r--r--   0        0        0    15544 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8300 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3396 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/teams/__init__.py
+-rw-r--r--   0        0        0    10785 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off/__init__.py
+-rw-r--r--   0        0        0    22208 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off_balances/__init__.py
+-rw-r--r--   0        0        0    15538 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off_balances/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5247 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    14549 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_token.py
+-rw-r--r--   0        0        0      555 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/available_actions.py
+-rw-r--r--   0        0        0     2399 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info.py
+-rw-r--r--   0        0        0      185 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_account_type.py
+-rw-r--r--   0        0        0      529 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_list_request_account_type.py
+-rw-r--r--   0        0        0      728 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_list_request_order_by.py
+-rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/benefit.py
+-rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     1962 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/company.py
+-rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_type_enum.py
+-rw-r--r--   0        0        0    35178 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/country_enum.py
+-rw-r--r--   0        0        0      870 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     2140 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/deduction.py
+-rw-r--r--   0        0        0     2143 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/earning.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/earning_type.py
+-rw-r--r--   0        0        0      949 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/earning_type_enum.py
+-rw-r--r--   0        0        0     6788 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee.py
+-rw-r--r--   0        0        0      205 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_employment_status.py
+-rw-r--r--   0        0        0      176 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_ethnicity.py
+-rw-r--r--   0        0        0      164 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_gender.py
+-rw-r--r--   0        0        0      193 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_marital_status.py
+-rw-r--r--   0        0        0     2796 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_run.py
+-rw-r--r--   0        0        0      829 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
+-rw-r--r--   0        0        0      845 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
+-rw-r--r--   0        0        0     6252 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request.py
+-rw-r--r--   0        0        0      212 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request_employment_status.py
+-rw-r--r--   0        0        0      183 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request_ethnicity.py
+-rw-r--r--   0        0        0      171 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request_gender.py
+-rw-r--r--   0        0        0      200 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request_marital_status.py
+-rw-r--r--   0        0        0     1109 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_response.py
+-rw-r--r--   0        0        0      739 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_employment_status.py
+-rw-r--r--   0        0        0    80247 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_expand.py
+-rw-r--r--   0        0        0     4067 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4115 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0    81343 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4131 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4179 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    18682 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment.py
+-rw-r--r--   0        0        0      199 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_employment_type.py
+-rw-r--r--   0        0        0      183 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_flsa_status.py
+-rw-r--r--   0        0        0      187 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_pay_currency.py
+-rw-r--r--   0        0        0      191 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_pay_frequency.py
+-rw-r--r--   0        0        0      179 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_pay_period.py
+-rw-r--r--   0        0        0      770 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_status_enum.py
+-rw-r--r--   0        0        0     1166 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_type_enum.py
+-rw-r--r--   0        0        0      777 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_expand.py
+-rw-r--r--   0        0        0      707 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_order_by.py
+-rw-r--r--   0        0        0     4219 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4267 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      793 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4283 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4331 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      522 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/error_validation_problem.py
+-rw-r--r--   0        0        0     2511 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/ethnicity_enum.py
+-rw-r--r--   0        0        0      986 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/flsa_status_enum.py
+-rw-r--r--   0        0        0     1146 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/gender_enum.py
+-rw-r--r--   0        0        0     2225 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/group.py
+-rw-r--r--   0        0        0      169 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/group_type.py
+-rw-r--r--   0        0        0     1136 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/group_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/ignore_common_model_request_reason.py
+-rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/issues_list_request_status.py
+-rw-r--r--   0        0        0      835 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0    11870 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/location.py
+-rw-r--r--   0        0        0      168 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/location_country.py
+-rw-r--r--   0        0        0      189 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/location_location_type.py
+-rw-r--r--   0        0        0      509 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/location_type_enum.py
+-rw-r--r--   0        0        0     1685 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/marital_status_enum.py
+-rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      893 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_bank_info_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_benefit_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_company_list.py
+-rw-r--r--   0        0        0      921 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      892 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employee_list.py
+-rw-r--r--   0        0        0      934 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
+-rw-r--r--   0        0        0      900 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employment_list.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_group_list.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      892 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_location_list.py
+-rw-r--r--   0        0        0      893 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_pay_group_list.py
+-rw-r--r--   0        0        0      901 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_payroll_run_list.py
+-rw-r--r--   0        0        0      901 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_team_list.py
+-rw-r--r--   0        0        0      918 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_time_off_balance_list.py
+-rw-r--r--   0        0        0      889 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_time_off_list.py
+-rw-r--r--   0        0        0    48882 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_currency_enum.py
+-rw-r--r--   0        0        0     1940 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_frequency_enum.py
+-rw-r--r--   0        0        0     1754 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_group.py
+-rw-r--r--   0        0        0     1798 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_period_enum.py
+-rw-r--r--   0        0        0     2811 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_run.py
+-rw-r--r--   0        0        0      175 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_run_run_state.py
+-rw-r--r--   0        0        0      171 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_run_run_type.py
+-rw-r--r--   0        0        0      801 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1104 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
+-rw-r--r--   0        0        0      813 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      817 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      829 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1305 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/policy_type_enum.py
+-rw-r--r--   0        0        0      814 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_response_response_type.py
+-rw-r--r--   0        0        0      723 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/request_format_enum.py
+-rw-r--r--   0        0        0     1312 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/request_type_enum.py
+-rw-r--r--   0        0        0      562 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/response_type_enum.py
+-rw-r--r--   0        0        0     1032 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/run_state_enum.py
+-rw-r--r--   0        0        0     1173 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/run_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1975 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/tax.py
+-rw-r--r--   0        0        0     1953 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/team.py
+-rw-r--r--   0        0        0     3481 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off.py
+-rw-r--r--   0        0        0     2517 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balance.py
+-rw-r--r--   0        0        0      187 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balance_policy_type.py
+-rw-r--r--   0        0        0     1272 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
+-rw-r--r--   0        0        0      751 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_expand.py
+-rw-r--r--   0        0        0     1595 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1223 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_request_type.py
+-rw-r--r--   0        0        0     1619 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1029 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_status.py
+-rw-r--r--   0        0        0     3199 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request.py
+-rw-r--r--   0        0        0      191 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request_request_type.py
+-rw-r--r--   0        0        0      193 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request_status.py
+-rw-r--r--   0        0        0      184 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request_type.py
+-rw-r--r--   0        0        0      166 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request_units.py
+-rw-r--r--   0        0        0     1106 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_response.py
+-rw-r--r--   0        0        0      767 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1627 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1651 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      186 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_status.py
+-rw-r--r--   0        0        0     1146 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_status_enum.py
+-rw-r--r--   0        0        0      159 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_units.py
+-rw-r--r--   0        0        0      495 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/units_enum.py
+-rw-r--r--   0        0        0      762 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/webhook_receiver.py
+-rw-r--r--   0        0        0     7030 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/__init__.py
+-rw-r--r--   0        0        0     8338 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/client.py
+-rw-r--r--   0        0        0      946 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2394 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2634 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/accounts/__init__.py
+-rw-r--r--   0        0        0     9020 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    17085 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2472 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/collections/__init__.py
+-rw-r--r--   0        0        0    19110 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/collections/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/comments/__init__.py
+-rw-r--r--   0        0        0    15411 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/comments/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/contacts/__init__.py
+-rw-r--r--   0        0        0    10333 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/contacts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2137 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3050 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2819 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10522 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8898 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10663 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7356 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/projects/__init__.py
+-rw-r--r--   0        0        0    13470 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/projects/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2829 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8228 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3372 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tags/__init__.py
+-rw-r--r--   0        0        0     8930 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/teams/__init__.py
+-rw-r--r--   0        0        0     8952 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tickets/__init__.py
+-rw-r--r--   0        0        0    41949 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tickets/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/users/__init__.py
+-rw-r--r--   0        0        0    10782 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5199 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0     9623 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/access_level_enum.py
+-rw-r--r--   0        0        0     1879 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account.py
+-rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_token.py
+-rw-r--r--   0        0        0     2201 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/attachment.py
+-rw-r--r--   0        0        0     1716 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/attachment_request.py
+-rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/available_actions.py
+-rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/category_enum.py
+-rw-r--r--   0        0        0     2535 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection.py
+-rw-r--r--   0        0        0      187 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection_access_level.py
+-rw-r--r--   0        0        0      199 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection_collection_type.py
+-rw-r--r--   0        0        0      536 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection_type_enum.py
+-rw-r--r--   0        0        0      527 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collections_list_request_collection_type.py
+-rw-r--r--   0        0        0      727 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collections_users_list_request_expand.py
+-rw-r--r--   0        0        0     2161 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment.py
+-rw-r--r--   0        0        0     1693 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment_request.py
+-rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment_response.py
+-rw-r--r--   0        0        0     1435 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comments_list_request_expand.py
+-rw-r--r--   0        0        0     1467 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py
+-rw-r--r--   0        0        0      997 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_type_enum.py
+-rw-r--r--   0        0        0     2024 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/contact.py
+-rw-r--r--   0        0        0      870 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0      522 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1193 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/field_format_enum.py
+-rw-r--r--   0        0        0     1179 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/field_type_enum.py
+-rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     1186 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_format_enum.py
+-rw-r--r--   0        0        0      964 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_schema.py
+-rw-r--r--   0        0        0     1172 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_type_enum.py
+-rw-r--r--   0        0        0      835 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_account_list.py
+-rw-r--r--   0        0        0      900 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      900 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_collection_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_comment_list.py
+-rw-r--r--   0        0        0      921 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_contact_list.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      888 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_project_list.py
+-rw-r--r--   0        0        0      926 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py
+-rw-r--r--   0        0        0      901 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_tag_list.py
+-rw-r--r--   0        0        0      876 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_team_list.py
+-rw-r--r--   0        0        0      884 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_ticket_list.py
+-rw-r--r--   0        0        0      876 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_user_list.py
+-rw-r--r--   0        0        0     3241 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/patched_ticket_request.py
+-rw-r--r--   0        0        0      184 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/patched_ticket_request_priority.py
+-rw-r--r--   0        0        0      195 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/patched_ticket_request_status.py
+-rw-r--r--   0        0        0      843 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/priority_enum.py
+-rw-r--r--   0        0        0     1704 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/project.py
+-rw-r--r--   0        0        0      715 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/projects_users_list_request_expand.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_data.py
+-rw-r--r--   0        0        0      880 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field.py
+-rw-r--r--   0        0        0     1284 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field_class.py
+-rw-r--r--   0        0        0      825 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field_request.py
+-rw-r--r--   0        0        0      986 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_response.py
+-rw-r--r--   0        0        0      723 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1559 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tag.py
+-rw-r--r--   0        0        0     1705 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/team.py
+-rw-r--r--   0        0        0     3778 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket.py
+-rw-r--r--   0        0        0      170 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_priority.py
+-rw-r--r--   0        0        0     3258 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_request.py
+-rw-r--r--   0        0        0      177 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_request_priority.py
+-rw-r--r--   0        0        0      188 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_request_status.py
+-rw-r--r--   0        0        0     1101 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_response.py
+-rw-r--r--   0        0        0      181 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_status.py
+-rw-r--r--   0        0        0      926 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_status_enum.py
+-rw-r--r--   0        0        0     1126 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticketing_attachment_response.py
+-rw-r--r--   0        0        0      743 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py
+-rw-r--r--   0        0        0    37875 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_expand.py
+-rw-r--r--   0        0        0      810 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_priority.py
+-rw-r--r--   0        0        0     1635 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1659 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      845 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_status.py
+-rw-r--r--   0        0        0    38387 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1667 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1691 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1949 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/user.py
+-rw-r--r--   0        0        0      683 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/users_list_request_expand.py
+-rw-r--r--   0        0        0      699 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/users_retrieve_request_expand.py
+-rw-r--r--   0        0        0      762 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/webhook_receiver.py
+-rw-r--r--   0        0        0     5686 1970-01-01 00:00:00.000000 mergepythonclient-0.1.1/PKG-INFO
```

### Comparing `mergepythonclient-0.1.0/LICENSE.md` & `mergepythonclient-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/README.md` & `mergepythonclient-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-
 # Merge Python Library
 
-[![pypi](https://img.shields.io/pypi/v/fern-merge.svg)](https://pypi.python.org/pypi/fern-merge)
+[![pypi](https://img.shields.io/pypi/v/MergePythonClient.svg)](https://pypi.python.org/pypi/MergePythonClient)
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
 
 The Merge Python library provides access to the Merge API from Python.
 
 ## Documentation
 
 API reference documentation is available [here](https://docs.merge.dev/).
@@ -18,133 +17,156 @@
 
 ## Instantiation
 
 ```python
 import merge
 from merge.client import Merge
 
-client = Merge(api_key="YOUR_API_KEY", account_token="YOUR_ACCOUNT_TOKEN")
+client = Merge(api_key="Bearer YOUR_API_KEY", account_token="YOUR_ACCOUNT_TOKEN")
 ```
 
 ## Categories
 
 This SDK contains both the ATS, HRIS, CRM, Ticketing, and Accounting categories. Even if you do not plan on using more than one Merge API category right now, the SDK provides upgrade-flexibility in case you find new Merge API categories useful in the future.
 
-Each category is namespaced: 
+Each category is namespaced:
+
 ```python
-client = Merge(api_key="YOUR_API_KEY")
+client = Merge(api_key="Bearer YOUR_API_KEY")
 
 client.ats. # APIs specific to the ATS Category
 
 client.hris. # APIs specific to the HRIS Category
 ```
 
-## Usage 
+## Usage
 
-## Create Link Token 
+## Create Link Token
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 link_token_response = merge_client.ats.link_token.create(
     end_user_email_address="john.smith@gmail.com",
     end_user_organization_name="acme",
     end_user_origin_id="1234",
     categories=[CategoriesEnum.ATS],
     link_expiry_mins=30,
 )
 
 print("Created link token", link_token_response.link_token)
 ```
 
-## Get Employee 
+## Get Employee
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 employee = merge_client.hris.employees.retrieve(
     id="0958cbc6-6040-430a-848e-aafacbadf4ae")
 ```
 
-## Get Candidate 
+## Get Candidate
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 candidate = merge_client.ats.candiates.retrieve(
     id="521b18c2-4d01-4297-b451-19858d07c133")
 ```
 
-## Filter Candidate 
+## Filter Candidate
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 candidates_response = merge_client.ats.candidates.list(
     created_after="2030-01-01")
 
 print(candidates_response.result)
 ```
 
-## Get Contact 
+## Get Contact
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 contact = merge_client.accounting.contacts.retrieve(
     id="c640b80b-fac9-409f-aa19-1f9221aec445")
 ```
 
 ## Create Ticket
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 merge_client.ticketing.tickets.create(
     model=merge.ticketing.TicketRequest(
         name="Please add more integrations",
         assignees=[
             "17a54124-287f-494d-965e-3c5b330c9a68"
         ],
         creator="3fa85f64-5717-4562-b3fc-2c963f66afa6",
         due_date="2022-10-11T00:00:00Z",
         status=merge.ticketing.TicketRequestStatus.OPEN,
     ))
 ```
 
+## Pagination
+
+The SDK may return paginated results. Endpoints that return paginated results will 
+include a `next` and `prev` property on the response. To get the next page, you can 
+pass in the value of `next` to the cursor property on the request. Similarly, to 
+get the previous page, you can pass in the value of `prev` to the cursor property on 
+the request. 
+
+Below is an example of iterating over all pages:
+```python
+
+# response contains the first page
+response = merge_client.hris.employees.list(created_after="2030-01-01")
+
+# if there is a next page, load it by passing `next` to the cursor argument
+while response.next is not None:
+    response = hris_client.employees.list(
+        cursor=response.next, 
+        created_after="2030-01-01")
+```
+
+
 ## Beta status
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning the package version to a specific version in your package.json file. This way, you can install the same version each time without breaking changes unless you are intentionally looking for the latest version.
 
 ## Contributing
 
 While we value open-source contributions to this SDK, this library is generated programmatically. Additions made directly to this library would have to be moved over to our generation code, otherwise they would be overwritten upon the next generated release. Feel free to open a PR as a proof of concept, but know that we will not be able to merge it as-is. We suggest opening an issue first to discuss with us!
```

### Comparing `mergepythonclient-0.1.0/pyproject.toml` & `mergepythonclient-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MergePythonClient"
-version = "0.1.0"
+version = "0.1.1"
 description = "Client library for the merge API"
 readme = "README.md"
 authors = ["Merge <hello@merge.dev>"]
 license = "custom"
 repository = "https://github.com/merge-api/merge-python-client"
 packages = [
     { include = "merge", from = "src"}
```

### Comparing `mergepythonclient-0.1.0/src/merge/client.py` & `mergepythonclient-0.1.1/src/merge/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/core/__init__.py` & `mergepythonclient-0.1.1/src/merge/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/core/client_wrapper.py` & `mergepythonclient-0.1.1/src/merge/core/client_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._account_token = account_token
         self.api_key = api_key
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {}
         if self._account_token is not None:
             headers["X-Account-Token"] = self._account_token
-        headers["Authorization"] = self.api_key
+        headers["Authorization"] = f"Bearer {self.api_key}"
         return headers
 
 
 class SyncClientWrapper(BaseClientWrapper):
     def __init__(self, *, account_token: typing.Optional[str] = None, api_key: str, httpx_client: httpx.Client):
         super().__init__(account_token=account_token, api_key=api_key)
         self.httpx_client = httpx_client
```

### Comparing `mergepythonclient-0.1.0/src/merge/core/datetime_utils.py` & `mergepythonclient-0.1.1/src/merge/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/core/jsonable_encoder.py` & `mergepythonclient-0.1.1/src/merge/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/account_details/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/account_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/accounts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/accounts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/addresses/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/addresses/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/attachments/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/available_actions/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/balance_sheets/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/balance_sheets/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/cash_flow_statements/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/cash_flow_statements/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/company_info/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/company_info/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/contacts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/contacts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/credit_notes/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/credit_notes/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/delete_account/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/expenses/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/expenses/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/force_resync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/generate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/income_statements/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/income_statements/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/invoices/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/invoices/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/issues/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/items/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/items/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/journal_entries/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/journal_entries/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/link_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/linked_accounts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/passthrough/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/payments/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/payments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/phone_numbers/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/phone_numbers/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/purchase_orders/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/purchase_orders/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/regenerate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/selective_sync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/sync_status/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/tax_rates/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tax_rates/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/tracking_categories/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tracking_categories/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/transactions/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/transactions/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/vendor_credits/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/vendor_credits/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_details.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_details_and_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/account_token.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_attachment.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_attachment_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_attachment_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_phone_number.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_phone_number.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounting_phone_number_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_phone_number_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/address.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/address.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/address_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/address_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/available_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/balance_sheet.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/cash_flow_statement.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/categories_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/category_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/category_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/category_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/classification_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/classification_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/company_info.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/company_info_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/condition_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/condition_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/contact.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/contact_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/contact_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/contacts_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contacts_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/country_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_note.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_note_line_item.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_line_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_note_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/currency_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/currency_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/debug_mode_log.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/debug_model_log_summary.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/enabled_actions_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/encoding_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/error_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_line.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_line.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_line_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_line_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/expense_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/expenses_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expenses_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/income_statement.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/income_statement.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_line_item.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_line_item_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoice_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoices_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoices_list_request_type.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_list_request_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/issue.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/issue_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/item.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/items_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/items_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/items_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/items_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entries_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entries_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_entry_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_line.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_line.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/journal_line_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_line_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/link_token.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_condition.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_condition_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_account_status.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/meta_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/method_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/model_operation.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/multipart_form_field_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/operator_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_account_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_account_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_balance_sheet_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_balance_sheet_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_company_info_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_company_info_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_contact_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_contact_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_credit_note_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_credit_note_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_expense_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_expense_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_income_statement_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_income_statement_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_invoice_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_invoice_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_issue_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_item_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_item_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_journal_entry_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_journal_entry_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_payment_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_payment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_purchase_order_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_purchase_order_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_tax_rate_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_tax_rate_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_tracking_category_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_tracking_category_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_transaction_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_transaction_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/paginated_vendor_credit_list.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_vendor_credit_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/payment.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/payment_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/payment_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/payments_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/payments_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/posting_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/posting_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_line_item.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_line_item_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_request.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_order_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/remote_data.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/remote_key.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/remote_response.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/report_item.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/report_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/request_format_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/response_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/status_7_d_1_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/status_7_d_1_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/sync_status.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/sync_status_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/tax_rate.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/tax_rate.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/tracking_category.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/tracking_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/transaction.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/transaction_line_item.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction_line_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/transactions_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/transactions_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/validation_problem_source.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/vendor_credit.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/vendor_credit_line.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit_line.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/warning_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/accounting/types/webhook_receiver.py` & `mergepythonclient-0.1.1/src/merge/resources/accounting/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/account_details/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/account_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/activities/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/activities/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/applications/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/applications/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/attachments/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/available_actions/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/candidates/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/candidates/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/delete_account/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/departments/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/departments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/eeocs/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/eeocs/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/force_resync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/generate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/interviews/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/interviews/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/issues/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/job_interview_stages/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/job_interview_stages/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/jobs/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/jobs/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/link_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/linked_accounts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/offers/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/offers/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/offices/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/offices/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/passthrough/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/regenerate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/reject_reasons/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/reject_reasons/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/scorecards/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/scorecards/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/selective_sync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/sync_status/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/tags/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/users/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/access_role_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/access_role_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/account_details.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/account_details_and_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/account_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/account_token.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/activities_list_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/activity.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/activity.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/activity_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/application.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/application.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/application_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/application_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/application_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/application_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/applications_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/applications_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/applications_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/applications_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/attachment_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/available_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/candidate.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/candidate_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/candidate_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/candidates_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidates_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/candidates_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidates_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/categories_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/category_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/condition_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/condition_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/debug_mode_log.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/debug_model_log_summary.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/department.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/department.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/disability_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/disability_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/eeoc.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/email_address.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/email_address_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/email_address_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/enabled_actions_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/encoding_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/error_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/gender_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/interviews_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/interviews_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/interviews_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/interviews_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/issue.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/issue_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/job.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/job.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/job_interview_stage.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/job_interview_stage.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/job_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/job_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/jobs_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/jobs_list_request_status.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_list_request_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/jobs_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/link_token.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_condition.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_condition_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_account_status.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/meta_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/method_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/model_operation.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/multipart_form_field_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/offer.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/offer.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/offer_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/offer_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/offers_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/offers_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/offers_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/offers_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/office.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/office.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/operator_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/overall_recommendation_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/overall_recommendation_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_activity_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_activity_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_application_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_attachment_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_candidate_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_candidate_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_department_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_department_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_eeoc_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_eeoc_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_issue_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_job_interview_stage_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_job_interview_stage_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_job_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_job_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_offer_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_offer_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_office_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_office_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_reject_reason_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_reject_reason_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_remote_user_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_remote_user_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_scheduled_interview_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_scheduled_interview_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_scorecard_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_scorecard_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/paginated_tag_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/patched_candidate_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/patched_candidate_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/phone_number.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/phone_number_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/phone_number_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/race_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/race_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/reason_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/reject_reason.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/reject_reason.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_data.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_key.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/remote_user.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_user.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/request_format_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/response_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/scheduled_interview_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/scorecard.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecard.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/scorecards_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecards_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/sync_status.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/sync_status_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/tag.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/tag.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/url.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/url.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/url_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/url_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/url_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/url_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/validation_problem_source.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/veteran_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/veteran_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/visibility_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/visibility_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/warning_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ats/types/webhook_receiver.py` & `mergepythonclient-0.1.1/src/merge/resources/ats/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/account_details/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/account_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/accounts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/accounts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/association_types/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/association_types/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/associations/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/associations/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/available_actions/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/contacts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/contacts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/custom_object_classes/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_object_classes/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/custom_objects/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_objects/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/delete_account/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/engagement_types/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagement_types/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/engagements/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagements/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/force_resync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/generate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/issues/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/leads/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/leads/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/link_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/linked_accounts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/notes/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/notes/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/opportunities/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/opportunities/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/passthrough/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/regenerate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/selective_sync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/stages/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/stages/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/sync_status/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/tasks/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/tasks/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/users/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/account.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/account.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/account_details.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/account_details_and_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/account_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/account_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/account_token.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/activity_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/address.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/address.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/address_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/address_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/address_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/address_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/association.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/association.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/association_sub_type.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/association_sub_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/association_type.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/association_type_request_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type_request_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/available_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/cardinality_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/cardinality_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/categories_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/category_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/condition_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/condition_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/contact.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/contact.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/contact_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/contact_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/country_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/crm_account_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_account_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/crm_association_type_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_association_type_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/crm_contact_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_contact_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/crm_custom_object_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_custom_object_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/custom_object.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/custom_object_class.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object_class.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/custom_object_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/debug_mode_log.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/debug_model_log_summary.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/direction_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/direction_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/email_address.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/email_address.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/email_address_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/email_address_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/enabled_actions_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/encoding_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/engagement_type.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/engagements_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagements_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/engagements_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagements_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/error_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/field_format_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/field_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/field_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/field_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/ignore_common_model_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/ignore_common_model_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/issue.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/issue_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/item_format_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/item_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/item_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/item_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/item_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/item_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/lead.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/lead.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/lead_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/lead_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/lead_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/lead_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/leads_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/leads_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/leads_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/leads_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/link_token.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_condition.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_condition_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_account_status.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/meta_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/method_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/model_operation.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/multipart_form_field_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/note.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/note.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/note_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/note_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/note_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/note_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/notes_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/notes_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/notes_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/notes_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/object_class_description_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/object_class_description_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/operator_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunities_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunities_list_request_status.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_list_request_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/opportunity_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/origin_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/origin_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_account_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_account_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_association_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_association_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_association_type_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_association_type_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_contact_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_contact_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_custom_object_class_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_custom_object_class_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_custom_object_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_custom_object_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_engagement_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_engagement_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_engagement_type_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_engagement_type_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_issue_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_lead_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_lead_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_note_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_note_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_opportunity_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_opportunity_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_remote_field_class_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_remote_field_class_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_stage_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_task_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_task_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/paginated_user_list.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_account_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_account_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_contact_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_contact_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_engagement_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_engagement_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_opportunity_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_opportunity_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/patched_task_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_task_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/phone_number.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/phone_number_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/phone_number_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/reason_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_data.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_class.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_field_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_key.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/remote_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/request_format_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/response_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/stage.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/stage.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/sync_status.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/sync_status_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/task.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/task.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/task_request.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/task_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/task_response.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/task_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/task_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/task_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/tasks_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/tasks_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/tasks_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/tasks_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/user.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/user.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/validation_problem_source.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/warning_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/crm/types/webhook_receiver.py` & `mergepythonclient-0.1.1/src/merge/resources/crm/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/account_details/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/account_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/available_actions/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/bank_info/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/bank_info/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/benefits/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/benefits/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/companies/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/companies/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/delete_account/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/employee_payroll_runs/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/employee_payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/employees/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/employees/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/employments/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/employments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/force_resync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/generate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/groups/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/groups/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/issues/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/link_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/linked_accounts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/locations/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/locations/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/passthrough/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/pay_groups/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/pay_groups/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/payroll_runs/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/regenerate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/selective_sync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/sync_status/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/teams/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/teams/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/time_off/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/time_off_balances/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off_balances/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/account_details.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/account_details_and_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/account_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/account_token.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/account_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/available_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/bank_info.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/bank_info_list_request_account_type.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_list_request_account_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/bank_info_list_request_order_by.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/benefit.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/benefit.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/categories_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/category_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/company.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/company.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/condition_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/condition_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/country_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/debug_mode_log.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/debug_model_log_summary.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/deduction.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/deduction.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/earning.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/earning.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/earning_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/earning_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employee.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_payroll_run.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_run.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_request.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employee_response.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_list_request_employment_status.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_employment_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_list_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employment.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employment_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employment_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_list_request_order_by.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_list_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/enabled_actions_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/encoding_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/error_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/ethnicity_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/ethnicity_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/flsa_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/flsa_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/gender_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/group.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/group.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/group_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/group_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/issue.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/issue_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/link_token.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_condition.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_condition_request.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_account_status.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/location.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/location.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/marital_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/meta_response.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/method_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/model_operation.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/multipart_form_field_request.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/operator_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_bank_info_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_bank_info_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_benefit_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_benefit_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_company_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_company_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_employee_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employee_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_employment_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_group_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_issue_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_location_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_location_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_pay_group_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_pay_group_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_payroll_run_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_team_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_time_off_balance_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_time_off_balance_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/paginated_time_off_list.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_time_off_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/pay_currency_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_currency_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/pay_frequency_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_frequency_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/pay_group.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_group.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/pay_period_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_period_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_run.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_run.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/policy_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/policy_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/reason_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/remote_data.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/remote_key.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/remote_response.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/request_format_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/request_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/request_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/response_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/run_state_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/run_state_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/run_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/run_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/sync_status.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/sync_status_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/tax.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/tax.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/team.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/team.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_balance.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balance.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_request_type.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_request_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_list_request_status.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_request.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_response.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/time_off_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/validation_problem_source.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/warning_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/hris/types/webhook_receiver.py` & `mergepythonclient-0.1.1/src/merge/resources/hris/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/account_details/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/account_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/accounts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/accounts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/attachments/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/available_actions/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/collections/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/collections/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/comments/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/comments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/contacts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/contacts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/delete_account/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/force_resync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/generate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/issues/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/link_token/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/linked_accounts/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/passthrough/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/projects/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/projects/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/regenerate_key/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/selective_sync/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/sync_status/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/tags/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/teams/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/teams/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/tickets/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tickets/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/users/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/__init__.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/access_level_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/access_level_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_details.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_details_and_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_integration.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/account_token.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/attachment.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/attachment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/attachment_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/attachment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/available_actions.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/categories_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/category_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collection.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collection_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collections_list_request_collection_type.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collections_list_request_collection_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/collections_users_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collections_users_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comment.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comment_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comment_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comments_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/condition_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/condition_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/contact.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/contact.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/debug_mode_log.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/debug_model_log_summary.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/enabled_actions_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/encoding_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/error_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/field_format_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/field_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/field_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/field_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/issue.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/issue_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/item_format_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/item_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/item_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/link_token.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_condition.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_condition_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_account_status.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/meta_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/method_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/model_operation.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/multipart_form_field_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/operator_schema.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_account_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_account_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_attachment_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_collection_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_collection_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_comment_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_comment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_contact_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_contact_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_issue_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_project_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_project_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_tag_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_team_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_ticket_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_ticket_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/paginated_user_list.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/patched_ticket_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/patched_ticket_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/priority_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/priority_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/project.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/project.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/projects_users_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/projects_users_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_data.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_field.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_field_class.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field_class.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_field_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_key.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/remote_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/request_format_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/response_type_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/sync_status.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/sync_status_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tag.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tag.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/team.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/team.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_request.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticket_status_enum.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/ticketing_attachment_response.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticketing_attachment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_priority.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_priority.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_list_request_status.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/user.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/user.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/users_list_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/users_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/users_retrieve_request_expand.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/users_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/validation_problem_source.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/warning_validation_problem.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/src/merge/resources/ticketing/types/webhook_receiver.py` & `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.0/PKG-INFO` & `mergepythonclient-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergepythonclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: Client library for the merge API
 Home-page: https://github.com/merge-api/merge-python-client
 License: custom
 Author: Merge
 Author-email: hello@merge.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -15,18 +15,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (==0.23.3)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Project-URL: Repository, https://github.com/merge-api/merge-python-client
 Description-Content-Type: text/markdown
 
-
 # Merge Python Library
 
-[![pypi](https://img.shields.io/pypi/v/fern-merge.svg)](https://pypi.python.org/pypi/fern-merge)
+[![pypi](https://img.shields.io/pypi/v/MergePythonClient.svg)](https://pypi.python.org/pypi/MergePythonClient)
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
 
 The Merge Python library provides access to the Merge API from Python.
 
 ## Documentation
 
 API reference documentation is available [here](https://docs.merge.dev/).
@@ -39,133 +38,156 @@
 
 ## Instantiation
 
 ```python
 import merge
 from merge.client import Merge
 
-client = Merge(api_key="YOUR_API_KEY", account_token="YOUR_ACCOUNT_TOKEN")
+client = Merge(api_key="Bearer YOUR_API_KEY", account_token="YOUR_ACCOUNT_TOKEN")
 ```
 
 ## Categories
 
 This SDK contains both the ATS, HRIS, CRM, Ticketing, and Accounting categories. Even if you do not plan on using more than one Merge API category right now, the SDK provides upgrade-flexibility in case you find new Merge API categories useful in the future.
 
-Each category is namespaced: 
+Each category is namespaced:
+
 ```python
-client = Merge(api_key="YOUR_API_KEY")
+client = Merge(api_key="Bearer YOUR_API_KEY")
 
 client.ats. # APIs specific to the ATS Category
 
 client.hris. # APIs specific to the HRIS Category
 ```
 
-## Usage 
+## Usage
 
-## Create Link Token 
+## Create Link Token
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 link_token_response = merge_client.ats.link_token.create(
     end_user_email_address="john.smith@gmail.com",
     end_user_organization_name="acme",
     end_user_origin_id="1234",
     categories=[CategoriesEnum.ATS],
     link_expiry_mins=30,
 )
 
 print("Created link token", link_token_response.link_token)
 ```
 
-## Get Employee 
+## Get Employee
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 employee = merge_client.hris.employees.retrieve(
     id="0958cbc6-6040-430a-848e-aafacbadf4ae")
 ```
 
-## Get Candidate 
+## Get Candidate
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 candidate = merge_client.ats.candiates.retrieve(
     id="521b18c2-4d01-4297-b451-19858d07c133")
 ```
 
-## Filter Candidate 
+## Filter Candidate
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 candidates_response = merge_client.ats.candidates.list(
     created_after="2030-01-01")
 
 print(candidates_response.result)
 ```
 
-## Get Contact 
+## Get Contact
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 contact = merge_client.accounting.contacts.retrieve(
     id="c640b80b-fac9-409f-aa19-1f9221aec445")
 ```
 
 ## Create Ticket
 
 ```python
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
-    api_key="Bearer <YOUR_API_KEY>", 
+    api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
 merge_client.ticketing.tickets.create(
     model=merge.ticketing.TicketRequest(
         name="Please add more integrations",
         assignees=[
             "17a54124-287f-494d-965e-3c5b330c9a68"
         ],
         creator="3fa85f64-5717-4562-b3fc-2c963f66afa6",
         due_date="2022-10-11T00:00:00Z",
         status=merge.ticketing.TicketRequestStatus.OPEN,
     ))
 ```
 
+## Pagination
+
+The SDK may return paginated results. Endpoints that return paginated results will 
+include a `next` and `prev` property on the response. To get the next page, you can 
+pass in the value of `next` to the cursor property on the request. Similarly, to 
+get the previous page, you can pass in the value of `prev` to the cursor property on 
+the request. 
+
+Below is an example of iterating over all pages:
+```python
+
+# response contains the first page
+response = merge_client.hris.employees.list(created_after="2030-01-01")
+
+# if there is a next page, load it by passing `next` to the cursor argument
+while response.next is not None:
+    response = hris_client.employees.list(
+        cursor=response.next, 
+        created_after="2030-01-01")
+```
+
+
 ## Beta status
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning the package version to a specific version in your package.json file. This way, you can install the same version each time without breaking changes unless you are intentionally looking for the latest version.
 
 ## Contributing
 
 While we value open-source contributions to this SDK, this library is generated programmatically. Additions made directly to this library would have to be moved over to our generation code, otherwise they would be overwritten upon the next generated release. Feel free to open a PR as a proof of concept, but know that we will not be able to merge it as-is. We suggest opening an issue first to discuss with us!
```

