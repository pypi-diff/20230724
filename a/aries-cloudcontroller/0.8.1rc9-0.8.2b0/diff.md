# Comparing `tmp/aries_cloudcontroller-0.8.1rc9.tar.gz` & `tmp/aries_cloudcontroller-0.8.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aries_cloudcontroller-0.8.1rc9.tar", last modified: Tue Jun 13 09:19:57 2023, max compression
+gzip compressed data, was "aries_cloudcontroller-0.8.2b0.tar", last modified: Mon Jul 24 10:05:56 2023, max compression
```

## Comparing `aries_cloudcontroller-0.8.1rc9.tar` & `aries_cloudcontroller-0.8.2b0.tar`

### file list

```diff
@@ -1,333 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:57.890184 aries_cloudcontroller-0.8.1rc9/
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-13 09:19:57.890184 aries_cloudcontroller-0.8.1rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:57.850184 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/acapy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:57.858184 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/action_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/basicmessage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/did_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/discover_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/discover_features_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/endorse_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/introduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/issue_credential_v1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/issue_credential_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/jsonld.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/ledger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/mediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/multitenancy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/out_of_band.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/present_proof_v1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/present_proof_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/trustping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:57.890184 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/
--rw-r--r--   0 runner    (1001) docker     (123)    29725 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/action_menu_fetch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_status_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_status_readiness.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/aml_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator_data1_jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator_data_jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator_data_jws_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attachment_def.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attribute_mime_types_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/claim_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/clear_pending_revocations_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/conn_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_metadata_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_static_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_static_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_wallet_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_wallet_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_def_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_def_value_primary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_def_value_revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_info_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_rev_indy_records_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_rev_record_details_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_rev_record_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_revoked_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definition_get_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definition_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definitions_created_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_status_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_endpoint_with_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/didx_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_proof_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/disclose.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/disclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/endorser_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/endpoints_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/generated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/get_did_endpoint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/get_did_verkey_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/get_nym_role_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_attr_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_cred_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_cred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_cred_precis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_eq_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_ge_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_ge_proof_pred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_key_correctness_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_non_revoc_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_non_revocation_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_pres_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_pres_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_pres_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_primary_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_req_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_req_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_request_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_requested_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_def_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_entry_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/input_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/invitation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/invitation_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/invitation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/invitation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/issuer_cred_rev_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/issuer_rev_reg_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_query_filter_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_query_paginate.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_update_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ld_proof_vc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ld_proof_vc_detail_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ledger_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ledger_config_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/linked_data_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_id_match_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu_form_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/model_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/oob_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/perform_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ping_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ping_request_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/presentation_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/presentation_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/presentation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/protocol_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/publish_revocations.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/query_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/raw_encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/receive_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/remove_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/resolution_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_issued_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_regs_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/revoke_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/route_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schema_get_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schema_input_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schema_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schemas_created_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schemas_input_descriptor_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/send_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/service_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/sign_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/sign_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/signature_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/signed_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/submission_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_accept.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/tails_delete_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/transaction_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/transaction_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/transaction_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_publish_revocations_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/update_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_store_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_exchange_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_indy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_filter_indy.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_request_free.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_store_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_discovery_exchange_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_issue_cred_schema_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_ex_record_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_proposal_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_request_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/vc_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/vc_record_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/verify_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/verify_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/w3_c_credentials_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/wallet_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/write_ledger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/uplink_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:57.890184 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/util/create_client_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/util/pydantic_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:57.850184 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-13 09:19:57.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-06-13 09:19:57.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:19:57.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 09:19:57.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 09:19:57.000000 aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:19:57.890184 aries_cloudcontroller-0.8.1rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:57.890184 aries_cloudcontroller-0.8.1rc9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/compare_dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:57.890184 aries_cloudcontroller-0.8.1rc9/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/model/test_credential_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/model/test_invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/model/test_presentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/model/test_v20_cred_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/model/test_v20_pres_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-13 09:19:48.000000 aries_cloudcontroller-0.8.1rc9/tests/test_acapy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.390951 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/acapy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.394952 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/action_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/basicmessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/did_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/discover_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/discover_features_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/endorse_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/issue_credential_v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/issue_credential_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/ledger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/mediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/multitenancy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/out_of_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/present_proof_v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/present_proof_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/trustping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/action_menu_fetch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status_readiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/aml_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data1_jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data_jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data_jws_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attachment_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attribute_mime_types_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/claim_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/clear_pending_revocations_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/conn_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_metadata_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_static_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_static_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value_primary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_info_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_indy_records_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_record_details_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_record_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_revoked_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definitions_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_status_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_endpoint_with_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/didx_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_proof_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/disclose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/disclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/endorser_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/endpoints_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_did_endpoint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_did_verkey_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_nym_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_attr_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_precis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_eq_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_ge_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_ge_proof_pred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_key_correctness_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_non_revoc_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_non_revocation_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_primary_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_request_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_entry_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/input_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/issuer_cred_rev_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/issuer_rev_reg_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query_filter_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query_paginate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ld_proof_vc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ld_proof_vc_detail_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ledger_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ledger_config_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/linked_data_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_id_match_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_form_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/model_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/oob_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/perform_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ping_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ping_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/profile_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/protocol_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/publish_revocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/query_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/raw_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/receive_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/remove_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/resolution_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_issued_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_regs_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/revoke_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/route_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_input_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schemas_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schemas_input_descriptor_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/send_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/service_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/sign_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/sign_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/signature_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/signed_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/submission_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_accept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/tails_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_publish_revocations_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/update_profile_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/update_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_exchange_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_indy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter_indy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_exchange_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_issue_cred_schema_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_request_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/vc_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/vc_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/verify_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/verify_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/w3_c_credentials_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/wallet_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/write_ledger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/uplink_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/acapy_client_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/pydantic_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.390951 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/client/test_acapy_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/client/test_pydantic_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_credential_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_presentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_v20_cred_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_v20_pres_ex_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/util/compare_dicts.py
```

### Comparing `aries_cloudcontroller-0.8.1rc9/LICENSE` & `aries_cloudcontroller-0.8.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/PKG-INFO` & `aries_cloudcontroller-0.8.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aries_cloudcontroller
-Version: 0.8.1rc9
+Version: 0.8.2b0
 Summary: A simple python package for controlling an aries agent through the admin-api interface
 Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.8.1rc9 Summary: A
+Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.8.2b0 Summary: A
 simple python package for controlling an aries agent through the admin-api
 interface Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/
 tree/main/aries_cloudcontroller Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `aries_cloudcontroller-0.8.1rc9/README.md` & `aries_cloudcontroller-0.8.2b0/README.md`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/__init__.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     OutOfBandApi,
     PresentProofV10Api,
     PresentProofV20Api,
     ResolverApi,
     RevocationApi,
     SchemaApi,
     ServerApi,
+    SettingsApi,
     TrustpingApi,
     WalletApi,
 )
 
 from aries_cloudcontroller.model import (
     AMLRecord,
     ActionMenuFetchResult,
@@ -178,14 +179,15 @@
     OobRecord,
     PerformRequest,
     PingRequest,
     PingRequestResponse,
     PresentationDefinition,
     PresentationProposal,
     PresentationRequest,
+    ProfileSettings,
     ProtocolDescriptor,
     PublishRevocations,
     Queries,
     Query,
     QueryItem,
     RawEncoded,
     ReceiveInvitationRequest,
@@ -223,14 +225,15 @@
     TransactionList,
     TransactionRecord,
     TxnOrCredentialDefinitionSendResult,
     TxnOrPublishRevocationsResult,
     TxnOrRegisterLedgerNymResponse,
     TxnOrRevRegResult,
     TxnOrSchemaSendResult,
+    UpdateProfileSettings,
     UpdateWalletRequest,
     V10CredentialBoundOfferRequest,
     V10CredentialConnFreeOfferRequest,
     V10CredentialCreate,
     V10CredentialExchange,
     V10CredentialExchangeListResult,
     V10CredentialFreeOfferRequest,
@@ -452,14 +455,15 @@
     "OobRecord",
     "PerformRequest",
     "PingRequest",
     "PingRequestResponse",
     "PresentationDefinition",
     "PresentationProposal",
     "PresentationRequest",
+    "ProfileSettings",
     "ProtocolDescriptor",
     "PublishRevocations",
     "Queries",
     "Query",
     "QueryItem",
     "RawEncoded",
     "ReceiveInvitationRequest",
@@ -497,14 +501,15 @@
     "TransactionList",
     "TransactionRecord",
     "TxnOrCredentialDefinitionSendResult",
     "TxnOrPublishRevocationsResult",
     "TxnOrRegisterLedgerNymResponse",
     "TxnOrRevRegResult",
     "TxnOrSchemaSendResult",
+    "UpdateProfileSettings",
     "UpdateWalletRequest",
     "V10CredentialBoundOfferRequest",
     "V10CredentialConnFreeOfferRequest",
     "V10CredentialCreate",
     "V10CredentialExchange",
     "V10CredentialExchangeListResult",
     "V10CredentialFreeOfferRequest",
@@ -594,10 +599,11 @@
     "OutOfBandApi",
     "PresentProofV10Api",
     "PresentProofV20Api",
     "ResolverApi",
     "RevocationApi",
     "SchemaApi",
     "ServerApi",
+    "SettingsApi",
     "TrustpingApi",
     "WalletApi",
 ]
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/acapy_client.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/acapy_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 from typing import Optional
 
 from aiohttp.client import ClientSession
 
 from aries_cloudcontroller.client import Client
