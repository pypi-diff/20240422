# Comparing `tmp/lago-python-client-1.1.0.tar.gz` & `tmp/lago-python-client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/lago-python-client/lago-python-client/dist/.tmp-dag7xis_/lago-python-client-1.1.0.tar", last modified: Tue Mar 26 10:08:32 2024, max compression
+gzip compressed data, was "/home/runner/work/lago-python-client/lago-python-client/dist/.tmp-qs5bfr58/lago-python-client-1.2.0.tar", last modified: Mon Apr 22 08:44:34 2024, max compression
```

## Comparing `lago-python-client-1.1.0.tar` & `lago-python-client-1.2.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/add_ons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/add_ons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/add_ons/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/billable_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/billable_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/billable_metrics/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/coupons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/coupons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/coupons/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/credit_notes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/credit_notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/credit_notes/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/customers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/customers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/customers/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/events/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/fees/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/fees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/fees/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/functools_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/gross_revenues/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/gross_revenues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/gross_revenues/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/invoice_collections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/invoice_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/invoice_collections/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/invoiced_usages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/invoiced_usages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/invoiced_usages/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/invoices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/invoices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/invoices/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/applied_coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/billable_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/credit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/credit_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/customer_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/fee.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/gross_revenue.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/invoice_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/invoiced_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/minimum_commitment.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/mrr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/wallet_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/models/webhook_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/mrrs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/mrrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/mrrs/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/organizations/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/plans/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/plans/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/services/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/services/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/services/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/subscriptions/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/taxes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/taxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/taxes/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/wallets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/wallets/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/webhook_endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/webhook_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/webhook_endpoints/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/lago_python_client/webhooks/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/lago_python_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:32.000000 lago-python-client-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_add_on_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_applied_coupon_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_billable_metric_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_coupon_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_credit_note_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_customer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_event_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_fee_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_functools_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_gross_revenue_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_group_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_invoice_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_invoice_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_invoiced_usage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_json_services.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_mrr_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_organization_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_plan_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_request_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_response_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_subscription_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_tax_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_wallet_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_wallet_transaction_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_webhook_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-26 10:08:23.000000 lago-python-client-1.1.0/tests/test_webhook_endpoint_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/add_ons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/add_ons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/add_ons/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/billable_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/billable_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/billable_metrics/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/coupons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/coupons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/coupons/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/credit_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/credit_notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/credit_notes/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/customers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/customers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/customers/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/events/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/fees/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/fees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/fees/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/functools_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/gross_revenues/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/gross_revenues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/gross_revenues/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/invoice_collections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoice_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoice_collections/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/invoiced_usages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoiced_usages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoiced_usages/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/invoices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoices/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/applied_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/billable_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/customer_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/gross_revenue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/invoice_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/invoiced_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/minimum_commitment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/mrr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/wallet_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/webhook_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/mrrs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/mrrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/mrrs/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/organizations/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/plans/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/plans/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/services/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/services/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/services/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/subscriptions/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/taxes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/taxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/taxes/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/wallets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/wallets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/wallets/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/webhook_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/webhook_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/webhook_endpoints/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/webhooks/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_add_on_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_applied_coupon_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_billable_metric_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_coupon_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_credit_note_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_customer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_event_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_fee_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_functools_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_gross_revenue_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_group_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_invoice_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_invoice_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_invoiced_usage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_json_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_mrr_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_organization_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_plan_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_request_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_response_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_subscription_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_tax_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_wallet_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_wallet_transaction_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_webhook_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_webhook_endpoint_client.py
```

### Comparing `lago-python-client-1.1.0/LICENSE` & `lago-python-client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/PKG-INFO` & `lago-python-client-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lago-python-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: Lago Python API Client
 Home-page: https://github.com/getlago/lago-python-client
 Author: Lovro Colic
 Author-email: lovro@getlago.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lago-python-client-1.1.0/README.md` & `lago-python-client-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/add_ons/clients.py` & `lago-python-client-1.2.0/lago_python_client/add_ons/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/base_client.py` & `lago-python-client-1.2.0/lago_python_client/base_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/billable_metrics/clients.py` & `lago-python-client-1.2.0/lago_python_client/billable_metrics/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/client.py` & `lago-python-client-1.2.0/lago_python_client/client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/coupons/clients.py` & `lago-python-client-1.2.0/lago_python_client/coupons/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/credit_notes/clients.py` & `lago-python-client-1.2.0/lago_python_client/credit_notes/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/customers/clients.py` & `lago-python-client-1.2.0/lago_python_client/customers/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/events/clients.py` & `lago-python-client-1.2.0/lago_python_client/events/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/exceptions.py` & `lago-python-client-1.2.0/lago_python_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/functools_ext.py` & `lago-python-client-1.2.0/lago_python_client/functools_ext.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/gross_revenues/clients.py` & `lago-python-client-1.2.0/lago_python_client/gross_revenues/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/invoice_collections/clients.py` & `lago-python-client-1.2.0/lago_python_client/invoice_collections/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/invoiced_usages/clients.py` & `lago-python-client-1.2.0/lago_python_client/invoiced_usages/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/invoices/clients.py` & `lago-python-client-1.2.0/lago_python_client/invoices/clients.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,14 +78,28 @@
         )
 
         return prepare_object_response(
             response_model=self.RESPONSE_MODEL,
             data=get_response_data(response=api_response, key=self.ROOT_NAME),
         )
 
