# Comparing `tmp/affixapi-1.1.60.tar.gz` & `tmp/affixapi-1.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.60.tar", last modified: Fri Apr 19 14:32:31 2024, max compression
+gzip compressed data, was "affixapi-1.1.61.tar", last modified: Mon Apr 22 00:39:09 2024, max compression
```

## Comparing `affixapi-1.1.60.tar` & `affixapi-1.1.61.tar`

### file list

```diff
@@ -1,146 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:32:31.545628 affixapi-1.1.60/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-19 14:32:28.000000 affixapi-1.1.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21425 2024-04-19 14:32:31.545628 affixapi-1.1.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21073 2024-04-19 14:32:28.000000 affixapi-1.1.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:32:31.545628 affixapi-1.1.60/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21425 2024-04-19 14:32:31.000000 affixapi-1.1.60/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-19 14:32:31.000000 affixapi-1.1.60/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:32:31.000000 affixapi-1.1.60/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 14:32:31.000000 affixapi-1.1.60/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 14:32:31.000000 affixapi-1.1.60/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:32:31.525628 affixapi-1.1.60/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:32:31.525628 affixapi-1.1.60/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    52716 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    52731 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:32:31.525628 affixapi-1.1.60/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:32:31.537628 affixapi-1.1.60/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18293 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    23196 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24581 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17983 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:32:31.537628 affixapi-1.1.60/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-19 14:32:28.000000 affixapi-1.1.60/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 14:32:31.545628 affixapi-1.1.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-19 14:32:28.000000 affixapi-1.1.60/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:32:31.545628 affixapi-1.1.60/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-19 14:32:28.000000 affixapi-1.1.60/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:39:09.865101 affixapi-1.1.61/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-22 00:39:06.000000 affixapi-1.1.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-04-22 00:39:09.865101 affixapi-1.1.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21499 2024-04-22 00:39:06.000000 affixapi-1.1.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:39:09.865101 affixapi-1.1.61/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-04-22 00:39:09.000000 affixapi-1.1.61/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-22 00:39:09.000000 affixapi-1.1.61/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 00:39:09.000000 affixapi-1.1.61/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 00:39:09.000000 affixapi-1.1.61/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 00:39:09.000000 affixapi-1.1.61/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:39:09.845101 affixapi-1.1.61/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:39:09.845101 affixapi-1.1.61/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    53156 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53171 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:39:09.845101 affixapi-1.1.61/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:39:09.853101 affixapi-1.1.61/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18293 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25519 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/employment_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17983 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:39:09.853101 affixapi-1.1.61/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-22 00:39:06.000000 affixapi-1.1.61/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 00:39:09.865101 affixapi-1.1.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-22 00:39:06.000000 affixapi-1.1.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:39:09.865101 affixapi-1.1.61/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_employment_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-22 00:39:06.000000 affixapi-1.1.61/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.60/LICENSE` & `affixapi-1.1.61/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/PKG-INFO` & `affixapi-1.1.61/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.60
+Version: 1.1.61
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -268,14 +268,15 @@
 
 import time
 import openapi_client
 from pprint import pprint
 from openapi_client.api import 2023_03_01_api
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
+from openapi_client.model.employment_status import EmploymentStatus
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -354,23 +355,28 @@
  - [AddressResponse](docs/AddressResponse.md)
  - [ClientRequest](docs/ClientRequest.md)
  - [ClientResponse](docs/ClientResponse.md)
  - [Companies20230301Response](docs/Companies20230301Response.md)
  - [CompanyResponse](docs/CompanyResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
+ - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
+ - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
  - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
  - [EmploymentResponse](docs/EmploymentResponse.md)
+ - [EmploymentStatus](docs/EmploymentStatus.md)
+ - [EmploymentStatusNotNullRequest](docs/EmploymentStatusNotNullRequest.md)
+ - [EmploymentStatusResponse](docs/EmploymentStatusResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
  - [IdAndMessageResponse](docs/IdAndMessageResponse.md)
  - [IdentityResponse](docs/IdentityResponse.md)
  - [InlineResponse400](docs/InlineResponse400.md)
```

### Comparing `affixapi-1.1.60/README.md` & `affixapi-1.1.61/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 
 import time
 import openapi_client
 from pprint import pprint
 from openapi_client.api import 2023_03_01_api
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
+from openapi_client.model.employment_status import EmploymentStatus
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -340,23 +341,28 @@
  - [AddressResponse](docs/AddressResponse.md)
  - [ClientRequest](docs/ClientRequest.md)
  - [ClientResponse](docs/ClientResponse.md)
  - [Companies20230301Response](docs/Companies20230301Response.md)
  - [CompanyResponse](docs/CompanyResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
+ - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
+ - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
  - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
  - [EmploymentResponse](docs/EmploymentResponse.md)
+ - [EmploymentStatus](docs/EmploymentStatus.md)
+ - [EmploymentStatusNotNullRequest](docs/EmploymentStatusNotNullRequest.md)
+ - [EmploymentStatusResponse](docs/EmploymentStatusResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
  - [IdAndMessageResponse](docs/IdAndMessageResponse.md)
  - [IdentityResponse](docs/IdentityResponse.md)
  - [InlineResponse400](docs/InlineResponse400.md)
```

### Comparing `affixapi-1.1.60/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.61/affixapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.60
+Version: 1.1.61
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -268,14 +268,15 @@
 
 import time
 import openapi_client
 from pprint import pprint
 from openapi_client.api import 2023_03_01_api
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
+from openapi_client.model.employment_status import EmploymentStatus
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -354,23 +355,28 @@
  - [AddressResponse](docs/AddressResponse.md)
  - [ClientRequest](docs/ClientRequest.md)
  - [ClientResponse](docs/ClientResponse.md)
  - [Companies20230301Response](docs/Companies20230301Response.md)
  - [CompanyResponse](docs/CompanyResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
+ - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
+ - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
  - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
  - [EmploymentResponse](docs/EmploymentResponse.md)
+ - [EmploymentStatus](docs/EmploymentStatus.md)
+ - [EmploymentStatusNotNullRequest](docs/EmploymentStatusNotNullRequest.md)
+ - [EmploymentStatusResponse](docs/EmploymentStatusResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
  - [IdAndMessageResponse](docs/IdAndMessageResponse.md)
  - [IdentityResponse](docs/IdentityResponse.md)
  - [InlineResponse400](docs/InlineResponse400.md)
```

### Comparing `affixapi-1.1.60/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.61/affixapi.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,28 @@
 openapi_client/model/address_response.py
 openapi_client/model/client_request.py
 openapi_client/model/client_response.py
 openapi_client/model/companies20230301_response.py
 openapi_client/model/company_response.py
 openapi_client/model/create_employee_request.py
 openapi_client/model/create_employee_request_bank_account.py
+openapi_client/model/create_employee_request_dependents.py
+openapi_client/model/create_employee_request_emergency_contacts.py
 openapi_client/model/create_employee_request_manager.py
 openapi_client/model/currency_not_null_request.py
 openapi_client/model/currency_response.py
 openapi_client/model/disconnect_response.py
 openapi_client/model/employee_response.py
 openapi_client/model/employee_response_manager.py
 openapi_client/model/employees20230301_response.py
 openapi_client/model/employment_no_null_enum_request.py
 openapi_client/model/employment_response.py
+openapi_client/model/employment_status.py
+openapi_client/model/employment_status_not_null_request.py
+openapi_client/model/employment_status_response.py
 openapi_client/model/group_no_null_enum_request.py
 openapi_client/model/group_response.py
 openapi_client/model/groups20230301_response.py
 openapi_client/model/groups_no_null_enum_request.py
 openapi_client/model/id_and_message_response.py
 openapi_client/model/identity_response.py
 openapi_client/model/inline_response400.py
@@ -82,23 +87,28 @@
 test/test_client_request.py
 test/test_client_response.py
 test/test_companies20230301_response.py
 test/test_company_response.py
 test/test_core_api.py
 test/test_create_employee_request.py
 test/test_create_employee_request_bank_account.py
+test/test_create_employee_request_dependents.py
+test/test_create_employee_request_emergency_contacts.py
 test/test_create_employee_request_manager.py
 test/test_currency_not_null_request.py
 test/test_currency_response.py
 test/test_disconnect_response.py
 test/test_employee_response.py
 test/test_employee_response_manager.py
 test/test_employees20230301_response.py
 test/test_employment_no_null_enum_request.py
 test/test_employment_response.py
+test/test_employment_status.py
+test/test_employment_status_not_null_request.py
+test/test_employment_status_response.py
 test/test_group_no_null_enum_request.py
 test/test_group_response.py
 test/test_groups20230301_response.py
 test/test_groups_no_null_enum_request.py
 test/test_id_and_message_response.py
 test/test_identity_response.py
 test/test_inline_response400.py
```

### Comparing `affixapi-1.1.60/openapi_client/__init__.py` & `affixapi-1.1.61/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.61/openapi_client/api/2023_03_01_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
+from openapi_client.model.employment_status import EmploymentStatus
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -166,14 +167,15 @@
             asynchronous HTTP request, please pass async_req=True
 
             >>> thread = api.xhr_employees20230301(async_req=True)
             >>> result = thread.get()
 
 
             Keyword Args:
+                employment_status (EmploymentStatus): Enable server-side filtering of the `employment_status` attribute . [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
                 _request_timeout (float/tuple): timeout setting for this request. If one
                     number provided, it will be total request timeout. It can also
@@ -225,14 +227,15 @@
                 'endpoint_path': '/2023-03-01/xhr/employees',
                 'operation_id': 'xhr_employees20230301',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'employment_status',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -240,18 +243,22 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'employment_status':
+                        (EmploymentStatus,),
                 },
                 'attribute_map': {
+                    'employment_status': 'employment_status',
                 },
                 'location_map': {
+                    'employment_status': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
```

### Comparing `affixapi-1.1.60/openapi_client/api/core_api.py` & `affixapi-1.1.61/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/api/management_api.py` & `affixapi-1.1.61/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.61/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
+from openapi_client.model.employment_status import EmploymentStatus
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -166,14 +167,15 @@
             asynchronous HTTP request, please pass async_req=True
 
             >>> thread = api.xhr_employees20230301(async_req=True)
             >>> result = thread.get()
 
 
             Keyword Args:
+                employment_status (EmploymentStatus): Enable server-side filtering of the `employment_status` attribute . [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
                 _request_timeout (float/tuple): timeout setting for this request. If one
                     number provided, it will be total request timeout. It can also
@@ -225,14 +227,15 @@
                 'endpoint_path': '/2023-03-01/xhr/employees',
                 'operation_id': 'xhr_employees20230301',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'employment_status',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -240,18 +243,22 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'employment_status':
+                        (EmploymentStatus,),
                 },
                 'attribute_map': {
+                    'employment_status': 'employment_status',
                 },
                 'location_map': {
+                    'employment_status': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
```

### Comparing `affixapi-1.1.60/openapi_client/api_client.py` & `affixapi-1.1.61/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/apis/__init__.py` & `affixapi-1.1.61/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/configuration.py` & `affixapi-1.1.61/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/exceptions.py` & `affixapi-1.1.61/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.61/openapi_client/model/address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/address_response.py` & `affixapi-1.1.61/openapi_client/model/address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/client_request.py` & `affixapi-1.1.61/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/client_response.py` & `affixapi-1.1.61/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.61/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/company_response.py` & `affixapi-1.1.61/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/create_employee_request.py` & `affixapi-1.1.61/openapi_client/model/create_employee_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,22 +26,28 @@
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
     from openapi_client.model.address_no_non_null_request import AddressNoNonNullRequest
     from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
+    from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
+    from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
     from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
     from openapi_client.model.employment_no_null_enum_request import EmploymentNoNullEnumRequest
+    from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
     from openapi_client.model.groups_no_null_enum_request import GroupsNoNullEnumRequest
     from openapi_client.model.location_no_non_null_request import LocationNoNonNullRequest
     globals()['AddressNoNonNullRequest'] = AddressNoNonNullRequest
     globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
+    globals()['CreateEmployeeRequestDependents'] = CreateEmployeeRequestDependents
+    globals()['CreateEmployeeRequestEmergencyContacts'] = CreateEmployeeRequestEmergencyContacts
     globals()['CreateEmployeeRequestManager'] = CreateEmployeeRequestManager
     globals()['EmploymentNoNullEnumRequest'] = EmploymentNoNullEnumRequest
+    globals()['EmploymentStatusNotNullRequest'] = EmploymentStatusNotNullRequest
     globals()['GroupsNoNullEnumRequest'] = GroupsNoNullEnumRequest
     globals()['LocationNoNonNullRequest'] = LocationNoNonNullRequest
 
 
 class CreateEmployeeRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -85,21 +91,14 @@
         },
         ('marital_status',): {
             'None': None,
             'SINGLE': "single",
             'MARRIED': "married",
             'NOT_SPECIFIED': "not_specified",
         },
-        ('employment_status',): {
-            'None': None,
-            'ACTIVE': "active",
-            'INACTIVE': "inactive",
-            'PENDING': "pending",
-            'LEAVE': "leave",
-        },
         ('employment_type',): {
             'None': None,
             'FULL_TIME': "full_time",
             'PART_TIME': "part_time",
             'CONTRACTOR': "contractor",
             'OTHER': "other",
         },
@@ -134,26 +133,28 @@
             'personal_email': (str, none_type,),  # noqa: E501
             'mobile_phone_number': (str, none_type,),  # noqa: E501
             'tax_id': (str, none_type,),  # noqa: E501
             'gender': (str, none_type,),  # noqa: E501
             'ethnicity': (str, none_type,),  # noqa: E501
             'marital_status': (str, none_type,),  # noqa: E501
             'date_of_birth': (date, none_type,),  # noqa: E501
-            'employment_status': (str, none_type,),  # noqa: E501
+            'employment_status': (EmploymentStatusNotNullRequest,),  # noqa: E501
             'employment_type': (str, none_type,),  # noqa: E501
             'start_date': (date, none_type,),  # noqa: E501
             'termination_date': (date, none_type,),  # noqa: E501
             'avatar': (str, none_type,),  # noqa: E501
             'home_location': (AddressNoNonNullRequest,),  # noqa: E501
             'work_location': (LocationNoNonNullRequest,),  # noqa: E501
             'manager': (CreateEmployeeRequestManager,),  # noqa: E501
             'bank_account': (CreateEmployeeRequestBankAccount,),  # noqa: E501
             'employments': ([EmploymentNoNullEnumRequest], none_type,),  # noqa: E501
             'custom_fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'groups': (GroupsNoNullEnumRequest,),  # noqa: E501
+            'dependents': ([CreateEmployeeRequestDependents], none_type,),  # noqa: E501
+            'emergency_contacts': ([CreateEmployeeRequestEmergencyContacts], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -180,14 +181,16 @@
         'home_location': 'home_location',  # noqa: E501
         'work_location': 'work_location',  # noqa: E501
         'manager': 'manager',  # noqa: E501
         'bank_account': 'bank_account',  # noqa: E501
         'employments': 'employments',  # noqa: E501
         'custom_fields': 'custom_fields',  # noqa: E501
         'groups': 'groups',  # noqa: E501
+        'dependents': 'dependents',  # noqa: E501
+        'emergency_contacts': 'emergency_contacts',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
@@ -244,26 +247,28 @@
             personal_email (str, none_type): the personal email of the individual. [optional]  # noqa: E501
             mobile_phone_number (str, none_type): +1234567890. [optional]  # noqa: E501
             tax_id (str, none_type): [optional]  # noqa: E501
             gender (str, none_type): [optional]  # noqa: E501
             ethnicity (str, none_type): [optional]  # noqa: E501
             marital_status (str, none_type): [optional]  # noqa: E501
             date_of_birth (date, none_type): [optional]  # noqa: E501
-            employment_status (str, none_type): [optional]  # noqa: E501
+            employment_status (EmploymentStatusNotNullRequest): [optional]  # noqa: E501
             employment_type (str, none_type): [optional]  # noqa: E501
             start_date (date, none_type): [optional]  # noqa: E501
             termination_date (date, none_type): [optional]  # noqa: E501
             avatar (str, none_type): [optional]  # noqa: E501
             home_location (AddressNoNonNullRequest): [optional]  # noqa: E501
             work_location (LocationNoNonNullRequest): [optional]  # noqa: E501
             manager (CreateEmployeeRequestManager): [optional]  # noqa: E501
             bank_account (CreateEmployeeRequestBankAccount): [optional]  # noqa: E501
             employments ([EmploymentNoNullEnumRequest], none_type): [optional]  # noqa: E501
             custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
             groups (GroupsNoNullEnumRequest): [optional]  # noqa: E501
+            dependents ([CreateEmployeeRequestDependents], none_type): [optional]  # noqa: E501
+            emergency_contacts ([CreateEmployeeRequestEmergencyContacts], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `affixapi-1.1.60/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.61/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.61/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/currency_not_null_request.py` & `affixapi-1.1.61/openapi_client/model/currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/currency_response.py` & `affixapi-1.1.61/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/disconnect_response.py` & `affixapi-1.1.61/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/employee_response.py` & `affixapi-1.1.61/openapi_client/model/employee_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,22 +26,28 @@
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
     from openapi_client.model.address_response import AddressResponse
     from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
+    from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
+    from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
     from openapi_client.model.employee_response_manager import EmployeeResponseManager
     from openapi_client.model.employment_response import EmploymentResponse
+    from openapi_client.model.employment_status_response import EmploymentStatusResponse
     from openapi_client.model.groups20230301_response import Groups20230301Response
     from openapi_client.model.location_response import LocationResponse
     globals()['AddressResponse'] = AddressResponse
     globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
+    globals()['CreateEmployeeRequestDependents'] = CreateEmployeeRequestDependents
+    globals()['CreateEmployeeRequestEmergencyContacts'] = CreateEmployeeRequestEmergencyContacts
     globals()['EmployeeResponseManager'] = EmployeeResponseManager
     globals()['EmploymentResponse'] = EmploymentResponse
+    globals()['EmploymentStatusResponse'] = EmploymentStatusResponse
     globals()['Groups20230301Response'] = Groups20230301Response
     globals()['LocationResponse'] = LocationResponse
 
 
 class EmployeeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -89,22 +95,14 @@
             'None': None,
             'SINGLE': "single",
             'MARRIED': "married",
             'NOT_SPECIFIED': "not_specified",
             'OTHER': "other",
             'NULL': "null",
         },
-        ('employment_status',): {
-            'None': None,
-            'NULL': "null",
-            'ACTIVE': "active",
-            'INACTIVE': "inactive",
-            'PENDING': "pending",
-            'LEAVE': "leave",
-        },
         ('employment_type',): {
             'None': None,
             'NULL': "null",
             'FULL_TIME': "full_time",
             'PART_TIME': "part_time",
             'CONTRACTOR': "contractor",
             'OTHER': "other",
@@ -142,27 +140,29 @@
             'personal_email': (str, none_type,),  # noqa: E501
             'mobile_phone_number': (str, none_type,),  # noqa: E501
             'tax_id': (str, none_type,),  # noqa: E501
             'gender': (str, none_type,),  # noqa: E501
             'ethnicity': (str, none_type,),  # noqa: E501
             'marital_status': (str, none_type,),  # noqa: E501
             'date_of_birth': (date, none_type,),  # noqa: E501
-            'employment_status': (str, none_type,),  # noqa: E501
+            'employment_status': (EmploymentStatusResponse,),  # noqa: E501
             'employment_type': (str, none_type,),  # noqa: E501
             'start_date': (date, none_type,),  # noqa: E501
             'remote_created_at': (date, none_type,),  # noqa: E501
             'termination_date': (date, none_type,),  # noqa: E501
             'avatar': (str, none_type,),  # noqa: E501
             'home_location': (AddressResponse,),  # noqa: E501
             'work_location': (LocationResponse,),  # noqa: E501
             'manager': (EmployeeResponseManager,),  # noqa: E501
             'bank_account': (CreateEmployeeRequestBankAccount,),  # noqa: E501
             'employments': ([EmploymentResponse], none_type,),  # noqa: E501
             'custom_fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'groups': (Groups20230301Response,),  # noqa: E501
+            'dependents': ([CreateEmployeeRequestDependents], none_type,),  # noqa: E501
+            'emergency_contacts': ([CreateEmployeeRequestEmergencyContacts], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -192,29 +192,31 @@
         'home_location': 'home_location',  # noqa: E501
         'work_location': 'work_location',  # noqa: E501
         'manager': 'manager',  # noqa: E501
         'bank_account': 'bank_account',  # noqa: E501
         'employments': 'employments',  # noqa: E501
         'custom_fields': 'custom_fields',  # noqa: E501
         'groups': 'groups',  # noqa: E501
+        'dependents': 'dependents',  # noqa: E501
+        'emergency_contacts': 'emergency_contacts',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, remote_id, employee_number, first_name, last_name, display_full_name, nationality, job_title, work_email, personal_email, mobile_phone_number, tax_id, gender, ethnicity, marital_status, date_of_birth, employment_status, employment_type, start_date, remote_created_at, termination_date, avatar, home_location, work_location, manager, bank_account, employments, custom_fields, groups, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, remote_id, employee_number, first_name, last_name, display_full_name, nationality, job_title, work_email, personal_email, mobile_phone_number, tax_id, gender, ethnicity, marital_status, date_of_birth, employment_status, employment_type, start_date, remote_created_at, termination_date, avatar, home_location, work_location, manager, bank_account, employments, custom_fields, groups, dependents, emergency_contacts, *args, **kwargs):  # noqa: E501
         """EmployeeResponse - a model defined in OpenAPI
 
         Args:
             id (str): The Affix-assigned id of the individual
             remote_id (str): the remote system-assigned id of the individual
             employee_number (str, none_type):
             first_name (str): the first name of the individual
@@ -226,27 +228,29 @@
             personal_email (str, none_type): the personal email of the individual
             mobile_phone_number (str, none_type): +1234567890
             tax_id (str, none_type):
             gender (str, none_type):
             ethnicity (str, none_type):
             marital_status (str, none_type): `other` option can include co-habitating, civil partnership, separated, divorced, widowed, etc 
             date_of_birth (date, none_type):
-            employment_status (str, none_type):
+            employment_status (EmploymentStatusResponse):
             employment_type (str, none_type):
             start_date (date, none_type):
             remote_created_at (date, none_type):
             termination_date (date, none_type):
             avatar (str, none_type):
             home_location (AddressResponse):
             work_location (LocationResponse):
             manager (EmployeeResponseManager):
             bank_account (CreateEmployeeRequestBankAccount):
             employments ([EmploymentResponse], none_type):
             custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type):
             groups (Groups20230301Response):
+            dependents ([CreateEmployeeRequestDependents], none_type):
+            emergency_contacts ([CreateEmployeeRequestEmergencyContacts], none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -325,14 +329,16 @@
         self.home_location = home_location
         self.work_location = work_location
         self.manager = manager
         self.bank_account = bank_account
         self.employments = employments
         self.custom_fields = custom_fields
         self.groups = groups
+        self.dependents = dependents
+        self.emergency_contacts = emergency_contacts
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `affixapi-1.1.60/openapi_client/model/employee_response_manager.py` & `affixapi-1.1.61/openapi_client/model/employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.61/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/employment_no_null_enum_request.py` & `affixapi-1.1.61/openapi_client/model/employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/employment_response.py` & `affixapi-1.1.61/openapi_client/model/employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.61/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/group_response.py` & `affixapi-1.1.61/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.61/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.61/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.61/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/identity_response.py` & `affixapi-1.1.61/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/inline_response400.py` & `affixapi-1.1.61/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/inline_response401.py` & `affixapi-1.1.61/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/inline_response409.py` & `affixapi-1.1.61/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/introspect_response.py` & `affixapi-1.1.61/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.61/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/location_response.py` & `affixapi-1.1.61/openapi_client/model/location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/message_response.py` & `affixapi-1.1.61/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/mode_request.py` & `affixapi-1.1.61/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/mode_response.py` & `affixapi-1.1.61/openapi_client/model/mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/payrun_response.py` & `affixapi-1.1.61/openapi_client/model/payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.61/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/payslip_response.py` & `affixapi-1.1.61/openapi_client/model/payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.61/openapi_client/model/payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.61/openapi_client/model/payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.61/openapi_client/model/payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.61/openapi_client/model/payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.61/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/provider_request.py` & `affixapi-1.1.61/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/provider_response.py` & `affixapi-1.1.61/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/providers_response.py` & `affixapi-1.1.61/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/scopes_request.py` & `affixapi-1.1.61/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/scopes_response.py` & `affixapi-1.1.61/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.61/openapi_client/model/time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.61/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.61/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.61/openapi_client/model/time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/timesheet_response.py` & `affixapi-1.1.61/openapi_client/model/timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.61/openapi_client/model/timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/token_request.py` & `affixapi-1.1.61/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/token_response.py` & `affixapi-1.1.61/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/tokens_response.py` & `affixapi-1.1.61/openapi_client/model/tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model/work_locations20230301_response.py` & `affixapi-1.1.61/openapi_client/model/work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/model_utils.py` & `affixapi-1.1.61/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/openapi_client/models/__init__.py` & `affixapi-1.1.61/openapi_client/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,28 @@
 from openapi_client.model.address_response import AddressResponse
 from openapi_client.model.client_request import ClientRequest
 from openapi_client.model.client_response import ClientResponse
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.company_response import CompanyResponse
 from openapi_client.model.create_employee_request import CreateEmployeeRequest
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
+from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
+from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
 from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
 from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
 from openapi_client.model.currency_response import CurrencyResponse
 from openapi_client.model.disconnect_response import DisconnectResponse
 from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employee_response_manager import EmployeeResponseManager
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.employment_no_null_enum_request import EmploymentNoNullEnumRequest
 from openapi_client.model.employment_response import EmploymentResponse
+from openapi_client.model.employment_status import EmploymentStatus
+from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
+from openapi_client.model.employment_status_response import EmploymentStatusResponse
 from openapi_client.model.group_no_null_enum_request import GroupNoNullEnumRequest
 from openapi_client.model.group_response import GroupResponse
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.groups_no_null_enum_request import GroupsNoNullEnumRequest
 from openapi_client.model.id_and_message_response import IdAndMessageResponse
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response400 import InlineResponse400
```

### Comparing `affixapi-1.1.60/openapi_client/rest.py` & `affixapi-1.1.61/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/setup.py` & `affixapi-1.1.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.60"
+VERSION = "1.1.61"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.60/test/test_2023_03_01_api.py` & `affixapi-1.1.61/test/test_2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_address_no_non_null_request.py` & `affixapi-1.1.61/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_address_response.py` & `affixapi-1.1.61/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_client_request.py` & `affixapi-1.1.61/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_client_response.py` & `affixapi-1.1.61/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_companies20230301_response.py` & `affixapi-1.1.61/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_company_response.py` & `affixapi-1.1.61/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_core_api.py` & `affixapi-1.1.61/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_create_employee_request.py` & `affixapi-1.1.61/test/test_create_employee_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,28 @@
 
 import sys
 import unittest
 
 import openapi_client
 from openapi_client.model.address_no_non_null_request import AddressNoNonNullRequest
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
+from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
+from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
 from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
 from openapi_client.model.employment_no_null_enum_request import EmploymentNoNullEnumRequest
+from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
 from openapi_client.model.groups_no_null_enum_request import GroupsNoNullEnumRequest
 from openapi_client.model.location_no_non_null_request import LocationNoNonNullRequest
 globals()['AddressNoNonNullRequest'] = AddressNoNonNullRequest
 globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
+globals()['CreateEmployeeRequestDependents'] = CreateEmployeeRequestDependents
+globals()['CreateEmployeeRequestEmergencyContacts'] = CreateEmployeeRequestEmergencyContacts
 globals()['CreateEmployeeRequestManager'] = CreateEmployeeRequestManager
 globals()['EmploymentNoNullEnumRequest'] = EmploymentNoNullEnumRequest
+globals()['EmploymentStatusNotNullRequest'] = EmploymentStatusNotNullRequest
 globals()['GroupsNoNullEnumRequest'] = GroupsNoNullEnumRequest
 globals()['LocationNoNonNullRequest'] = LocationNoNonNullRequest
 from openapi_client.model.create_employee_request import CreateEmployeeRequest
 
 
 class TestCreateEmployeeRequest(unittest.TestCase):
     """CreateEmployeeRequest unit test stubs"""
```

### Comparing `affixapi-1.1.60/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.61/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_create_employee_request_manager.py` & `affixapi-1.1.61/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_currency_not_null_request.py` & `affixapi-1.1.61/test/test_currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_currency_response.py` & `affixapi-1.1.61/test/test_currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_disconnect_response.py` & `affixapi-1.1.61/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_employee_response.py` & `affixapi-1.1.61/test/test_employee_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,28 @@
 
 import sys
 import unittest
 
 import openapi_client
 from openapi_client.model.address_response import AddressResponse
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
+from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
+from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
 from openapi_client.model.employee_response_manager import EmployeeResponseManager
 from openapi_client.model.employment_response import EmploymentResponse
+from openapi_client.model.employment_status_response import EmploymentStatusResponse
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.location_response import LocationResponse
 globals()['AddressResponse'] = AddressResponse
 globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
+globals()['CreateEmployeeRequestDependents'] = CreateEmployeeRequestDependents
+globals()['CreateEmployeeRequestEmergencyContacts'] = CreateEmployeeRequestEmergencyContacts
 globals()['EmployeeResponseManager'] = EmployeeResponseManager
 globals()['EmploymentResponse'] = EmploymentResponse
+globals()['EmploymentStatusResponse'] = EmploymentStatusResponse
 globals()['Groups20230301Response'] = Groups20230301Response
 globals()['LocationResponse'] = LocationResponse
 from openapi_client.model.employee_response import EmployeeResponse
 
 
 class TestEmployeeResponse(unittest.TestCase):
     """EmployeeResponse unit test stubs"""
```

### Comparing `affixapi-1.1.60/test/test_employee_response_manager.py` & `affixapi-1.1.61/test/test_employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_employees20230301_response.py` & `affixapi-1.1.61/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_employment_no_null_enum_request.py` & `affixapi-1.1.61/test/test_employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_employment_response.py` & `affixapi-1.1.61/test/test_employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_group_no_null_enum_request.py` & `affixapi-1.1.61/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_group_response.py` & `affixapi-1.1.61/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_groups20230301_response.py` & `affixapi-1.1.61/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.61/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_id_and_message_response.py` & `affixapi-1.1.61/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_identity_response.py` & `affixapi-1.1.61/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_inline_response400.py` & `affixapi-1.1.61/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_inline_response401.py` & `affixapi-1.1.61/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_inline_response409.py` & `affixapi-1.1.61/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_introspect_response.py` & `affixapi-1.1.61/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_location_no_non_null_request.py` & `affixapi-1.1.61/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_location_response.py` & `affixapi-1.1.61/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_management_api.py` & `affixapi-1.1.61/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_message_response.py` & `affixapi-1.1.61/test/test_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_mode_request.py` & `affixapi-1.1.61/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_mode_response.py` & `affixapi-1.1.61/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_payrun_response.py` & `affixapi-1.1.61/test/test_payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_payruns20230301_response.py` & `affixapi-1.1.61/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_payslip_response.py` & `affixapi-1.1.61/test/test_payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_payslip_response_contributions.py` & `affixapi-1.1.61/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_payslip_response_deductions.py` & `affixapi-1.1.61/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_payslip_response_earnings.py` & `affixapi-1.1.61/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_payslip_response_taxes.py` & `affixapi-1.1.61/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_payslips20230301_response.py` & `affixapi-1.1.61/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_provider_request.py` & `affixapi-1.1.61/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_provider_response.py` & `affixapi-1.1.61/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_providers_response.py` & `affixapi-1.1.61/test/test_providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_scopes_request.py` & `affixapi-1.1.61/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_scopes_response.py` & `affixapi-1.1.61/test/test_scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_time_off_balance_response.py` & `affixapi-1.1.61/test/test_time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.61/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.61/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_time_off_entry_response.py` & `affixapi-1.1.61/test/test_time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_timesheet_response.py` & `affixapi-1.1.61/test/test_timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_timesheets20230301_response.py` & `affixapi-1.1.61/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_token_request.py` & `affixapi-1.1.61/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_token_response.py` & `affixapi-1.1.61/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_tokens_response.py` & `affixapi-1.1.61/test/test_tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_work_locations20230301_response.py` & `affixapi-1.1.61/test/test_work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.60/test/test_xhr__vertically_integrated_api.py` & `affixapi-1.1.61/test/test_xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