-from aries_cloudcontroller.util.create_client_session import create_client_session
+from aries_cloudcontroller.util.acapy_client_session import AcaPyClientSession
 from aries_cloudcontroller.util.pydantic_converter import PydanticConverter
 
 
 class AcaPyClient(Client):
     def __init__(
         self,
         base_url: str,
         *,
         client_session: Optional[ClientSession] = None,
         api_key: Optional[str] = None,
         admin_insecure: Optional[bool] = False,
         tenant_jwt: Optional[str] = None,
     ):
+        self.base_url = base_url
+
         self._should_close_session = False  # only close ClientSession when created here
         # A provided ClientSession should be closed externally.
 
         if client_session and not api_key:
             api_key = client_session.headers.get("x-api-key")
 
         if not api_key and not admin_insecure:
             raise Exception(
                 "api_key property is missing. Use admin_insecure=True if you want"
                 " to use the controller without authentication."
             )
 
         if not client_session:
-            client_session = create_client_session(
+            self.client_session = AcaPyClientSession(
                 api_key=api_key, tenant_jwt=tenant_jwt
-            )
+            ).client_session
             self._should_close_session = True
-
-        self.client_session = client_session
+        else:
+            self.client_session = client_session
 
         super().__init__(
-            base_url,
+            self.base_url,
             client=self.client_session,
             extra_service_params={"converter": PydanticConverter()},
         )
 
+    async def __aenter__(self):
+        return self
+
     async def __aexit__(self, exc_type, exc_value, traceback):
         if self._should_close_session and not self.client_session.closed:
             await self.client_session.close()
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/__init__.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from aries_cloudcontroller.api.out_of_band import OutOfBandApi
 from aries_cloudcontroller.api.present_proof_v1_0 import PresentProofV10Api
 from aries_cloudcontroller.api.present_proof_v2_0 import PresentProofV20Api
 from aries_cloudcontroller.api.resolver import ResolverApi
 from aries_cloudcontroller.api.revocation import RevocationApi
 from aries_cloudcontroller.api.schema import SchemaApi
 from aries_cloudcontroller.api.server import ServerApi
+from aries_cloudcontroller.api.settings import SettingsApi
 from aries_cloudcontroller.api.trustping import TrustpingApi
 from aries_cloudcontroller.api.wallet import WalletApi
 
 __all__ = [
     "ActionMenuApi",
     "BasicmessageApi",
     "ConnectionApi",
@@ -48,10 +49,11 @@
     "OutOfBandApi",
     "PresentProofV10Api",
     "PresentProofV20Api",
     "ResolverApi",
     "RevocationApi",
     "SchemaApi",
     "ServerApi",
+    "SettingsApi",
     "TrustpingApi",
     "WalletApi",
 ]
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/action_menu.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/action_menu.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,16 @@
             conn_id=conn_id,
         )
 
     async def perform_action(
         self, *, conn_id: str, body: Optional[PerformRequest] = None
     ) -> Dict[str, Any]:
         """Perform an action associated with the active menu"""
+        if not body:
+            body = PerformRequest()
         return await self.__perform_action(
             conn_id=conn_id,
             body=body,
         )
 
     async def request_active_menu(self, *, conn_id: str) -> Dict[str, Any]:
         """Request the active menu"""
@@ -50,14 +52,16 @@
             conn_id=conn_id,
         )
 
     async def send_menu(
         self, *, conn_id: str, body: Optional[SendMenu] = None
     ) -> Dict[str, Any]:
         """Send an action menu to a connection"""
+        if not body:
+            body = SendMenu()
         return await self.__send_menu(
             conn_id=conn_id,
             body=body,
         )
 
     @returns.json
     @post("/action-menu/{conn_id}/close")
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/basicmessage.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/basicmessage.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 
 class BasicmessageApi(Consumer):
     async def send_message(
         self, *, conn_id: str, body: Optional[SendMessage] = None
     ) -> Dict[str, Any]:
         """Send a basic message to a connection"""
+        if not body:
+            body = SendMessage()
         return await self.__send_message(
             conn_id=conn_id,
             body=body,
         )
 
     @returns.json
     @json
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/connection.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,26 +69,30 @@
         alias: Optional[str] = None,
         auto_accept: Optional[bool] = None,
         multi_use: Optional[bool] = None,
         public: Optional[bool] = None,
         body: Optional[CreateInvitationRequest] = None
     ) -> InvitationResult:
         """Create a new connection invitation"""
+        if not body:
+            body = CreateInvitationRequest()
         return await self.__create_invitation(
             alias=alias,
             auto_accept=bool_query(auto_accept),
             multi_use=bool_query(multi_use),
             public=bool_query(public),
             body=body,
         )
 
     async def create_static_connection(
         self, *, body: Optional[ConnectionStaticRequest] = None
     ) -> ConnectionStaticResult:
         """Create a new static connection"""
+        if not body:
+            body = ConnectionStaticRequest()
         return await self.__create_static_connection(
             body=body,
         )
 
     async def delete_connection(self, *, conn_id: str) -> Dict[str, Any]:
         """Remove an existing connection record"""
         return await self.__delete_connection(
@@ -154,25 +158,29 @@
         *,
         alias: Optional[str] = None,
         auto_accept: Optional[bool] = None,
         mediation_id: Optional[str] = None,
         body: Optional[ReceiveInvitationRequest] = None
     ) -> ConnRecord:
         """Receive a new connection invitation"""
+        if not body:
+            body = ReceiveInvitationRequest()
         return await self.__receive_invitation(
             alias=alias,
             auto_accept=bool_query(auto_accept),
             mediation_id=mediation_id,
             body=body,
         )
 
     async def set_metadata(
         self, *, conn_id: str, body: Optional[ConnectionMetadataSetRequest] = None
     ) -> ConnectionMetadata:
         """Set connection metadata"""
+        if not body:
+            body = ConnectionMetadataSetRequest()
         return await self.__set_metadata(
             conn_id=conn_id,
             body=body,
         )
 
     @returns.json
     @post("/connections/{conn_id}/accept-invitation")
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/credential_definition.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/credential_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         self,
         *,
         conn_id: Optional[str] = None,
         create_transaction_for_endorser: Optional[bool] = None,
         body: Optional[CredentialDefinitionSendRequest] = None
     ) -> TxnOrCredentialDefinitionSendResult:
         """Sends a credential definition to the ledger"""
+        if not body:
+            body = CredentialDefinitionSendRequest()
         return await self.__publish_cred_def(
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
             body=body,
         )
 
     @returns.json
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/credentials.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,16 @@
         *,
         count: Optional[str] = None,
         start: Optional[str] = None,
         wql: Optional[str] = None,
         body: Optional[W3CCredentialsListRequest] = None
     ) -> VCRecordList:
         """Fetch W3C credentials from wallet"""
+        if not body:
+            body = W3CCredentialsListRequest()
         return await self.__get_w3c_credentials(
             count=count,
             start=start,
             wql=wql,
             body=body,
         )
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/did_exchange.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/did_exchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,16 @@
         alias: Optional[str] = None,
         auto_accept: Optional[bool] = None,
         mediation_id: Optional[str] = None,
         my_endpoint: Optional[str] = None,
         body: Optional[DIDXRequest] = None
     ) -> ConnRecord:
         """Receive request against public DID's implicit invitation"""
