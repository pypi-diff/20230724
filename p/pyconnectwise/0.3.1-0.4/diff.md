# Comparing `tmp/pyconnectwise-0.3.1.tar.gz` & `tmp/pyconnectwise-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconnectwise-0.3.1.tar", last modified: Thu Jul 20 00:42:16 2023, max compression
+gzip compressed data, was "pyconnectwise-0.4.tar", last modified: Mon Jul 24 08:14:36 2023, max compression
```

## Comparing `pyconnectwise-0.3.1.tar` & `pyconnectwise-0.4.tar`

### file list

```diff
@@ -1,2444 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.848374 pyconnectwise-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-20 00:42:16.848374 pyconnectwise-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 00:42:16.848374 pyconnectwise-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.576369 pyconnectwise-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.576369 pyconnectwise-0.3.1/src/pyconnectwise/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.580370 pyconnectwise-0.3.1/src/pyconnectwise/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/clients/manage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.580370 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.580370 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/base/connectwise_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.768373 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyAddressFormatsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyAddressFormatsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyAddressFormatsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyAddressFormatsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyAddressFormatsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyAddressFormatsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyBillingSetupsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCommunicationTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCommunicationTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCommunicationTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCommunicationTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCommunicationTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCommunicationTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCommunicationTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCommunicationTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesDefaultEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdCustomStatusNotesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdCustomStatusNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdCustomStatusNotesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdGroupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdGroupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdGroupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdManagementReportNotificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdManagementReportNotificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdManagementReportNotificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdManagementReportSetupEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdManagementReportSetupIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdManagementSummaryReportsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdManagementSummaryReportsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdManagementSummaryReportsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdMergeEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdNotesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdNotesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdSitesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdSitesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdSitesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdSitesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdSitesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdSurveysCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdTeamsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdTeamsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdTeamsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdTracksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdTracksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdTracksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdTypeAssociationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdTypeAssociationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdTypeAssociationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesInfoTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesInfoTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesInfoTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesStatusesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesStatusesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompaniesTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompanyFinanceIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompanyPickerItemsClearEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompanyPickerItemsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompanyPickerItemsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompanyPickerItemsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompanyTypeAssociationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompanyTypeAssociationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCompanyTypeAssociationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsBulkEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsIdChangeTypeEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsStatusesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsStatusesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsStatusesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsStatusesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsStatusesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdQuestionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdQuestionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdQuestionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdQuestionsIdValuesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdQuestionsIdValuesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdQuestionsIdValuesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdQuestionsIdValuesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdQuestionsIdValuesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyConfigurationsTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactTypeAssociationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactTypeAssociationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactTypeAssociationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsDefaultEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsDepartmentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsDepartmentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsDepartmentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsDepartmentsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsDepartmentsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsDepartmentsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsDepartmentsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsDepartmentsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdCommunicationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdCommunicationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdCommunicationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdGroupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdGroupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdGroupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdImageEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdNotesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdNotesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdPortalSecurityEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdTracksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdTracksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdTracksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdTypeAssociationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdTypeAssociationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdTypeAssociationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsRelationshipsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsRelationshipsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsRelationshipsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsRequestPasswordEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsTypesCountInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyContactsValidatePortalCredentialsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCountriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCountriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCountriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCountriesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCountriesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyCountriesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyEntityTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyEntityTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyEntityTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyEntityTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyEntitytypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyEntitytypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyExpenseTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdCrossReferencesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdCrossReferencesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdCrossReferencesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdLoginsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdLoginsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdLoginsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdNotificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdNotificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdNotificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagedDevicesIntegrationsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementBackupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementBackupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementBackupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementIdExecuteManagedItSyncEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementIdLogDownloadEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementIdLogsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementIdManagementReportNotificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementIdManagementReportNotificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementIdManagementReportNotificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementItSolutionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementItSolutionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementItSolutionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementItSolutionsIdManagementProductsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementItSolutionsIdManagementProductsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementItSolutionsIdManagementProductsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementItSolutionsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyManagementItSolutionsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyMarketDescriptionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyMarketDescriptionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyMarketDescriptionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyMarketDescriptionsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyMarketDescriptionsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyMarketDescriptionsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyMarketDescriptionsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyMarketDescriptionsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyNoteTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyNoteTypesCountInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyNoteTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyNoteTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyNoteTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyNoteTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyOwnershipTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyOwnershipTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyOwnershipTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyOwnershipTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyOwnershipTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyOwnershipTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPaymentTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdInvoiceSetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdInvoiceSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdInvoiceSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdInvoiceSetupsIdTestTransactionEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdOpportunitySetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdOpportunitySetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdPasswordEmailSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdPasswordEmailSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdProjectSetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdProjectSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdProjectSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdServiceSetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdServiceSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsIdServiceSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsInvoiceSetupPaymentProcessorsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsInvoiceSetupPaymentProcessorsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalConfigurationsInvoiceSetupPaymentProcessorsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalSecurityLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalSecurityLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalSecurityLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalSecuritySettingsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalSecuritySettingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyPortalSecuritySettingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyStatesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyStatesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyStatesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyStatesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyStatesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyStatesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyStatesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyStatesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTeamRolesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTeamRolesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTeamRolesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTeamRolesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTeamRolesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTeamRolesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTeamRolesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTeamRolesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTracksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTracksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTracksIdActionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTracksIdActionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTracksIdActionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/CompanyTracksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ConfigurationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ConfigurationsTypesIdQuestionsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ConfigurationsTypesIdQuestionsIdValuesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ConfigurationsTypesIdQuestionsIdValuesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ConfigurationsTypesIdQuestionsIdValuesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ConfigurationsTypesIdQuestionsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ConfigurationsTypesIdQuestionsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ConfigurationsTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ConfigurationsTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseClassificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseClassificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseClassificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseEntriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseEntriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseEntriesIdAuditsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseEntriesIdAuditsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseEntriesIdAuditsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseEntriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseInfoTaxTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseInfoTaxTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseInfoTaxTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpensePaymentTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpensePaymentTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpensePaymentTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpensePaymentTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpensePaymentTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseReportsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseReportsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseReportsIdAuditsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseReportsIdAuditsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseReportsIdAuditsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseReportsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseReportsIdReverseEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseReportsIdSubmitEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ExpenseTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingBatchesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingBatchesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingBatchesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingBatchesIdEntriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingBatchesIdEntriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingBatchesIdEntriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingBatchesIdExportEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingExportEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingPackageSetupCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingPackageSetupEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingPackageSetupIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingPackagesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingPackagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingPackagesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedexpensesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedexpensesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedexpensesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedexpensesIdTaxableLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedexpensesIdTaxableLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedexpensesIdTaxableLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedinvoicesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedinvoicesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedinvoicesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedinvoicesIdTaxableLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedinvoicesIdTaxableLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedinvoicesIdTaxableLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedprocurementCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedprocurementEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedprocurementIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedprocurementIdTaxableLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedprocurementIdTaxableLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAccountingUnpostedprocurementIdTaxableLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdBoardDefaultsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdBoardDefaultsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdBoardDefaultsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkRoleExclusionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkRoleExclusionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkRoleExclusionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkTypeExclusionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkTypeExclusionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkTypeExclusionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkrolesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkrolesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkrolesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkrolesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkrolesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorkrolesInfoIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorktypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorktypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementTypesIdWorktypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdAdditionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdAdditionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdAdditionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdAdjustmentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdAdjustmentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdAdjustmentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdBoardDefaultsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdBoardDefaultsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdBoardDefaultsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdConfigurationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdConfigurationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdConfigurationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdSitesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdSitesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdSitesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorkRoleExclusionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorkRoleExclusionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorkRoleExclusionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorkTypeExclusionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorkTypeExclusionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorkTypeExclusionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorkrolesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorkrolesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorkrolesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorktypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorktypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsIdWorktypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceAgreementsTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBatchSetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBatchSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBatchSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingCyclesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingCyclesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingCyclesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingCyclesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingCyclesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingCyclesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingCyclesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingCyclesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingSetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingSetupsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingSetupsIdRoutingsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingSetupsIdRoutingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingSetupsIdRoutingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingSetupsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingStatusesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingStatusesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingStatusesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingStatusesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingStatusesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingTermsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingTermsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingTermsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingTermsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingTermsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingTermsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingTermsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceBillingTermsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceClosedInvoicesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCompanyFinanceCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCompanyFinanceEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCompanyFinanceIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCurrenciesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCurrenciesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCurrenciesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCurrenciesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCurrenciesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCurrenciesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCurrenciesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceCurrenciesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceDeliveryMethodsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceDeliveryMethodsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceDeliveryMethodsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlAccountsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlAccountsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlAccountsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlAccountsMappedTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlAccountsMappedTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlCaptionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlCaptionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlCaptionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlpathsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlpathsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceGlpathsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInfoCurrencyCodesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInfoCurrencyCodesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInfoCurrencyCodesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInfoInvoiceIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInfoTaxIntegrationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInfoTaxIntegrationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInfoTaxIntegrationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceEmailTemplatesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceEmailTemplatesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceEmailTemplatesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceEmailTemplatesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceEmailTemplatesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceEmailTemplatesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceEmailTemplatesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceEmailTemplatesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceTemplateSetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceTemplateSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceTemplateSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceTemplatesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceTemplatesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceTemplatesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceTemplatesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoiceTemplatesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoicesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoicesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoicesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoicesIdPaymentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoicesIdPaymentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceInvoicesIdPdfEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdExpenseTypeExemptionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdExpenseTypeExemptionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdExpenseTypeExemptionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdExpenseTypeExemptionsIdTaxableExpenseTypeLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdExpenseTypeExemptionsIdTaxableExpenseTypeLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdExpenseTypeExemptionsIdTaxableExpenseTypeLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdProductTypeExemptionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdProductTypeExemptionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdProductTypeExemptionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdProductTypeExemptionsIdTaxableProductTypeLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdProductTypeExemptionsIdTaxableProductTypeLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdProductTypeExemptionsIdTaxableProductTypeLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdTaxCodeLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdTaxCodeLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdTaxCodeLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdTaxCodeXRefsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdTaxCodeXRefsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdTaxCodeXRefsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdTaxCodeXRefsIdTaxableXRefLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdTaxCodeXRefsIdTaxableXRefLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdTaxCodeXRefsIdTaxableXRefLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdWorkRoleExemptionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdWorkRoleExemptionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdWorkRoleExemptionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdWorkRoleExemptionsIdTaxableWorkRoleLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdWorkRoleExemptionsIdTaxableWorkRoleLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesIdWorkRoleExemptionsIdTaxableWorkRoleLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxCodesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxIntegrationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxIntegrationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/FinanceTaxIntegrationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdActivitiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdActivitiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdAuditsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdAuditsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdAuditsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdEmailsOpenedCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdEmailsOpenedEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdEmailsOpenedIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdFormsSubmittedCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdFormsSubmittedEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdFormsSubmittedIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdLinksClickedCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdLinksClickedEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdLinksClickedIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdOpportunitiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsIdOpportunitiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsSubTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsSubTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsSubTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsTypesIdSubTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsTypesIdSubTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsTypesIdSubTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingCampaignsTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsIdCompaniesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsIdCompaniesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsIdCompaniesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsIdContactsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsIdContactsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsIdContactsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/MarketingGroupsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsIdDetailsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsIdDetailsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsIdDetailsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementAdjustmentsTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdComponentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdComponentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdComponentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdInventoryCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdInventoryEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdInventoryIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdMinimumStockByWarehouseCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdMinimumStockByWarehouseEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdMinimumStockByWarehouseIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogIdPricingEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalogInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCatalog{catalogItemIdentifier}QuantityOnHandEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesIdSubcategoriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesIdSubcategoriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesIdSubcategoriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesIdSubcategoriesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesIdSubcategoriesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesIdSubcategoriesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementCategoriesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementManufacturersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementManufacturersCountInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementManufacturersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementManufacturersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementManufacturersIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementManufacturersInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementOnhandserialnumbersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementOnhandserialnumbersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementOnhandserialnumbersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPricingschedulesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPricingschedulesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPricingschedulesIdDetailsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPricingschedulesIdDetailsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPricingschedulesIdDetailsIdBreaksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPricingschedulesIdDetailsIdBreaksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPricingschedulesIdDetailsIdBreaksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPricingschedulesIdDetailsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPricingschedulesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsIdComponentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsIdComponentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsIdComponentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsIdDetachEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsIdPickingShippingDetailsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsIdPickingShippingDetailsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementProductsIdPickingShippingDetailsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseordersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseordersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseordersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseordersIdLineitemsBulkEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseordersIdLineitemsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseordersIdLineitemsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseordersIdLineitemsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesIdEmailtemplatesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesIdEmailtemplatesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesIdEmailtemplatesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesIdNotificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesIdNotificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesIdNotificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchaseorderstatusesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementPurchasingDemandsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRMADispositionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRMADispositionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRMADispositionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRMADispositionsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRMADispositionsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRMADispositionsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaActionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaActionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaActionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaActionsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaActionsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaActionsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdEmailtemplatesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdEmailtemplatesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdEmailtemplatesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdNotificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdNotificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdNotificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaStatusesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaTagsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaTagsDefaultEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaTagsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementRmaTagsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSettingsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSettingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSettingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementShipmentmethodsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementShipmentmethodsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementShipmentmethodsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementShipmentmethodsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementShipmentmethodsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementShipmentmethodsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementShipmentmethodsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementShipmentmethodsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSubcategoriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSubcategoriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSubcategoriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSubcategoriesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSubcategoriesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSubcategoriesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSubcategoriesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementSubcategoriesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementUnitOfMeasuresCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementUnitOfMeasuresEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementUnitOfMeasuresIdConversionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementUnitOfMeasuresIdConversionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementUnitOfMeasuresIdConversionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementUnitOfMeasuresIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehouseBinsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehouseBinsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehouseBinsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehouseBinsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehouseBinsIdInventoryOnHandCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehouseBinsIdInventoryOnHandEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehouseBinsIdInventoryOnHandIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehouseBinsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehouseBinsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehousesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehousesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehousesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehousesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehousesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProcurementWarehousesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectBoardsIdTeamsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectBoardsIdTeamsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectBoardsIdTeamsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectBoardsIdTeamsIdInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectBoardsIdTeamsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectBoardsIdTeamsIdMembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectBoardsIdTeamsIdMembersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectBoardsIdTeamsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectPhaseStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectPhaseStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectPhaseStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectPhaseStatusesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectPhaseStatusesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdContactsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdContactsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdNotesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdNotesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdPhasesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdPhasesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdPhasesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdTeamMembersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdTeamMembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectProjectsIdTeamMembersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectSecurityRolesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectSecurityRolesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectSecurityRolesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectSecurityRolesIdSettingsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectSecurityRolesIdSettingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectSecurityRolesIdSettingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectStatusIndicatorsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectStatusIndicatorsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectStatusIndicatorsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectStatusesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectStatusesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectStatusesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketNoteIdMarkAsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdActivitiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdActivitiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdAllNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdConfigurationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdConfigurationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdConfigurationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdConvertEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdDocumentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdDocumentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdNotesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdNotesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdProductsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdProductsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdScheduleentriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdScheduleentriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdTasksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdTasksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdTasksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdTimeentriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsIdTimeentriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ProjectTicketsSearchEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesStatusesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesStatusesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesStatusesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesActivitiesTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesCommissionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesCommissionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesCommissionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesCommissionsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesCommissionsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesDefaultEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdContactsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdContactsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdContactsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdConvertToAgreementEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdConvertToProjectEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdConvertToSalesOrderEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdConvertToServiceTicketEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdForecastCopyIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdForecastCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdForecastEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdForecastIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdNotesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdNotesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdTeamCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdTeamEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesIdTeamIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesRatingsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesRatingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesRatingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesRatingsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesRatingsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesRatingsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesStatusesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesStatusesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesStatusesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesStatusesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesStatusesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOpportunitiesTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersIdConvertToServiceTicketEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdEmailtemplatesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdEmailtemplatesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdEmailtemplatesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdNotificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdNotificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdNotificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesOrdersStatusesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesProbabilitiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesProbabilitiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesProbabilitiesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesProbabilitiesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesProbabilitiesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesProbabilitiesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesQuotasCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesQuotasEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesQuotasIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesRolesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesRolesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesRolesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesSalesTeamsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesSalesTeamsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesSalesTeamsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesSalesTeamsIdMembersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesSalesTeamsIdMembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesSalesTeamsIdMembersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesScheduleHolidaylistsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesServicePriorityInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesStagesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesStagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesStagesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesStagesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesStagesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesStagesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesStagesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SalesStagesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleCalendarsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleCalendarsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleCalendarsIdCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleCalendarsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleCalendarsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleCalendarsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleCalendarsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleCalendarsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleCalendarsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleColorsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleColorsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleColorsIdClearEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleColorsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleColorsResetEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleDetailsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleDetailsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleDetailsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleEntriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleEntriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleEntriesIdDetailsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleEntriesIdDetailsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleEntriesIdDetailsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleEntriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidayListsCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidayListsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidayListsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidayListsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidayListsIdHolidaysCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidayListsIdHolidaysEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidayListsIdHolidaysIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidayListsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidayListsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidaylistsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleHolidaylistsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SchedulePortalcalendarsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SchedulePortalcalendarsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SchedulePortalcalendarsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleReminderTimesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleReminderTimesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleReminderTimesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ScheduleTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdAutoAssignResourcesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdAutoAssignResourcesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdAutoAssignResourcesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdAutoTemplatesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdAutoTemplatesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdAutoTemplatesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdExcludedMembersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdExcludedMembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdExcludedMembersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdItemsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdItemsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdItemsIdAssociationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdItemsIdAssociationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdItemsIdAssociationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdItemsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdItemsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdItemsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdNotificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdNotificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdNotificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesIdNotificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesIdNotificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesIdNotificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdStatusesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdSubtypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdSubtypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdSubtypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdSubtypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdSubtypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdSubtypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdSubtypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdSubtypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTeamsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTeamsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTeamsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTeamsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTeamsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTeamsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTeamsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTypeSubTypeItemAssociationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTypeSubTypeItemAssociationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTypeSubTypeItemAssociationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceBoardsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceCodesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceCodesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceCodesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceEmailTemplatesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceEmailTemplatesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceEmailTemplatesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceEmailTemplatesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceEmailTemplatesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceImpactsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceImpactsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceImpactsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceInfoBoardsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceInfoBoardsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceInfoBoardsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceInfoBoardtypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceInfoBoardtypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceInfoBoardtypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseArticlesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseArticlesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseArticlesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseCategoriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseCategoriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseCategoriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseSubCategoriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseSubCategoriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseSubCategoriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseSubCategoriesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgeBaseSubCategoriesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgebasesettingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceKnowledgebasesettingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceLocationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceLocationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceLocationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceLocationsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceLocationsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceLocationsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServicePrioritiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServicePrioritiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServicePrioritiesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServicePrioritiesIdImageEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServicePrioritiesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServicePrioritiesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServicePriorityIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServicePriorityInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSLAsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSLAsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSLAsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSLAsIdPrioritiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSLAsIdPrioritiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSLAsIdPrioritiesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSLAsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSLAsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSLAsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSchedulingMembersIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSchedulingMembersInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSchedulingMembersInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceServiceSignoffCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceServiceSignoffEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceServiceSignoffIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceServiceSignoffIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceServiceSignoffIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceServiceSignoffIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceServiceSignoffInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceServiceSignoffInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSeveritiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSeveritiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSeveritiesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSlainfoIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSlainfoInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSourcesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSourcesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSourcesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSourcesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSourcesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSourcesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSourcesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSourcesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdQuestionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdQuestionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdQuestionsIdCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdQuestionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdQuestionsIdOptionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdQuestionsIdOptionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdQuestionsIdOptionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdResultsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdResultsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdResultsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceSurveysIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTeamMembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTeamsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTeamsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTeamsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTemplatesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTemplatesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTemplatesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTemplatesIdGenerateEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTemplatesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTemplatesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTemplatesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketLinksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketLinksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketLinksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketLinksIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketLinksInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketLinksInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketSyncsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketSyncsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketSyncsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdActivitiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdActivitiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdAllNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdAttachChildrenEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdConfigurationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdConfigurationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdConfigurationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdConvertEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdDocumentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdDocumentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdMergeEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdNotesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdNotesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdProductsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdProductsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdScheduleentriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdScheduleentriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdTasksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdTasksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdTasksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdTimeentriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsIdTimeentriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/ServiceTicketsSearchEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAllowedfiletypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAllowedfiletypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAllowedfiletypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAllowedoriginsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAllowedoriginsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAllowedoriginsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemApiMembersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemApiMembersDefaultEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemApiMembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemApiMembersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAudittrailCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAudittrailEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAuthAnvilsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAuthAnvilsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAuthAnvilsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAuthAnvilsTestConnectionEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAutoSyncTimeCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAutoSyncTimeEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemAutoSyncTimeIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemBundlesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemBundlesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCallbacksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCallbacksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCallbacksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCertificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCertificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCertificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCertificationsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCertificationsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemConnectWiseHostedScreensCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemConnectWiseHostedScreensEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemConnectWiseHostedScreensIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemConnectwisehostedsetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemConnectwisehostedsetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemConnectwisehostedsetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCustomReportsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCustomReportsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCustomReportsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCustomReportsIdParametersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCustomReportsIdParametersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCustomReportsIdParametersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCwTimeZonesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCwTimeZonesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemCwTimeZonesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDepartmentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDepartmentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDepartmentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDepartmentsIdLocationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDepartmentsIdLocationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDepartmentsIdLocationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDepartmentsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDepartmentsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDocumentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDocumentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDocumentsIdDownloadEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDocumentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDocumentsIdThumbnailEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemDocumentsUploadsampleEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEPayConfigurationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEPayConfigurationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEPayConfigurationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsIdParsingStylesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsIdParsingStylesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsIdParsingStylesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsIdParsingStylesIdParsingRulesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsIdParsingStylesIdParsingRulesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsIdParsingStylesIdParsingRulesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailConnectorsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailExclusionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailExclusionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailExclusionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailTokensCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailTokensEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEmailTokensIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemExperimentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemExperimentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemExperimentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemFileuploadsettingsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemFileuploadsettingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemFileuploadsettingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemGoogleemailsetupCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemGoogleemailsetupEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemGoogleemailsetupIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemGoogleemailsetupIdTestConnectionEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemImapsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemImapsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemImapsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemImapsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemImapsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemImapsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemImportMassMaintenanceIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInOutBoardsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInOutBoardsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInOutBoardsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInOutTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInOutTypesCountInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInOutTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInOutTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInOutTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInOutTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoDepartmentlocationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoDepartmentlocationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoDepartmentlocationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoDepartmentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoDepartmentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoDepartmentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLinksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLinksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLinksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLinksIdResolveurlEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLocalesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLocalesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLocalesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLocationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLocationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoLocationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoMembersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoMembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoMembersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoPersonasCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoPersonasEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoPersonasIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoStandardNotesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoStandardNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemInfoStandardNotesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemIntegratorTagsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemIntegratorTagsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemIntegratorTagsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemIntegratorloginsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemIntegratorloginsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemIntegratorloginsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemKpiCategoriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemKpiCategoriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemKpiCategoriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemKpisCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemKpisEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemKpisIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLdapConfigurationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLdapConfigurationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLdapConfigurationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLdapConfigurationsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLdapConfigurationsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLdapConfigurationsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLdapConfigurationsTestLinkEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLinksCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLinksEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLinksIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsIdDepartmentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsIdDepartmentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsIdDepartmentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsIdWorkRolesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsIdWorkRolesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemLocationsIdWorkRolesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemManagementNetworkSecuritiesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemManagementNetworkSecuritiesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemManagementNetworkSecuritiesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemManagementNetworkSecuritiesIdTestCredentialsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMarketplaceimportGetdefinitionIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMarketplaceimportImportEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdAccrualsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdAccrualsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdAccrualsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdCertificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdCertificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdCertificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdDeactivateEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdDelegationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdDelegationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdDelegationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdImageEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdLinkSsoUserEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdManagedDeviceAccountsBulkEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdManagedDeviceAccountsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdMycertificationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdMycertificationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdMycertificationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdNotificationSettingsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdNotificationSettingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdNotificationSettingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdPersonasCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdPersonasEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdPersonasIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdSkillsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdSkillsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdSkillsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdSubmitEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdUnlinkSsoUserEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdUnusedTimeSheetsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembersWithSsoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMembers{memberIdentifier}TokensEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMenuEntriesIdLocationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMenuEntriesIdLocationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMenuEntriesIdLocationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMenuentriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMenuentriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMenuentriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMenuentriesIdImageEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyAccountIdDelegationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyAccountIdDelegationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyAccountIdDelegationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyAccountIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyAccountIdSkillsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyAccountIdSkillsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyAccountIdSkillsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCorporateStructureCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCorporateStructureEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCorporateStructureIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCorporateStructureIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCorporateStructureInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCorporateStructureInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCorporateStructureLevelsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCorporateStructureLevelsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCorporateStructureLevelsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCrmCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCrmEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCrmIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCrmIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCrmInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyCrmInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyOtherCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyOtherEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyOtherIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyTimeExpenseCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyTimeExpenseEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyCompanyTimeExpenseIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyMembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMyMembersInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMySecurityCustomizeItemsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMySecurityEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMycompanyDocumentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMycompanyDocumentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMycompanyInfoServicesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMycompanyInfoServicesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMycompanyReportingServicesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMycompanyReportingServicesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMycompanyReportingServicesIdTestConnectionEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMycompanyServicesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemMycompanyServicesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemNotificationRecipientsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemNotificationRecipientsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemNotificationRecipientsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemOffice365EmailSetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemOffice365EmailSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemOffice365EmailSetupsIdAuthorizeEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemOffice365EmailSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemOffice365EmailSetupsIdTestConnectionEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemOsgradeweightsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemOsgradeweightsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemOsgradeweightsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemParsingTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemParsingTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemParsingTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemParsingVariablesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemParsingVariablesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemParsingVariablesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemPortalReportsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemPortalReportsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemPortalReportsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemQuoteLinkSetupCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemQuoteLinkSetupEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemQuoteLinkSetupIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemQuoteLinkSetupTestConnectionEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportCardsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportCardsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportCardsIdDetailsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportCardsIdDetailsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportCardsIdDetailsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportCardsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportCardsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportCardsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportCardsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportsIdColumnsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportsIdCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemReportsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSecurityRolesIdSettingsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSecurityRolesIdSettingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSecurityRolesIdSettingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSecurityrolesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSecurityrolesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSecurityrolesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSecurityrolesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSecurityrolesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSecurityrolesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSettingsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSettingsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSettingsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSetupScreensCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSetupScreensEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSetupScreensIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSkillCategoriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSkillCategoriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSkillCategoriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSkillsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSkillsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSkillsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSkillsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSkillsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSkillsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSsoConfigurationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSsoConfigurationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSsoConfigurationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSsoConfigurationsIdRegistertokenEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSsoConfigurationsIdSubmitmembersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSsoUsersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSsoUsersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSsoUsersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemStandardNotesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemStandardNotesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemStandardNotesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysIdCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysIdQuestionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysIdQuestionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysIdQuestionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysIdQuestionsIdValuesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysIdQuestionsIdValuesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemSurveysInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemTimeZoneSetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemTimeZoneSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemTimeZoneSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemTimeZoneSetupsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemTimeZoneSetupsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemTimeZoneSetupsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemTodayPageCategoriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemTodayPageCategoriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemTodayPageCategoriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemUserDefinedFieldsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemUserDefinedFieldsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemUserDefinedFieldsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemUserDefinedFieldsIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemUserDefinedFieldsInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemUserDefinedFieldsInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowActionsIdAutomateParametersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowActionsIdAutomateParametersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowActionsIdAutomateParametersIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdAttachmentsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdAttachmentsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdAttachmentsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdEventsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdEventsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdEventsIdActionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdEventsIdActionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdEventsIdActionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdEventsIdCopyEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdEventsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdEventsIdTestEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdNotifyTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdNotifyTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdNotifyTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdNotifyTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdNotifyTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdNotifyTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdTriggersCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdTriggersEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdTriggersIdOptionsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsIdTriggersIdOptionsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsTableTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsTableTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsTableTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsTableTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsTableTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsTableTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsUserdefinedfieldsActionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsUserdefinedfieldsEventsIdActionsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsUserdefinedfieldsEventsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/SystemWorkflowsUserdefinedfieldsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeAccrualsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeAccrualsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeAccrualsIdDetailsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeAccrualsIdDetailsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeAccrualsIdDetailsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeAccrualsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeActivitystopwatchesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeActivitystopwatchesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeActivitystopwatchesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesIdExpenseTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesIdExpenseTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesIdExpenseTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeChargeCodesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeEntriesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeEntriesDefaultsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeEntriesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeEntriesIdAuditsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeEntriesIdAuditsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeEntriesIdAuditsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeEntriesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeInfoChargeCodeExpenseTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeInfoChargeCodeExpenseTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSchedulestopwatchesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSchedulestopwatchesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSchedulestopwatchesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsIdApproveEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsIdAuditsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsIdAuditsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsIdAuditsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsIdRejectEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsIdReverseEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeSheetsIdSubmitEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTicketstopwatchesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTicketstopwatchesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTicketstopwatchesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTimePeriodSetupsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTimePeriodSetupsDefaultEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTimePeriodSetupsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTimePeriodSetupsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTimePeriodSetupsIdPeriodsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTimePeriodSetupsIdPeriodsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeTimePeriodSetupsIdPeriodsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesIdLocationsCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesIdLocationsEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesIdLocationsIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkRolesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkTypesCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkTypesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkTypesIdEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkTypesIdInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkTypesIdUsagesEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkTypesIdUsagesListEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkTypesInfoCountEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/TimeWorkTypesInfoEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/endpoints/manage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.768373 pyconnectwise-0.3.1/src/pyconnectwise/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.768373 pyconnectwise-0.3.1/src/pyconnectwise/models/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/base/connectwise_model.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/base/message_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.848374 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AccountingBatchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AccountingPackageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AccountingPackageReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AccountingPackageSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ActivityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ActivityReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ActivityStatusInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ActivityStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ActivityStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ActivityStopwatchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ActivityTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ActivityTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AdditionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AddressFormatInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AddressFormatModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AddressFormatReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AdjustmentDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AdjustmentDetailReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AdjustmentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AdjustmentReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AdjustmentTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AdjustmentTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AdjustmentTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementBatchSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementBillingInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementSiteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementTypeBoardDefaultModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementTypeWorkRoleExclusionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementTypeWorkRoleInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementTypeWorkRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementTypeWorkTypeExclusionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementTypeWorkTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementWorkRoleExclusionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementWorkRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementWorkTypeExclusionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AgreementWorkTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AllowedFileTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AllowedOriginModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ApiMemberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AuditTrailEntryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AuthAnvilModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AutoSyncTimeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/AutomateScriptReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BatchEntryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingCycleInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingCycleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingCycleReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingDeliveryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingSetupInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingSetupReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingSetupRoutingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingStatusInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingTermInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingTermModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BillingTermsReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardAutoAssignResourceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardAutoTemplateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardDefaultModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardExcludedMemberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardItemAssociationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardItemModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardNotificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardStatusInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardStatusNotificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardSubTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardSubTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardTeamInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BoardTypeSubTypeItemAssociationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BulkResultModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BundleResultModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/BundleResultsCollectionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CalendarInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CalendarModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CalendarReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CalendarSetupReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CallbackEntryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignAuditModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignSubTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignSubTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CampaignTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CatalogComponentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CatalogInventoryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CatalogItemInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CatalogItemModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CatalogItemReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CatalogPricingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CategoryInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CategoryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CertificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CertificationReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ChargeCodeExpenseTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ChargeCodeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ChargeCodeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ChargeCodeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ClassificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ClassificationReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ClearPickerRequestModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ClosedInvoiceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CodeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CommissionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CommunicationTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CommunicationTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CommunicationTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyCustomNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyFinanceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyGroupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyManagementSummaryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyNoteTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyNoteTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyPickerItemModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanySiteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyTypeAssociationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CompanyTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationQuestionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationStatusInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationTypeQuestionInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationTypeQuestionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationTypeQuestionReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationTypeQuestionValueInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationTypeQuestionValueModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConfigurationTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConnectWiseHostedScreenModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConnectWiseHostedSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactCommunicationItemModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactCommunicationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactDepartmentInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactDepartmentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactDepartmentReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactGroupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactRelationshipModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactTrackModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactTypeAssociationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ContactTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ConversionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CorporateStructureInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CorporateStructureLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CorporateStructureLevelReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CorporateStructureModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CountModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CountryInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CountryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CountryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CrmInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CrmModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CurrencyCodeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CurrencyCodeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CurrencyInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CurrencyModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CurrencyReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CustomFieldValueModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CustomReportModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CustomReportParameterModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CustomReportReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/CwTimeZoneModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/DeliveryMethodModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/DepartmentInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/DepartmentLocationInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/DepartmentLocationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/DepartmentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/DocumentInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/DocumentReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/DocumentSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EPayConfigurationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailConnectorInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailConnectorModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailConnectorParsingRuleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailConnectorParsingStyleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailConnectorParsingStyleReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailConnectorParsingTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailConnectorParsingVariableReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailConnectorReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailExclusionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailOpenedModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailTemplateReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EmailTokenModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EntityTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EntityTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/EntityTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ErrorResponseMessageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseDetailReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseEntryAuditModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseEntryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseReportAuditModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseReportModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseReportReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseTaxModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseTaxTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseTaxTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseTypeExemptionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExpenseTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ExperimentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/FileUploadSettingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ForecastItemModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ForecastModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ForecastRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/FormSubmittedModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLAccountModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLCaptionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportAdjustmentTransactionDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportAdjustmentTransactionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportCustomerModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportCustomerTaxLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportExpenseBillDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportExpenseBillModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportExpenseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportExpenseOffsetModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportInventoryTransferModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportInventoryTransferOffsetModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportPurchaseTransactionDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportPurchaseTransactionDetailTaxModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportPurchaseTransactionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportPurchaseTransactionTaxLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportSettingsModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportTransactionDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportTransactionDetailTaxLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportTransactionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportTransactionTaxLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLExportVendorModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GLPathModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GenericBoardTeamReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GenericIdIdentifierReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GoogleEmailSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GoogleEmailSetupReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GroupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/GroupReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/HolidayListInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/HolidayListModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/HolidayListReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/HolidayModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/IRestIdentifiedItemModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ImapInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ImapModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ImapSetupReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ImpactModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ImportMassMaintenanceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InOutBoardModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InOutTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InOutTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InOutTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InclusiveRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/IntegratorLoginModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/IntegratorLoginReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/IntegratorTagModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InventoryOnHandModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceEmailTemplateInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceEmailTemplateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceGroupingReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceTemplateDetailReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceTemplateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceTemplateReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/InvoiceTemplateSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/IvItemReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/KBCategoryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/KPICategoryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/KPICategoryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/KPIModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/KPIReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/KnowledgeBaseArticleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/KnowledgeBaseCategoryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/KnowledgeBaseSettingsModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/KnowledgeBaseSubCategoryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LdapConfigurationInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LdapConfigurationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LdapConfigurationReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LegacySubCategoryInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LegacySubCategoryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LicenseBitModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LinkClickedModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LinkInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LinkModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LinkResolveUrlInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LocaleInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LocaleReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LocationDepartmentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LocationInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LocationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LocationWorkRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/LostRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagedDeviceAccountModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagedDevicesIntegrationCrossReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagedDevicesIntegrationInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagedDevicesIntegrationLoginModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagedDevicesIntegrationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagedDevicesIntegrationNotificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagedDevicesIntegrationReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagementBackupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagementItSolutionAgreementInterfaceParameterModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagementItSolutionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagementLogDocumentInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagementModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagementNetworkSecurityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagementReportNotificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagementReportSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManagementSolutionReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManufacturerInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManufacturerModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ManufacturerReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MappedRecordReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MappedTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MappedTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MarketDescriptionInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MarketDescriptionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MarketDescriptionReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MarketingCompanyModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MarketingContactModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MarketplaceImportModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberAccrualModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberCertificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationCompanyTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationDepartmentMananagerModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationDispatchMemberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationDutyManagerModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationKnowledgebaseArticleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationMyCompanyCOORoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationMyCompanyControllerRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationMyCompanyDispatchRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationMyCompanyDutyManagerRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationMyCompanyPresidentRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationMyCompanyServiceManagerRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationOpportunityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationProjectManagerModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationSalesActivityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationSalesTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationSendFromEmailNotifyModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationServiceMangerModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationServiceTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationServiceTemplateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationStatusWorkflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDeactivationWorkflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberDelegationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberNotificationSettingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberOffice365Model.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberPersonaModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberSkillModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberSsoSettingsReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MemberTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MenuEntryLocationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MenuEntryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MenuLocationReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MinimumStockByWarehouseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MyAccountModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MyMemberInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MyMemberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MySecurityCustomizeItemModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/MySecurityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/NoteTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/NotificationRecipientModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/NotificationRecipientReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/NotifyTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/Office365EmailSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/Office365EmailSetupReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OnHandSerialNumberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OnHandSerialNumberReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpenRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityContactModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityPriorityReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityProbabilityReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityRatingInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityRatingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityRatingReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunitySalesRoleReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityStageInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityStageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityStageReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityStatusInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OpportunityTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OrderModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OrderStatusEmailTemplateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OrderStatusEmailTemplateReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OrderStatusInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OrderStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OrderStatusNotificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OrderStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OsGradeWeightModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/Other1RevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/Other2RevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OtherModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OwnershipTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OwnershipTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/OwnershipTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ParsingTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ParsingVariableModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PaymentMethodReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PaymentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PaymentTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PaymentTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PersonasInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PhaseStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PhaseStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalCalendarModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalConfigurationInvoiceSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalConfigurationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalConfigurationOpportunitySetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalConfigurationPasswordEmailSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalConfigurationPaymentProcessorModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalConfigurationPaymentProcessorReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalConfigurationProjectSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalConfigurationReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalConfigurationServiceSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalReportModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalSecurityLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalSecurityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PortalSecuritySettingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PricingBreakModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PricingDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PricingScheduleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PricingScheduleReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PriorityInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PriorityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PriorityReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProcurementAdjustmentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProcurementSettingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductCategoryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductComponentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductDemandModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductDetachModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductItemModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductItemReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductPickingShippingDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductRecurringModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductSubCategoryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductTypeExemptionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProductTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectBoardReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectBoardTeamInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectBoardTeamMemberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectBoardTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectContactModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectPhaseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectPhaseReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectRoleReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectSecurityRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectSecurityRoleSettingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectStatusInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectTeamMemberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectTicketModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectTicketNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ProjectTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchaseOrderLineItemModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchaseOrderLineItemReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchaseOrderModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchaseOrderReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchaseOrderStatusEmailTemplateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchaseOrderStatusEmailTemplateReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchaseOrderStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchaseOrderStatusNotificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchaseOrderStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/PurchasingDemandModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/QuoteLinkModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RelationshipReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ReminderReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ReportCardDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ReportCardInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ReportCardModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ReportCardReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ReportDataResponseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ReportModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ReportingServiceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ResultInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaActionInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaActionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaActionReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaDispositionInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaDispositionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaDispositionReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaStatusEmailTemplateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaStatusEmailTemplateReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaStatusInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaStatusNotificationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RmaTagModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/RoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SLAInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SLAModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SLAPriorityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SLAReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SalesOrderReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SalesProbabilityInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SalesProbabilityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SalesQuotaModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SalesTeamMemberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SalesTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SalesTeamReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleColorModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleEntryDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleEntryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleEntryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleReminderTimeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleSpanReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleStatusModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleStopwatchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ScheduleTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SchedulingMemberInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SecurityRoleInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SecurityRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SecurityRoleReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SecurityRoleSettingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceCodeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceEmailTemplateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceEmailTemplateReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceItemReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceLocationInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceLocationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceLocationReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceSignoffInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceSignoffModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceSignoffReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceSourceReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceStatusReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceSubTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceSurveyModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceSurveyQuestionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceSurveyQuestionOptionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceSurveyReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceTeamReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceTemplateInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceTemplateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceTemplateReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceTicketLinkInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceTicketLinkModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceTicketNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ServiceTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SetupScreenModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SeverityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ShipmentMethodInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ShipmentMethodModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ShipmentMethodReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SicCodeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SiteReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SkillCategoryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SkillCategoryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SkillInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SkillModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SkillReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SourceInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SourceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SsoConfigurationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SsoUserModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/StandardNoteInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/StandardNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/StateInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/StateModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/StateReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/StatusIndicatorModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/StatusIndicatorReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/StructureReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SubCategoryInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SubCategoryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SuccessResponseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SurveyInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SurveyModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SurveyOptionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SurveyQuestionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SurveyQuestionReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SurveyQuestionValueModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SurveyReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SurveyResultDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SurveyResultModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SystemDepartmentReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SystemLocationReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SystemMenuEntryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/SystemSettingModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaskModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxCodeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxCodeLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxCodeLevelReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxCodeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxCodeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxCodeXRefModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxIntegrationInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxIntegrationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxableExpenseTypeLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxableProductTypeLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxableWorkRoleLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TaxableXRefLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TeamMemberModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TeamModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TeamRoleInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TeamRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TeamRoleReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TemplateGeneratedCountsModelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TicketInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TicketModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TicketNoteModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TicketReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TicketStopwatchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TicketSyncModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TicketTaskModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeAccrualDetailModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeAccrualModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeAccrualReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeEntryAuditModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeEntryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeEntryReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeExpenseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimePeriodModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimePeriodSetupDefaultsModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimePeriodSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimePeriodSetupReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeSheetAuditModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeSheetModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeSheetReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeZoneReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeZoneSetupInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeZoneSetupModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TimeZoneSetupReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TodayPageCategoryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TokenModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TrackActionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TrackModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/TrackReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UnitOfMeasureModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UnitOfMeasureReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UnpostedExpenseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UnpostedExpenseTaxableLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UnpostedInvoiceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UnpostedInvoiceTaxableLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UnpostedProcurementModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UnpostedProcurementTaxableLevelModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UsageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UserDefinedFieldInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UserDefinedFieldModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UserDefinedFieldOptionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/UserDefinedFieldReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ValidatePortalResponseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/ValidationErrorModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WarehouseBinInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WarehouseBinModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WarehouseBinReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WarehouseInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WarehouseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WarehouseReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WonRevenueReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkRoleExemptionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkRoleInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkRoleLocationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkRoleModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkRoleReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowActionAutomateParameterModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowActionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowActionUserDefinedFieldModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowAttachmentModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowEventModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowNotifyTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowNotifyTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowTableTypeInfoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowTableTypeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowTableTypeReferenceModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowTriggerModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/WorkflowTriggerOptionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/models/manage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.848374 pyconnectwise-0.3.1/src/pyconnectwise/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/responses/paginated_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.848374 pyconnectwise-0.3.1/src/pyconnectwise/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.848374 pyconnectwise-0.3.1/src/pyconnectwise/utils/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/experimental/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/experimental/patch_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.848374 pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/client_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/endpoint_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/model_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-20 00:42:05.000000 pyconnectwise-0.3.1/src/pyconnectwise/utils/naming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:42:16.580370 pyconnectwise-0.3.1/src/pyconnectwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-20 00:42:16.000000 pyconnectwise-0.3.1/src/pyconnectwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   167959 2023-07-20 00:42:16.000000 pyconnectwise-0.3.1/src/pyconnectwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 00:42:16.000000 pyconnectwise-0.3.1/src/pyconnectwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 00:42:16.000000 pyconnectwise-0.3.1/src/pyconnectwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 00:42:16.000000 pyconnectwise-0.3.1/src/pyconnectwise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.584779 pyconnectwise-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 08:14:23.000000 pyconnectwise-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-24 08:14:36.584779 pyconnectwise-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-24 08:14:23.000000 pyconnectwise-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 08:14:36.584779 pyconnectwise-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-24 08:14:23.000000 pyconnectwise-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.572779 pyconnectwise-0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.576779 pyconnectwise-0.4/src/pyconnectwise/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.576779 pyconnectwise-0.4/src/pyconnectwise/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/clients/automate_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/clients/manage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.576779 pyconnectwise-0.4/src/pyconnectwise/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.576779 pyconnectwise-0.4/src/pyconnectwise/endpoints/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/endpoints/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/endpoints/base/connectwise_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.576779 pyconnectwise-0.4/src/pyconnectwise/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.576779 pyconnectwise-0.4/src/pyconnectwise/models/automate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.576779 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.576779 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/Models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.580779 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/Models/Monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/Models/Monitors/RoutineParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/Models/Monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/Models/TemporaryApiContracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99828 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.580779 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/RESTApi/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/RESTApi/Models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/RESTApi/RpcContracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/RESTApi/Security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/RESTApi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/LabTech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.580779 pyconnectwise-0.4/src/pyconnectwise/models/automate/System/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/System/Threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/System/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/automate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.580779 pyconnectwise-0.4/src/pyconnectwise/models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/base/connectwise_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/base/message_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.580779 pyconnectwise-0.4/src/pyconnectwise/models/manage/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/Agreement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.580779 pyconnectwise-0.4/src/pyconnectwise/models/manage/Campaign/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/Campaign/SubType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/Campaign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/Company.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/CompanyCompanyTypeAssociation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/ContactContactTypeAssociation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/Finance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.580779 pyconnectwise-0.4/src/pyconnectwise/models/manage/Type/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/Type/SubType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/Type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   735106 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/models/manage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.584779 pyconnectwise-0.4/src/pyconnectwise/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/responses/paginated_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.584779 pyconnectwise-0.4/src/pyconnectwise/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.584779 pyconnectwise-0.4/src/pyconnectwise/utils/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/experimental/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/experimental/patch_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.584779 pyconnectwise-0.4/src/pyconnectwise/utils/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/generator/client_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/generator/endpoint_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/generator/model_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/generator/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/generator/path_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/generator/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-24 08:14:23.000000 pyconnectwise-0.4/src/pyconnectwise/utils/naming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:14:36.576779 pyconnectwise-0.4/src/pyconnectwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-24 08:14:36.000000 pyconnectwise-0.4/src/pyconnectwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-24 08:14:36.000000 pyconnectwise-0.4/src/pyconnectwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:14:36.000000 pyconnectwise-0.4/src/pyconnectwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 08:14:36.000000 pyconnectwise-0.4/src/pyconnectwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 08:14:36.000000 pyconnectwise-0.4/src/pyconnectwise.egg-info/top_level.txt
```

### Comparing `pyconnectwise-0.3.1/LICENSE` & `pyconnectwise-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconnectwise-0.3.1/PKG-INFO` & `pyconnectwise-0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconnectwise
-Version: 0.3.1
+Version: 0.4
 Summary: A full-featured Python client for the ConnectWise API's
 Home-page: https://github.com/HealthITAU/pyconnectwise
 Author: Health IT
 Author-email: dev@healthit.com.au
 License: gpl-3.0
 Keywords: ConnectWise,Manage,Automate,API,Python,Client,Annotated,Typed,MSP
 Classifier: Development Status :: 4 - Beta