+    def lose_dispute(self, resource_id: str) -> InvoiceResponse:
+        api_response: Response = send_put_request(
+            url=make_url(
+                origin=self.base_url,
+                path_parts=(self.API_RESOURCE, resource_id, 'lose_dispute'),
+            ),
+            headers=make_headers(api_key=self.api_key),
+        )
+
+        return prepare_object_response(
+            response_model=self.RESPONSE_MODEL,
+            data=get_response_data(response=api_response, key=self.ROOT_NAME),
+        )
+
     def payment_url(self, resource_id: str) -> str:
         api_response: Response = send_post_request(
             url=make_url(
                 origin=self.base_url,
                 path_parts=(self.API_RESOURCE, resource_id, 'payment_url'),
             ),
             headers=make_headers(api_key=self.api_key),
```

### Comparing `lago-python-client-1.1.0/lago_python_client/mixins.py` & `lago-python-client-1.2.0/lago_python_client/mixins.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/__init__.py` & `lago-python-client-1.2.0/lago_python_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/add_on.py` & `lago-python-client-1.2.0/lago_python_client/models/add_on.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/applied_coupon.py` & `lago-python-client-1.2.0/lago_python_client/models/applied_coupon.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/billable_metric.py` & `lago-python-client-1.2.0/lago_python_client/models/coupon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,48 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, List, Optional
 
 from lago_python_client.base_model import BaseModel
 
 from ..base_model import BaseResponseModel
 
 
-class BillableMetricGroup(BaseModel):
-    key: Optional[str]
-    values: Optional[List[Union[str, Dict[str, Any]]]]
+class LimitationConfiguration(BaseModel):
+    plan_codes: Optional[List[Any]]
+    billable_metric_codes: Optional[List[Any]]
 
 
-class BillableMetric(BaseModel):
+class Coupon(BaseModel):
     name: Optional[str]
     code: Optional[str]
     description: Optional[str]
-    recurring: Optional[bool]
-    aggregation_type: Optional[str]
-    weighted_interval: Optional[str]
-    field_name: Optional[str]
-    group: Optional[BillableMetricGroup]
+    amount_cents: Optional[int]
+    amount_currency: Optional[str]
+    expiration: Optional[str]
+    expiration_at: Optional[str]
+    percentage_rate: Optional[float]
+    coupon_type: Optional[str]
+    reusable: Optional[bool]
+    frequency: Optional[str]
+    frequency_duration: Optional[int]
+    applies_to: Optional[LimitationConfiguration]
 
 
-class BillableMetricResponse(BaseResponseModel):
+class CouponResponse(BaseResponseModel):
     lago_id: str
     name: str
     code: str
     description: Optional[str]
-    recurring: Optional[bool]
-    aggregation_type: Optional[str]
-    weighted_interval: Optional[str]
-    field_name: Optional[str]
+    amount_cents: Optional[int]
+    amount_currency: Optional[str]
     created_at: str
-    group: BillableMetricGroup
-    active_subscriptions_count: int
-    draft_invoices_count: int
-    plans_count: int
+    expiration: str
+    expiration_at: Optional[str]
+    terminated_at: Optional[str]
+    percentage_rate: Optional[float]
+    coupon_type: Optional[str]
+    reusable: Optional[bool]
+    frequency: Optional[str]
+    frequency_duration: Optional[int]
+    plan_codes: Optional[List[Any]]
+    limited_plans: Optional[bool]
+    billable_metric_codes: Optional[List[Any]]
+    limited_billable_metrics: Optional[bool]
```

### Comparing `lago-python-client-1.1.0/lago_python_client/models/charge.py` & `lago-python-client-1.2.0/lago_python_client/models/charge.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,36 @@
     invoice_display_name: Optional[str]
 
 
 class GroupPropertiesList(BaseModel):
     __root__: List[GroupProperties]
 
 
+class ChargeFilter(BaseModel):
+    invoice_display_name: Optional[str]
+    properties: Optional[Dict[str, Any]]
+    values: Optional[Dict[str, List[str]]]
+
+
+class ChargeFilters(BaseModel):
+    __root__: List[ChargeFilter]
+
+
 class Charge(BaseModel):
     id: Optional[str]
     billable_metric_id: Optional[str]
     charge_model: Optional[str]
     pay_in_advance: Optional[bool]
     prorated: Optional[bool]
     invoiceable: Optional[bool]
     invoice_display_name: Optional[str]
     min_amount_cents: Optional[int]
     properties: Optional[Dict[str, Any]]
     group_properties: Optional[GroupPropertiesList]
+    filters: Optional[ChargeFilters]
     tax_codes: Optional[List[str]]
 
 
 class Charges(BaseModel):
     __root__: List[Charge]
 
 
@@ -42,25 +53,27 @@
     pay_in_advance: Optional[bool]
     prorated: Optional[bool]
     invoiceable: Optional[bool]
     invoice_display_name: Optional[str]
     min_amount_cents: Optional[int]
     properties: Optional[Dict[str, Any]]
     group_properties: Optional[GroupPropertiesList]
+    filters: Optional[ChargeFilters]
     taxes: Optional[TaxesResponse]
 
 
 class ChargesResponse(BaseResponseModel):
     __root__: List[ChargeResponse]
 
 
 class ChargeOverrides(BaseModel):
     id: Optional[str]
     invoice_display_name: Optional[str]
     min_amount_cents: Optional[int]
     properties: Optional[Dict[str, Any]]
     group_properties: Optional[GroupPropertiesList]
+    filters: Optional[ChargeFilters]
     tax_codes: Optional[List[str]]
 
 
 class ChargesOverrides(BaseModel):
     __root__: List[ChargeOverrides]
```

### Comparing `lago-python-client-1.1.0/lago_python_client/models/coupon.py` & `lago-python-client-1.2.0/lago_python_client/models/billable_metric.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from lago_python_client.base_model import BaseModel
 
 from ..base_model import BaseResponseModel
 
 
-class LimitationConfiguration(BaseModel):
-    plan_codes: Optional[List[Any]]
-    billable_metric_codes: Optional[List[Any]]
+class BillableMetricGroup(BaseModel):
+    key: Optional[str]
+    values: Optional[List[Union[str, Dict[str, Any]]]]
 
 
-class Coupon(BaseModel):
+class BillableMetricFilter(BaseModel):
+    key: Optional[str]
+    values: Optional[List[str]]
+
+
+class BillableMetricFilters(BaseModel):
+    __root__: List[BillableMetricFilter]
+
+
+class BillableMetric(BaseModel):
     name: Optional[str]
     code: Optional[str]
     description: Optional[str]
-    amount_cents: Optional[int]
-    amount_currency: Optional[str]
-    expiration: Optional[str]
-    expiration_at: Optional[str]
-    percentage_rate: Optional[float]
-    coupon_type: Optional[str]
-    reusable: Optional[bool]
-    frequency: Optional[str]
-    frequency_duration: Optional[int]
-    applies_to: Optional[LimitationConfiguration]
+    recurring: Optional[bool]
+    aggregation_type: Optional[str]
+    weighted_interval: Optional[str]
+    field_name: Optional[str]
+    group: Optional[BillableMetricGroup]
+    filters: Optional[BillableMetricFilters]
 
 
-class CouponResponse(BaseResponseModel):
+class BillableMetricResponse(BaseResponseModel):
     lago_id: str
     name: str
     code: str
     description: Optional[str]
-    amount_cents: Optional[int]
-    amount_currency: Optional[str]
+    recurring: Optional[bool]
+    aggregation_type: Optional[str]
+    weighted_interval: Optional[str]
+    field_name: Optional[str]
     created_at: str
-    expiration: str
-    expiration_at: Optional[str]
-    terminated_at: Optional[str]
-    percentage_rate: Optional[float]
-    coupon_type: Optional[str]
-    reusable: Optional[bool]
-    frequency: Optional[str]
-    frequency_duration: Optional[int]
-    plan_codes: Optional[List[Any]]
-    limited_plans: Optional[bool]
-    billable_metric_codes: Optional[List[Any]]
-    limited_billable_metrics: Optional[bool]
+    group: BillableMetricGroup
+    filters: BillableMetricFilters
+    active_subscriptions_count: int
+    draft_invoices_count: int
+    plans_count: int
```

### Comparing `lago-python-client-1.1.0/lago_python_client/models/credit.py` & `lago-python-client-1.2.0/lago_python_client/models/credit.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/credit_note.py` & `lago-python-client-1.2.0/lago_python_client/models/credit_note.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/customer.py` & `lago-python-client-1.2.0/lago_python_client/models/customer.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/customer_usage.py` & `lago-python-client-1.2.0/lago_python_client/models/customer_usage.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,34 +14,45 @@
 class Group(BaseModel):
     lago_id: str
     key: Optional[str]
     value: str
     units: str
     amount_cents: int
 
+
+class ChargeFilterUsage(BaseModel):
+    invoice_display_name: Optional[str]
+    values: Dict[str, List[str]]
+    units: str
+    amount_cents: int
+    events_count: int
+
+
 class ChargeObject(BaseModel):
     lago_id: str
     charge_model: str
     invoice_display_name: Optional[str]
 
 class GroupedUsage(BaseModel):
     amount_cents: int
     events_count: int
     units: float
     grouped_by: Dict[str, str]
     groups: List[Group]
+    filters: List[ChargeFilterUsage]
 
 class ChargeUsage(BaseModel):
     units: float
     events_count: int
     amount_cents: int
     amount_currency: str
     charge: ChargeObject
     billable_metric: Metric
     groups: List[Group]
+    filters: List[ChargeFilterUsage]
     grouped_usage: Optional[List[GroupedUsage]]
 
 
 class CustomerUsageResponse(BaseResponseModel):
     from_datetime: str
     to_datetime: str
     issuing_date: str
```

### Comparing `lago-python-client-1.1.0/lago_python_client/models/event.py` & `lago-python-client-1.2.0/lago_python_client/models/event.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/fee.py` & `lago-python-client-1.2.0/lago_python_client/models/fee.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 class FeeAppliedTaxes(BaseResponseModel):
     __root__: List[FeeAppliedTax]
 
 
 class FeeResponse(BaseResponseModel):
     lago_id: Optional[str]
     lago_group_id: Optional[str]
+    lago_charge_filter_id: Optional[str]
     lago_invoice_id: Optional[str]
     lago_true_up_fee_id: Optional[str]
     lago_true_up_parent_fee_id: Optional[str]
     external_subscription_id: Optional[str]
     amount_cents: Optional[int]
     amount_currency: Optional[str]
     taxes_amount_cents: Optional[int]
```

### Comparing `lago-python-client-1.1.0/lago_python_client/models/invoice.py` & `lago-python-client-1.2.0/lago_python_client/models/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,18 @@
 
 class InvoiceAppliedTaxes(BaseResponseModel):
     __root__: List[InvoiceAppliedTax]
 
 
 class InvoiceResponse(BaseResponseModel):
     lago_id: str
-    sequential_id: int
+    sequential_id: Optional[int]
     number: str
     issuing_date: Optional[str]
+    payment_dispute_lost_at: Optional[str]
     payment_due_date: Optional[str]
     net_payment_term: int
     invoice_type: str
     version_number: int
     status: str
     payment_status: str
     currency: str
```

### Comparing `lago-python-client-1.1.0/lago_python_client/models/minimum_commitment.py` & `lago-python-client-1.2.0/lago_python_client/models/minimum_commitment.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/organization.py` & `lago-python-client-1.2.0/lago_python_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/plan.py` & `lago-python-client-1.2.0/lago_python_client/models/plan.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/subscription.py` & `lago-python-client-1.2.0/lago_python_client/models/subscription.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/tax.py` & `lago-python-client-1.2.0/lago_python_client/models/tax.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/models/wallet.py` & `lago-python-client-1.2.0/lago_python_client/models/wallet.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/mrrs/clients.py` & `lago-python-client-1.2.0/lago_python_client/mrrs/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/plans/clients.py` & `lago-python-client-1.2.0/lago_python_client/plans/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/services/json.py` & `lago-python-client-1.2.0/lago_python_client/services/json.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/services/request.py` & `lago-python-client-1.2.0/lago_python_client/services/request.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/services/response.py` & `lago-python-client-1.2.0/lago_python_client/services/response.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/subscriptions/clients.py` & `lago-python-client-1.2.0/lago_python_client/subscriptions/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/taxes/clients.py` & `lago-python-client-1.2.0/lago_python_client/taxes/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/wallets/clients.py` & `lago-python-client-1.2.0/lago_python_client/wallets/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/webhook_endpoints/clients.py` & `lago-python-client-1.2.0/lago_python_client/webhook_endpoints/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client/webhooks/clients.py` & `lago-python-client-1.2.0/lago_python_client/webhooks/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/lago_python_client.egg-info/PKG-INFO` & `lago-python-client-1.2.0/lago_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lago-python-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: Lago Python API Client
 Home-page: https://github.com/getlago/lago-python-client
 Author: Lovro Colic
 Author-email: lovro@getlago.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lago-python-client-1.1.0/lago_python_client.egg-info/SOURCES.txt` & `lago-python-client-1.2.0/lago_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/setup.cfg` & `lago-python-client-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_add_on_client.py` & `lago-python-client-1.2.0/tests/test_add_on_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_applied_coupon_client.py` & `lago-python-client-1.2.0/tests/test_applied_coupon_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_billable_metric_client.py` & `lago-python-client-1.2.0/tests/test_billable_metric_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_coupon_client.py` & `lago-python-client-1.2.0/tests/test_coupon_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_credit_note_client.py` & `lago-python-client-1.2.0/tests/test_credit_note_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_customer_client.py` & `lago-python-client-1.2.0/tests/test_customer_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_event_client.py` & `lago-python-client-1.2.0/tests/test_event_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_fee_client.py` & `lago-python-client-1.2.0/tests/test_fee_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_functools_ext.py` & `lago-python-client-1.2.0/tests/test_functools_ext.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_gross_revenue_client.py` & `lago-python-client-1.2.0/tests/test_gross_revenue_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_group_client.py` & `lago-python-client-1.2.0/tests/test_group_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_invoice_client.py` & `lago-python-client-1.2.0/tests/test_invoice_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,23 @@
 
     httpx_mock.add_response(method='PUT', url='https://api.getlago.com/api/v1/invoices/5eb02857-a71e-4ea2-bcf9-57d3a41bc6ba/refresh', content=mock_response())
     response = client.invoices.refresh('5eb02857-a71e-4ea2-bcf9-57d3a41bc6ba')
 
     assert response.lago_id == '5eb02857-a71e-4ea2-bcf9-57d3a41bc6ba'
 
 
+def test_valid_lose_dispute_invoice_request(httpx_mock: HTTPXMock):
+    client = Client(api_key='886fe239-927d-4072-ab72-6dd345e8dd0d')
+
+    httpx_mock.add_response(method='PUT', url='https://api.getlago.com/api/v1/invoices/5eb02857-a71e-4ea2-bcf9-57d3a41bc6ba/lose_dispute', content=mock_response())
+    response = client.invoices.lose_dispute('5eb02857-a71e-4ea2-bcf9-57d3a41bc6ba')
+
+    assert response.lago_id == '5eb02857-a71e-4ea2-bcf9-57d3a41bc6ba'
+
+
 def test_valid_finalize_invoice_request(httpx_mock: HTTPXMock):
     client = Client(api_key='886fe239-927d-4072-ab72-6dd345e8dd0d')
 
     httpx_mock.add_response(method='PUT', url='https://api.getlago.com/api/v1/invoices/5eb02857-a71e-4ea2-bcf9-57d3a41bc6ba/finalize', content=mock_response())
     response = client.invoices.finalize('5eb02857-a71e-4ea2-bcf9-57d3a41bc6ba')
 
     assert response.lago_id == '5eb02857-a71e-4ea2-bcf9-57d3a41bc6ba'
```

### Comparing `lago-python-client-1.1.0/tests/test_invoice_collection_client.py` & `lago-python-client-1.2.0/tests/test_invoice_collection_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_invoiced_usage_client.py` & `lago-python-client-1.2.0/tests/test_invoiced_usage_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_json_services.py` & `lago-python-client-1.2.0/tests/test_json_services.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_mrr_client.py` & `lago-python-client-1.2.0/tests/test_mrr_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_organization_client.py` & `lago-python-client-1.2.0/tests/test_organization_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_plan_client.py` & `lago-python-client-1.2.0/tests/test_plan_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_request_services.py` & `lago-python-client-1.2.0/tests/test_request_services.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_response_services.py` & `lago-python-client-1.2.0/tests/test_response_services.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_subscription_client.py` & `lago-python-client-1.2.0/tests/test_subscription_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_tax_client.py` & `lago-python-client-1.2.0/tests/test_tax_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_wallet_client.py` & `lago-python-client-1.2.0/tests/test_wallet_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_wallet_transaction_client.py` & `lago-python-client-1.2.0/tests/test_wallet_transaction_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_webhook_client.py` & `lago-python-client-1.2.0/tests/test_webhook_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.1.0/tests/test_webhook_endpoint_client.py` & `lago-python-client-1.2.0/tests/test_webhook_endpoint_client.py`

 * *Files identical despite different names*