+        if not body:
+            body = DIDXRequest()
         return await self.__receive_request(
             alias=alias,
             auto_accept=bool_query(auto_accept),
             mediation_id=mediation_id,
             my_endpoint=my_endpoint,
             body=body,
         )
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/discover_features.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/discover_features.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/discover_features_v2_0.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/discover_features_v2_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/endorse_transaction.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/endorse_transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         self,
         *,
         tran_id: str,
         endorser_write_txn: Optional[bool] = None,
         body: Optional[Date] = None
     ) -> TransactionRecord:
         """For author to send a transaction request"""
+        if not body:
+            body = Date()
         return await self.__create_request(
             tran_id=tran_id,
             endorser_write_txn=bool_query(endorser_write_txn),
             body=body,
         )
 
     async def endorse_transaction(
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/introduction.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/introduction.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/issue_credential_v1_0.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/issue_credential_v1_0.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,22 +49,26 @@
 
 
 class IssueCredentialV10Api(Consumer):
     async def create_credential(
         self, *, body: Optional[V10CredentialCreate] = None
     ) -> V10CredentialExchange:
         """Create a credential record without sending (generally for use with Out-Of-Band)"""
+        if not body:
+            body = V10CredentialCreate()
         return await self.__create_credential(
             body=body,
         )
 
     async def create_offer(
         self, *, body: Optional[V10CredentialConnFreeOfferRequest] = None
     ) -> V10CredentialExchange:
         """Create a credential offer, independent of any proposal or connection"""
+        if not body:
+            body = V10CredentialConnFreeOfferRequest()
         return await self.__create_offer(
             body=body,
         )
 
     async def delete_record(self, *, cred_ex_id: str) -> Dict[str, Any]:
         """Remove an existing credential exchange record"""
         return await self.__delete_record(
@@ -93,74 +97,88 @@
             thread_id=thread_id,
         )
 
     async def issue_credential(
         self, *, cred_ex_id: str, body: Optional[V10CredentialIssueRequest] = None
     ) -> V10CredentialExchange:
         """Send holder a credential"""
+        if not body:
+            body = V10CredentialIssueRequest()
         return await self.__issue_credential(
             cred_ex_id=cred_ex_id,
             body=body,
         )
 
     async def issue_credential_automated(
         self, *, body: Optional[V10CredentialProposalRequestMand] = None
     ) -> V10CredentialExchange:
         """Send holder a credential, automating entire flow"""
+        if not body:
+            body = V10CredentialProposalRequestMand()
         return await self.__issue_credential_automated(
             body=body,
         )
 
     async def report_problem(
         self,
         *,
         cred_ex_id: str,
         body: Optional[V10CredentialProblemReportRequest] = None
     ) -> Dict[str, Any]:
         """Send a problem report for credential exchange"""
+        if not body:
+            body = V10CredentialProblemReportRequest()
         return await self.__report_problem(
             cred_ex_id=cred_ex_id,
             body=body,
         )
 
     async def send_offer(
         self, *, cred_ex_id: str, body: Optional[V10CredentialBoundOfferRequest] = None
     ) -> V10CredentialExchange:
         """Send holder a credential offer in reference to a proposal with preview"""
+        if not body:
+            body = V10CredentialBoundOfferRequest()
         return await self.__send_offer(
             cred_ex_id=cred_ex_id,
             body=body,
         )
 
     async def send_offer_free(
         self, *, body: Optional[V10CredentialFreeOfferRequest] = None
     ) -> V10CredentialExchange:
         """Send holder a credential offer, independent of any proposal"""
+        if not body:
+            body = V10CredentialFreeOfferRequest()
         return await self.__send_offer_free(
             body=body,
         )
 
     async def send_proposal(
         self, *, body: Optional[V10CredentialProposalRequestOpt] = None
     ) -> V10CredentialExchange:
         """Send issuer a credential proposal"""
+        if not body:
+            body = V10CredentialProposalRequestOpt()
         return await self.__send_proposal(
             body=body,
         )
 
     async def send_request(self, *, cred_ex_id: str) -> V10CredentialExchange:
         """Send issuer a credential request"""
         return await self.__send_request(
             cred_ex_id=cred_ex_id,
         )
 
     async def store_credential(
         self, *, cred_ex_id: str, body: Optional[V10CredentialStoreRequest] = None
     ) -> V10CredentialExchange:
         """Store a received credential"""
+        if not body:
+            body = V10CredentialStoreRequest()
         return await self.__store_credential(
             cred_ex_id=cred_ex_id,
             body=body,
         )
 
     @returns.json
     @json
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/issue_credential_v2_0.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/issue_credential_v2_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 
 
 class IssueCredentialV20Api(Consumer):
     async def create_credential(
         self, *, body: Optional[V20IssueCredSchemaCore] = None
     ) -> V20CredExRecord:
         """Create a credential record without sending (generally for use with Out-Of-Band)"""
+        if not body:
+            body = V20IssueCredSchemaCore()
         return await self.__create_credential(
             body=body,
         )
 
     async def delete_record(self, *, cred_ex_id: str) -> Dict[str, Any]:
         """Remove an existing credential exchange record"""
         return await self.__delete_record(
@@ -79,93 +81,113 @@
             thread_id=thread_id,
         )
 
     async def issue_credential(
         self, *, cred_ex_id: str, body: Optional[V20CredIssueRequest] = None
     ) -> V20CredExRecordDetail:
         """Send holder a credential"""
+        if not body:
+            body = V20CredIssueRequest()
         return await self.__issue_credential(
             cred_ex_id=cred_ex_id,
             body=body,
         )
 
     async def issue_credential20_create_offer_post(
         self, *, body: Optional[V20CredOfferConnFreeRequest] = None
     ) -> V20CredExRecord:
         """Create a credential offer, independent of any proposal or connection"""
+        if not body:
+            body = V20CredOfferConnFreeRequest()
         return await self.__issue_credential20_create_offer_post(
             body=body,
         )
 
     async def issue_credential_automated(
         self, *, body: Optional[V20CredExFree] = None
     ) -> V20CredExRecord:
         """Send holder a credential, automating entire flow"""
+        if not body:
+            body = V20CredExFree()
         return await self.__issue_credential_automated(
             body=body,
         )
 
     async def report_problem(
         self,
         *,
         cred_ex_id: str,
         body: Optional[V20CredIssueProblemReportRequest] = None
     ) -> Dict[str, Any]:
         """Send a problem report for credential exchange"""
+        if not body:
+            body = V20CredIssueProblemReportRequest()
         return await self.__report_problem(
             cred_ex_id=cred_ex_id,
             body=body,
         )
 
     async def send_offer(
         self, *, cred_ex_id: str, body: Optional[V20CredBoundOfferRequest] = None
     ) -> V20CredExRecord:
         """Send holder a credential offer in reference to a proposal with preview"""
+        if not body:
+            body = V20CredBoundOfferRequest()
         return await self.__send_offer(
             cred_ex_id=cred_ex_id,
             body=body,
         )
 
     async def send_offer_free(
         self, *, body: Optional[V20CredOfferRequest] = None
     ) -> V20CredExRecord:
         """Send holder a credential offer, independent of any proposal"""
+        if not body:
+            body = V20CredOfferRequest()
         return await self.__send_offer_free(
             body=body,
         )
 
     async def send_proposal(
         self, *, body: Optional[V20CredExFree] = None
     ) -> V20CredExRecord:
         """Send issuer a credential proposal"""
+        if not body:
+            body = V20CredExFree()
         return await self.__send_proposal(
             body=body,
         )
 
     async def send_request(
         self, *, cred_ex_id: str, body: Optional[V20CredRequestRequest] = None
     ) -> V20CredExRecord:
         """Send issuer a credential request"""
+        if not body:
+            body = V20CredRequestRequest()
         return await self.__send_request(
             cred_ex_id=cred_ex_id,
             body=body,
         )
 
     async def send_request_free(
         self, *, body: Optional[V20CredRequestFree] = None
     ) -> V20CredExRecord:
         """Send issuer a credential request not bound to an existing thread. Indy credentials cannot start at a request"""
+        if not body:
+            body = V20CredRequestFree()
         return await self.__send_request_free(
             body=body,
         )
 
     async def store_credential(
         self, *, cred_ex_id: str, body: Optional[V20CredStoreRequest] = None
     ) -> V20CredExRecordDetail:
         """Store a received credential"""
+        if not body:
+            body = V20CredStoreRequest()
         return await self.__store_credential(
             cred_ex_id=cred_ex_id,
             body=body,
         )
 
     @returns.json
     @json
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/jsonld.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/jsonld.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,20 +22,24 @@
 from aries_cloudcontroller.model.verify_request import VerifyRequest
 from aries_cloudcontroller.model.verify_response import VerifyResponse
 
 
 class JsonldApi(Consumer):
     async def sign(self, *, body: Optional[SignRequest] = None) -> SignResponse:
         """Sign a JSON-LD structure and return it"""
+        if not body:
+            body = SignRequest()
         return await self.__sign(
             body=body,
         )
 
     async def verify(self, *, body: Optional[VerifyRequest] = None) -> VerifyResponse:
         """Verify a JSON-LD structure."""
+        if not body:
+            body = VerifyRequest()
         return await self.__verify(
             body=body,
         )
 
     @returns.json
     @json
     @post("/jsonld/sign")
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/ledger.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/ledger.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 )
 from aries_cloudcontroller.model.write_ledger_request import WriteLedgerRequest
 
 
 class LedgerApi(Consumer):
     async def accept_taa(self, *, body: Optional[TAAAccept] = None) -> Dict[str, Any]:
         """Accept the transaction author agreement"""