@@ -15,127 +15,167 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Health IT Logo](https://healthit.com.au/wp-content/uploads/2019/06/HIT-proper-logo.png)](https://healthit.com.au)
 
-# pyConnectWise - a library for simplifying interactions with the ConnectWise Manage API in Python
+# pyConnectWise - An API library for ConnectWise Manage and ConnectWise Automate, written in Python
 
-pyConnectWise is a full featured, type annotated API client written in Python for the ConnectWise APIs. 
+pyConnectWise is a full-featured, type annotated API client written in Python for the ConnectWise APIs based off their OpenAPI schemas. 
 
 This library has been developed with the intention of making the ConnectWise APIs simple and accessible to non-coders while allowing experienced coders to utilize all features the API has to offer without the boilerplate.
 
-pyConnectWise currently only supports ConnectWise Manage, but more is planned.
+pyConnectWise currently supports both ConnectWise Manage and ConnectWise Automate.
 
 Features:
 =========
-- 100% API Coverage. All endpoints and response models have had their code generated from the ConnectWise Manage OpenAPI spec.
-- Non-coder friendly
-- Focus on type annotations and DX (Developer Experience). Models are declared and parsed using [Pydantic](https://github.com/pydantic/pydantic)
+- **100% API Coverage.** All endpoints and response models have had their code generated from the ConnectWise Manage and ConnectWise Automate OpenAPI schemas.
+- **Non-coder friendly.** 100% annotated for full IDE auto-completion. Clients handle requests and authentication - just plug the right details in and go!
+- **Fully annotated.** This library has a strong focus on type safety and type hinting. Models are declared and parsed using [Pydantic](https://github.com/pydantic/pydantic)
 
 pyConnectWise is currently in **pre-release**. This means that while it does work, you may come across issues and inconsistencies. 
 
 As all Endpoint and Model code has been generated, not all of it has been tested. YMMV.
 
+Endpoint generation is custom-built, but Pydantic models have been generated using a customised fork of [datamodel-code-generator](https://github.com/koxudaxi/datamodel-code-generator)
+
 Known Issues:
 =============
-- The ConnectWise API spec doesn't label optional fields correctly - for example, the mergedParentTicket field on a service ticket is only included in an API response if the ticket has a parent.
-  - Because these aren't labelled, the models generated can't correctly identify what exactly an optional field is. There's 3 potential solutions for this, all with caveats:
-    - Manually edit the schema or models
-      - This isn't maintainable - if a new version comes out, it'll need to be re-done. It's also very manual labour intensive.
-    - Annotate every field in a model as ```<type> | None```
-      - This negatively impacts DX (Developer Experience). Every field would need to be checked for None manually otherwise the type checker would yell at you.
-    - Opt out of Pydantic validation altogether.
-      - We miss out on the best part of Pydantic this way, and it also introduces the risk of accessing fields (such as ```TicketModel.mergedParentTicket```) without being notified of it potentially being None.
-      - This is the option I've opted for for the time being. I'd like to find a better solution to this.
 - Currently only parses **Response** models. No input models yet.
 - As this project is still a WIP, documentation or code commentary may not always align. 
 - Little to no error handling just yet
 
 Roadmap:
 =============
-- Automate API Support - :construction: In Progress
-- Robust error handling - :construction: In Progress
-- Input model validation - :chart_with_upwards_trend: Planned
-- ScreenConnect (Control) API Support - :chart_with_upwards_trend: Planned
-- Batch requests - :chart_with_upwards_trend: Planned
+- **Automate API Support** - Done :white_check_mark:
+- **Robust error handling** - In Progress :construction: 
+- **Input model validation** - Planned :chart_with_upwards_trend: 
+- **ScreenConnect (Control) API Support** - Planned :chart_with_upwards_trend:
+- **Batch requests** - Planned :chart_with_upwards_trend:
 
 How-to:
 =============
 - [Install](#install)
-- [Initialize API client](#initialize-api-client)
+- [Initializing the API Clients](#initialize-api-client)
+  - [ConnectWise Manage](#connectwise-manage)
+  - [ConnectWise Automate](#connectwise-automate)
 - [Working with Endpoints](#working-with-endpoints)
-  - [Child Endpoints](#child-endpoints)
+  - [Get Many](#get-many)
+  - [Get One](#get-one)
+  - [Get With Params](#get-with-params)
+  - [Path Parameters](#child-endpoints)
 - [Pagination](#pagination)
 - [Examples](#examples)
 - [Contributing](#contributing)
 - [Supporting the project](#supporting-the-project)
 
 # Install
 Open a terminal and run ```pip install pyconnectwise```
 
-# Initialize API client
+# Initializing the API Clients
+
+### ConnectWise Manage
 ```python
 from pyconnectwise import ConnectWiseManageAPIClient
 
 # init client
-api = ConnectWiseManageAPIClient(
+manage_api_client = ConnectWiseManageAPIClient(
   # your company name,
   # manage instance url,
   # your api client id,
   # your api public key,
   # your api private key
 )
 ```
 
+### ConnectWise Automate
+```python
+from pyconnectwise import ConnectWiseAutomateAPIClient
+
+# init client
+automate_api_client = ConnectWiseAutomateAPIClient(
+  # your automate url
+  # your client id
+  # automate api username
+  # automate api password
+)
+```
+
+
 # Working with Endpoints
-Endpoints are 1:1 to what's available with ConnectWise Manage as code is generated from their OpenAPI spec.
+Endpoints are 1:1 to what's available for both the ConnectWise Manage and ConnectWise Automate as code is generated from their OpenAPI spec.
 
-For more information, check out the [ConnectWise Manage REST API Docs (requires ConnectWise Developer account)](https://developer.connectwise.com/Products/ConnectWise_PSA/REST)
+For more information, check out the following resources:
+- [ConnectWise Manage REST API Docs (requires ConnectWise Developer account)](https://developer.connectwise.com/Products/ConnectWise_PSA/REST)
+- [ConnectWise Automate REST API Docs (requires ConnectWise Developer account)](https://developer.connectwise.com/Products/ConnectWise_Automate/Integrating_with_Automate/API/REST)
 
-### Get
+### Get many
 ```python
-# sends get request to /company/companies endpoint
-companies = api.company.companies.get()
+### Manage ###
+
+# sends GET request to /company/companies endpoint
+companies = manage_api_client.company.companies.get()
+
+### Automate ###
+
+# sends GET request to /clients endpoint
+clients = automate_api_client.clients.get()
 ```
 
 ### Get one
 ```python
-# sends get request to /company/companies/{id} endpoint
-companies = api.company.companies.id(250).get()
+### Manage ###
+
+# sends GET request to /company/companies/{id} endpoint
+company = manage_api_client.company.companies.id(250).get()
+
+### Automate ###
+
+# sends GET request to /clients/{id} endpoint
+client = automate_api_client.clients.id(250).get()
 ```
 
 ### Get with params
 ```python
-# sends get request to /company/companies with a condition query string
-conditional_get = api.company.companies.get(params={
+### Manage ###
+
+# sends GET request to /company/companies with a conditions query string
+conditional_company = manage_api_client.company.companies.get(params={
   'conditions': 'company/id=250'
 })
+
+### Automate ###
+# sends GET request to /clients endpoint with a condition query string
+# note that the Automate API expects the string 'condition' where-as the Manage API expects the string 'conditions'
+conditional_client = automate_api_client.clients.get(params={
+  'condition': 'company/id=250'
+})
 ```
 
 # Child Endpoints
-The ConnectWise API has many instances of nested endpoints - for example, ```/company/companies/{company_id}/sites```
+The ConnectWise APIs have many instances of endpoints with path parameters - for example, ```/company/companies/{company_id}/sites```
 
-This is replicated in the library. Endpoints provide an ```id``` method for setting the ID and traversing down the path.
+This also exists in the library. Endpoints provide an ```id``` method for setting the ID and traversing down the path.
 
 ##### Example using ```/company/companies/{company_id}/sites```
 ```python
-sites = api.company.companies.id(250).sites.get()
+# equivalent to GET /company/companies/250/sites  
+sites = manage_api_client.company.companies.id(250).sites.get()
 ```
 
 # Pagination
-The ConnectWise API paginates data for performance reasons through the ```page``` and ```pageSize``` query parameters. ```pageSize``` is limited to a maximum of 1000.
+The ConnectWise Manage API paginates data for performance reasons through the ```page``` and ```pageSize``` query parameters. ```pageSize``` is limited to a maximum of 1000.
 
 To make working with paginated data easy, Endpoints that implement a GET response with an array also supply a ```paginated()``` method. Under the hood this wraps a GET request, but does a lot of neat stuff to make working with pages easier.
 
 Working with pagination
 ```python
 # initialize a PaginatedResponse instance for /company/companies, starting on page 1 with a pageSize of 100
-paginated_companies = api.company.companies.paginated(1,100)
+paginated_companies = manage_api_client.company.companies.paginated(1,100)
 
 # access the data from the current page using the .data field
 page_one_data = paginated_companies.data
 
 # if there's a next page, retrieve the next page worth of data
 paginated_companies.get_next_page()
```

### Comparing `pyconnectwise-0.3.1/README.md` & `pyconnectwise-0.4/src/pyconnectwise.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,122 +1,181 @@
+Metadata-Version: 2.1
+Name: pyconnectwise
+Version: 0.4
+Summary: A full-featured Python client for the ConnectWise API's
+Home-page: https://github.com/HealthITAU/pyconnectwise
+Author: Health IT
+Author-email: dev@healthit.com.au
+License: gpl-3.0
+Keywords: ConnectWise,Manage,Automate,API,Python,Client,Annotated,Typed,MSP
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10.1
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Health IT Logo](https://healthit.com.au/wp-content/uploads/2019/06/HIT-proper-logo.png)](https://healthit.com.au)
 
-# pyConnectWise - a library for simplifying interactions with the ConnectWise Manage API in Python
+# pyConnectWise - An API library for ConnectWise Manage and ConnectWise Automate, written in Python
 
-pyConnectWise is a full featured, type annotated API client written in Python for the ConnectWise APIs. 
+pyConnectWise is a full-featured, type annotated API client written in Python for the ConnectWise APIs based off their OpenAPI schemas. 
 
 This library has been developed with the intention of making the ConnectWise APIs simple and accessible to non-coders while allowing experienced coders to utilize all features the API has to offer without the boilerplate.
 
-pyConnectWise currently only supports ConnectWise Manage, but more is planned.
+pyConnectWise currently supports both ConnectWise Manage and ConnectWise Automate.
 
 Features:
 =========
-- 100% API Coverage. All endpoints and response models have had their code generated from the ConnectWise Manage OpenAPI spec.
-- Non-coder friendly
-- Focus on type annotations and DX (Developer Experience). Models are declared and parsed using [Pydantic](https://github.com/pydantic/pydantic)
+- **100% API Coverage.** All endpoints and response models have had their code generated from the ConnectWise Manage and ConnectWise Automate OpenAPI schemas.
+- **Non-coder friendly.** 100% annotated for full IDE auto-completion. Clients handle requests and authentication - just plug the right details in and go!
+- **Fully annotated.** This library has a strong focus on type safety and type hinting. Models are declared and parsed using [Pydantic](https://github.com/pydantic/pydantic)
 
 pyConnectWise is currently in **pre-release**. This means that while it does work, you may come across issues and inconsistencies. 
 
 As all Endpoint and Model code has been generated, not all of it has been tested. YMMV.
 
+Endpoint generation is custom-built, but Pydantic models have been generated using a customised fork of [datamodel-code-generator](https://github.com/koxudaxi/datamodel-code-generator)
+
 Known Issues:
 =============
-- The ConnectWise API spec doesn't label optional fields correctly - for example, the mergedParentTicket field on a service ticket is only included in an API response if the ticket has a parent.
-  - Because these aren't labelled, the models generated can't correctly identify what exactly an optional field is. There's 3 potential solutions for this, all with caveats:
-    - Manually edit the schema or models
-      - This isn't maintainable - if a new version comes out, it'll need to be re-done. It's also very manual labour intensive.
-    - Annotate every field in a model as ```<type> | None```
-      - This negatively impacts DX (Developer Experience). Every field would need to be checked for None manually otherwise the type checker would yell at you.
-    - Opt out of Pydantic validation altogether.
-      - We miss out on the best part of Pydantic this way, and it also introduces the risk of accessing fields (such as ```TicketModel.mergedParentTicket```) without being notified of it potentially being None.
-      - This is the option I've opted for for the time being. I'd like to find a better solution to this.
 - Currently only parses **Response** models. No input models yet.
 - As this project is still a WIP, documentation or code commentary may not always align. 
 - Little to no error handling just yet
 
 Roadmap:
 =============
-- Automate API Support - :construction: In Progress
-- Robust error handling - :construction: In Progress
-- Input model validation - :chart_with_upwards_trend: Planned
-- ScreenConnect (Control) API Support - :chart_with_upwards_trend: Planned
-- Batch requests - :chart_with_upwards_trend: Planned
+- **Automate API Support** - Done :white_check_mark:
+- **Robust error handling** - In Progress :construction: 
+- **Input model validation** - Planned :chart_with_upwards_trend: 
+- **ScreenConnect (Control) API Support** - Planned :chart_with_upwards_trend:
+- **Batch requests** - Planned :chart_with_upwards_trend:
 
 How-to:
 =============
 - [Install](#install)
-- [Initialize API client](#initialize-api-client)
+- [Initializing the API Clients](#initialize-api-client)
+  - [ConnectWise Manage](#connectwise-manage)
+  - [ConnectWise Automate](#connectwise-automate)
 - [Working with Endpoints](#working-with-endpoints)
-  - [Child Endpoints](#child-endpoints)
+  - [Get Many](#get-many)
+  - [Get One](#get-one)
+  - [Get With Params](#get-with-params)
+  - [Path Parameters](#child-endpoints)
 - [Pagination](#pagination)
 - [Examples](#examples)
 - [Contributing](#contributing)
 - [Supporting the project](#supporting-the-project)
 
 # Install
 Open a terminal and run ```pip install pyconnectwise```
 
-# Initialize API client
+# Initializing the API Clients
+
+### ConnectWise Manage
 ```python
 from pyconnectwise import ConnectWiseManageAPIClient
 
 # init client
-api = ConnectWiseManageAPIClient(
+manage_api_client = ConnectWiseManageAPIClient(
   # your company name,
   # manage instance url,
   # your api client id,
   # your api public key,
   # your api private key
 )
 ```
 
+### ConnectWise Automate
+```python
+from pyconnectwise import ConnectWiseAutomateAPIClient
+
+# init client
+automate_api_client = ConnectWiseAutomateAPIClient(
+  # your automate url
+  # your client id
+  # automate api username
+  # automate api password
+)
+```
+
+
 # Working with Endpoints
-Endpoints are 1:1 to what's available with ConnectWise Manage as code is generated from their OpenAPI spec.
+Endpoints are 1:1 to what's available for both the ConnectWise Manage and ConnectWise Automate as code is generated from their OpenAPI spec.
 
-For more information, check out the [ConnectWise Manage REST API Docs (requires ConnectWise Developer account)](https://developer.connectwise.com/Products/ConnectWise_PSA/REST)
+For more information, check out the following resources:
+- [ConnectWise Manage REST API Docs (requires ConnectWise Developer account)](https://developer.connectwise.com/Products/ConnectWise_PSA/REST)
+- [ConnectWise Automate REST API Docs (requires ConnectWise Developer account)](https://developer.connectwise.com/Products/ConnectWise_Automate/Integrating_with_Automate/API/REST)
 
-### Get
+### Get many
 ```python
-# sends get request to /company/companies endpoint
-companies = api.company.companies.get()
+### Manage ###
+
+# sends GET request to /company/companies endpoint
+companies = manage_api_client.company.companies.get()
+
+### Automate ###
+
+# sends GET request to /clients endpoint
+clients = automate_api_client.clients.get()
 ```
 
 ### Get one
 ```python
-# sends get request to /company/companies/{id} endpoint
-companies = api.company.companies.id(250).get()
+### Manage ###
+
+# sends GET request to /company/companies/{id} endpoint
+company = manage_api_client.company.companies.id(250).get()
+
+### Automate ###
+
+# sends GET request to /clients/{id} endpoint
+client = automate_api_client.clients.id(250).get()
 ```
 
 ### Get with params
 ```python
-# sends get request to /company/companies with a condition query string
-conditional_get = api.company.companies.get(params={
+### Manage ###
+
+# sends GET request to /company/companies with a conditions query string
+conditional_company = manage_api_client.company.companies.get(params={
   'conditions': 'company/id=250'
 })
+
+### Automate ###
+# sends GET request to /clients endpoint with a condition query string
+# note that the Automate API expects the string 'condition' where-as the Manage API expects the string 'conditions'
+conditional_client = automate_api_client.clients.get(params={
+  'condition': 'company/id=250'
+})
 ```
 
 # Child Endpoints
-The ConnectWise API has many instances of nested endpoints - for example, ```/company/companies/{company_id}/sites```
+The ConnectWise APIs have many instances of endpoints with path parameters - for example, ```/company/companies/{company_id}/sites```
 
-This is replicated in the library. Endpoints provide an ```id``` method for setting the ID and traversing down the path.
+This also exists in the library. Endpoints provide an ```id``` method for setting the ID and traversing down the path.
 
 ##### Example using ```/company/companies/{company_id}/sites```
 ```python
-sites = api.company.companies.id(250).sites.get()
+# equivalent to GET /company/companies/250/sites  
+sites = manage_api_client.company.companies.id(250).sites.get()
 ```
 
 # Pagination
-The ConnectWise API paginates data for performance reasons through the ```page``` and ```pageSize``` query parameters. ```pageSize``` is limited to a maximum of 1000.
+The ConnectWise Manage API paginates data for performance reasons through the ```page``` and ```pageSize``` query parameters. ```pageSize``` is limited to a maximum of 1000.
 
 To make working with paginated data easy, Endpoints that implement a GET response with an array also supply a ```paginated()``` method. Under the hood this wraps a GET request, but does a lot of neat stuff to make working with pages easier.
 
 Working with pagination
 ```python
 # initialize a PaginatedResponse instance for /company/companies, starting on page 1 with a pageSize of 100
-paginated_companies = api.company.companies.paginated(1,100)
+paginated_companies = manage_api_client.company.companies.paginated(1,100)
 
 # access the data from the current page using the .data field
 page_one_data = paginated_companies.data
 
 # if there's a next page, retrieve the next page worth of data
 paginated_companies.get_next_page()
```

### Comparing `pyconnectwise-0.3.1/setup.py` & `pyconnectwise-0.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyconnectwise-0.3.1/src/pyconnectwise/clients/manage_client.py` & `pyconnectwise-0.4/src/pyconnectwise/clients/manage_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import base64
+
 import requests
+
 from pyconnectwise.endpoints.manage.CompanyEndpoint import CompanyEndpoint
 from pyconnectwise.endpoints.manage.ConfigurationsEndpoint import ConfigurationsEndpoint
 from pyconnectwise.endpoints.manage.ExpenseEndpoint import ExpenseEndpoint
 from pyconnectwise.endpoints.manage.FinanceEndpoint import FinanceEndpoint
 from pyconnectwise.endpoints.manage.MarketingEndpoint import MarketingEndpoint
 from pyconnectwise.endpoints.manage.ProcurementEndpoint import ProcurementEndpoint
 from pyconnectwise.endpoints.manage.ProjectEndpoint import ProjectEndpoint
 from pyconnectwise.endpoints.manage.SalesEndpoint import SalesEndpoint
 from pyconnectwise.endpoints.manage.ScheduleEndpoint import ScheduleEndpoint
 from pyconnectwise.endpoints.manage.ServiceEndpoint import ServiceEndpoint
 from pyconnectwise.endpoints.manage.SystemEndpoint import SystemEndpoint
 from pyconnectwise.endpoints.manage.TimeEndpoint import TimeEndpoint
 
+
 class ConnectWiseManageAPIClient:
     """
     ConnectWise Manage API client. Handles the connection to the ConnectWise Manage API
     and the configuration of all the available endpoints.
     """
+
     def __init__(
         self,
         company_name: str,
         manage_url: str,
         client_id: str,
         public_key: str,
         private_key: str,
@@ -40,28 +44,27 @@
             codebase (str, optional): Your ConnectWise Manage Codebase. If not provided, it will be fetched from the API. Defaults to None.
         """
         self.client_id = client_id
         self.company_name = company_name
         self.manage_url = manage_url
         self.public_key = public_key
         self.private_key = private_key
-        
+
         # Retrieve codebase from the API if not provided
         if not codebase:
-            codebase_request = self.__try_get_codebase_from_api(
+            codebase_request = self._try_get_codebase_from_api(
                 manage_url=manage_url,
                 company_name=company_name,
-                headers=self.get_headers(),
+                headers=self._get_headers(),
             )
 
             if codebase_request is None:
                 # we need to except here
                 raise Exception("Could not retrieve codebase from API.")
             self.codebase = codebase_request
-            
 
         # Initializing endpoints
         self.company = CompanyEndpoint(self)
         self.configurations = ConfigurationsEndpoint(self)
         self.expense = ExpenseEndpoint(self)
         self.finance = FinanceEndpoint(self)
         self.marketing = MarketingEndpoint(self)
@@ -69,65 +72,63 @@
         self.project = ProjectEndpoint(self)
         self.sales = SalesEndpoint(self)
         self.schedule = ScheduleEndpoint(self)
         self.service = ServiceEndpoint(self)
         self.system = SystemEndpoint(self)
         self.time = TimeEndpoint(self)
 
-    def get_url(self) -> str:
+    def _get_url(self) -> str:
         """
         Generates and returns the URL for the ConnectWise Manage API endpoints based on the company url and codebase.
 
         Returns:
             str: API URL.
         """
         return f"https://{self.manage_url}/{self.codebase.strip('/')}/apis/3.0"
 
-    def __try_get_codebase_from_api(self, manage_url: str, company_name: str, headers: dict[str, str]) -> str | None:
+    def _try_get_codebase_from_api(self, manage_url: str, company_name: str, headers: dict[str, str]) -> str | None:
         """
         Tries to retrieve the codebase from the API using the provided company url, company name and headers.
 
         Parameters:
             company_url (str): URL of the company.
             company_name (str): Name of the company.
             headers (dict[str, str]): Headers to be sent in the request.
 
         Returns:
             str: Codebase string or None if an error occurs.
         """
         result = ""
         try:
             url = f"https://{manage_url}/login/companyinfo/{company_name}"
-            result = (
-                requests.request("GET", url, headers=headers).json().get("Codebase")
-            )
+            result = requests.request("GET", url, headers=headers).json().get("Codebase")
         except:
             result = None
         return result
 
-    def __get_auth_string(self) -> str:
+    def _get_auth_string(self) -> str:
         """
         Creates and returns the base64 encoded authorization string required for API requests.
 
         Returns:
             str: Base64 encoded authorization string.
         """
         return "Basic " + base64.b64encode(
             bytes(
                 f"{self.company_name}+{self.public_key}:{self.private_key}",
                 encoding="utf8",
             )
         ).decode("ascii")
 
-    def get_headers(self) -> dict[str, str]:
+    def _get_headers(self) -> dict[str, str]:
         """
         Generates and returns the headers required for making API requests.
 
         Returns:
             dict[str, str]: Dictionary of headers including Content-Type, Client ID, and Authorization.
         """
         headers = {
             "Content-Type": "application/json",
             "clientId": self.client_id,
-            "Authorization": self.__get_auth_string(),
+            "Authorization": self._get_auth_string(),
         }
         return headers
```

### Comparing `pyconnectwise-0.3.1/src/pyconnectwise/endpoints/base/connectwise_endpoint.py` & `pyconnectwise-0.4/src/pyconnectwise/endpoints/base/connectwise_endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from __future__ import annotations
 import requests
 from requests import Response
-from pydantic import BaseModel
-from pyconnectwise.responses.paginated_response import PaginatedResponse
-from pyconnectwise.models.base.connectwise_model import ConnectWiseModel
-from typing import Any, TypeVar, Generic, TYPE_CHECKING
-from pyconnectwise.utils.experimental.patch_maker import PatchGroup
-from typing import TypeVar, Type, List, Union
+from typing import Any
+from typing import TypeVar, Type
 
 TChildEndpoint = TypeVar("TChildEndpoint", bound="ConnectWiseEndpoint")
 TSelf = TypeVar("TSelf", bound="ConnectWiseEndpoint")
 T = TypeVar("T", bound="BaseModel")
 
 
 class ConnectWiseEndpoint:
@@ -50,29 +46,36 @@
         _id (int): The ID of the current resource, if applicable.
         _child_endpoints (List[ConnectWiseEndpoint]): A list of registered child endpoints.
 
     Generic Type:
         TModel: The model class for the endpoint.
     """
 
-    def __init__(self, client, endpoint_url: str, parent_endpoint: ConnectWiseEndpoint | None = None):
+    def __init__(
+        self,
+        client,
+        endpoint_url: str,
+        parent_endpoint: ConnectWiseEndpoint | None = None,
+    ):
         """
         Initialize a ConnectWiseEndpoint instance with the client and endpoint base.
 
         Args:
             client: The ConnectWiseAPIClient instance.
             endpoint_base (str): The base URL for the specific endpoint.
         """
         self.client = client
         self.endpoint_base = endpoint_url
         self._parent_endpoint = parent_endpoint
         self._id = None
         self._child_endpoints: list[ConnectWiseEndpoint] = []
 
-    def register_child_endpoint(self, child_endpoint: TChildEndpoint) -> TChildEndpoint:
+    def _register_child_endpoint(
+        self, child_endpoint: TChildEndpoint
+    ) -> TChildEndpoint:
         """
         Register a child endpoint to the current endpoint.
 
         Args:
             child_endpoint (ConnectWiseEndpoint): The child endpoint instance.
 
         Returns:
@@ -90,24 +93,33 @@
 
         Returns:
             str: The joined URL string.
         """
         url_parts = [str(arg).strip("/") for arg in args]
         return "/".join(url_parts)
 
-    def __get_replaced_url(self) -> str:
+    def _get_replaced_url(self) -> str:
         if self._id is None:
             return self.endpoint_base
         return self.endpoint_base.replace("{id}", str(self._id))
-    
-    def make_request_and_get_json(self, endpoint=None, data: dict[str, Any] = {}, params: dict[str, int | str] = {}) -> dict[str, Any]:
-        return self.make_request("GET", endpoint, data, params).json()
 
-    def make_request(
-        self, method: str, endpoint=None, data: dict[str, Any] = {}, params: dict[str, int | str] = {}
+    def _make_request_and_get_json(
+        self,
+        endpoint=None,
+        data: dict[str, Any] = {},
+        params: dict[str, int | str] = {},
+    ) -> dict[str, Any]:
+        return self._make_request("GET", endpoint, data, params).json()
+
+    def _make_request(
+        self,
+        method: str,
+        endpoint=None,
+        data: dict[str, Any] = {},
+        params: dict[str, int | str] = {},
     ) -> Response:
         """
         Make an API request using the specified method, endpoint, data, and parameters.
         This function isn't intended for use outside of this class.
         Please use the available CRUD methods as intended.
 
         Args:
@@ -130,51 +142,43 @@
 
         def build_url(endpoint: ConnectWiseEndpoint) -> str:
             if endpoint._parent_endpoint is not None:
                 parent_url = build_url(endpoint._parent_endpoint)
                 if endpoint._parent_endpoint._id is not None:
                     return self._url_join(
                         parent_url,
-                        endpoint.__get_replaced_url(),
+                        endpoint._get_replaced_url(),
                     )
                 else:
-                    return self._url_join(parent_url, endpoint.__get_replaced_url())
+                    return self._url_join(parent_url, endpoint._get_replaced_url())
             else:
                 return self._url_join(
-                    self.client.get_url(), endpoint.__get_replaced_url()
+                    self.client._get_url(), endpoint._get_replaced_url()
                 )
 
         url = build_url(self)
         if endpoint:
             url = self._url_join(url, endpoint)
 
         response = requests.request(
-            method, url, headers=self.client.get_headers(), json=data, params=params
+            method, url, headers=self.client._get_headers(), json=data, params=params
         )
 
         if response.status_code >= 400:
             raise Exception(
                 f"Request failed with status code {response.status_code}: {response.text}"
             )
 
         return response
 
     def _parse_many(self, model_type: Type[T], data: list[dict[str, Any]]) -> list[T]:
-        # use the model's construct method to create instances from the data
-        # ideally, we'd use the model's parse method, but
-        # due to issues validating optional fields in the ConnectWise Manage schema
-        # we have to use the construct method instead until a better solution is found
-        return [model_type.model_construct(**d) for d in data]
+        return [model_type.model_validate(d) for d in data]
 
     def _parse_one(self, model_type: Type[T], data: dict[str, Any]) -> T:
-        # use the model's construct method to create instances from the data
-        # ideally, we'd use the model's parse method, but
-        # due to issues validating optional fields in the ConnectWise Manage schema
-        # we have to use the construct method instead until a better solution is found
-        return model_type.model_construct(**data)
+        return model_type.model_validate(data)
 
     def id(self: TSelf, id: int) -> TSelf:
         """
         Set the ID for the current endpoint.
 
         Args:
             id (int): The ID to set.
```

### Comparing `pyconnectwise-0.3.1/src/pyconnectwise/responses/paginated_response.py` & `pyconnectwise-0.4/src/pyconnectwise/responses/paginated_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     """
 
     def __init__(
         self,
         response,
         response_model: Type[TModel],
         endpoint: ConnectWiseEndpoint,
+        page,
         page_size,
     ):
         """
         PaginatedResponse is a wrapper class for handling paginated responses from the
         ConnectWise API. It provides methods for navigating through the pages of the response
         and accessing the data contained within each page.
 
@@ -41,60 +42,74 @@
         parse the API response into model instances. It also supports iteration, allowing
         the user to loop through the items within the paginated response.
 
         PaginatedResponse uses a generic type variable TModel, which represents the
         expected model type for the response data. This allows for type-safe handling
         of model instances throughout the class.
         """
-        self._initialize(response, response_model, endpoint, page_size)
+        self._initialize(response, response_model, endpoint, page, page_size)
 
     def _initialize(
-        self, response, response_model, endpoint: ConnectWiseEndpoint, page_size
+        self, response, response_model, endpoint: ConnectWiseEndpoint, page, page_size
     ):
         """
         Initialize the instance variables using the provided response, endpoint, and page size.
 
         Args:
             response: The raw response object from the API.
             endpoint (ConnectWiseEndpoint[TModel]): The endpoint associated with the response.
             page_size (int): The number of items per page.
         """
         self.response = response
         self.response_model = response_model
         self.endpoint = endpoint
-        self._page_size = page_size
+        self.page_size = page_size
         self.parsed_link_headers = parse_link_headers(response.headers)
-        self.has_next_page: bool = self.parsed_link_headers.get("has_next_page", False)
-        self.has_prev_page: bool = self.parsed_link_headers.get("has_prev_page", False)
-        self.first_page: int = self.parsed_link_headers.get("first_page", None)
-        self.prev_page: int = self.parsed_link_headers.get("prev_page", None)
-        self.next_page: int = self.parsed_link_headers.get("next_page", None)
-        self.last_page: int = self.parsed_link_headers.get("last_page", None)
+        if self.parsed_link_headers is not None:
+            # ConnectWise Manage API gives us handy headers to parse for Pagination
+            self.has_next_page: bool = self.parsed_link_headers.get("has_next_page", False)
+            self.has_prev_page: bool = self.parsed_link_headers.get("has_prev_page", False)
+            self.first_page: int = self.parsed_link_headers.get("first_page", None)
+            self.prev_page: int = self.parsed_link_headers.get("prev_page", None)
+            self.next_page: int = self.parsed_link_headers.get("next_page", None)
+            self.last_page: int = self.parsed_link_headers.get("last_page", None)
+        else:
+            # ConnectWise Automate doesn't...
+            # So, we'll brute force it, with some guesses.
+            self.has_next_page: bool = True
+            self.has_prev_page: bool = page > 1
+            self.first_page: int = 1
+            self.prev_page = page - 1 if page > 1 else 1
+            self.next_page = page + 1
+            self.last_page = 999999
         self.data: list[TModel] = endpoint._parse_many(response_model, response.json())
         self.has_data = self.data and len(self.data) > 0
         self.index = 0
 
     def get_next_page(self) -> PaginatedResponse[TModel]:
         """
         Fetch the next page of the paginated response.
 
         Returns:
             PaginatedResponse[TModel]: The updated PaginatedResponse instance
             with the data from the next page or None if there is no next page.
         """
+        print(f'has next page? {self.has_next_page}')
+        print(f'next_page: {self.next_page}')
         if not self.has_next_page or not self.next_page:
             self.has_data = False
             return self
 
-        next_response = self.endpoint.paginated(self.next_page, self._page_size)
+        next_response = self.endpoint.paginated(self.next_page, self.page_size)
         self._initialize(
             next_response.response,
             next_response.response_model,
             next_response.endpoint,
-            next_response._page_size,
+            self.next_page,
+            next_response.page_size,
         )
         return self
 
     def get_previous_page(self) -> PaginatedResponse[TModel]:
         """
         Fetch the next page of the paginated response.
 
@@ -102,20 +117,21 @@
             PaginatedResponse[TModel]: The updated PaginatedResponse instance
             with the data from the next page or None if there is no next page.
         """
         if not self.has_prev_page or not self.prev_page:
             self.has_data = False
             return self
 
-        prev_response = self.endpoint.paginated(self.prev_page, self._page_size)
+        prev_response = self.endpoint.paginated(self.prev_page, self.page_size)
         self._initialize(
             prev_response.response,
             prev_response.response_model,
             prev_response.endpoint,
-            prev_response._page_size,
+            self.prev_page,
+            prev_response.page_size,
         )
         return self
 
     def all(self):
         """
         Iterate through all items in the paginated response, across all pages.
```

### Comparing `pyconnectwise-0.3.1/src/pyconnectwise/utils/experimental/condition.py` & `pyconnectwise-0.4/src/pyconnectwise/utils/experimental/condition.py`

 * *Files identical despite different names*

### Comparing `pyconnectwise-0.3.1/src/pyconnectwise/utils/experimental/patch_maker.py` & `pyconnectwise-0.4/src/pyconnectwise/utils/experimental/patch_maker.py`

 * *Files identical despite different names*

### Comparing `pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/endpoint_gen.py` & `pyconnectwise-0.4/src/pyconnectwise/utils/generator/endpoint_gen.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,96 @@
-### THIS CODE IS NOT INTENDED FOR REGULAR USE
-### It's used to generate Endpoints from the schema
-### It's messy and not very readable
-### Works as is but proceed at your own risk.
-
+# endpoint_gen.py in src/pyconnectwise/utils/generator
+import os
+from pyconnectwise.utils.fs import save_py_file
 from pyconnectwise.utils.generator.templates import (
     endpoint_template,
-    top_level_endpoint_template,
 )
-from pyconnectwise.utils.fs import save_py_file
-from pyconnectwise.utils.naming import to_title_case_preserve_case
-from pyconnectwise.utils.generator.model_gen import generate_model
-import os
-import re
+from pyconnectwise.utils.generator.path_formatting import (
+    format_endpoint_path,
+    get_endpoint_class_name_from_path,
+    normalize_path_parameters,
+)
+from pyconnectwise.utils.naming import to_snake_case, ensure_not_reserved
 
-def format_endpoint_path(path: str) -> str:
-    return re.sub("{id}|{parentId}|{grandparentId}|{reportName}|{externalId}", "Id", path).rstrip("/")
 
 def generate_endpoint(
     endpoint_output_directory: str,
     model_output_directory: str,
     path: str,
     path_info: dict,
     relationships: dict,
-    models: dict,
 ):
+    print(path)
     formatted_path = format_endpoint_path(path)
-    endpoint_class_name = "".join(to_title_case_preserve_case(word) for word in formatted_path.split("/")) + "Endpoint"
+    endpoint_class_name = get_endpoint_class_name_from_path(formatted_path)
     model_class_name = endpoint_class_name.replace("Endpoint", "Model")
     model_module_name = model_class_name.lower()
-    is_top_level_endpoint = False
-
-    top_level_check = formatted_path.lstrip("/").split("/")
-    if len(top_level_check) == 1:
-        is_top_level_endpoint = True
+    endpoint_import_directory = endpoint_output_directory.split("/")[-1]
+    model_import_directory = model_output_directory.split("/")[-1]
 
     operations = list(path_info.keys())
 
-    child_endpoints = relationships.get(formatted_path, [])
+    child_endpoints = list(
+        set(format_endpoint_path(child) for child in relationships.get(path, []))
+    )
 
     print(f"Generating {endpoint_class_name}")
 
     id_child_endpoint_class_name = None
     has_id_child = False
     additional_imports = []
     child_endpoint_definitions = []
     for child_endpoint in child_endpoints:
         if not child_endpoint:
             continue
 
         if "Id" in child_endpoint:
-            id_child_endpoint_class_name = endpoint_class_name.replace("Endpoint", f"IdEndpoint")
+            id_child_endpoint_class_name = endpoint_class_name.replace(
+                "Endpoint", f"IdEndpoint"
+            )
             if endpoint_class_name == id_child_endpoint_class_name:
                 continue
 
-            additional_imports.append(f"from pyconnectwise.endpoints.manage.{id_child_endpoint_class_name} import {id_child_endpoint_class_name}")
+            additional_imports.append(
+                f"from pyconnectwise.endpoints.{endpoint_import_directory}.{id_child_endpoint_class_name} import {id_child_endpoint_class_name}"
+            )
             has_id_child = True
         else:
             child_endpoint_path = child_endpoint
-            child_endpoint_class_name = "".join(to_title_case_preserve_case(word) for word in child_endpoint.split("/")) + "Endpoint"
+            child_endpoint_class_name = get_endpoint_class_name_from_path(
+                child_endpoint
+            )
             if endpoint_class_name == child_endpoint_class_name:
                 continue
 
-            field_name = None
-            name_segments = child_endpoint.split("/")
-            if len(name_segments) == 1:
-                field_name = name_segments[0]
-            else:
-                field_name = name_segments[-1]
             child_endpoint_definitions.append(
                 {
-                    "field_name": field_name,
-                    "class_name": endpoint_class_name.replace("Endpoint", child_endpoint_class_name),
+                    "field_name": ensure_not_reserved(
+                        to_snake_case(child_endpoint.split("/")[-1])
+                    ),
+                    "class_name": endpoint_class_name.replace(
+                        "Endpoint", child_endpoint_class_name
+                    ),
                     "path": child_endpoint_path.split("/")[-1],
                 }
             )
-            additional_imports.append(f"from pyconnectwise.endpoints.manage.{endpoint_class_name.replace('Endpoint', child_endpoint_class_name)} import {endpoint_class_name.replace('Endpoint', child_endpoint_class_name)}")
+            additional_imports.append(
+                f"from pyconnectwise.endpoints.{endpoint_import_directory}.{endpoint_class_name.replace('Endpoint', child_endpoint_class_name)} import {endpoint_class_name.replace('Endpoint', child_endpoint_class_name)}"
+            )
 
     imported_models = []
     op_definitions = []
     pagination_model_class = None
     for operation in operations:
         print(f"        Processing OP: {operation}")
+        if (
+            path_info.get(operation) is None
+            or path_info[operation].get("responses") is None
+        ):
+            continue
         operation_responses = path_info[operation]["responses"]
         operation_params = []
 
         if path_info[operation].get("parameters") is not None:
             operation_params = path_info[operation]["parameters"]
 
         for response in operation_responses.values():
@@ -102,42 +108,60 @@
                 schema_object = resp_content.get(list(resp_content)[0]).get("schema")
                 schema_ref = None
                 is_array = False
 
                 if schema_object.get("type") == "array":
                     is_array = True
                     schema_ref = schema_object.get("items").get("$ref")
-                elif schema_object.get("type") == "object" and schema_object.get("additionalProperties") is not None and schema_object.get("$ref") is not None:
+                elif (
+                    schema_object.get("type") == "object"
+                    and schema_object.get("additionalProperties") is not None
+                    and schema_object.get("$ref") is not None
+                ):
                     schema_ref = schema_object.get("additionalProperties").get("$ref")
                 else:
                     schema_ref = schema_object.get("$ref")
-                    
+
                 if schema_ref:
                     model_name = schema_ref.split("/")[-1]
-                    model_schema = models[model_name]
-                    generated_class_name = generate_model(
-                        model_output_directory, model_name, model_schema, models
-                    )
-                    return_type = generated_class_name
+                    absolute_model_name = ".".join(model_name.split(".")[:-1])
+                    if not absolute_model_name:
+                        absolute_model_name = model_name
+
+                    nested_import = False
+                    if len(absolute_model_name.split(".")) > 1:
+                        nested_import = True
+
+                    if nested_import:
+                        model_name = model_name.split(".")[-1]
+                    else:
+                        model_name = absolute_model_name
+
+                    return_type = model_name
                     return_class = return_type
 
                     for param in operation_params:
-                        param_name = param.get('name')
+                        param_name = param.get("name")
                         if param_name is not None:
                             if "page" in param_name:
-                                pagination_model_class = generated_class_name
+                                pagination_model_class = model_name
 
                     if is_array:
                         return_type = f"list[{return_type}]"
 
-                    if generated_class_name not in imported_models:
-                        additional_imports.append(
-                            f"from pyconnectwise.models.manage.{generated_class_name} import {generated_class_name}"
-                        )
-                        imported_models.append(generated_class_name)
+                    if absolute_model_name not in imported_models:
+                        if nested_import:
+                            additional_imports.append(
+                                f"from pyconnectwise.models.{model_import_directory}.{absolute_model_name} import {model_name}"
+                            )
+                        else:
+                            additional_imports.append(
+                                f"from pyconnectwise.models.{model_import_directory} import {model_name}"
+                            )
+                        imported_models.append(absolute_model_name)
 
                     op_definitions.append(
                         {
                             "name": operation,
                             "return_type": return_type,
                             "return_class": return_class,
                             "returns_single": not is_array,
@@ -145,64 +169,20 @@
                     )
 
     endpoint_code = endpoint_template.render(
         endpoint_class=endpoint_class_name,
         model_class=model_class_name,
         model_module=model_module_name,
         pagination_model_class=pagination_model_class,
-        endpoint_path=path.split("/")[-1],
+        endpoint_path=normalize_path_parameters(path.split("/")[-1]).rstrip("/"),
         operations=op_definitions,
         child_endpoints=child_endpoint_definitions,
         additional_imports=additional_imports,
         id_child_endpoint_class=id_child_endpoint_class_name,
         has_id_child=has_id_child,
         raw_path=path,
     )
 
     save_py_file(
         os.path.join(endpoint_output_directory, endpoint_class_name), endpoint_code
     )
-    return is_top_level_endpoint, endpoint_class_name
-
-
-
-def generate_top_level_endpoint(
-    endpoint_output_directory: str, path: str, path_info: dict, relationships: dict
-):
-    formatted_path = format_endpoint_path(path)
-    endpoint_class_name = "".join(to_title_case_preserve_case(word) for word in formatted_path.split("/")) + "Endpoint"
-    child_endpoints = relationships.get(formatted_path, [])
-
-    print(f"Generating {endpoint_class_name}")
-
-    additional_imports = []
-    for child_endpoint in child_endpoints:
-        child_endpoint_path = child_endpoint
-        child_endpoint_class = "".join(to_title_case_preserve_case(word) for word in child_endpoint.split("/")) + "Endpoint"
-        additional_imports.append(
-            f"from pyconnectwise.endpoints.manage.{endpoint_class_name.replace('Endpoint', child_endpoint_class)} import {endpoint_class_name.replace('Endpoint', child_endpoint_class)}"
-        )
-
-    child_endpoint_definitions = []
-    for child_endpoint in child_endpoints:
-        child_endpoint_path = child_endpoint
-        child_endpoint_class = "".join(to_title_case_preserve_case(word) for word in child_endpoint.split("/")) + "Endpoint"
-        child_endpoint_definitions.append(
-            {
-                "field_name": child_endpoint.split("/")[-1],
-                "class_name": endpoint_class_name.replace("Endpoint", child_endpoint_class),
-                "path": child_endpoint_path,
-            }
-        )
-
-    endpoint_code = top_level_endpoint_template.render(
-        endpoint_class=endpoint_class_name,
-        child_endpoints=child_endpoint_definitions,
-        additional_imports=additional_imports,
-        endpoint_path=path.split("/")[-1],
-    )
-
-    save_py_file(
-        os.path.join(endpoint_output_directory, endpoint_class_name), endpoint_code
-    )
-
     return endpoint_class_name
```

### Comparing `pyconnectwise-0.3.1/src/pyconnectwise/utils/generator/templates.py` & `pyconnectwise-0.4/src/pyconnectwise/utils/generator/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from jinja2 import Template
 
 endpoint_template = Template(
-"""from pyconnectwise.models.base.message_model import GenericMessageModel
+    """from pyconnectwise.models.base.message_model import GenericMessageModel
 from pyconnectwise.endpoints.base.connectwise_endpoint import ConnectWiseEndpoint
 from pyconnectwise.responses.paginated_response import PaginatedResponse
 from typing import Any
 {%- if additional_imports is defined %}
 {%- for additional_import in additional_imports %}
 {{ additional_import }}
 {%- endfor %}
 {%- endif %}
 
 class {{ endpoint_class }}(ConnectWiseEndpoint):
     def __init__(self, client, parent_endpoint=None):
         super().__init__(client, "{{ endpoint_path }}", parent_endpoint=parent_endpoint)
         {% if child_endpoints is defined %}
         {%- for child_endpoint in child_endpoints %}
-        self.{{ child_endpoint.field_name }} = self.register_child_endpoint(
+        self.{{ child_endpoint.field_name }} = self._register_child_endpoint(
             {{ child_endpoint.class_name }}(client, parent_endpoint=self)
         )
         {%- endfor %}
         {%- endif %}
     
     {% if has_id_child %}
     def id(self, id: int) -> {{ id_child_endpoint_class }}:
@@ -48,20 +48,21 @@
             params (dict[str, int | str]): The parameters to send in the request query string.
         Returns:
             PaginatedResponse[{{ pagination_model_class }}]: The initialized PaginatedResponse object.
         \"""
         params["page"] = page
         params["pageSize"] = page_size
         return PaginatedResponse(
-            super().make_request(
+            super()._make_request(
                 "GET",
                 params=params
             ),
             {{ pagination_model_class }},
             self,
+            page,
             page_size,
         )
     {% endif %}
 
     {%- for operation in operations %}
     def {{ operation.name }}(self, data: dict[str, Any] = {}, params: dict[str, int | str] = {}) -> {{ operation.return_type }}:
         \"""
@@ -70,79 +71,24 @@
         Parameters:
             data (dict[str, Any]): The data to send in the request body.
             params (dict[str, int | str]): The parameters to send in the request query string.
         Returns:
             {{ operation.return_type }}: The parsed response data.
         \"""
         {%- if operation.returns_single %}
-        return self._parse_one({{operation.return_class}}, super().make_request("{{ operation.name.upper() }}", data=data, params=params).json())
+        return self._parse_one({{operation.return_class}}, super()._make_request("{{ operation.name.upper() }}", data=data, params=params).json())
         {% else %}
-        return self._parse_many({{operation.return_class}}, super().make_request("{{ operation.name.upper() }}", data=data, params=params).json())
+        return self._parse_many({{operation.return_class}}, super()._make_request("{{ operation.name.upper() }}", data=data, params=params).json())
         {% endif %}
     {%- endfor %}
 """
 )
 
-top_level_endpoint_template = Template(
-"""from pyconnectwise.endpoints.base.connectwise_endpoint import ConnectWiseEndpoint
-{%- if additional_imports is defined %}
-{%- for additional_import in additional_imports %}
-{{ additional_import }}
-{%- endfor %}
-{%- endif %}
-
-class {{ endpoint_class }}(ConnectWiseEndpoint):
-    def __init__(self, client):
-        super().__init__(client, "{{ endpoint_path }}")
-        {% if child_endpoints is defined %}
-        {%- for child_endpoint in child_endpoints %}
-        self.{{ child_endpoint.field_name }} = self.register_child_endpoint(
-            {{ child_endpoint.class_name }}(client, parent_endpoint=self)
-        )
-        {%- endfor %}
-        {%- endif %}
-"""
-)
-
-model_template = Template(
-"""from __future__ import annotations
-from typing import Any
-from datetime import datetime
-from pyconnectwise.utils.naming import to_camel_case
-from pyconnectwise.models.base.connectwise_model import ConnectWiseModel
-
-{%- if imports is defined %}
-{%- for import in imports %}
-{{ import }}
-{%- endfor %}
-{%- endif %}
-
-{%- if mod_enums is defined %}
-{%- for mod_enum in mod_enums %}
-class {{ mod_enum.e_name }}(str, Enum):
-    {%- for enum_value in mod_enum.fields %}
-    {{ enum_value.v_name }} = '{{ enum_value.v_value }}'
-    {%- endfor %}
-
-{%- endfor %}
-{%- endif %}
-
-class {{ model_class }}(ConnectWiseModel):
-    {%- for field in fields %}
-    {{ field.name }}: {{ field.type }}
-    {%- endfor %}
-
-    {%- if empty_model == True %}
-    pass
-    {%- endif %}
-"""
-)
-
 manage_client_template = Template(
-"""import base64
+    """import base64
 import requests
 {%- if imports is defined %}
 {%- for import in imports %}
 {{ import }}
 {%- endfor %}
 {%- endif %}
 
@@ -176,41 +122,41 @@
         self.company_name = company_name
         self.manage_url = manage_url
         self.public_key = public_key
         self.private_key = private_key
         
         # Retrieve codebase from the API if not provided
         if not codebase:
-            codebase_request = self.__try_get_codebase_from_api(
+            codebase_request = self._try_get_codebase_from_api(
                 manage_url=manage_url,
                 company_name=company_name,
-                headers=self.get_headers(),
+                headers=self._get_headers(),
             )
 
             if codebase_request is None:
                 # we need to except here
                 raise Exception("Could not retrieve codebase from API.")
             self.codebase = codebase_request
             
 
         # Initializing endpoints
         {%- for endpoint in endpoints %}
         self.{{ endpoint.field_name }} = {{ endpoint.class_name }}(self)
         {%- endfor %}
 
-    def get_url(self) -> str:
+    def _get_url(self) -> str:
         \"""
         Generates and returns the URL for the ConnectWise Manage API endpoints based on the company url and codebase.
 
         Returns:
             str: API URL.
         \"""
         return f"https://{self.manage_url}/{self.codebase.strip('/')}/apis/3.0"
 
-    def __try_get_codebase_from_api(self, manage_url: str, company_name: str, headers: dict[str, str]) -> str | None:
+    def _try_get_codebase_from_api(self, manage_url: str, company_name: str, headers: dict[str, str]) -> str | None:
         \"""
         Tries to retrieve the codebase from the API using the provided company url, company name and headers.
 
         Parameters:
             company_url (str): URL of the company.
             company_name (str): Name of the company.
             headers (dict[str, str]): Headers to be sent in the request.
@@ -224,47 +170,47 @@
             result = (
                 requests.request("GET", url, headers=headers).json().get("Codebase")
             )
         except:
             result = None
         return result
 
-    def __get_auth_string(self) -> str:
+    def _get_auth_string(self) -> str:
         \"""
         Creates and returns the base64 encoded authorization string required for API requests.
 
         Returns:
             str: Base64 encoded authorization string.
         \"""
         return "Basic " + base64.b64encode(
             bytes(
                 f"{self.company_name}+{self.public_key}:{self.private_key}",
                 encoding="utf8",
             )
         ).decode("ascii")
 
-    def get_headers(self) -> dict[str, str]:
+    def _get_headers(self) -> dict[str, str]:
         \"""
         Generates and returns the headers required for making API requests.
 
         Returns:
             dict[str, str]: Dictionary of headers including Content-Type, Client ID, and Authorization.
         \"""
         headers = {
             "Content-Type": "application/json",
             "clientId": self.client_id,
-            "Authorization": self.__get_auth_string(),
+            "Authorization": self._get_auth_string(),
         }
         return headers
 
 """
 )
 
 automate_client_template = Template(
-"""import base64
+    """import base64
 import requests
 from datetime import datetime
 {%- if imports is defined %}
 {%- for import in imports %}
 {{ import }}
 {%- endfor %}
 {%- endif %}
@@ -291,45 +237,62 @@
             username (str): Your ConnectWise Automate API username.
             password (str): Your ConnectWise Automate API password.
         \"""
         self.client_id = client_id
         self.automate_url = automate_url
         self.username = username
         self.password = password
-        self.token_expiry_time: datetime = datetime.now().isoformat()
+        self.token_expiry_time: datetime = datetime.utcnow()
 
         # Grab first access token
-        self.access_token: str = __get_access_token()
+        self.access_token: str = self._get_access_token()
                 
         # Initializing endpoints
         {%- for endpoint in endpoints %}
         self.{{ endpoint.field_name }} = {{ endpoint.class_name }}(self)
         {%- endfor %}
 
-    def get_url(self) -> str:
+    def _get_url(self) -> str:
         \"""
         Generates and returns the URL for the ConnectWise Automate API endpoints based on the company url and codebase.
         Logs in an obtains an access token.
         Returns:
             str: API URL.
         \"""
-        return f"https://{self.automate_url}/cwa"
+        return f"https://{self.automate_url}/cwa/api/v1"
 
-    def __get_access_token() -> str:
-        token = ""
+    def _get_access_token(self) -> str:
+        \"""
+        Performs a request to the ConnectWise Automate API to obtain an access token.
+        \"""
+        token: str = ""
         try:
-            result
+            auth_response = requests.post(f'{self._get_url()}/apitoken', json={
+                "UserName": self.username,
+                "Password": self.password
+            }, headers={'Content-Type': 'application/json', 'ClientId': self.client_id}).json()
+            token = auth_response['AccessToken']
+            self.token_expiry_time = datetime.fromisoformat(auth_response['ExpirationDate'])
+        except Exception as e:
+            print(e)
+            return token
+        return token
+    
+    def _refresh_access_token_if_necessary(self):
+        if datetime.utcnow() > self.token_expiry_time:
+            self.access_token = self._get_access_token()
 
-    def get_headers(self) -> dict[str, str]:
+    def _get_headers(self) -> dict[str, str]:
         \"""
-        Generates and returns the headers required for making API requests.
+        Generates and returns the headers required for making API requests. The access token is refreshed if necessary before returning.
 
         Returns:
             dict[str, str]: Dictionary of headers including Content-Type, Client ID, and Authorization.
         \"""
+        self._refresh_access_token_if_necessary()
         headers = {
             "Content-Type": "application/json",
             "clientId": self.client_id,
             "Authorization": f"Bearer {self.access_token}",
         }
         return headers
```