+        if not body:
+            body = TAAAccept()
         return await self.__accept_taa(
             body=body,
         )
 
     async def fetch_taa(self) -> TAAResult:
         """Fetch the current transaction author agreement, if any"""
         return await self.__fetch_taa()
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/mediation.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/mediation.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
             mediation_id=mediation_id,
         )
 
     async def deny_mediation_request(
         self, *, mediation_id: str, body: Optional[AdminMediationDeny] = None
     ) -> MediationDeny:
         """Deny a stored mediation request"""
+        if not body:
+            body = AdminMediationDeny()
         return await self.__deny_mediation_request(
             mediation_id=mediation_id,
             body=body,
         )
 
     async def get_default_mediator(self) -> MediationRecord:
         """Get default mediator"""
@@ -85,23 +87,27 @@
             mediation_id=mediation_id,
         )
 
     async def mediation_update_keylist_conn_id_post(
         self, *, conn_id: str, body: Optional[MediationIdMatchInfo] = None
     ) -> KeylistUpdate:
         """Update keylist for a connection"""
+        if not body:
+            body = MediationIdMatchInfo()
         return await self.__mediation_update_keylist_conn_id_post(
             conn_id=conn_id,
             body=body,
         )
 
     async def request_mediation(
         self, *, conn_id: str, body: Optional[MediationCreateRequest] = None
     ) -> MediationRecord:
         """Request mediation from connection"""
+        if not body:
+            body = MediationCreateRequest()
         return await self.__request_mediation(
             conn_id=conn_id,
             body=body,
         )
 
     async def retrieve_keylists(
         self, *, conn_id: Optional[str] = None, role: Optional[str] = "server"
@@ -117,25 +123,29 @@
         *,
         mediation_id: str,
         paginate_limit: Optional[int] = -1,
         paginate_offset: Optional[int] = 0,
         body: Optional[KeylistQueryFilterRequest] = None
     ) -> KeylistQuery:
         """Send keylist query to mediator"""
+        if not body:
+            body = KeylistQueryFilterRequest()
         return await self.__send_keylist_query(
             mediation_id=mediation_id,
             paginate_limit=paginate_limit,
             paginate_offset=paginate_offset,
             body=body,
         )
 
     async def send_keylist_update(
         self, *, mediation_id: str, body: Optional[KeylistUpdateRequest] = None
     ) -> KeylistUpdate:
         """Send keylist update to mediator"""
+        if not body:
+            body = KeylistUpdateRequest()
         return await self.__send_keylist_update(
             mediation_id=mediation_id,
             body=body,
         )
 
     async def set_default_mediator(self, *, mediation_id: str) -> MediationRecord:
         """Set default mediator"""
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/multitenancy.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/multitenancy.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,31 +32,37 @@
 
 
 class MultitenancyApi(Consumer):
     async def create_wallet(
         self, *, body: Optional[CreateWalletRequest] = None
     ) -> CreateWalletResponse:
         """Create a subwallet"""
+        if not body:
+            body = CreateWalletRequest()
         return await self.__create_wallet(
             body=body,
         )
 
     async def delete_wallet(
         self, *, wallet_id: str, body: Optional[RemoveWalletRequest] = None
     ) -> Dict[str, Any]:
         """Remove a subwallet"""
+        if not body:
+            body = RemoveWalletRequest()
         return await self.__delete_wallet(
             wallet_id=wallet_id,
             body=body,
         )
 
     async def get_auth_token(
         self, *, wallet_id: str, body: Optional[CreateWalletTokenRequest] = None
     ) -> CreateWalletTokenResponse:
         """Get auth token for a subwallet"""
+        if not body:
+            body = CreateWalletTokenRequest()
         return await self.__get_auth_token(
             wallet_id=wallet_id,
             body=body,
         )
 
     async def get_wallet(self, *, wallet_id: str) -> WalletRecord:
         """Get a single subwallet"""
@@ -70,14 +76,16 @@
             wallet_name=wallet_name,
         )
 
     async def update_wallet(
         self, *, wallet_id: str, body: Optional[UpdateWalletRequest] = None
     ) -> WalletRecord:
         """Update a subwallet"""
+        if not body:
+            body = UpdateWalletRequest()
         return await self.__update_wallet(
             wallet_id=wallet_id,
             body=body,
         )
 
     @returns.json
     @json
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/out_of_band.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/out_of_band.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         self,
         *,
         auto_accept: Optional[bool] = None,
         multi_use: Optional[bool] = None,
         body: Optional[InvitationCreateRequest] = None
     ) -> InvitationRecord:
         """Create a new connection invitation"""
+        if not body:
+            body = InvitationCreateRequest()
         return await self.__create_invitation(
             auto_accept=bool_query(auto_accept),
             multi_use=bool_query(multi_use),
             body=body,
         )
 
     async def receive_invitation(
@@ -46,14 +48,16 @@
         alias: Optional[str] = None,
         auto_accept: Optional[bool] = None,
         mediation_id: Optional[str] = None,
         use_existing_connection: Optional[bool] = None,
         body: Optional[InvitationMessage] = None
     ) -> OobRecord:
         """Receive a new connection invitation"""
+        if not body:
+            body = InvitationMessage()
         return await self.__receive_invitation(
             alias=alias,
             auto_accept=bool_query(auto_accept),
             mediation_id=mediation_id,
             use_existing_connection=bool_query(use_existing_connection),
             body=body,
         )
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/present_proof_v1_0.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/present_proof_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 
 
 class PresentProofV10Api(Consumer):
     async def create_proof_request(
         self, *, body: Optional[V10PresentationCreateRequestRequest] = None
     ) -> V10PresentationExchange:
         """Creates a presentation request not bound to any proposal or connection"""
+        if not body:
+            body = V10PresentationCreateRequestRequest()
         return await self.__create_proof_request(
             body=body,
         )
 
     async def delete_record(self, *, pres_ex_id: str) -> Dict[str, Any]:
         """Remove an existing presentation exchange record"""
         return await self.__delete_record(
@@ -100,52 +102,62 @@
     async def report_problem(
         self,
         *,
         pres_ex_id: str,
         body: Optional[V10PresentationProblemReportRequest] = None
     ) -> Dict[str, Any]:
         """Send a problem report for presentation exchange"""
+        if not body:
+            body = V10PresentationProblemReportRequest()
         return await self.__report_problem(
             pres_ex_id=pres_ex_id,
             body=body,
         )
 
     async def send_presentation(
         self, *, pres_ex_id: str, body: Optional[IndyPresSpec] = None
     ) -> V10PresentationExchange:
         """Sends a proof presentation"""
+        if not body:
+            body = IndyPresSpec()
         return await self.__send_presentation(
             pres_ex_id=pres_ex_id,
             body=body,
         )
 
     async def send_proposal(
         self, *, body: Optional[V10PresentationProposalRequest] = None
     ) -> V10PresentationExchange:
         """Sends a presentation proposal"""
+        if not body:
+            body = V10PresentationProposalRequest()
         return await self.__send_proposal(
             body=body,
         )
 
     async def send_request(
         self,
         *,
         pres_ex_id: str,
         body: Optional[V10PresentationSendRequestToProposal] = None
     ) -> V10PresentationExchange:
         """Sends a presentation request in reference to a proposal"""
+        if not body:
+            body = V10PresentationSendRequestToProposal()
         return await self.__send_request(
             pres_ex_id=pres_ex_id,
             body=body,
         )
 
     async def send_request_free(
         self, *, body: Optional[V10PresentationSendRequestRequest] = None
     ) -> V10PresentationExchange:
         """Sends a free presentation request not bound to any proposal"""
+        if not body:
+            body = V10PresentationSendRequestRequest()
         return await self.__send_request_free(
             body=body,
         )
 
     async def verify_presentation(self, *, pres_ex_id: str) -> V10PresentationExchange:
         """Verify a received presentation"""
         return await self.__verify_presentation(
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/present_proof_v2_0.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/present_proof_v2_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 
 class PresentProofV20Api(Consumer):
     async def create_proof_request(
         self, *, body: Optional[V20PresCreateRequestRequest] = None
     ) -> V20PresExRecord:
         """Creates a presentation request not bound to any proposal or connection"""
+        if not body:
+            body = V20PresCreateRequestRequest()
         return await self.__create_proof_request(
             body=body,
         )
 
     async def delete_record(self, *, pres_ex_id: str) -> Dict[str, Any]:
         """Remove an existing presentation exchange record"""
         return await self.__delete_record(
@@ -93,52 +95,62 @@
             thread_id=thread_id,
         )
 
     async def report_problem(
         self, *, pres_ex_id: str, body: Optional[V20PresProblemReportRequest] = None
     ) -> Dict[str, Any]:
         """Send a problem report for presentation exchange"""
+        if not body:
+            body = V20PresProblemReportRequest()
         return await self.__report_problem(
             pres_ex_id=pres_ex_id,
             body=body,
         )
 
     async def send_presentation(
         self, *, pres_ex_id: str, body: Optional[V20PresSpecByFormatRequest] = None
     ) -> V20PresExRecord:
         """Sends a proof presentation"""
+        if not body:
+            body = V20PresSpecByFormatRequest()
         return await self.__send_presentation(
             pres_ex_id=pres_ex_id,
             body=body,
         )
 
     async def send_proposal(
         self, *, body: Optional[V20PresProposalRequest] = None
     ) -> V20PresExRecord:
         """Sends a presentation proposal"""
+        if not body:
+            body = V20PresProposalRequest()
         return await self.__send_proposal(
             body=body,
         )
 
     async def send_request(
         self,
         *,
         pres_ex_id: str,
         body: Optional[V20PresentationSendRequestToProposal] = None
     ) -> V20PresExRecord:
         """Sends a presentation request in reference to a proposal"""
+        if not body:
+            body = V20PresentationSendRequestToProposal()
         return await self.__send_request(
             pres_ex_id=pres_ex_id,
             body=body,
         )
 
     async def send_request_free(
         self, *, body: Optional[V20PresSendRequestRequest] = None
     ) -> V20PresExRecord:
         """Sends a free presentation request not bound to any proposal"""
+        if not body:
+            body = V20PresSendRequestRequest()
         return await self.__send_request_free(
             body=body,
         )
 
     async def verify_presentation(self, *, pres_ex_id: str) -> V20PresExRecord:
         """Verify a received presentation"""
         return await self.__verify_presentation(
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/resolver.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/resolver.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/revocation.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/revocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,26 @@
 
 
 class RevocationApi(Consumer):
     async def clear_pending_revocations(
         self, *, body: Optional[ClearPendingRevocationsRequest] = None
     ) -> PublishRevocations:
         """Clear pending revocations"""
+        if not body:
+            body = ClearPendingRevocationsRequest()
         return await self.__clear_pending_revocations(
             body=body,
         )
 
     async def create_registry(
         self, *, body: Optional[RevRegCreateRequest] = None
     ) -> RevRegResult:
         """Creates a new revocation registry"""
+        if not body:
+            body = RevRegCreateRequest()
         return await self.__create_registry(
             body=body,
         )
 
     async def download_tails_file(self, *, rev_reg_id: str) -> bytes:
         """Download tails file"""
         return await self.__download_tails_file(
@@ -142,14 +146,16 @@
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
         )
 
     async def publish_revocations(
         self, *, body: Optional[PublishRevocations] = None
     ) -> TxnOrPublishRevocationsResult:
         """Publish pending revocations to ledger"""
+        if not body:
+            body = PublishRevocations()
         return await self.__publish_revocations(
             body=body,
         )
 
     async def revocation_registry_delete_tails_file_delete(
         self, *, cred_def_id: Optional[str] = None, rev_reg_id: Optional[str] = None
     ) -> TailsDeleteResponse:
@@ -186,14 +192,16 @@
             rev_reg_id=rev_reg_id,
         )
 
     async def revoke_credential(
         self, *, body: Optional[RevokeRequest] = None
     ) -> Dict[str, Any]:
         """Revoke an issued credential"""
+        if not body:
+            body = RevokeRequest()
         return await self.__revoke_credential(
             body=body,
         )
 
     async def set_registry_state(self, *, rev_reg_id: str, state: str) -> RevRegResult:
         """Set revocation registry state manually"""
         return await self.__set_registry_state(
@@ -201,14 +209,16 @@
             state=state,
         )
 
     async def update_registry(
         self, *, rev_reg_id: str, body: Optional[RevRegUpdateTailsFileUri] = None
     ) -> RevRegResult:
         """Update revocation registry with new public URI to its tails file"""
+        if not body:
+            body = RevRegUpdateTailsFileUri()
         return await self.__update_registry(
             rev_reg_id=rev_reg_id,
             body=body,
         )
 
     async def upload_tails_file(self, *, rev_reg_id: str) -> Dict[str, Any]:
         """Upload local tails file to server"""
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/schema.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         self,
         *,
         conn_id: Optional[str] = None,
         create_transaction_for_endorser: Optional[bool] = None,
         body: Optional[SchemaSendRequest] = None
     ) -> TxnOrSchemaSendResult:
         """Sends a schema to the ledger"""
+        if not body:
+            body = SchemaSendRequest()
         return await self.__publish_schema(
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
             body=body,
         )
 
     async def write_record(self, *, schema_id: str) -> SchemaGetResult:
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/server.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/server.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/api/wallet.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/wallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from aries_cloudcontroller.model.did_list import DIDList
 from aries_cloudcontroller.model.did_result import DIDResult
 
 
 class WalletApi(Consumer):
     async def create_did(self, *, body: Optional[DIDCreate] = None) -> DIDResult:
         """Create a local DID"""
+        if not body:
+            body = DIDCreate()
         return await self.__create_did(
             body=body,
         )
 
     async def get_did_endpoint(self, *, did: str) -> DIDEndpoint:
         """Query DID endpoint in wallet"""
         return await self.__get_did_endpoint(
@@ -69,14 +71,16 @@
         self,
         *,
         conn_id: Optional[str] = None,
         create_transaction_for_endorser: Optional[bool] = None,
         body: Optional[DIDEndpointWithType] = None
     ) -> Dict[str, Any]:
         """Update endpoint in wallet and on ledger if posted to it"""
+        if not body:
+            body = DIDEndpointWithType()
         return await self.__set_did_endpoint(
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
             body=body,
         )
 
     async def set_public_did(
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/client.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from contextlib import AbstractAsyncContextManager
 from typing import Dict
 
 import uplink
+
 from aries_cloudcontroller.api import (
     ActionMenuApi,
     BasicmessageApi,
     ConnectionApi,
     CredentialDefinitionApi,
     CredentialsApi,
     DefaultApi,
@@ -23,14 +24,15 @@
     OutOfBandApi,
     PresentProofV10Api,
     PresentProofV20Api,
     ResolverApi,
     RevocationApi,
     SchemaApi,
     ServerApi,
+    SettingsApi,
     TrustpingApi,
     WalletApi,
 )
 
 
 class Client(AbstractAsyncContextManager):
     action_menu: ActionMenuApi
@@ -53,14 +55,15 @@
     out_of_band: OutOfBandApi
     present_proof_v1_0: PresentProofV10Api
     present_proof_v2_0: PresentProofV20Api
     resolver: ResolverApi
     revocation: RevocationApi
     schema: SchemaApi
     server: ServerApi
+    settings: SettingsApi
     trustping: TrustpingApi
     wallet: WalletApi
 
     def __init__(
         self,
         base_url: str,
         client: uplink.AiohttpClient,
@@ -96,14 +99,15 @@
         self.out_of_band = OutOfBandApi(**service_params)
         self.present_proof_v1_0 = PresentProofV10Api(**service_params)
         self.present_proof_v2_0 = PresentProofV20Api(**service_params)
         self.resolver = ResolverApi(**service_params)
         self.revocation = RevocationApi(**service_params)
         self.schema = SchemaApi(**service_params)
         self.server = ServerApi(**service_params)
+        self.settings = SettingsApi(**service_params)
         self.trustping = TrustpingApi(**service_params)
         self.wallet = WalletApi(**service_params)
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.client.close()
 
     async def close(self):
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/__init__.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,15 @@
 from aries_cloudcontroller.model.oob_record import OobRecord
 from aries_cloudcontroller.model.perform_request import PerformRequest
 from aries_cloudcontroller.model.ping_request import PingRequest
 from aries_cloudcontroller.model.ping_request_response import PingRequestResponse
 from aries_cloudcontroller.model.presentation_definition import PresentationDefinition
 from aries_cloudcontroller.model.presentation_proposal import PresentationProposal
 from aries_cloudcontroller.model.presentation_request import PresentationRequest
+from aries_cloudcontroller.model.profile_settings import ProfileSettings
 from aries_cloudcontroller.model.protocol_descriptor import ProtocolDescriptor
 from aries_cloudcontroller.model.publish_revocations import PublishRevocations
 from aries_cloudcontroller.model.queries import Queries
 from aries_cloudcontroller.model.query import Query
 from aries_cloudcontroller.model.query_item import QueryItem
 from aries_cloudcontroller.model.raw_encoded import RawEncoded
 from aries_cloudcontroller.model.receive_invitation_request import (
@@ -275,14 +276,15 @@
     TxnOrPublishRevocationsResult,
 )
 from aries_cloudcontroller.model.txn_or_register_ledger_nym_response import (
     TxnOrRegisterLedgerNymResponse,
 )
 from aries_cloudcontroller.model.txn_or_rev_reg_result import TxnOrRevRegResult
 from aries_cloudcontroller.model.txn_or_schema_send_result import TxnOrSchemaSendResult
+from aries_cloudcontroller.model.update_profile_settings import UpdateProfileSettings
 from aries_cloudcontroller.model.update_wallet_request import UpdateWalletRequest
 from aries_cloudcontroller.model.v10_credential_bound_offer_request import (
     V10CredentialBoundOfferRequest,
 )
 from aries_cloudcontroller.model.v10_credential_conn_free_offer_request import (
     V10CredentialConnFreeOfferRequest,
 )
@@ -572,14 +574,15 @@
     "OobRecord",
     "PerformRequest",
     "PingRequest",
     "PingRequestResponse",
     "PresentationDefinition",
     "PresentationProposal",
     "PresentationRequest",
+    "ProfileSettings",
     "ProtocolDescriptor",
     "PublishRevocations",
     "Queries",
     "Query",
     "QueryItem",
     "RawEncoded",
     "ReceiveInvitationRequest",
@@ -617,14 +620,15 @@
     "TransactionList",
     "TransactionRecord",
     "TxnOrCredentialDefinitionSendResult",
     "TxnOrPublishRevocationsResult",
     "TxnOrRegisterLedgerNymResponse",
     "TxnOrRevRegResult",
     "TxnOrSchemaSendResult",
+    "UpdateProfileSettings",
     "UpdateWalletRequest",
     "V10CredentialBoundOfferRequest",
     "V10CredentialConnFreeOfferRequest",
     "V10CredentialCreate",
     "V10CredentialExchange",
     "V10CredentialExchangeListResult",
     "V10CredentialFreeOfferRequest",
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/action_menu_fetch_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/action_menu_fetch_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_config.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_config.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_mediation_deny.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_mediation_deny.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_modules.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_modules.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_status.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_status_liveliness.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status_liveliness.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/admin_status_readiness.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status_readiness.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/aml_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/aml_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator_data.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator_data1_jws.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data1_jws.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator_data_jws.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data_jws.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attach_decorator_data_jws_header.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data_jws_header.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attachment_def.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attachment_def.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/attribute_mime_types_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attribute_mime_types_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/claim_format.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/claim_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/clear_pending_revocations_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/clear_pending_revocations_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/conn_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/conn_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_invitation.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_invitation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_metadata.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_metadata.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_metadata_set_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_metadata_set_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_static_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_static_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/connection_static_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_static_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/constraints.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/constraints.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_invitation_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_invitation_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_wallet_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 
 class CreateWalletRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
     CreateWalletRequest - a model defined in OpenAPI
+        extra_settings: Agent config key-value pairs [Optional].
         image_url: Image url for this wallet. This image url is publicized            (self-attested) to other agents as part of forming a connection. [Optional].
         key_management_mode: Key management method to use for this wallet. [Optional].
         label: Label for this wallet. This label is publicized            (self-attested) to other agents as part of forming a connection. [Optional].
         wallet_dispatch_type: Webhook target dispatch type for this wallet.             default - Dispatch only to webhooks associated with this wallet.             base - Dispatch only to webhooks associated with the base wallet.             both - Dispatch to both webhook targets. [Optional].
         wallet_key: Master key used for key derivation. [Optional].
         wallet_key_derivation: Key derivation [Optional].
         wallet_name: Wallet name [Optional].
         wallet_type: Type of the wallet to create [Optional].
         wallet_webhook_urls: List of Webhook URLs associated with this subwallet [Optional].
     """
 
+    extra_settings: Optional[Dict[str, Any]] = None
     image_url: Optional[str] = None
     key_management_mode: Optional[Literal["managed"]] = None
     label: Optional[str] = None
     wallet_dispatch_type: Optional[Literal["default", "both", "base"]] = None
     wallet_key: Optional[str] = None
     wallet_key_derivation: Optional[Literal["ARGON2I_MOD", "ARGON2I_INT", "RAW"]] = None
     wallet_name: Optional[str] = None
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_wallet_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_wallet_token_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_token_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/create_wallet_token_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_token_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_attr_spec.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_def_value.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_def_value_primary.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value_primary.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_def_value_revocation.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value_revocation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_info_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_info_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_rev_indy_records_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_indy_records_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_rev_record_details_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_record_details_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_rev_record_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_record_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/cred_revoked_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_revoked_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definition.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definition_get_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_get_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definition_send_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_send_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definition_send_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_definitions_created_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definitions_created_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_offer.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_offer.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_preview.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_preview.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_proposal.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/credential_status_options.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_status_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/date.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/date.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_create.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_create.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_create_options.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_create_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_endpoint.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_endpoint.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_endpoint_with_type.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_endpoint_with_type.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/did_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/didx_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/didx_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_field.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_field.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_holder.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_holder.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_options.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_pres_spec.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_pres_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_proof_proposal.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_proof_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/dif_proof_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_proof_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/disclose.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/disclose.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/disclosures.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/disclosures.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/doc.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/doc.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/endorser_info.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/endorser_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/endpoints_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/endpoints_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/filter.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/filter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/generated.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/generated.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/get_did_endpoint_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_did_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/get_did_verkey_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_did_verkey_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/get_nym_role_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_nym_role_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_attr_value.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_attr_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_cred_abstract.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_abstract.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_cred_info.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_cred_precis.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_precis.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_cred_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_credential.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_credential.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_eq_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_eq_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_ge_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_ge_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_ge_proof_pred.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_ge_proof_pred.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_key_correctness_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_key_correctness_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_non_revoc_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_non_revoc_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_non_revocation_interval.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_non_revocation_interval.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_pres_attr_spec.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_pres_pred_spec.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_pred_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_pres_preview.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_preview.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_pres_spec.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_primary_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_primary_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_identifier.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_identifier.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_req_attr_spec.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_req_pred_spec.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_pred_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_request_non_revoked.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_request_non_revoked.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_requested_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_def.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_def_value.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_entry.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_entry.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/indy_rev_reg_entry_value.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_entry_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/input_descriptors.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/input_descriptors.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/invitation_create_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_create_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/invitation_message.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_message.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/invitation_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/invitation_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/issuer_cred_rev_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/issuer_cred_rev_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/issuer_rev_reg_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/issuer_rev_reg_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_query.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_query_filter_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query_filter_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_query_paginate.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query_paginate.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_update.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_update_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/keylist_update_rule.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update_rule.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ld_proof_vc_detail.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ld_proof_vc_detail.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ld_proof_vc_detail_options.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ld_proof_vc_detail_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ledger_config_instance.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ledger_config_instance.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ledger_config_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ledger_config_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/linked_data_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/linked_data_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_create_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_create_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_deny.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_deny.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_grant.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_grant.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_id_match_info.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_id_match_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/mediation_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu_form.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_form.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu_form_param.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_form_param.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu_json.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_json.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/menu_option.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_option.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/model_schema.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/model_schema.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/oob_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/oob_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/perform_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/perform_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ping_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ping_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/ping_request_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ping_request_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/presentation_definition.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_definition.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/presentation_proposal.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/presentation_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/protocol_descriptor.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/publish_revocations.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/publish_revocations.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/queries.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/queries.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/query.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/query.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/query_item.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/query_item.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/raw_encoded.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/raw_encoded.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/receive_invitation_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/receive_invitation_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/remove_wallet_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/remove_wallet_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/resolution_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/resolution_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_create_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_create_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_issued_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_issued_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/rev_regs_created.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_regs_created.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/revoke_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/revoke_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/route_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/route_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schema_get_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_get_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schema_input_descriptor.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_input_descriptor.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schema_send_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_send_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schema_send_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schemas_created_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schemas_created_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/schemas_input_descriptor_filter.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schemas_input_descriptor_filter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/send_menu.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/send_menu.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/send_message.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/send_message.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/service_decorator.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/service_decorator.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/sign_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/sign_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/sign_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/sign_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/signature_options.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/signature_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/signed_doc.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/signed_doc.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/submission_requirements.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/submission_requirements.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_accept.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_accept.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_acceptance.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_acceptance.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_info.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/taa_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/tails_delete_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/tails_delete_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/transaction_jobs.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_jobs.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/transaction_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/transaction_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_publish_revocations_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_publish_revocations_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_rev_reg_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_rev_reg_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/txn_or_schema_send_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_schema_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/update_wallet_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/update_wallet_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 
 class UpdateWalletRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
     UpdateWalletRequest - a model defined in OpenAPI
+        extra_settings: Agent config key-value pairs [Optional].
         image_url: Image url for this wallet. This image url is publicized            (self-attested) to other agents as part of forming a connection. [Optional].
         label: Label for this wallet. This label is publicized            (self-attested) to other agents as part of forming a connection. [Optional].
         wallet_dispatch_type: Webhook target dispatch type for this wallet.             default - Dispatch only to webhooks associated with this wallet.             base - Dispatch only to webhooks associated with the base wallet.             both - Dispatch to both webhook targets. [Optional].
         wallet_webhook_urls: List of Webhook URLs associated with this subwallet [Optional].
     """
 
+    extra_settings: Optional[Dict[str, Any]] = None
     image_url: Optional[str] = None
     label: Optional[str] = None
     wallet_dispatch_type: Optional[Literal["default", "both", "base"]] = None
     wallet_webhook_urls: Optional[List[str]] = None
 
     class Config:
         allow_population_by_field_name = True
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_bound_offer_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_bound_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_create.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_create.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_exchange.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_exchange.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_exchange_list_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_exchange_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_free_offer_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_free_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_issue_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_issue_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_problem_report_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_credential_store_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_store_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_discovery_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_discovery_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_create_request_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_create_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_exchange.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_exchange.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_exchange_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_exchange_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_problem_report_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_proposal_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_proposal_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_send_request_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_send_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_attr_spec.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_bound_offer_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_bound_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_free.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_free.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_detail.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_detail.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_indy.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_indy.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_filter.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_filter_indy.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter_indy.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_format.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_issue.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_issue_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_offer.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_offer_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_preview.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_preview.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_proposal.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_request_free.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request_free.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_request_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_cred_store_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_store_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_discovery_exchange_result.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_exchange_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_discovery_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_issue_cred_schema_core.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_issue_cred_schema_core.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_create_request_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_create_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_ex_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_ex_record_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_format.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_problem_report_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_proposal.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_proposal_by_format.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_proposal_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_request_by_format.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_request_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_send_request_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_send_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/vc_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/vc_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/vc_record_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/vc_record_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/verify_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/verify_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/verify_response.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/verify_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/w3_c_credentials_list_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/w3_c_credentials_list_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/wallet_list.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/wallet_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/wallet_record.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/wallet_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/model/write_ledger_request.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/write_ledger_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller/util/pydantic_converter.py` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/pydantic_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """
 This module defines a converter that uses :py:mod:`pydantic` models
 to deserialize and serialize values.
 """
 
-from typing import Any
 import typing
-from pydantic.json import ENCODERS_BY_TYPE
-from uplink.converters.interfaces import Factory, Converter
-from uplink.utils import is_subclass
+from dataclasses import asdict, is_dataclass
+from typing import Any
 
 from pydantic import BaseModel
-from dataclasses import asdict, is_dataclass
+from pydantic.json import ENCODERS_BY_TYPE
+from uplink.converters.interfaces import Converter
 from uplink.converters.pydantic_ import PydanticConverter as InitialConverter
-from uplink.converters.pydantic_ import (
-    _PydanticResponseBody as _InitialResponseBody,
-)
+from uplink.converters.pydantic_ import _PydanticResponseBody as _InitialResponseBody
+from uplink.utils import is_subclass
 
 
 def pydantic_encoder(obj: Any) -> Any:
     if isinstance(obj, BaseModel):
-        return obj.dict(exclude_unset=True, exclude_none=True, by_alias=True)
+        return obj.dict(by_alias=True, exclude_unset=True, exclude_none=True)
     elif is_dataclass(obj):
         return asdict(obj)
 
     # Check the class type and its superclasses for a matching encoder
     for base in obj.__class__.__mro__[:-1]:
         try:
             encoder = ENCODERS_BY_TYPE[base]
@@ -118,27 +116,26 @@
 
     def _get_model(self, type_):
         if is_subclass(type_, BaseModel):
             return type_
 
         # Uplink does not natively support Union types
         # See https://github.com/prkumar/uplink/issues/233
-        if typing.get_origin(type_) is typing.Union:
-            if all(
-                is_subclass(inner_type, BaseModel)
-                or (
-                    is_subclass(typing.get_origin(inner_type), typing.Collection)
-                    and all(
-                        is_subclass(inner_type_child, BaseModel)
-                        for inner_type_child in typing.get_args(inner_type)
-                    )
+        if typing.get_origin(type_) is typing.Union and all(
+            is_subclass(inner_type, BaseModel)
+            or (
+                is_subclass(typing.get_origin(inner_type), typing.Collection)
+                and all(
+                    is_subclass(inner_type_child, BaseModel)
+                    for inner_type_child in typing.get_args(inner_type)
                 )
-                for inner_type in typing.get_args(type_)
-            ):
-                return type_
+            )
+            for inner_type in typing.get_args(type_)
+        ):
+            return type_
 
         raise ValueError("Expected pydantic.BaseModel subclass or instance")
 
     def _make_converter(self, converter, type_):
         try:
             model = self._get_model(type_)
         except ValueError:
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller.egg-info/PKG-INFO` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aries-cloudcontroller
-Version: 0.8.1rc9
+Version: 0.8.2b0
 Summary: A simple python package for controlling an aries agent through the admin-api interface
 Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.8.1rc9 Summary: A
+Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.8.2b0 Summary: A
 simple python package for controlling an aries agent through the admin-api
 interface Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/
 tree/main/aries_cloudcontroller Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `aries_cloudcontroller-0.8.1rc9/aries_cloudcontroller.egg-info/SOURCES.txt` & `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 aries_cloudcontroller/api/out_of_band.py
 aries_cloudcontroller/api/present_proof_v1_0.py
 aries_cloudcontroller/api/present_proof_v2_0.py
 aries_cloudcontroller/api/resolver.py
 aries_cloudcontroller/api/revocation.py
 aries_cloudcontroller/api/schema.py
 aries_cloudcontroller/api/server.py
+aries_cloudcontroller/api/settings.py
 aries_cloudcontroller/api/trustping.py
 aries_cloudcontroller/api/wallet.py
 aries_cloudcontroller/model/__init__.py
 aries_cloudcontroller/model/action_menu_fetch_result.py
 aries_cloudcontroller/model/admin_config.py
 aries_cloudcontroller/model/admin_mediation_deny.py
 aries_cloudcontroller/model/admin_modules.py
@@ -186,14 +187,15 @@
 aries_cloudcontroller/model/oob_record.py
 aries_cloudcontroller/model/perform_request.py
 aries_cloudcontroller/model/ping_request.py
 aries_cloudcontroller/model/ping_request_response.py
 aries_cloudcontroller/model/presentation_definition.py
 aries_cloudcontroller/model/presentation_proposal.py
 aries_cloudcontroller/model/presentation_request.py
+aries_cloudcontroller/model/profile_settings.py
 aries_cloudcontroller/model/protocol_descriptor.py
 aries_cloudcontroller/model/publish_revocations.py
 aries_cloudcontroller/model/queries.py
 aries_cloudcontroller/model/query.py
 aries_cloudcontroller/model/query_item.py
 aries_cloudcontroller/model/raw_encoded.py
 aries_cloudcontroller/model/receive_invitation_request.py
@@ -231,14 +233,15 @@
 aries_cloudcontroller/model/transaction_list.py
 aries_cloudcontroller/model/transaction_record.py
 aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
 aries_cloudcontroller/model/txn_or_publish_revocations_result.py
 aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
 aries_cloudcontroller/model/txn_or_rev_reg_result.py
 aries_cloudcontroller/model/txn_or_schema_send_result.py
+aries_cloudcontroller/model/update_profile_settings.py
 aries_cloudcontroller/model/update_wallet_request.py
 aries_cloudcontroller/model/v10_credential_bound_offer_request.py
 aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py
 aries_cloudcontroller/model/v10_credential_create.py
 aries_cloudcontroller/model/v10_credential_exchange.py
 aries_cloudcontroller/model/v10_credential_exchange_list_result.py
 aries_cloudcontroller/model/v10_credential_free_offer_request.py
@@ -305,19 +308,22 @@
 aries_cloudcontroller/model/verify_request.py
 aries_cloudcontroller/model/verify_response.py
 aries_cloudcontroller/model/w3_c_credentials_list_request.py
 aries_cloudcontroller/model/wallet_list.py
 aries_cloudcontroller/model/wallet_record.py
 aries_cloudcontroller/model/write_ledger_request.py
 aries_cloudcontroller/util/__init__.py
-aries_cloudcontroller/util/create_client_session.py
+aries_cloudcontroller/util/acapy_client_session.py
 aries_cloudcontroller/util/pydantic_converter.py
 tests/__init__.py
-tests/compare_dicts.py
 tests/conftest.py
-tests/test_acapy_client.py
+tests/client/__init__.py
+tests/client/test_acapy_client.py
+tests/client/test_pydantic_converter.py
 tests/model/__init__.py
 tests/model/test_credential_offer.py
 tests/model/test_invitation.py
 tests/model/test_presentation.py
 tests/model/test_v20_cred_ex_record.py
-tests/model/test_v20_pres_ex_record.py
+tests/model/test_v20_pres_ex_record.py
+tests/util/__init__.py
+tests/util/compare_dicts.py
```

### Comparing `aries_cloudcontroller-0.8.1rc9/setup.py` & `aries_cloudcontroller-0.8.2b0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module setup."""
 
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 PACKAGE_NAME = "aries_cloudcontroller"
 
 with open(os.path.abspath("README.md"), "r") as fh:
     long_description = fh.read()
 
 
@@ -14,15 +15,15 @@
     lineiter = (line.strip() for line in open(filename))
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 if __name__ == "__main__":
     setup(
         name=PACKAGE_NAME,
-        version="0.8.1-rc9",
+        version="0.8.2-beta0",
         description="A simple python package for controlling an aries agent through the admin-api interface",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller",
         packages=find_packages(),
         include_package_data=True,
         package_data={
```

### Comparing `aries_cloudcontroller-0.8.1rc9/tests/compare_dicts.py` & `aries_cloudcontroller-0.8.2b0/tests/util/compare_dicts.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.1rc9/tests/model/test_credential_offer.py` & `aries_cloudcontroller-0.8.2b0/tests/model/test_credential_offer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import pydantic
 import pytest
 
 from aries_cloudcontroller.model import CredentialOffer
-from tests.compare_dicts import equal_dicts
+from tests.util.compare_dicts import equal_dicts
 
 LOGGER = logging.getLogger(__name__)
 
 sample_credential_offer = {
     "@id": "123456789abcdefghi",
     "@type": "https://didcomm.org/issue-credential/1.0/offer-credential",
     "comment": "This is a credential offer",
```

### Comparing `aries_cloudcontroller-0.8.1rc9/tests/model/test_invitation.py` & `aries_cloudcontroller-0.8.2b0/tests/model/test_invitation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import pydantic
 import pytest
 
 from aries_cloudcontroller.model import InvitationMessage
-from tests.compare_dicts import equal_dicts
+from tests.util.compare_dicts import equal_dicts
 
 LOGGER = logging.getLogger(__name__)
 
 sample_invitation_message = {
     "@type": "https://didcomm.org/out-of-band/%VER/invitation",
     "@id": "<id used for context as pthid>",
     "label": "Faber College",
```

### Comparing `aries_cloudcontroller-0.8.1rc9/tests/model/test_presentation.py` & `aries_cloudcontroller-0.8.2b0/tests/model/test_presentation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import pydantic
 import pytest
 
 from aries_cloudcontroller.model import V10PresentationExchange
-from tests.compare_dicts import equal_dicts
+from tests.util.compare_dicts import equal_dicts
 
 LOGGER = logging.getLogger(__name__)
 
 sample_presentation = {
     "auto_present": "false",
     "connection_id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
     "created_at": "2021-04-08 09:04:01Z",
```

### Comparing `aries_cloudcontroller-0.8.1rc9/tests/model/test_v20_cred_ex_record.py` & `aries_cloudcontroller-0.8.2b0/tests/model/test_v20_cred_ex_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import pydantic
 import pytest
 
 from aries_cloudcontroller.model import V20CredExRecord
-from tests.compare_dicts import equal_dicts
+from tests.util.compare_dicts import equal_dicts
 
 LOGGER = logging.getLogger(__name__)
 
 sample_cred_ex_record = {
     "auto_issue": "true",
     "auto_offer": "true",
     "auto_remove": "false",
```

### Comparing `aries_cloudcontroller-0.8.1rc9/tests/model/test_v20_pres_ex_record.py` & `aries_cloudcontroller-0.8.2b0/tests/model/test_v20_pres_ex_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import pydantic
 import pytest
 
 from aries_cloudcontroller.model import V20PresExRecord
-from tests.compare_dicts import equal_dicts
+from tests.util.compare_dicts import equal_dicts
 
 LOGGER = logging.getLogger(__name__)
 
 sample_pres_ex_record = {
     "auto_present": "true",
     "auto_verify": "true",
     "by_format": {"pres": {"attach_id": "sample_id"}},
```

### Comparing `aries_cloudcontroller-0.8.1rc9/tests/test_acapy_client.py` & `aries_cloudcontroller-0.8.2b0/tests/client/test_acapy_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import re
 
 import pytest
-from aiohttp import ClientSession
 
 from aries_cloudcontroller.acapy_client import AcaPyClient
+from aries_cloudcontroller.util.acapy_client_session import AcaPyClientSession
 
 LOGGER = logging.getLogger(__name__)
 
 
 class TestAcaPyClient:
     admin_host = "http://localhost:1000"
     api_key = "api_key"
@@ -26,15 +26,15 @@
             match=re.escape("api_key property is missing"),
         ):
             async with AcaPyClient(self.admin_host):
                 pass
 
     @pytest.mark.anyio
     async def test_client_session_stays_open(self):
-        async with ClientSession() as client_session:
+        async with AcaPyClientSession() as client_session:
             async with AcaPyClient(
                 self.admin_host, client_session=client_session, admin_insecure=True
             ):
                 pass
             # After AcaPyClient is closed, session should remain open
             assert client_session.closed is False
 
@@ -52,15 +52,15 @@
 
     @pytest.mark.anyio
     async def test_client_session_requires_api_key(self):
         with pytest.raises(
             Exception,
             match=re.escape("api_key property is missing"),
         ):
-            async with ClientSession() as client_session:
+            async with AcaPyClientSession() as client_session:
                 async with AcaPyClient(self.admin_host, client_session=client_session):
                     pass
 
     @pytest.mark.anyio
     async def test_client_session_creates_with_keys(self):
         async with AcaPyClient(
             self.admin_host, api_key=self.api_key, tenant_jwt=self.tenant_jwt
```

