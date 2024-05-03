# Comparing `tmp/orb_billing-1.47.1.tar.gz` & `tmp/orb_billing-1.48.0.tar.gz`

## Comparing `orb_billing-1.47.1.tar` & `orb_billing-1.48.0.tar`

### file list

```diff
@@ -1,174 +1,178 @@
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/__init__.py
--rw-r--r--   0        0        0    63372 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_base_client.py
--rw-r--r--   0        0        0    26172 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_compat.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_constants.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_files.py
--rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_legacy_response.py
--rw-r--r--   0        0        0    22361 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_qs.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_resource.py
--rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_response.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_streaming.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_types.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_version.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/py.typed
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_utils/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/lib/.keep
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/__init__.py
--rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/credit_notes.py
--rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/invoice_line_items.py
--rw-r--r--   0        0        0    39490 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/invoices.py
--rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/items.py
--rw-r--r--   0        0        0    16042 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/metrics.py
--rw-r--r--   0        0        0   154789 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/subscriptions.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/top_level.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/beta/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/beta/beta.py
--rw-r--r--   0        0        0    10750 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/beta/price.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/coupons/__init__.py
--rw-r--r--   0        0        0    20868 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/coupons/coupons.py
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/coupons/subscriptions.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/customers/__init__.py
--rw-r--r--   0        0        0    16064 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/customers/balance_transactions.py
--rw-r--r--   0        0        0    44875 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/customers/costs.py
--rw-r--r--   0        0        0   139777 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/customers/customers.py
--rw-r--r--   0        0        0    31811 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/customers/usage.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/customers/credits/__init__.py
--rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/customers/credits/credits.py
--rw-r--r--   0        0        0   203967 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/customers/credits/ledger.py
--rw-r--r--   0        0        0    34840 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/customers/credits/top_ups.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/events/__init__.py
--rw-r--r--   0        0        0    27733 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/events/backfills.py
--rw-r--r--   0        0        0    52838 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/events/events.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/plans/__init__.py
--rw-r--r--   0        0        0    13314 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/plans/external_plan_id.py
--rw-r--r--   0        0        0    25426 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/plans/plans.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/prices/__init__.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/prices/external_price_id.py
--rw-r--r--   0        0        0   113510 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/resources/prices/prices.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/__init__.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/coupon.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/coupon_create_params.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/coupon_list_params.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/credit_note.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/credit_note_list_params.py
--rw-r--r--   0        0        0    17584 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customer.py
--rw-r--r--   0        0        0    18502 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customer_create_params.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customer_list_params.py
--rw-r--r--   0        0        0    18262 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customer_update_by_external_id_params.py
--rw-r--r--   0        0        0    18238 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customer_update_params.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/event_deprecate_response.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/event_ingest_params.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/event_ingest_response.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/event_search_params.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/event_search_response.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/event_update_params.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/event_update_response.py
--rw-r--r--   0        0        0    34357 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/invoice.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/invoice_create_params.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/invoice_fetch_upcoming_params.py
--rw-r--r--   0        0        0    34398 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/invoice_fetch_upcoming_response.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/invoice_line_item_create_params.py
--rw-r--r--   0        0        0    11483 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/invoice_line_item_create_response.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/invoice_list_params.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/invoice_mark_paid_params.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/item.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/item_create_params.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/item_list_params.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/metric_create_params.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/metric_create_response.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/metric_fetch_response.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/metric_list_params.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/metric_list_response.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/plan.py
--rw-r--r--   0        0        0    20940 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/plan_create_params.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/plan_list_params.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/plan_update_params.py
--rw-r--r--   0        0        0    28661 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/price.py
--rw-r--r--   0        0        0    25056 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/price_create_params.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/price_list_params.py
--rw-r--r--   0        0        0    16838 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_cancel_params.py
--rw-r--r--   0        0        0    27674 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_create_params.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_fetch_costs_params.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_fetch_costs_response.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_fetch_schedule_params.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_fetch_schedule_response.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_fetch_usage_params.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_list_params.py
--rw-r--r--   0        0        0    30636 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_price_intervals_params.py
--rw-r--r--   0        0        0    28080 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_schedule_plan_change_params.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_trigger_phase_params.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_update_fixed_fee_quantity_params.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscription_usage.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/subscriptions.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/top_level_ping_response.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/beta/__init__.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/beta/evaluate_price_group.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/beta/price_evaluate_params.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/beta/price_evaluate_response.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/coupons/__init__.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/coupons/subscription_list_params.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/balance_transaction_create_params.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/balance_transaction_create_response.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/balance_transaction_list_params.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/balance_transaction_list_response.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/cost_list_by_external_id_params.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/cost_list_by_external_id_response.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/cost_list_params.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/cost_list_response.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credit_list_by_external_id_params.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credit_list_by_external_id_response.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credit_list_params.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credit_list_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/usage_update_by_external_id_params.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/usage_update_by_external_id_response.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/usage_update_params.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/usage_update_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/__init__.py
--rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
--rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
--rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/ledger_create_entry_params.py
--rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/ledger_create_entry_response.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/ledger_list_params.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/ledger_list_response.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/top_up_create_params.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/top_up_create_response.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/top_up_list_params.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/customers/credits/top_up_list_response.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/events/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/events/backfill_close_response.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/events/backfill_create_params.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/events/backfill_create_response.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/events/backfill_fetch_response.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/events/backfill_list_params.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/events/backfill_list_response.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/events/backfill_revert_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/plans/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/plans/external_plan_id_update_params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/prices/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/shared/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 orb_billing-1.47.1/src/orb/types/shared/discount.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 orb_billing-1.47.1/.gitignore
--rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.47.1/LICENSE
--rw-r--r--   0        0        0    12858 2020-02-02 00:00:00.000000 orb_billing-1.47.1/README.md
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 orb_billing-1.47.1/pyproject.toml
--rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 orb_billing-1.47.1/PKG-INFO
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/__init__.py
+-rw-r--r--   0        0        0    65289 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_base_client.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_constants.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_files.py
+-rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_legacy_response.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_qs.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_resource.py
+-rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_response.py
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_streaming.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_types.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_version.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/lib/.keep
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/__init__.py
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/credit_notes.py
+-rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/invoice_line_items.py
+-rw-r--r--   0        0        0    39562 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/invoices.py
+-rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/items.py
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/metrics.py
+-rw-r--r--   0        0        0   163148 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/subscriptions.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/top_level.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/webhooks.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/coupons/__init__.py
+-rw-r--r--   0        0        0    20895 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/coupons/coupons.py
+-rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/coupons/subscriptions.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/__init__.py
+-rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/balance_transactions.py
+-rw-r--r--   0        0        0    44927 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/costs.py
+-rw-r--r--   0        0        0   139802 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/customers.py
+-rw-r--r--   0        0        0    31859 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/usage.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/credits/__init__.py
+-rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/credits/credits.py
+-rw-r--r--   0        0        0   204046 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/credits/ledger.py
+-rw-r--r--   0        0        0    34978 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/credits/top_ups.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/events/__init__.py
+-rw-r--r--   0        0        0    27956 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/events/backfills.py
+-rw-r--r--   0        0        0    52976 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/events/events.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/plans/__init__.py
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/plans/external_plan_id.py
+-rw-r--r--   0        0        0    25451 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/plans/plans.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/prices/__init__.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/prices/external_price_id.py
+-rw-r--r--   0        0        0   134801 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/prices/prices.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/__init__.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupon.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupon_create_params.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupon_list_params.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/credit_note.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/credit_note_list_params.py
+-rw-r--r--   0        0        0    17584 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer.py
+-rw-r--r--   0        0        0    18502 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer_create_params.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer_list_params.py
+-rw-r--r--   0        0        0    18262 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer_update_by_external_id_params.py
+-rw-r--r--   0        0        0    18238 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer_update_params.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/evaluate_price_group.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_deprecate_response.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_ingest_params.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_ingest_response.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_search_params.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_search_response.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_update_params.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_update_response.py
+-rw-r--r--   0        0        0    34433 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_create_params.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_fetch_upcoming_params.py
+-rw-r--r--   0        0        0    34474 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_fetch_upcoming_response.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_line_item_create_params.py
+-rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_line_item_create_response.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_list_params.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_mark_paid_params.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/item.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/item_create_params.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/item_list_params.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_create_params.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_create_response.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_fetch_response.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_list_params.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_list_response.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plan.py
+-rw-r--r--   0        0        0    24502 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plan_create_params.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plan_list_params.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plan_update_params.py
+-rw-r--r--   0        0        0    36435 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price.py
+-rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price_create_params.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price_evaluate_params.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price_evaluate_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price_list_params.py
+-rw-r--r--   0        0        0    16838 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_cancel_params.py
+-rw-r--r--   0        0        0    31028 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_create_params.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_costs_params.py
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_costs_response.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_schedule_params.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_schedule_response.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_usage_params.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_list_params.py
+-rw-r--r--   0        0        0    33927 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_price_intervals_params.py
+-rw-r--r--   0        0        0    31434 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_schedule_plan_change_params.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_trigger_phase_params.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_update_params.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_usage.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscriptions.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/top_level_ping_response.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/beta/evaluate_price_group.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/beta/price_evaluate_params.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/beta/price_evaluate_response.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupons/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupons/subscription_list_params.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/balance_transaction_create_params.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/balance_transaction_create_response.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/balance_transaction_list_params.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/balance_transaction_list_response.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/cost_list_by_external_id_params.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/cost_list_by_external_id_response.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/cost_list_params.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/cost_list_response.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credit_list_by_external_id_params.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credit_list_by_external_id_response.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credit_list_params.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credit_list_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/usage_update_by_external_id_params.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/usage_update_by_external_id_response.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/usage_update_params.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/usage_update_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/__init__.py
+-rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
+-rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_params.py
+-rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_response.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_params.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_response.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_params.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_response.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_params.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_response.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_close_response.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_create_params.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_create_response.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_fetch_response.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_list_params.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_list_response.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_revert_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plans/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plans/external_plan_id_update_params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/prices/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared/discount.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared/pagination_metadata.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared_params/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 orb_billing-1.48.0/.gitignore
+-rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.48.0/LICENSE
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 orb_billing-1.48.0/pyproject.toml
+-rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 orb_billing-1.48.0/PKG-INFO
```

### Comparing `orb_billing-1.47.1/src/orb/__init__.py` & `orb_billing-1.48.0/src/orb/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from . import types
 from ._types import NOT_GIVEN, NoneType, NotGiven, Transport, ProxiesTypes
 from ._utils import file_from_path
 from ._client import Orb, Client, Stream, Timeout, AsyncOrb, Transport, AsyncClient, AsyncStream, RequestOptions
 from ._models import BaseModel
 from ._version import __title__, __version__
 from ._response import APIResponse as APIResponse, AsyncAPIResponse as AsyncAPIResponse
+from ._constants import DEFAULT_TIMEOUT, DEFAULT_MAX_RETRIES, DEFAULT_CONNECTION_LIMITS
 from ._exceptions import (
     APIError,
     OrbError,
     URLNotFound,
     ConflictError,
     NotFoundError,
     APIStatusError,
@@ -31,14 +32,15 @@
     OrbAuthenticationError,
     OrbInternalServerError,
     RequestValidationError,
     UnprocessableEntityError,
     DuplicateResourceCreation,
     APIResponseValidationError,
 )
+from ._base_client import DefaultHttpxClient, DefaultAsyncHttpxClient
 from ._utils._logs import setup_logging as _setup_logging
 
 __all__ = [
     "types",
     "__version__",
     "__title__",
     "NoneType",
@@ -78,14 +80,19 @@
     "AsyncClient",
     "Stream",
     "AsyncStream",
     "Orb",
     "AsyncOrb",
     "file_from_path",
     "BaseModel",
+    "DEFAULT_TIMEOUT",
+    "DEFAULT_MAX_RETRIES",
+    "DEFAULT_CONNECTION_LIMITS",
+    "DefaultHttpxClient",
+    "DefaultAsyncHttpxClient",
 ]
 
 _setup_logging()
 
 # Update the __module__ attribute for exported symbols so that
 # error messages point to this module instead of the module
 # it was originally defined in, e.g.
```

### Comparing `orb_billing-1.47.1/src/orb/_base_client.py` & `orb_billing-1.48.0/src/orb/_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     Iterator,
     Optional,
     Generator,
     AsyncIterator,
     cast,
     overload,
 )
-from functools import lru_cache
 from typing_extensions import Literal, override, get_origin
 
 import anyio
 import httpx
 import distro
 import pydantic
 from httpx import URL, Limits
@@ -57,31 +56,31 @@
     ProxiesTypes,
     RequestFiles,
     HttpxSendArgs,
     AsyncTransport,
     RequestOptions,
     ModelBuilderProtocol,
 )
-from ._utils import is_dict, is_list, is_given, is_mapping
+from ._utils import is_dict, is_list, is_given, lru_cache, is_mapping
 from ._compat import model_copy, model_dump
 from ._models import GenericModel, FinalRequestOptions, validate_type, construct_type
 from ._response import (
     APIResponse,
     BaseAPIResponse,
     AsyncAPIResponse,
     extract_response_type,
 )
 from ._constants import (
-    DEFAULT_LIMITS,
     DEFAULT_TIMEOUT,
     MAX_RETRY_DELAY,
     DEFAULT_MAX_RETRIES,
     INITIAL_RETRY_DELAY,
     RAW_RESPONSE_HEADER,
     OVERRIDE_CAST_TO_HEADER,
+    DEFAULT_CONNECTION_LIMITS,
 )
 from ._streaming import Stream, SSEDecoder, AsyncStream, SSEBytesDecoder
 from ._exceptions import (
     APIStatusError,
     APITimeoutError,
     APIConnectionError,
     APIResponseValidationError,
@@ -357,14 +356,19 @@
         self._proxies = proxies
         self._transport = transport
         self._custom_headers = custom_headers or {}
         self._custom_query = custom_query or {}
         self._strict_response_validation = _strict_response_validation
         self._idempotency_header = None
 
+        if max_retries is None:  # pyright: ignore[reportUnnecessaryComparison]
+            raise TypeError(
+                "max_retries cannot be None. If you want to disable retries, pass `0`; if you want unlimited retries, pass `math.inf` or a very high number; if you want the default behavior, pass `orb-billing.DEFAULT_MAX_RETRIES`"
+            )
+
     def _enforce_trailing_slash(self, url: URL) -> URL:
         if url.raw_path.endswith(b"/"):
             return url
         return url.copy_with(raw_path=url.raw_path + b"/")
 
     def _make_status_error_from_response(
         self,
@@ -707,15 +711,35 @@
         log.debug("Not retrying")
         return False
 
     def _idempotency_key(self) -> str:
         return f"stainless-python-retry-{uuid.uuid4()}"
 
 
-class SyncHttpxClientWrapper(httpx.Client):
+class _DefaultHttpxClient(httpx.Client):
+    def __init__(self, **kwargs: Any) -> None:
+        kwargs.setdefault("timeout", DEFAULT_TIMEOUT)
+        kwargs.setdefault("limits", DEFAULT_CONNECTION_LIMITS)
+        kwargs.setdefault("follow_redirects", True)
+        super().__init__(**kwargs)
+
+
+if TYPE_CHECKING:
+    DefaultHttpxClient = httpx.Client
+    """An alias to `httpx.Client` that provides the same defaults that this SDK
+    uses internally.
+
+    This is useful because overriding the `http_client` with your own instance of
+    `httpx.Client` will result in httpx's defaults being used, not ours.
+    """
+else:
+    DefaultHttpxClient = _DefaultHttpxClient
+
+
+class SyncHttpxClientWrapper(DefaultHttpxClient):
     def __del__(self) -> None:
         try:
             self.close()
         except Exception:
             pass
 
 
@@ -743,15 +767,15 @@
                 "The `connection_pool_limits` argument is deprecated. The `http_client` argument should be passed instead",
                 category=DeprecationWarning,
                 stacklevel=3,
             )
             if http_client is not None:
                 raise ValueError("The `http_client` argument is mutually exclusive with `connection_pool_limits`")
         else:
-            limits = DEFAULT_LIMITS
+            limits = DEFAULT_CONNECTION_LIMITS
 
         if transport is not None:
             warnings.warn(
                 "The `transport` argument is deprecated. The `http_client` argument should be passed instead",
                 category=DeprecationWarning,
                 stacklevel=3,
             )
@@ -918,14 +942,16 @@
         request = self._build_request(options)
         self._prepare_request(request)
 
         kwargs: HttpxSendArgs = {}
         if self.custom_auth is not None:
             kwargs["auth"] = self.custom_auth
 
+        log.debug("Sending HTTP Request: %s %s", request.method, request.url)
+
         try:
             response = self._client.send(
                 request,
                 stream=stream or self._should_stream_response_body(request=request),
                 **kwargs,
             )
         except httpx.TimeoutException as err:
@@ -956,15 +982,20 @@
                     response_headers=None,
                 )
 
             log.debug("Raising connection error")
             raise APIConnectionError(request=request) from err
 
         log.debug(
-            'HTTP Request: %s %s "%i %s"', request.method, request.url, response.status_code, response.reason_phrase
+            'HTTP Response: %s %s "%i %s" %s',
+            request.method,
+            request.url,
+            response.status_code,
+            response.reason_phrase,
+            response.headers,
         )
 
         try:
             response.raise_for_status()
         except httpx.HTTPStatusError as err:  # thrown on 4xx and 5xx status code
             log.debug("Encountered httpx.HTTPStatusError", exc_info=True)
 
@@ -1253,15 +1284,35 @@
         options: RequestOptions = {},
         method: str = "get",
     ) -> SyncPageT:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
 
 
-class AsyncHttpxClientWrapper(httpx.AsyncClient):
+class _DefaultAsyncHttpxClient(httpx.AsyncClient):
+    def __init__(self, **kwargs: Any) -> None:
+        kwargs.setdefault("timeout", DEFAULT_TIMEOUT)
+        kwargs.setdefault("limits", DEFAULT_CONNECTION_LIMITS)
+        kwargs.setdefault("follow_redirects", True)
+        super().__init__(**kwargs)
+
+
+if TYPE_CHECKING:
+    DefaultAsyncHttpxClient = httpx.AsyncClient
+    """An alias to `httpx.AsyncClient` that provides the same defaults that this SDK
+    uses internally.
+
+    This is useful because overriding the `http_client` with your own instance of
+    `httpx.AsyncClient` will result in httpx's defaults being used, not ours.
+    """
+else:
+    DefaultAsyncHttpxClient = _DefaultAsyncHttpxClient
+
+
+class AsyncHttpxClientWrapper(DefaultAsyncHttpxClient):
     def __del__(self) -> None:
         try:
             # TODO(someday): support non asyncio runtimes here
             asyncio.get_running_loop().create_task(self.aclose())
         except Exception:
             pass
 
@@ -1290,15 +1341,15 @@
                 "The `connection_pool_limits` argument is deprecated. The `http_client` argument should be passed instead",
                 category=DeprecationWarning,
                 stacklevel=3,
             )
             if http_client is not None:
                 raise ValueError("The `http_client` argument is mutually exclusive with `connection_pool_limits`")
         else:
-            limits = DEFAULT_LIMITS
+            limits = DEFAULT_CONNECTION_LIMITS
 
         if transport is not None:
             warnings.warn(
                 "The `transport` argument is deprecated. The `http_client` argument should be passed instead",
                 category=DeprecationWarning,
                 stacklevel=3,
             )
```

### Comparing `orb_billing-1.47.1/src/orb/_client.py` & `orb_billing-1.48.0/src/orb/_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,54 +55,64 @@
     invoice_line_items: resources.InvoiceLineItems
     invoices: resources.Invoices
     items: resources.Items
     metrics: resources.Metrics
     plans: resources.Plans
     prices: resources.Prices
     subscriptions: resources.Subscriptions
-    beta: resources.Beta
+    webhooks: resources.Webhooks
     with_raw_response: OrbWithRawResponse
     with_streaming_response: OrbWithStreamedResponse
 
     # client options
     api_key: str
+    webhook_secret: str | None
 
     def __init__(
         self,
         *,
         api_key: str | None = None,
+        webhook_secret: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
-        # Configure a custom httpx client. See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
+        # Configure a custom httpx client.
+        # We provide a `DefaultHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
+        # See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
         http_client: httpx.Client | None = None,
         # Enable or disable schema validation for data returned by the API.
         # When enabled an error APIResponseValidationError is raised
         # if the API responds with invalid data for the expected schema.
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous orb client instance.
 
-        This automatically infers the `api_key` argument from the `ORB_API_KEY` environment variable if it is not provided.
+        This automatically infers the following arguments from their corresponding environment variables if they are not provided:
+        - `api_key` from `ORB_API_KEY`
+        - `webhook_secret` from `ORB_WEBHOOK_SECRET`
         """
         if api_key is None:
             api_key = os.environ.get("ORB_API_KEY")
         if api_key is None:
             raise OrbError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the ORB_API_KEY environment variable"
             )
         self.api_key = api_key
 
+        if webhook_secret is None:
+            webhook_secret = os.environ.get("ORB_WEBHOOK_SECRET")
+        self.webhook_secret = webhook_secret
+
         if base_url is None:
             base_url = os.environ.get("ORB_BASE_URL")
         if base_url is None:
             base_url = f"https://api.withorb.com/v1"
 
         super().__init__(
             version=__version__,
@@ -125,16 +135,15 @@
         self.invoice_line_items = resources.InvoiceLineItems(self)
         self.invoices = resources.Invoices(self)
         self.items = resources.Items(self)
         self.metrics = resources.Metrics(self)
         self.plans = resources.Plans(self)
         self.prices = resources.Prices(self)
         self.subscriptions = resources.Subscriptions(self)
-        self.beta = resources.Beta(self)
-        self.with_raw_response = OrbWithRawResponse(self)
+        self.webhooks = resources.Webhooks(self)
         self.with_streaming_response = OrbWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="brackets")
 
@@ -153,14 +162,15 @@
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
         api_key: str | None = None,
+        webhook_secret: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.Client | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -187,14 +197,15 @@
             params = {**params, **default_query}
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
             api_key=api_key or self.api_key,
+            webhook_secret=webhook_secret or self.webhook_secret,
             base_url=base_url or self.base_url,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
@@ -295,54 +306,64 @@
     invoice_line_items: resources.AsyncInvoiceLineItems
     invoices: resources.AsyncInvoices
     items: resources.AsyncItems
     metrics: resources.AsyncMetrics
     plans: resources.AsyncPlans
     prices: resources.AsyncPrices
     subscriptions: resources.AsyncSubscriptions
-    beta: resources.AsyncBeta
+    webhooks: resources.AsyncWebhooks
     with_raw_response: AsyncOrbWithRawResponse
     with_streaming_response: AsyncOrbWithStreamedResponse
 
     # client options
     api_key: str
+    webhook_secret: str | None
 
     def __init__(
         self,
         *,
         api_key: str | None = None,
+        webhook_secret: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
-        # Configure a custom httpx client. See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
+        # Configure a custom httpx client.
+        # We provide a `DefaultAsyncHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
+        # See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
         http_client: httpx.AsyncClient | None = None,
         # Enable or disable schema validation for data returned by the API.
         # When enabled an error APIResponseValidationError is raised
         # if the API responds with invalid data for the expected schema.
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new async orb client instance.
 
-        This automatically infers the `api_key` argument from the `ORB_API_KEY` environment variable if it is not provided.
+        This automatically infers the following arguments from their corresponding environment variables if they are not provided:
+        - `api_key` from `ORB_API_KEY`
+        - `webhook_secret` from `ORB_WEBHOOK_SECRET`
         """
         if api_key is None:
             api_key = os.environ.get("ORB_API_KEY")
         if api_key is None:
             raise OrbError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the ORB_API_KEY environment variable"
             )
         self.api_key = api_key
 
+        if webhook_secret is None:
+            webhook_secret = os.environ.get("ORB_WEBHOOK_SECRET")
+        self.webhook_secret = webhook_secret
+
         if base_url is None:
             base_url = os.environ.get("ORB_BASE_URL")
         if base_url is None:
             base_url = f"https://api.withorb.com/v1"
 
         super().__init__(
             version=__version__,
@@ -365,15 +386,15 @@
         self.invoice_line_items = resources.AsyncInvoiceLineItems(self)
         self.invoices = resources.AsyncInvoices(self)
         self.items = resources.AsyncItems(self)
         self.metrics = resources.AsyncMetrics(self)
         self.plans = resources.AsyncPlans(self)
         self.prices = resources.AsyncPrices(self)
         self.subscriptions = resources.AsyncSubscriptions(self)
-        self.beta = resources.AsyncBeta(self)
+        self.webhooks = resources.AsyncWebhooks(self)
         self.with_raw_response = AsyncOrbWithRawResponse(self)
         self.with_streaming_response = AsyncOrbWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="brackets")
@@ -393,14 +414,15 @@
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
         api_key: str | None = None,
+        webhook_secret: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.AsyncClient | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -427,14 +449,15 @@
             params = {**params, **default_query}
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
             api_key=api_key or self.api_key,
+            webhook_secret=webhook_secret or self.webhook_secret,
             base_url=base_url or self.base_url,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
@@ -536,15 +559,14 @@
         self.invoice_line_items = resources.InvoiceLineItemsWithRawResponse(client.invoice_line_items)
         self.invoices = resources.InvoicesWithRawResponse(client.invoices)
         self.items = resources.ItemsWithRawResponse(client.items)
         self.metrics = resources.MetricsWithRawResponse(client.metrics)
         self.plans = resources.PlansWithRawResponse(client.plans)
         self.prices = resources.PricesWithRawResponse(client.prices)
         self.subscriptions = resources.SubscriptionsWithRawResponse(client.subscriptions)
-        self.beta = resources.BetaWithRawResponse(client.beta)
 
 
 class AsyncOrbWithRawResponse:
     def __init__(self, client: AsyncOrb) -> None:
         self.top_level = resources.AsyncTopLevelWithRawResponse(client.top_level)
         self.coupons = resources.AsyncCouponsWithRawResponse(client.coupons)
         self.credit_notes = resources.AsyncCreditNotesWithRawResponse(client.credit_notes)
@@ -553,15 +575,14 @@
         self.invoice_line_items = resources.AsyncInvoiceLineItemsWithRawResponse(client.invoice_line_items)
         self.invoices = resources.AsyncInvoicesWithRawResponse(client.invoices)
         self.items = resources.AsyncItemsWithRawResponse(client.items)
         self.metrics = resources.AsyncMetricsWithRawResponse(client.metrics)
         self.plans = resources.AsyncPlansWithRawResponse(client.plans)
         self.prices = resources.AsyncPricesWithRawResponse(client.prices)
         self.subscriptions = resources.AsyncSubscriptionsWithRawResponse(client.subscriptions)
-        self.beta = resources.AsyncBetaWithRawResponse(client.beta)
 
 
 class OrbWithStreamedResponse:
     def __init__(self, client: Orb) -> None:
         self.top_level = resources.TopLevelWithStreamingResponse(client.top_level)
         self.coupons = resources.CouponsWithStreamingResponse(client.coupons)
         self.credit_notes = resources.CreditNotesWithStreamingResponse(client.credit_notes)
@@ -570,15 +591,14 @@
         self.invoice_line_items = resources.InvoiceLineItemsWithStreamingResponse(client.invoice_line_items)
         self.invoices = resources.InvoicesWithStreamingResponse(client.invoices)
         self.items = resources.ItemsWithStreamingResponse(client.items)
         self.metrics = resources.MetricsWithStreamingResponse(client.metrics)
         self.plans = resources.PlansWithStreamingResponse(client.plans)
         self.prices = resources.PricesWithStreamingResponse(client.prices)
         self.subscriptions = resources.SubscriptionsWithStreamingResponse(client.subscriptions)
-        self.beta = resources.BetaWithStreamingResponse(client.beta)
 
 
 class AsyncOrbWithStreamedResponse:
     def __init__(self, client: AsyncOrb) -> None:
         self.top_level = resources.AsyncTopLevelWithStreamingResponse(client.top_level)
         self.coupons = resources.AsyncCouponsWithStreamingResponse(client.coupons)
         self.credit_notes = resources.AsyncCreditNotesWithStreamingResponse(client.credit_notes)
@@ -587,13 +607,12 @@
         self.invoice_line_items = resources.AsyncInvoiceLineItemsWithStreamingResponse(client.invoice_line_items)
         self.invoices = resources.AsyncInvoicesWithStreamingResponse(client.invoices)
         self.items = resources.AsyncItemsWithStreamingResponse(client.items)
         self.metrics = resources.AsyncMetricsWithStreamingResponse(client.metrics)
         self.plans = resources.AsyncPlansWithStreamingResponse(client.plans)
         self.prices = resources.AsyncPricesWithStreamingResponse(client.prices)
         self.subscriptions = resources.AsyncSubscriptionsWithStreamingResponse(client.subscriptions)
-        self.beta = resources.AsyncBetaWithStreamingResponse(client.beta)
 
 
 Client = Orb
 
 AsyncClient = AsyncOrb
```

### Comparing `orb_billing-1.47.1/src/orb/_compat.py` & `orb_billing-1.48.0/src/orb/_compat.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_exceptions.py` & `orb_billing-1.48.0/src/orb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_files.py` & `orb_billing-1.48.0/src/orb/_files.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_legacy_response.py` & `orb_billing-1.48.0/src/orb/_legacy_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_models.py` & `orb_billing-1.48.0/src/orb/_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
+import os
 import inspect
 from typing import TYPE_CHECKING, Any, Type, Union, Generic, TypeVar, Callable, cast
 from datetime import date, datetime
-from functools import lru_cache
 from typing_extensions import (
     Unpack,
     Literal,
     ClassVar,
     Protocol,
     Required,
     TypedDict,
@@ -32,16 +32,18 @@
     AnyMapping,
     HttpxRequestFiles,
 )
 from ._utils import (
     PropertyInfo,
     is_list,
     is_given,
+    lru_cache,
     is_mapping,
     parse_date,
+    coerce_boolean,
     parse_datetime,
     strip_not_given,
     extract_type_arg,
     is_annotated_type,
     strip_annotated_type,
 )
 from ._compat import (
@@ -70,26 +72,101 @@
 @runtime_checkable
 class _ConfigProtocol(Protocol):
     allow_population_by_field_name: bool
 
 
 class BaseModel(pydantic.BaseModel):
     if PYDANTIC_V2:
-        model_config: ClassVar[ConfigDict] = ConfigDict(extra="allow")
+        model_config: ClassVar[ConfigDict] = ConfigDict(
+            extra="allow", defer_build=coerce_boolean(os.environ.get("DEFER_PYDANTIC_BUILD", "true"))
+        )
     else:
 
         @property
         @override
         def model_fields_set(self) -> set[str]:
             # a forwards-compat shim for pydantic v2
             return self.__fields_set__  # type: ignore
 
         class Config(pydantic.BaseConfig):  # pyright: ignore[reportDeprecated]
             extra: Any = pydantic.Extra.allow  # type: ignore
 
+    def to_dict(
+        self,
+        *,
+        mode: Literal["json", "python"] = "python",
+        use_api_names: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        warnings: bool = True,
+    ) -> dict[str, object]:
+        """Recursively generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
+
+        By default, fields that were not set by the API will not be included,
+        and keys will match the API response, *not* the property names from the model.
+
+        For example, if the API responds with `"fooBar": true` but we've defined a `foo_bar: bool` property,
+        the output will use the `"fooBar"` key (unless `use_api_names=False` is passed).
+
+        Args:
+            mode:
+                If mode is 'json', the dictionary will only contain JSON serializable types. e.g. `datetime` will be turned into a string, `"2024-3-22T18:11:19.117000Z"`.
+                If mode is 'python', the dictionary may contain any Python objects. e.g. `datetime(2024, 3, 22)`
+
+            use_api_names: Whether to use the key that the API responded with or the property name. Defaults to `True`.
+            exclude_unset: Whether to exclude fields that have not been explicitly set.
+            exclude_defaults: Whether to exclude fields that are set to their default value from the output.
+            exclude_none: Whether to exclude fields that have a value of `None` from the output.
+            warnings: Whether to log warnings when invalid fields are encountered. This is only supported in Pydantic v2.
+        """
+        return self.model_dump(
+            mode=mode,
+            by_alias=use_api_names,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            warnings=warnings,
+        )
+
+    def to_json(
+        self,
+        *,
+        indent: int | None = 2,
+        use_api_names: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        warnings: bool = True,
+    ) -> str:
+        """Generates a JSON string representing this model as it would be received from or sent to the API (but with indentation).
+
+        By default, fields that were not set by the API will not be included,
+        and keys will match the API response, *not* the property names from the model.
+
+        For example, if the API responds with `"fooBar": true` but we've defined a `foo_bar: bool` property,
+        the output will use the `"fooBar"` key (unless `use_api_names=False` is passed).
+
+        Args:
+            indent: Indentation to use in the JSON output. If `None` is passed, the output will be compact. Defaults to `2`
+            use_api_names: Whether to use the key that the API responded with or the property name. Defaults to `True`.
+            exclude_unset: Whether to exclude fields that have not been explicitly set.
+            exclude_defaults: Whether to exclude fields that have the default value.
+            exclude_none: Whether to exclude fields that have a value of `None`.
+            warnings: Whether to show any warnings that occurred during serialization. This is only supported in Pydantic v2.
+        """
+        return self.model_dump_json(
+            indent=indent,
+            by_alias=use_api_names,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            warnings=warnings,
+        )
+
     @override
     def __str__(self) -> str:
         # mypy complains about an invalid self arg
         return f'{self.__repr_name__()}({self.__repr_str__(", ")})'  # type: ignore[misc]
 
     # Override the 'construct' method in a way that supports recursive parsing without validation.
     # Based on https://github.com/samuelcolvin/pydantic/issues/1168#issuecomment-817742836.
@@ -297,15 +374,15 @@
     """
     # we allow `object` as the input type because otherwise, passing things like
     # `Literal['value']` will be reported as a type error by type checkers
     type_ = cast("type[object]", type_)
 
     # unwrap `Annotated[T, ...]` -> `T`
     if is_annotated_type(type_):
-        meta = get_args(type_)[1:]
+        meta: tuple[Any, ...] = get_args(type_)[1:]
         type_ = extract_type_arg(type_, 0)
     else:
         meta = tuple()
 
     # we need to use the origin class for any types that are subscripted generics
     # e.g. Dict[str, object]
     origin = get_origin(type_) or type_
```

### Comparing `orb_billing-1.47.1/src/orb/_qs.py` & `orb_billing-1.48.0/src/orb/_qs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_resource.py` & `orb_billing-1.48.0/src/orb/_resource.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_response.py` & `orb_billing-1.48.0/src/orb/_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_streaming.py` & `orb_billing-1.48.0/src/orb/_streaming.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class Stream(Generic[_T]):
     """Provides the core interface to iterate over a synchronous stream response."""
 
     response: httpx.Response
 
-    _decoder: SSEDecoder | SSEBytesDecoder
+    _decoder: SSEBytesDecoder
 
     def __init__(
         self,
         *,
         cast_to: type[_T],
         response: httpx.Response,
         client: Orb,
@@ -42,18 +42,15 @@
         return self._iterator.__next__()
 
     def __iter__(self) -> Iterator[_T]:
         for item in self._iterator:
             yield item
 
     def _iter_events(self) -> Iterator[ServerSentEvent]:
-        if isinstance(self._decoder, SSEBytesDecoder):
-            yield from self._decoder.iter_bytes(self.response.iter_bytes())
-        else:
-            yield from self._decoder.iter(self.response.iter_lines())
+        yield from self._decoder.iter_bytes(self.response.iter_bytes())
 
     def __stream__(self) -> Iterator[_T]:
         cast_to = cast(Any, self._cast_to)
         response = self.response
         process_data = self._client._process_response_data
         iterator = self._iter_events()
 
@@ -108,20 +105,16 @@
         return await self._iterator.__anext__()
 
     async def __aiter__(self) -> AsyncIterator[_T]:
         async for item in self._iterator:
             yield item
 
     async def _iter_events(self) -> AsyncIterator[ServerSentEvent]:
-        if isinstance(self._decoder, SSEBytesDecoder):
-            async for sse in self._decoder.aiter_bytes(self.response.aiter_bytes()):
-                yield sse
-        else:
-            async for sse in self._decoder.aiter(self.response.aiter_lines()):
-                yield sse
+        async for sse in self._decoder.aiter_bytes(self.response.aiter_bytes()):
+            yield sse
 
     async def __stream__(self) -> AsyncIterator[_T]:
         cast_to = cast(Any, self._cast_to)
         response = self.response
         process_data = self._client._process_response_data
         iterator = self._iter_events()
 
@@ -201,29 +194,57 @@
 
     def __init__(self) -> None:
         self._event = None
         self._data = []
         self._last_event_id = None
         self._retry = None
 
-    def iter(self, iterator: Iterator[str]) -> Iterator[ServerSentEvent]:
-        """Given an iterator that yields lines, iterate over it & yield every event encountered"""
-        for line in iterator:
-            line = line.rstrip("\n")
-            sse = self.decode(line)
-            if sse is not None:
-                yield sse
-
-    async def aiter(self, iterator: AsyncIterator[str]) -> AsyncIterator[ServerSentEvent]:
-        """Given an async iterator that yields lines, iterate over it & yield every event encountered"""
-        async for line in iterator:
-            line = line.rstrip("\n")
-            sse = self.decode(line)
-            if sse is not None:
-                yield sse
+    def iter_bytes(self, iterator: Iterator[bytes]) -> Iterator[ServerSentEvent]:
+        """Given an iterator that yields raw binary data, iterate over it & yield every event encountered"""
+        for chunk in self._iter_chunks(iterator):
+            # Split before decoding so splitlines() only uses \r and \n
+            for raw_line in chunk.splitlines():
+                line = raw_line.decode("utf-8")
+                sse = self.decode(line)
+                if sse:
+                    yield sse
+
+    def _iter_chunks(self, iterator: Iterator[bytes]) -> Iterator[bytes]:
+        """Given an iterator that yields raw binary data, iterate over it and yield individual SSE chunks"""
+        data = b""
+        for chunk in iterator:
+            for line in chunk.splitlines(keepends=True):
+                data += line
+                if data.endswith((b"\r\r", b"\n\n", b"\r\n\r\n")):
+                    yield data
+                    data = b""
+        if data:
+            yield data
+
+    async def aiter_bytes(self, iterator: AsyncIterator[bytes]) -> AsyncIterator[ServerSentEvent]:
+        """Given an iterator that yields raw binary data, iterate over it & yield every event encountered"""
+        async for chunk in self._aiter_chunks(iterator):
+            # Split before decoding so splitlines() only uses \r and \n
+            for raw_line in chunk.splitlines():
+                line = raw_line.decode("utf-8")
+                sse = self.decode(line)
+                if sse:
+                    yield sse
+
+    async def _aiter_chunks(self, iterator: AsyncIterator[bytes]) -> AsyncIterator[bytes]:
+        """Given an iterator that yields raw binary data, iterate over it and yield individual SSE chunks"""
+        data = b""
+        async for chunk in iterator:
+            for line in chunk.splitlines(keepends=True):
+                data += line
+                if data.endswith((b"\r\r", b"\n\n", b"\r\n\r\n")):
+                    yield data
+                    data = b""
+        if data:
+            yield data
 
     def decode(self, line: str) -> ServerSentEvent | None:
         # See: https://html.spec.whatwg.org/multipage/server-sent-events.html#event-stream-interpretation  # noqa: E501
 
         if not line:
             if not self._event and not self._data and not self._last_event_id and self._retry is None:
                 return None
```

### Comparing `orb_billing-1.47.1/src/orb/_types.py` & `orb_billing-1.48.0/src/orb/_types.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/pagination.py` & `orb_billing-1.48.0/src/orb/pagination.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_utils/__init__.py` & `orb_billing-1.48.0/src/orb/_utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ._proxy import LazyProxy as LazyProxy
 from ._utils import (
     flatten as flatten,
     is_dict as is_dict,
     is_list as is_list,
     is_given as is_given,
     is_tuple as is_tuple,
+    lru_cache as lru_cache,
     is_mapping as is_mapping,
     is_tuple_t as is_tuple_t,
     parse_date as parse_date,
     is_iterable as is_iterable,
     is_sequence as is_sequence,
     coerce_float as coerce_float,
     is_mapping_t as is_mapping_t,
```

### Comparing `orb_billing-1.47.1/src/orb/_utils/_logs.py` & `orb_billing-1.48.0/src/orb/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_utils/_proxy.py` & `orb_billing-1.48.0/src/orb/_utils/_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 T = TypeVar("T")
 
 
 class LazyProxy(Generic[T], ABC):
     """Implements data methods to pretend that an instance is another instance.
 
-    This includes forwarding attribute access and othe methods.
+    This includes forwarding attribute access and other methods.
     """
 
     # Note: we have to special case proxies that themselves return proxies
     # to support using a proxy as a catch-all for any random access, e.g. `proxy.foo.bar.baz`
 
     def __getattr__(self, attr: str) -> object:
         proxied = self.__get_proxied__()
```

### Comparing `orb_billing-1.47.1/src/orb/_utils/_sync.py` & `orb_billing-1.48.0/src/orb/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_utils/_transform.py` & `orb_billing-1.48.0/src/orb/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_utils/_typing.py` & `orb_billing-1.48.0/src/orb/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/_utils/_utils.py` & `orb_billing-1.48.0/src/orb/_utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,16 @@
             else:  # no break
                 if len(variants) > 1:
                     variations = human_join(
                         ["(" + human_join([quote(arg) for arg in variant], final="and") + ")" for variant in variants]
                     )
                     msg = f"Missing required arguments; Expected either {variations} arguments to be given"
                 else:
+                    assert len(variants) > 0
+
                     # TODO: this error message is not deterministic
                     missing = list(set(variants[0]) - given_params)
                     if len(missing) > 1:
                         msg = f"Missing required arguments: {human_join([quote(arg) for arg in missing])}"
                     else:
                         msg = f"Missing required argument: {quote(missing[0])}"
                 raise TypeError(msg)
@@ -385,7 +387,17 @@
 
 
 def get_async_library() -> str:
     try:
         return sniffio.current_async_library()
     except Exception:
         return "false"
+
+
+def lru_cache(*, maxsize: int | None = 128) -> Callable[[CallableT], CallableT]:
+    """A version of functools.lru_cache that retains the type signature
+    for the wrapped function arguments.
+    """
+    wrapper = functools.lru_cache(  # noqa: TID251
+        maxsize=maxsize,
+    )
+    return cast(Any, wrapper)  # type: ignore[no-any-return]
```

### Comparing `orb_billing-1.47.1/src/orb/resources/__init__.py` & `orb_billing-1.48.0/src/orb/resources/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,9 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
-from .beta import (
-    Beta,
-    AsyncBeta,
-    BetaWithRawResponse,
-    AsyncBetaWithRawResponse,
-    BetaWithStreamingResponse,
-    AsyncBetaWithStreamingResponse,
-)
 from .items import (
     Items,
     AsyncItems,
     ItemsWithRawResponse,
     AsyncItemsWithRawResponse,
     ItemsWithStreamingResponse,
     AsyncItemsWithStreamingResponse,
@@ -60,14 +52,18 @@
     Invoices,
     AsyncInvoices,
     InvoicesWithRawResponse,
     AsyncInvoicesWithRawResponse,
     InvoicesWithStreamingResponse,
     AsyncInvoicesWithStreamingResponse,
 )
+from .webhooks import (
+    Webhooks,
+    AsyncWebhooks,
+)
 from .customers import (
     Customers,
     AsyncCustomers,
     CustomersWithRawResponse,
     AsyncCustomersWithRawResponse,
     CustomersWithStreamingResponse,
     AsyncCustomersWithStreamingResponse,
@@ -174,14 +170,10 @@
     "AsyncPricesWithStreamingResponse",
     "Subscriptions",
     "AsyncSubscriptions",
     "SubscriptionsWithRawResponse",
     "AsyncSubscriptionsWithRawResponse",
     "SubscriptionsWithStreamingResponse",
     "AsyncSubscriptionsWithStreamingResponse",
-    "Beta",
-    "AsyncBeta",
-    "BetaWithRawResponse",
-    "AsyncBetaWithRawResponse",
-    "BetaWithStreamingResponse",
-    "AsyncBetaWithStreamingResponse",
+    "Webhooks",
+    "AsyncWebhooks",
 ]
```

### Comparing `orb_billing-1.47.1/src/orb/resources/credit_notes.py` & `orb_billing-1.48.0/src/orb/resources/credit_notes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from __future__ import annotations
 
 from typing import Optional
 
 import httpx
 
 from .. import _legacy_response
-from ..types import CreditNote, credit_note_list_params
+from ..types import credit_note_list_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import (
     AsyncPaginator,
     make_request_options,
 )
+from ..types.credit_note import CreditNote
 
 __all__ = ["CreditNotes", "AsyncCreditNotes"]
 
 
 class CreditNotes(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> CreditNotesWithRawResponse:
```

### Comparing `orb_billing-1.47.1/src/orb/resources/invoice_line_items.py` & `orb_billing-1.48.0/src/orb/resources/invoice_line_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 
 from typing import Union
 from datetime import date
 
 import httpx
 
 from .. import _legacy_response
-from ..types import InvoiceLineItemCreateResponse, invoice_line_item_create_params
+from ..types import invoice_line_item_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from .._base_client import (
     make_request_options,
 )
+from ..types.invoice_line_item_create_response import InvoiceLineItemCreateResponse
 
 __all__ = ["InvoiceLineItems", "AsyncInvoiceLineItems"]
 
 
 class InvoiceLineItems(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> InvoiceLineItemsWithRawResponse:
```

### Comparing `orb_billing-1.47.1/src/orb/resources/invoices.py` & `orb_billing-1.48.0/src/orb/resources/invoices.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from datetime import date, datetime
 from typing_extensions import Literal
 
 import httpx
 
 from .. import _legacy_response
 from ..types import (
-    Invoice,
-    InvoiceFetchUpcomingResponse,
     invoice_list_params,
     invoice_create_params,
     invoice_mark_paid_params,
     invoice_fetch_upcoming_params,
 )
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
@@ -26,14 +24,16 @@
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import (
     AsyncPaginator,
     make_request_options,
 )
+from ..types.invoice import Invoice
+from ..types.invoice_fetch_upcoming_response import InvoiceFetchUpcomingResponse
 
 __all__ = ["Invoices", "AsyncInvoices"]
 
 
 class Invoices(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> InvoicesWithRawResponse:
@@ -303,15 +303,15 @@
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Invoice:
         """This endpoint allows an eligible invoice to be issued manually.
 
         This is only
-        possible with invoices where status is `draft`, `will_auto_issue` is true, and
+        possible with invoices where status is `draft`, `will_auto_issue` is false, and
         an `eligible_to_issue_at` is a time in the past. Issuing an invoice could
         possibly trigger side effects, some of which could be customer-visible (e.g.
         sending emails, auto-collecting payment, syncing the invoice to external
         providers, etc).
 
         Args:
           extra_headers: Send extra headers
@@ -714,15 +714,15 @@
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Invoice:
         """This endpoint allows an eligible invoice to be issued manually.
 
         This is only
-        possible with invoices where status is `draft`, `will_auto_issue` is true, and
+        possible with invoices where status is `draft`, `will_auto_issue` is false, and
         an `eligible_to_issue_at` is a time in the past. Issuing an invoice could
         possibly trigger side effects, some of which could be customer-visible (e.g.
         sending emails, auto-collecting payment, syncing the invoice to external
         providers, etc).
 
         Args:
           extra_headers: Send extra headers
```

### Comparing `orb_billing-1.47.1/src/orb/resources/items.py` & `orb_billing-1.48.0/src/orb/resources/items.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from __future__ import annotations
 
 from typing import Optional
 
 import httpx
 
 from .. import _legacy_response
-from ..types import Item, item_list_params, item_create_params
+from ..types import item_list_params, item_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..pagination import SyncPage, AsyncPage
+from ..types.item import Item
 from .._base_client import (
     AsyncPaginator,
     make_request_options,
 )
 
 __all__ = ["Items", "AsyncItems"]
```

### Comparing `orb_billing-1.47.1/src/orb/resources/metrics.py` & `orb_billing-1.48.0/src/orb/resources/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,34 +4,31 @@
 
 from typing import Dict, Union, Optional
 from datetime import datetime
 
 import httpx
 
 from .. import _legacy_response
-from ..types import (
-    MetricListResponse,
-    MetricFetchResponse,
-    MetricCreateResponse,
-    metric_list_params,
-    metric_create_params,
-)
+from ..types import metric_list_params, metric_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import (
     AsyncPaginator,
     make_request_options,
 )
+from ..types.metric_list_response import MetricListResponse
+from ..types.metric_fetch_response import MetricFetchResponse
+from ..types.metric_create_response import MetricCreateResponse
 
 __all__ = ["Metrics", "AsyncMetrics"]
 
 
 class Metrics(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> MetricsWithRawResponse:
```

### Comparing `orb_billing-1.47.1/src/orb/resources/subscriptions.py` & `orb_billing-1.48.0/src/orb/resources/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 from datetime import date, datetime
 from typing_extensions import Literal
 
 import httpx
 
 from .. import _legacy_response
 from ..types import (
-    Subscription,
-    SubscriptionUsage,
-    SubscriptionFetchCostsResponse,
-    SubscriptionFetchScheduleResponse,
     subscription_list_params,
     subscription_cancel_params,
     subscription_create_params,
+    subscription_update_params,
     subscription_fetch_costs_params,
     subscription_fetch_usage_params,
     subscription_trigger_phase_params,
     subscription_fetch_schedule_params,
     subscription_price_intervals_params,
     subscription_schedule_plan_change_params,
     subscription_update_fixed_fee_quantity_params,
@@ -35,14 +32,18 @@
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import (
     AsyncPaginator,
     make_request_options,
 )
+from ..types.subscription import Subscription
+from ..types.subscription_usage import SubscriptionUsage
+from ..types.subscription_fetch_costs_response import SubscriptionFetchCostsResponse
+from ..types.subscription_fetch_schedule_response import SubscriptionFetchScheduleResponse
 
 __all__ = ["Subscriptions", "AsyncSubscriptions"]
 
 
 class Subscriptions(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> SubscriptionsWithRawResponse:
@@ -532,14 +533,91 @@
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Subscription,
         )
 
+    def update(
+        self,
+        subscription_id: str,
+        *,
+        auto_collection: Optional[bool] | NotGiven = NOT_GIVEN,
+        default_invoice_memo: Optional[str] | NotGiven = NOT_GIVEN,
+        invoicing_threshold: Optional[str] | NotGiven = NOT_GIVEN,
+        metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
+        net_terms: Optional[int] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Subscription:
+        """
+        This endpoint can be used to update the `metadata`, `net terms`,
+        `auto_collection`, `invoicing_threshold`, and `default_invoice_memo` properties
+        on a subscription.
+
+        Args:
+          auto_collection: Determines whether issued invoices for this subscription will automatically be
+              charged with the saved payment method on the due date. This property defaults to
+              the plan's behavior.
+
+          default_invoice_memo: Determines the default memo on this subscription's invoices. Note that if this
+              is not provided, it is determined by the plan configuration.
+
+          invoicing_threshold: When this subscription's accrued usage reaches this threshold, an invoice will
+              be issued for the subscription. If not specified, invoices will only be issued
+              at the end of the billing period.
+
+          metadata: User-specified key/value pairs for the resource. Individual keys can be removed
+              by setting the value to `null`, and the entire metadata mapping can be cleared
+              by setting `metadata` to `null`.
+
+          net_terms: Determines the difference between the invoice issue date for subscription
+              invoices as the date that they are due. A value of `0` here represents that the
+              invoice is due on issue, whereas a value of `30` represents that the customer
+              has a month to pay the invoice.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        if not subscription_id:
+            raise ValueError(f"Expected a non-empty value for `subscription_id` but received {subscription_id!r}")
+        return self._put(
+            f"/subscriptions/{subscription_id}",
+            body=maybe_transform(
+                {
+                    "auto_collection": auto_collection,
+                    "default_invoice_memo": default_invoice_memo,
+                    "invoicing_threshold": invoicing_threshold,
+                    "metadata": metadata,
+                    "net_terms": net_terms,
+                },
+                subscription_update_params.SubscriptionUpdateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=Subscription,
+        )
+
     def list(
         self,
         *,
         created_at_gt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_gte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
@@ -1331,14 +1409,19 @@
 
         Price overrides are used to update some or all prices in the target plan.
         Minimums and maximums, much like price overrides, can be useful when a new
         customer has negotiated a new or different minimum or maximum spend cap than the
         default for the plan. The request format for price overrides, maximums, and
         minimums are the same as those in [subscription creation](create-subscription).
 
+        ## Scheduling multiple plan changes
+
+        When scheduling multiple plan changes with the same date, the latest plan change
+        on that day takes effect.
+
         ## Prorations for in-advance fees
 
         By default, Orb calculates the prorated difference in any fixed fees when making
         a plan change, adjusting the customer balance as needed. For details on this
         behavior, see
         [Modifying subscriptions](../guides/product-catalog/modifying-subscriptions.md#prorations-for-in-advance-fees).
 
@@ -2162,14 +2245,91 @@
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Subscription,
         )
 
+    async def update(
+        self,
+        subscription_id: str,
+        *,
+        auto_collection: Optional[bool] | NotGiven = NOT_GIVEN,
+        default_invoice_memo: Optional[str] | NotGiven = NOT_GIVEN,
+        invoicing_threshold: Optional[str] | NotGiven = NOT_GIVEN,
+        metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
+        net_terms: Optional[int] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Subscription:
+        """
+        This endpoint can be used to update the `metadata`, `net terms`,
+        `auto_collection`, `invoicing_threshold`, and `default_invoice_memo` properties
+        on a subscription.
+
+        Args:
+          auto_collection: Determines whether issued invoices for this subscription will automatically be
+              charged with the saved payment method on the due date. This property defaults to
+              the plan's behavior.
+
+          default_invoice_memo: Determines the default memo on this subscription's invoices. Note that if this
+              is not provided, it is determined by the plan configuration.
+
+          invoicing_threshold: When this subscription's accrued usage reaches this threshold, an invoice will
+              be issued for the subscription. If not specified, invoices will only be issued
+              at the end of the billing period.
+
+          metadata: User-specified key/value pairs for the resource. Individual keys can be removed
+              by setting the value to `null`, and the entire metadata mapping can be cleared
+              by setting `metadata` to `null`.
+
+          net_terms: Determines the difference between the invoice issue date for subscription
+              invoices as the date that they are due. A value of `0` here represents that the
+              invoice is due on issue, whereas a value of `30` represents that the customer
+              has a month to pay the invoice.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        if not subscription_id:
+            raise ValueError(f"Expected a non-empty value for `subscription_id` but received {subscription_id!r}")
+        return await self._put(
+            f"/subscriptions/{subscription_id}",
+            body=await async_maybe_transform(
+                {
+                    "auto_collection": auto_collection,
+                    "default_invoice_memo": default_invoice_memo,
+                    "invoicing_threshold": invoicing_threshold,
+                    "metadata": metadata,
+                    "net_terms": net_terms,
+                },
+                subscription_update_params.SubscriptionUpdateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=Subscription,
+        )
+
     def list(
         self,
         *,
         created_at_gt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_gte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
@@ -2961,14 +3121,19 @@
 
         Price overrides are used to update some or all prices in the target plan.
         Minimums and maximums, much like price overrides, can be useful when a new
         customer has negotiated a new or different minimum or maximum spend cap than the
         default for the plan. The request format for price overrides, maximums, and
         minimums are the same as those in [subscription creation](create-subscription).
 
+        ## Scheduling multiple plan changes
+
+        When scheduling multiple plan changes with the same date, the latest plan change
+        on that day takes effect.
+
         ## Prorations for in-advance fees
 
         By default, Orb calculates the prorated difference in any fixed fees when making
         a plan change, adjusting the customer balance as needed. For details on this
         behavior, see
         [Modifying subscriptions](../guides/product-catalog/modifying-subscriptions.md#prorations-for-in-advance-fees).
 
@@ -3306,14 +3471,17 @@
 class SubscriptionsWithRawResponse:
     def __init__(self, subscriptions: Subscriptions) -> None:
         self._subscriptions = subscriptions
 
         self.create = _legacy_response.to_raw_response_wrapper(
             subscriptions.create,
         )
+        self.update = _legacy_response.to_raw_response_wrapper(
+            subscriptions.update,
+        )
         self.list = _legacy_response.to_raw_response_wrapper(
             subscriptions.list,
         )
         self.cancel = _legacy_response.to_raw_response_wrapper(
             subscriptions.cancel,
         )
         self.fetch = _legacy_response.to_raw_response_wrapper(
@@ -3354,14 +3522,17 @@
 class AsyncSubscriptionsWithRawResponse:
     def __init__(self, subscriptions: AsyncSubscriptions) -> None:
         self._subscriptions = subscriptions
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
             subscriptions.create,
         )
+        self.update = _legacy_response.async_to_raw_response_wrapper(
+            subscriptions.update,
+        )
         self.list = _legacy_response.async_to_raw_response_wrapper(
             subscriptions.list,
         )
         self.cancel = _legacy_response.async_to_raw_response_wrapper(
             subscriptions.cancel,
         )
         self.fetch = _legacy_response.async_to_raw_response_wrapper(
@@ -3402,14 +3573,17 @@
 class SubscriptionsWithStreamingResponse:
     def __init__(self, subscriptions: Subscriptions) -> None:
         self._subscriptions = subscriptions
 
         self.create = to_streamed_response_wrapper(
             subscriptions.create,
         )
+        self.update = to_streamed_response_wrapper(
+            subscriptions.update,
+        )
         self.list = to_streamed_response_wrapper(
             subscriptions.list,
         )
         self.cancel = to_streamed_response_wrapper(
             subscriptions.cancel,
         )
         self.fetch = to_streamed_response_wrapper(
@@ -3450,14 +3624,17 @@
 class AsyncSubscriptionsWithStreamingResponse:
     def __init__(self, subscriptions: AsyncSubscriptions) -> None:
         self._subscriptions = subscriptions
 
         self.create = async_to_streamed_response_wrapper(
             subscriptions.create,
         )
+        self.update = async_to_streamed_response_wrapper(
+            subscriptions.update,
+        )
         self.list = async_to_streamed_response_wrapper(
             subscriptions.list,
         )
         self.cancel = async_to_streamed_response_wrapper(
             subscriptions.cancel,
         )
         self.fetch = async_to_streamed_response_wrapper(
```

### Comparing `orb_billing-1.47.1/src/orb/resources/top_level.py` & `orb_billing-1.48.0/src/orb/resources/top_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import httpx
 
 from .. import _legacy_response
-from ..types import TopLevelPingResponse
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from .._base_client import (
     make_request_options,
 )
+from ..types.top_level_ping_response import TopLevelPingResponse
 
 __all__ = ["TopLevel", "AsyncTopLevel"]
 
 
 class TopLevel(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> TopLevelWithRawResponse:
```

### Comparing `orb_billing-1.47.1/src/orb/resources/coupons/__init__.py` & `orb_billing-1.48.0/src/orb/resources/coupons/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/resources/coupons/coupons.py` & `orb_billing-1.48.0/src/orb/resources/coupons/coupons.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from typing import Optional
 
 import httpx
 
 from ... import _legacy_response
-from ...types import Coupon, coupon_list_params, coupon_create_params
+from ...types import coupon_list_params, coupon_create_params
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
@@ -25,14 +25,15 @@
     SubscriptionsWithStreamingResponse,
     AsyncSubscriptionsWithStreamingResponse,
 )
 from ..._base_client import (
     AsyncPaginator,
     make_request_options,
 )
+from ...types.coupon import Coupon
 
 __all__ = ["Coupons", "AsyncCoupons"]
 
 
 class Coupons(SyncAPIResource):
     @cached_property
     def subscriptions(self) -> Subscriptions:
```

### Comparing `orb_billing-1.47.1/src/orb/resources/coupons/subscriptions.py` & `orb_billing-1.48.0/src/orb/resources/coupons/subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from __future__ import annotations
 
 from typing import Optional
 
 import httpx
 
 from ... import _legacy_response
-from ...types import Subscription
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import (
     AsyncPaginator,
     make_request_options,
 )
 from ...types.coupons import subscription_list_params
+from ...types.subscription import Subscription
 
 __all__ = ["Subscriptions", "AsyncSubscriptions"]
 
 
 class Subscriptions(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> SubscriptionsWithRawResponse:
```

### Comparing `orb_billing-1.47.1/src/orb/resources/customers/__init__.py` & `orb_billing-1.48.0/src/orb/resources/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/resources/customers/balance_transactions.py` & `orb_billing-1.48.0/src/orb/resources/customers/balance_transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,17 @@
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import (
     AsyncPaginator,
     make_request_options,
 )
-from ...types.customers import (
-    BalanceTransactionListResponse,
-    BalanceTransactionCreateResponse,
-    balance_transaction_list_params,
-    balance_transaction_create_params,
-)
+from ...types.customers import balance_transaction_list_params, balance_transaction_create_params
+from ...types.customers.balance_transaction_list_response import BalanceTransactionListResponse
+from ...types.customers.balance_transaction_create_response import BalanceTransactionCreateResponse
 
 __all__ = ["BalanceTransactions", "AsyncBalanceTransactions"]
 
 
 class BalanceTransactions(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> BalanceTransactionsWithRawResponse:
```

### Comparing `orb_billing-1.47.1/src/orb/resources/customers/costs.py` & `orb_billing-1.48.0/src/orb/resources/customers/costs.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,20 +16,17 @@
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
-from ...types.customers import (
-    CostListResponse,
-    CostListByExternalIDResponse,
-    cost_list_params,
-    cost_list_by_external_id_params,
-)
+from ...types.customers import cost_list_params, cost_list_by_external_id_params
+from ...types.customers.cost_list_response import CostListResponse
+from ...types.customers.cost_list_by_external_id_response import CostListByExternalIDResponse
 
 __all__ = ["Costs", "AsyncCosts"]
 
 
 class Costs(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> CostsWithRawResponse:
@@ -37,15 +34,15 @@
 
     @cached_property
     def with_streaming_response(self) -> CostsWithStreamingResponse:
         return CostsWithStreamingResponse(self)
 
     def list(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         timeframe_end: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         timeframe_start: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         view_mode: Optional[Literal["periodic", "cumulative"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -226,15 +223,15 @@
                 ),
             ),
             cast_to=CostListResponse,
         )
 
     def list_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         timeframe_end: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         timeframe_start: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         view_mode: Optional[Literal["periodic", "cumulative"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -427,15 +424,15 @@
 
     @cached_property
     def with_streaming_response(self) -> AsyncCostsWithStreamingResponse:
         return AsyncCostsWithStreamingResponse(self)
 
     async def list(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         timeframe_end: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         timeframe_start: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         view_mode: Optional[Literal["periodic", "cumulative"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -616,15 +613,15 @@
                 ),
             ),
             cast_to=CostListResponse,
         )
 
     async def list_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         timeframe_end: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         timeframe_start: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         view_mode: Optional[Literal["periodic", "cumulative"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
```

### Comparing `orb_billing-1.47.1/src/orb/resources/customers/customers.py` & `orb_billing-1.48.0/src/orb/resources/customers/customers.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     AsyncUsage,
     UsageWithRawResponse,
     AsyncUsageWithRawResponse,
     UsageWithStreamingResponse,
     AsyncUsageWithStreamingResponse,
 )
 from ...types import (
-    Customer,
     customer_list_params,
     customer_create_params,
     customer_update_params,
     customer_update_by_external_id_params,
 )
 from .credits import (
     Credits,
@@ -50,14 +49,15 @@
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import (
     AsyncPaginator,
     make_request_options,
 )
 from .credits.credits import Credits, AsyncCredits
+from ...types.customer import Customer
 from .balance_transactions import (
     BalanceTransactions,
     AsyncBalanceTransactions,
     BalanceTransactionsWithRawResponse,
     AsyncBalanceTransactionsWithRawResponse,
     BalanceTransactionsWithStreamingResponse,
     AsyncBalanceTransactionsWithStreamingResponse,
```

### Comparing `orb_billing-1.47.1/src/orb/resources/customers/usage.py` & `orb_billing-1.48.0/src/orb/resources/customers/usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Union, Iterable, Optional
+from typing import Union, Iterable
 from datetime import datetime
 
 import httpx
 
 from ... import _legacy_response
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
@@ -15,20 +15,17 @@
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
-from ...types.customers import (
-    UsageUpdateResponse,
-    UsageUpdateByExternalIDResponse,
-    usage_update_params,
-    usage_update_by_external_id_params,
-)
+from ...types.customers import usage_update_params, usage_update_by_external_id_params
+from ...types.customers.usage_update_response import UsageUpdateResponse
+from ...types.customers.usage_update_by_external_id_response import UsageUpdateByExternalIDResponse
 
 __all__ = ["Usage", "AsyncUsage"]
 
 
 class Usage(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> UsageWithRawResponse:
@@ -36,15 +33,15 @@
 
     @cached_property
     def with_streaming_response(self) -> UsageWithStreamingResponse:
         return UsageWithStreamingResponse(self)
 
     def update(
         self,
-        id: Optional[str],
+        id: str,
         *,
         events: Iterable[usage_update_params.Event],
         timeframe_end: Union[str, datetime] | NotGiven = NOT_GIVEN,
         timeframe_start: Union[str, datetime] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -189,15 +186,15 @@
                 ),
             ),
             cast_to=UsageUpdateResponse,
         )
 
     def update_by_external_id(
         self,
-        id: Optional[str],
+        id: str,
         *,
         events: Iterable[usage_update_by_external_id_params.Event],
         timeframe_end: Union[str, datetime] | NotGiven = NOT_GIVEN,
         timeframe_start: Union[str, datetime] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -352,15 +349,15 @@
 
     @cached_property
     def with_streaming_response(self) -> AsyncUsageWithStreamingResponse:
         return AsyncUsageWithStreamingResponse(self)
 
     async def update(
         self,
-        id: Optional[str],
+        id: str,
         *,
         events: Iterable[usage_update_params.Event],
         timeframe_end: Union[str, datetime] | NotGiven = NOT_GIVEN,
         timeframe_start: Union[str, datetime] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -505,15 +502,15 @@
                 ),
             ),
             cast_to=UsageUpdateResponse,
         )
 
     async def update_by_external_id(
         self,
-        id: Optional[str],
+        id: str,
         *,
         events: Iterable[usage_update_by_external_id_params.Event],
         timeframe_end: Union[str, datetime] | NotGiven = NOT_GIVEN,
         timeframe_start: Union[str, datetime] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
```

### Comparing `orb_billing-1.47.1/src/orb/resources/customers/credits/__init__.py` & `orb_billing-1.48.0/src/orb/resources/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/resources/customers/credits/credits.py` & `orb_billing-1.48.0/src/orb/resources/customers/credits/credits.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,20 +29,17 @@
 from ...._resource import SyncAPIResource, AsyncAPIResource
 from ...._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ....pagination import SyncPage, AsyncPage
 from ...._base_client import (
     AsyncPaginator,
     make_request_options,
 )
-from ....types.customers import (
-    CreditListResponse,
-    CreditListByExternalIDResponse,
-    credit_list_params,
-    credit_list_by_external_id_params,
-)
+from ....types.customers import credit_list_params, credit_list_by_external_id_params
+from ....types.customers.credit_list_response import CreditListResponse
+from ....types.customers.credit_list_by_external_id_response import CreditListByExternalIDResponse
 
 __all__ = ["Credits", "AsyncCredits"]
 
 
 class Credits(SyncAPIResource):
     @cached_property
     def ledger(self) -> Ledger:
@@ -58,29 +55,32 @@
 
     @cached_property
     def with_streaming_response(self) -> CreditsWithStreamingResponse:
         return CreditsWithStreamingResponse(self)
 
     def list(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[CreditListResponse]:
         """
         Returns a paginated list of unexpired, non-zero credit blocks for a customer.
 
+        Note that `currency` defaults to credits if not specified. To use a real world
+        currency, set `currency` to an ISO 4217 string.
+
         Args:
           currency: The ledger currency or custom pricing unit to use.
 
           cursor: Cursor for pagination. This can be populated by the `next_cursor` value returned
               from the initial request.
 
           limit: The number of items to fetch. Defaults to 20.
@@ -113,29 +113,32 @@
                 ),
             ),
             model=CreditListResponse,
         )
 
     def list_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[CreditListByExternalIDResponse]:
         """
         Returns a paginated list of unexpired, non-zero credit blocks for a customer.
 
+        Note that `currency` defaults to credits if not specified. To use a real world
+        currency, set `currency` to an ISO 4217 string.
+
         Args:
           currency: The ledger currency or custom pricing unit to use.
 
           cursor: Cursor for pagination. This can be populated by the `next_cursor` value returned
               from the initial request.
 
           limit: The number of items to fetch. Defaults to 20.
@@ -188,29 +191,32 @@
 
     @cached_property
     def with_streaming_response(self) -> AsyncCreditsWithStreamingResponse:
         return AsyncCreditsWithStreamingResponse(self)
 
     def list(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[CreditListResponse, AsyncPage[CreditListResponse]]:
         """
         Returns a paginated list of unexpired, non-zero credit blocks for a customer.
 
+        Note that `currency` defaults to credits if not specified. To use a real world
+        currency, set `currency` to an ISO 4217 string.
+
         Args:
           currency: The ledger currency or custom pricing unit to use.
 
           cursor: Cursor for pagination. This can be populated by the `next_cursor` value returned
               from the initial request.
 
           limit: The number of items to fetch. Defaults to 20.
@@ -243,29 +249,32 @@
                 ),
             ),
             model=CreditListResponse,
         )
 
     def list_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[CreditListByExternalIDResponse, AsyncPage[CreditListByExternalIDResponse]]:
         """
         Returns a paginated list of unexpired, non-zero credit blocks for a customer.
 
+        Note that `currency` defaults to credits if not specified. To use a real world
+        currency, set `currency` to an ISO 4217 string.
+
         Args:
           currency: The ledger currency or custom pricing unit to use.
 
           cursor: Cursor for pagination. This can be populated by the `next_cursor` value returned
               from the initial request.
 
           limit: The number of items to fetch. Defaults to 20.
```

### Comparing `orb_billing-1.47.1/src/orb/resources/customers/credits/ledger.py` & `orb_billing-1.48.0/src/orb/resources/customers/credits/ledger.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 from ...._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ....pagination import SyncPage, AsyncPage
 from ...._base_client import (
     AsyncPaginator,
     make_request_options,
 )
 from ....types.customers.credits import (
-    LedgerListResponse,
-    LedgerCreateEntryResponse,
-    LedgerListByExternalIDResponse,
-    LedgerCreateEntryByExternalIDResponse,
     ledger_list_params,
     ledger_create_entry_params,
     ledger_list_by_external_id_params,
     ledger_create_entry_by_external_id_params,
 )
+from ....types.customers.credits.ledger_list_response import LedgerListResponse
+from ....types.customers.credits.ledger_create_entry_response import LedgerCreateEntryResponse
+from ....types.customers.credits.ledger_list_by_external_id_response import LedgerListByExternalIDResponse
+from ....types.customers.credits.ledger_create_entry_by_external_id_response import (
+    LedgerCreateEntryByExternalIDResponse,
+)
 
 __all__ = ["Ledger", "AsyncLedger"]
 
 
 class Ledger(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> LedgerWithRawResponse:
@@ -44,15 +46,15 @@
 
     @cached_property
     def with_streaming_response(self) -> LedgerWithStreamingResponse:
         return LedgerWithStreamingResponse(self)
 
     def list(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         created_at_gt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_gte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
@@ -205,15 +207,15 @@
             ),
             model=cast(Any, LedgerListResponse),  # Union types cannot be passed in as arguments in the type system
         )
 
     @overload
     def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float,
         entry_type: Literal["increment"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         effective_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         expiry_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
@@ -361,16 +363,16 @@
               per_unit_cost_basis, as the calculation of the invoice total is done on that
               basis.
 
           metadata: User-specified key/value pairs for the resource. Individual keys can be removed
               by setting the value to `null`, and the entire metadata mapping can be cleared
               by setting `metadata` to `null`.
 
-          per_unit_cost_basis: Can only be specified when entry_type=increment. How much, in USD, a customer
-              paid for a single credit in this block
+          per_unit_cost_basis: Can only be specified when entry_type=increment. How much, in the customer's
+              currency, a customer paid for a single credit in this block
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
@@ -379,15 +381,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float,
         entry_type: Literal["decrement"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -535,15 +537,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         entry_type: Literal["expiration_change"],
         expiry_date: Union[str, datetime, None],
         target_expiry_date: Union[str, date],
         amount: Optional[float] | NotGiven = NOT_GIVEN,
         block_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
@@ -703,15 +705,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float,
         block_id: str,
         entry_type: Literal["void"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
@@ -865,15 +867,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float,
         block_id: str,
         entry_type: Literal["amendment"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
@@ -1030,15 +1032,15 @@
         ["amount", "entry_type"],
         ["entry_type", "expiry_date", "target_expiry_date"],
         ["amount", "block_id", "entry_type"],
         ["amount", "block_id", "entry_type"],
     )
     def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float | None | NotGiven = NOT_GIVEN,
         entry_type: Literal["increment"]
         | Literal["decrement"]
         | Literal["expiration_change"]
         | Literal["void"]
         | Literal["amendment"],
@@ -1096,15 +1098,15 @@
                 ),  # Union types cannot be passed in as arguments in the type system
             ),
         )
 
     @overload
     def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float,
         entry_type: Literal["increment"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         effective_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         expiry_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
@@ -1254,16 +1256,16 @@
               per_unit_cost_basis, as the calculation of the invoice total is done on that
               basis.
 
           metadata: User-specified key/value pairs for the resource. Individual keys can be removed
               by setting the value to `null`, and the entire metadata mapping can be cleared
               by setting `metadata` to `null`.
 
-          per_unit_cost_basis: Can only be specified when entry_type=increment. How much, in USD, a customer
-              paid for a single credit in this block
+          per_unit_cost_basis: Can only be specified when entry_type=increment. How much, in the customer's
+              currency, a customer paid for a single credit in this block
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
@@ -1272,15 +1274,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float,
         entry_type: Literal["decrement"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -1428,15 +1430,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         entry_type: Literal["expiration_change"],
         expiry_date: Union[str, datetime, None],
         target_expiry_date: Union[str, date],
         amount: Optional[float] | NotGiven = NOT_GIVEN,
         block_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
@@ -1596,15 +1598,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float,
         block_id: str,
         entry_type: Literal["void"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
@@ -1758,15 +1760,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float,
         block_id: str,
         entry_type: Literal["amendment"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
@@ -1923,15 +1925,15 @@
         ["amount", "entry_type"],
         ["entry_type", "expiry_date", "target_expiry_date"],
         ["amount", "block_id", "entry_type"],
         ["amount", "block_id", "entry_type"],
     )
     def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float | None | NotGiven = NOT_GIVEN,
         entry_type: Literal["increment"]
         | Literal["decrement"]
         | Literal["expiration_change"]
         | Literal["void"]
         | Literal["amendment"],
@@ -1992,15 +1994,15 @@
                     Any, LedgerCreateEntryByExternalIDResponse
                 ),  # Union types cannot be passed in as arguments in the type system
             ),
         )
 
     def list_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         created_at_gt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_gte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
@@ -2166,15 +2168,15 @@
 
     @cached_property
     def with_streaming_response(self) -> AsyncLedgerWithStreamingResponse:
         return AsyncLedgerWithStreamingResponse(self)
 
     def list(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         created_at_gt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_gte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
@@ -2327,15 +2329,15 @@
             ),
             model=cast(Any, LedgerListResponse),  # Union types cannot be passed in as arguments in the type system
         )
 
     @overload
     async def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float,
         entry_type: Literal["increment"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         effective_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         expiry_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
@@ -2483,16 +2485,16 @@
               per_unit_cost_basis, as the calculation of the invoice total is done on that
               basis.
 
           metadata: User-specified key/value pairs for the resource. Individual keys can be removed
               by setting the value to `null`, and the entire metadata mapping can be cleared
               by setting `metadata` to `null`.
 
-          per_unit_cost_basis: Can only be specified when entry_type=increment. How much, in USD, a customer
-              paid for a single credit in this block
+          per_unit_cost_basis: Can only be specified when entry_type=increment. How much, in the customer's
+              currency, a customer paid for a single credit in this block
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
@@ -2501,15 +2503,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     async def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float,
         entry_type: Literal["decrement"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -2657,15 +2659,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     async def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         entry_type: Literal["expiration_change"],
         expiry_date: Union[str, datetime, None],
         target_expiry_date: Union[str, date],
         amount: Optional[float] | NotGiven = NOT_GIVEN,
         block_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
@@ -2825,15 +2827,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     async def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float,
         block_id: str,
         entry_type: Literal["void"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
@@ -2987,15 +2989,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     async def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float,
         block_id: str,
         entry_type: Literal["amendment"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
@@ -3152,15 +3154,15 @@
         ["amount", "entry_type"],
         ["entry_type", "expiry_date", "target_expiry_date"],
         ["amount", "block_id", "entry_type"],
         ["amount", "block_id", "entry_type"],
     )
     async def create_entry(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: float | None | NotGiven = NOT_GIVEN,
         entry_type: Literal["increment"]
         | Literal["decrement"]
         | Literal["expiration_change"]
         | Literal["void"]
         | Literal["amendment"],
@@ -3218,15 +3220,15 @@
                 ),  # Union types cannot be passed in as arguments in the type system
             ),
         )
 
     @overload
     async def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float,
         entry_type: Literal["increment"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         effective_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         expiry_date: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
@@ -3376,16 +3378,16 @@
               per_unit_cost_basis, as the calculation of the invoice total is done on that
               basis.
 
           metadata: User-specified key/value pairs for the resource. Individual keys can be removed
               by setting the value to `null`, and the entire metadata mapping can be cleared
               by setting `metadata` to `null`.
 
-          per_unit_cost_basis: Can only be specified when entry_type=increment. How much, in USD, a customer
-              paid for a single credit in this block
+          per_unit_cost_basis: Can only be specified when entry_type=increment. How much, in the customer's
+              currency, a customer paid for a single credit in this block
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
@@ -3394,15 +3396,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     async def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float,
         entry_type: Literal["decrement"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -3550,15 +3552,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     async def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         entry_type: Literal["expiration_change"],
         expiry_date: Union[str, datetime, None],
         target_expiry_date: Union[str, date],
         amount: Optional[float] | NotGiven = NOT_GIVEN,
         block_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
@@ -3718,15 +3720,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     async def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float,
         block_id: str,
         entry_type: Literal["void"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
@@ -3880,15 +3882,15 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
     @overload
     async def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float,
         block_id: str,
         entry_type: Literal["amendment"],
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
@@ -4045,15 +4047,15 @@
         ["amount", "entry_type"],
         ["entry_type", "expiry_date", "target_expiry_date"],
         ["amount", "block_id", "entry_type"],
         ["amount", "block_id", "entry_type"],
     )
     async def create_entry_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: float | None | NotGiven = NOT_GIVEN,
         entry_type: Literal["increment"]
         | Literal["decrement"]
         | Literal["expiration_change"]
         | Literal["void"]
         | Literal["amendment"],
@@ -4114,15 +4116,15 @@
                     Any, LedgerCreateEntryByExternalIDResponse
                 ),  # Union types cannot be passed in as arguments in the type system
             ),
         )
 
     def list_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         created_at_gt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_gte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         currency: Optional[str] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
```

### Comparing `orb_billing-1.47.1/src/orb/resources/customers/credits/top_ups.py` & `orb_billing-1.48.0/src/orb/resources/customers/credits/top_ups.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 from ...._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ....pagination import SyncPage, AsyncPage
 from ...._base_client import (
     AsyncPaginator,
     make_request_options,
 )
 from ....types.customers.credits import (
-    TopUpListResponse,
-    TopUpCreateResponse,
-    TopUpListByExternalIDResponse,
-    TopUpCreateByExternalIDResponse,
     top_up_list_params,
     top_up_create_params,
     top_up_list_by_external_id_params,
     top_up_create_by_external_id_params,
 )
+from ....types.customers.credits.top_up_list_response import TopUpListResponse
+from ....types.customers.credits.top_up_create_response import TopUpCreateResponse
+from ....types.customers.credits.top_up_list_by_external_id_response import TopUpListByExternalIDResponse
+from ....types.customers.credits.top_up_create_by_external_id_response import TopUpCreateByExternalIDResponse
 
 __all__ = ["TopUps", "AsyncTopUps"]
 
 
 class TopUps(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> TopUpsWithRawResponse:
@@ -42,15 +42,15 @@
 
     @cached_property
     def with_streaming_response(self) -> TopUpsWithStreamingResponse:
         return TopUpsWithStreamingResponse(self)
 
     def create(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: str,
         currency: str,
         invoice_settings: top_up_create_params.InvoiceSettings,
         per_unit_cost_basis: str,
         threshold: str,
         expires_after: Optional[int] | NotGiven = NOT_GIVEN,
@@ -124,15 +124,15 @@
                 idempotency_key=idempotency_key,
             ),
             cast_to=TopUpCreateResponse,
         )
 
     def list(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -178,15 +178,15 @@
             model=TopUpListResponse,
         )
 
     def delete(
         self,
         top_up_id: str,
         *,
-        customer_id: Optional[str],
+        customer_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
@@ -220,15 +220,15 @@
                 idempotency_key=idempotency_key,
             ),
             cast_to=NoneType,
         )
 
     def create_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: str,
         currency: str,
         invoice_settings: top_up_create_by_external_id_params.InvoiceSettings,
         per_unit_cost_basis: str,
         threshold: str,
         expires_after: Optional[int] | NotGiven = NOT_GIVEN,
@@ -306,15 +306,15 @@
             cast_to=TopUpCreateByExternalIDResponse,
         )
 
     def delete_by_external_id(
         self,
         top_up_id: str,
         *,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
@@ -350,15 +350,15 @@
                 idempotency_key=idempotency_key,
             ),
             cast_to=NoneType,
         )
 
     def list_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -414,15 +414,15 @@
 
     @cached_property
     def with_streaming_response(self) -> AsyncTopUpsWithStreamingResponse:
         return AsyncTopUpsWithStreamingResponse(self)
 
     async def create(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         amount: str,
         currency: str,
         invoice_settings: top_up_create_params.InvoiceSettings,
         per_unit_cost_basis: str,
         threshold: str,
         expires_after: Optional[int] | NotGiven = NOT_GIVEN,
@@ -496,15 +496,15 @@
                 idempotency_key=idempotency_key,
             ),
             cast_to=TopUpCreateResponse,
         )
 
     def list(
         self,
-        customer_id: Optional[str],
+        customer_id: str,
         *,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -550,15 +550,15 @@
             model=TopUpListResponse,
         )
 
     async def delete(
         self,
         top_up_id: str,
         *,
-        customer_id: Optional[str],
+        customer_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
@@ -592,15 +592,15 @@
                 idempotency_key=idempotency_key,
             ),
             cast_to=NoneType,
         )
 
     async def create_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         amount: str,
         currency: str,
         invoice_settings: top_up_create_by_external_id_params.InvoiceSettings,
         per_unit_cost_basis: str,
         threshold: str,
         expires_after: Optional[int] | NotGiven = NOT_GIVEN,
@@ -678,15 +678,15 @@
             cast_to=TopUpCreateByExternalIDResponse,
         )
 
     async def delete_by_external_id(
         self,
         top_up_id: str,
         *,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
@@ -722,15 +722,15 @@
                 idempotency_key=idempotency_key,
             ),
             cast_to=NoneType,
         )
 
     def list_by_external_id(
         self,
-        external_customer_id: Optional[str],
+        external_customer_id: str,
         *,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
```

### Comparing `orb_billing-1.47.1/src/orb/resources/events/__init__.py` & `orb_billing-1.48.0/src/orb/resources/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/resources/events/backfills.py` & `orb_billing-1.48.0/src/orb/resources/events/backfills.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,20 @@
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import (
     AsyncPaginator,
     make_request_options,
 )
-from ...types.events import (
-    BackfillListResponse,
-    BackfillCloseResponse,
-    BackfillFetchResponse,
-    BackfillCreateResponse,
-    BackfillRevertResponse,
-    backfill_list_params,
-    backfill_create_params,
-)
+from ...types.events import backfill_list_params, backfill_create_params
+from ...types.events.backfill_list_response import BackfillListResponse
+from ...types.events.backfill_close_response import BackfillCloseResponse
+from ...types.events.backfill_fetch_response import BackfillFetchResponse
+from ...types.events.backfill_create_response import BackfillCreateResponse
+from ...types.events.backfill_revert_response import BackfillRevertResponse
 
 __all__ = ["Backfills", "AsyncBackfills"]
 
 
 class Backfills(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> BackfillsWithRawResponse:
```

### Comparing `orb_billing-1.47.1/src/orb/resources/events/events.py` & `orb_billing-1.48.0/src/orb/resources/events/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,15 @@
 
 from typing import List, Union, Iterable, Optional
 from datetime import datetime
 
 import httpx
 
 from ... import _legacy_response
-from ...types import (
-    EventIngestResponse,
-    EventSearchResponse,
-    EventUpdateResponse,
-    EventDeprecateResponse,
-    event_ingest_params,
-    event_search_params,
-    event_update_params,
-)
+from ...types import event_ingest_params, event_search_params, event_update_params
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from ..._compat import cached_property
 from .backfills import (
@@ -32,14 +24,18 @@
     AsyncBackfillsWithStreamingResponse,
 )
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
+from ...types.event_ingest_response import EventIngestResponse
+from ...types.event_search_response import EventSearchResponse
+from ...types.event_update_response import EventUpdateResponse
+from ...types.event_deprecate_response import EventDeprecateResponse
 
 __all__ = ["Events", "AsyncEvents"]
 
 
 class Events(SyncAPIResource):
     @cached_property
     def backfills(self) -> Backfills:
```

### Comparing `orb_billing-1.47.1/src/orb/resources/plans/__init__.py` & `orb_billing-1.48.0/src/orb/resources/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/resources/plans/external_plan_id.py` & `orb_billing-1.48.0/src/orb/resources/plans/external_plan_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from __future__ import annotations
 
 from typing import Dict, Optional
 
 import httpx
 
 from ... import _legacy_response
-from ...types import Plan
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
+from ...types.plan import Plan
 from ...types.plans import external_plan_id_update_params
 from ..._base_client import (
     make_request_options,
 )
 
 __all__ = ["ExternalPlanID", "AsyncExternalPlanID"]
```

### Comparing `orb_billing-1.47.1/src/orb/resources/plans/plans.py` & `orb_billing-1.48.0/src/orb/resources/plans/plans.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from typing import Dict, Union, Iterable, Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 import httpx
 
 from ... import _legacy_response
-from ...types import Plan, plan_list_params, plan_create_params, plan_update_params
+from ...types import plan_list_params, plan_create_params, plan_update_params
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ...pagination import SyncPage, AsyncPage
+from ...types.plan import Plan
 from ..._base_client import (
     AsyncPaginator,
     make_request_options,
 )
 from .external_plan_id import (
     ExternalPlanID,
     AsyncExternalPlanID,
```

### Comparing `orb_billing-1.47.1/src/orb/resources/prices/__init__.py` & `orb_billing-1.48.0/src/orb/resources/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/resources/prices/external_price_id.py` & `orb_billing-1.48.0/src/orb/resources/prices/external_price_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from __future__ import annotations
 
 from typing import Any, cast
 
 import httpx
 
 from ... import _legacy_response
-from ...types import Price
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
+from ...types.price import Price
 from ..._base_client import (
     make_request_options,
 )
 
 __all__ = ["ExternalPriceID", "AsyncExternalPriceID"]
```

### Comparing `orb_billing-1.47.1/src/orb/resources/prices/prices.py` & `orb_billing-1.48.0/src/orb/resources/prices/prices.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Any, Dict, Optional, cast, overload
+from typing import Any, Dict, List, Union, Optional, cast, overload
+from datetime import datetime
 from typing_extensions import Literal
 
 import httpx
 
 from ... import _legacy_response
-from ...types import Price, price_list_params, price_create_params
+from ...types import price_list_params, price_create_params, price_evaluate_params
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
     required_args,
     maybe_transform,
     async_maybe_transform,
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ...pagination import SyncPage, AsyncPage
+from ...types.price import Price
 from ..._base_client import (
     AsyncPaginator,
     make_request_options,
 )
 from .external_price_id import (
     ExternalPriceID,
     AsyncExternalPriceID,
     ExternalPriceIDWithRawResponse,
     AsyncExternalPriceIDWithRawResponse,
     ExternalPriceIDWithStreamingResponse,
     AsyncExternalPriceIDWithStreamingResponse,
 )
+from ...types.price_evaluate_response import PriceEvaluateResponse
 
 __all__ = ["Prices", "AsyncPrices"]
 
 
 class Prices(SyncAPIResource):
     @cached_property
     def external_price_id(self) -> ExternalPriceID:
@@ -56,14 +59,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["unit"],
         name: str,
         unit_config: price_create_params.NewFloatingUnitPriceUnitConfig,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -95,14 +99,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -126,14 +132,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["package"],
         name: str,
         package_config: price_create_params.NewFloatingPackagePricePackageConfig,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -165,14 +172,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -196,14 +205,15 @@
         currency: str,
         item_id: str,
         matrix_config: price_create_params.NewFloatingMatrixPriceMatrixConfig,
         model_type: Literal["matrix"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -235,14 +245,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -266,14 +278,15 @@
         currency: str,
         item_id: str,
         matrix_with_allocation_config: price_create_params.NewFloatingMatrixWithAllocationPriceMatrixWithAllocationConfig,
         model_type: Literal["matrix_with_allocation"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -305,14 +318,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -336,14 +351,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered"],
         name: str,
         tiered_config: price_create_params.NewFloatingTieredPriceTieredConfig,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -375,14 +391,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -406,14 +424,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered_bps"],
         name: str,
         tiered_bps_config: price_create_params.NewFloatingTieredBpsPriceTieredBpsConfig,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -445,14 +464,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -476,14 +497,15 @@
         cadence: Literal["annual", "monthly", "quarterly", "one_time"],
         currency: str,
         item_id: str,
         model_type: Literal["bps"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -515,14 +537,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -546,14 +570,15 @@
         cadence: Literal["annual", "monthly", "quarterly", "one_time"],
         currency: str,
         item_id: str,
         model_type: Literal["bulk_bps"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -585,14 +610,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -616,14 +643,15 @@
         cadence: Literal["annual", "monthly", "quarterly", "one_time"],
         currency: str,
         item_id: str,
         model_type: Literal["bulk"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -655,14 +683,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -686,14 +716,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["threshold_total_amount"],
         name: str,
         threshold_total_amount_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -725,14 +756,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -756,14 +789,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered_package"],
         name: str,
         tiered_package_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -795,14 +829,89 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
+          external_price_id: An alias for the price.
+
+          fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
+              applied.
+
+          invoice_grouping_key: The property used to group this price on an invoice
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        ...
+
+    @overload
+    def create(
+        self,
+        *,
+        cadence: Literal["annual", "monthly", "quarterly", "one_time"],
+        currency: str,
+        grouped_tiered_config: Dict[str, object],
+        item_id: str,
+        model_type: Literal["grouped_tiered"],
+        name: str,
+        billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
+        billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
+        external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
+        fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
+        invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Price:
+        """This endpoint is used to create a [price](../reference/price).
+
+        A price created
+        using this endpoint is always an add-on, meaning that it’s not associated with a
+        specific plan and can instead be individually added to subscriptions, including
+        subscriptions on different plans.
+
+        An `external_price_id` can be optionally specified as an alias to allow
+        ergonomic interaction with prices in the Orb API.
+
+        See the [Price resource](../reference/price) for the specification of different
+        price model configurations possible in this endpoint.
+
+        Args:
+          cadence: The cadence to bill for this price on.
+
+          currency: An ISO 4217 currency string for which this price is billed in.
+
+          item_id: The id of the item the plan will be associated with.
+
+          name: The name of the price.
+
+          billable_metric_id: The id of the billable metric for the price. Only needed if the price is
+              usage-based.
+
+          billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
+              this is true, and in-arrears if this is false.
+
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -826,14 +935,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered_with_minimum"],
         name: str,
         tiered_with_minimum_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -865,14 +975,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -896,14 +1008,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["package_with_allocation"],
         name: str,
         package_with_allocation_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -935,14 +1048,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -966,14 +1081,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered_package_with_minimum"],
         name: str,
         tiered_package_with_minimum_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1005,14 +1121,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1036,14 +1154,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["unit_with_percent"],
         name: str,
         unit_with_percent_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1075,14 +1194,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1106,14 +1227,15 @@
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_bps_config"],
         ["bps_config", "cadence", "currency", "item_id", "model_type", "name"],
         ["bulk_bps_config", "cadence", "currency", "item_id", "model_type", "name"],
         ["bulk_config", "cadence", "currency", "item_id", "model_type", "name"],
         ["cadence", "currency", "item_id", "model_type", "name", "threshold_total_amount_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_package_config"],
+        ["cadence", "currency", "grouped_tiered_config", "item_id", "model_type", "name"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_with_minimum_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "package_with_allocation_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_package_with_minimum_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "unit_with_percent_config"],
     )
     def create(
         self,
@@ -1128,36 +1250,39 @@
         | Literal["tiered"]
         | Literal["tiered_bps"]
         | Literal["bps"]
         | Literal["bulk_bps"]
         | Literal["bulk"]
         | Literal["threshold_total_amount"]
         | Literal["tiered_package"]
+        | Literal["grouped_tiered"]
         | Literal["tiered_with_minimum"]
         | Literal["package_with_allocation"]
         | Literal["tiered_package_with_minimum"]
         | Literal["unit_with_percent"],
         name: str,
         unit_config: price_create_params.NewFloatingUnitPriceUnitConfig | NotGiven = NOT_GIVEN,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         package_config: price_create_params.NewFloatingPackagePricePackageConfig | NotGiven = NOT_GIVEN,
         matrix_config: price_create_params.NewFloatingMatrixPriceMatrixConfig | NotGiven = NOT_GIVEN,
         matrix_with_allocation_config: price_create_params.NewFloatingMatrixWithAllocationPriceMatrixWithAllocationConfig
         | NotGiven = NOT_GIVEN,
         tiered_config: price_create_params.NewFloatingTieredPriceTieredConfig | NotGiven = NOT_GIVEN,
         tiered_bps_config: price_create_params.NewFloatingTieredBpsPriceTieredBpsConfig | NotGiven = NOT_GIVEN,
         bps_config: price_create_params.NewFloatingBpsPriceBpsConfig | NotGiven = NOT_GIVEN,
         bulk_bps_config: price_create_params.NewFloatingBulkBpsPriceBulkBpsConfig | NotGiven = NOT_GIVEN,
         bulk_config: price_create_params.NewFloatingBulkPriceBulkConfig | NotGiven = NOT_GIVEN,
         threshold_total_amount_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_package_config: Dict[str, object] | NotGiven = NOT_GIVEN,
+        grouped_tiered_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_with_minimum_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         package_with_allocation_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_package_with_minimum_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         unit_with_percent_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -1176,27 +1301,29 @@
                         "currency": currency,
                         "item_id": item_id,
                         "model_type": model_type,
                         "name": name,
                         "unit_config": unit_config,
                         "billable_metric_id": billable_metric_id,
                         "billed_in_advance": billed_in_advance,
+                        "conversion_rate": conversion_rate,
                         "external_price_id": external_price_id,
                         "fixed_price_quantity": fixed_price_quantity,
                         "invoice_grouping_key": invoice_grouping_key,
                         "package_config": package_config,
                         "matrix_config": matrix_config,
                         "matrix_with_allocation_config": matrix_with_allocation_config,
                         "tiered_config": tiered_config,
                         "tiered_bps_config": tiered_bps_config,
                         "bps_config": bps_config,
                         "bulk_bps_config": bulk_bps_config,
                         "bulk_config": bulk_config,
                         "threshold_total_amount_config": threshold_total_amount_config,
                         "tiered_package_config": tiered_package_config,
+                        "grouped_tiered_config": grouped_tiered_config,
                         "tiered_with_minimum_config": tiered_with_minimum_config,
                         "package_with_allocation_config": package_with_allocation_config,
                         "tiered_package_with_minimum_config": tiered_package_with_minimum_config,
                         "unit_with_percent_config": unit_with_percent_config,
                     },
                     price_create_params.PriceCreateParams,
                 ),
@@ -1256,14 +1383,107 @@
                     },
                     price_list_params.PriceListParams,
                 ),
             ),
             model=cast(Any, Price),  # Union types cannot be passed in as arguments in the type system
         )
 
+    def evaluate(
+        self,
+        price_id: str,
+        *,
+        timeframe_end: Union[str, datetime],
+        timeframe_start: Union[str, datetime],
+        customer_id: Optional[str] | NotGiven = NOT_GIVEN,
+        external_customer_id: Optional[str] | NotGiven = NOT_GIVEN,
+        filter: Optional[str] | NotGiven = NOT_GIVEN,
+        grouping_keys: List[str] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> PriceEvaluateResponse:
+        """
+        This endpoint is used to evaluate the output of a price for a given customer and
+        time range. It enables filtering and grouping the output using
+        [computed properties](../guides/extensibility/advanced-metrics#computed-properties),
+        supporting the following workflows:
+
+        1. Showing detailed usage and costs to the end customer.
+        2. Auditing subtotals on invoice line items.
+
+        For these workflows, the expressiveness of computed properties in both the
+        filters and grouping is critical. For example, if you'd like to show your
+        customer their usage grouped by hour and another property, you can do so with
+        the following `grouping_keys`:
+        `["hour_floor_timestamp_millis(timestamp_millis)", "my_property"]`. If you'd
+        like to examine a customer's usage for a specific property value, you can do so
+        with the following `filter`:
+        `my_property = 'foo' AND my_other_property = 'bar'`.
+
+        By default, the start of the time range must be no more than 100 days ago and
+        the length of the results must be no greater than 1000. Note that this is a POST
+        endpoint rather than a GET endpoint because it employs a JSON body rather than
+        query parameters.
+
+        Args:
+          timeframe_end: The exclusive upper bound for event timestamps
+
+          timeframe_start: The inclusive lower bound for event timestamps
+
+          customer_id: The ID of the customer to which this evaluation is scoped.
+
+          external_customer_id: The external customer ID of the customer to which this evaluation is scoped.
+
+          filter: A boolean
+              [computed property](../guides/extensibility/advanced-metrics#computed-properties)
+              used to filter the underlying billable metric
+
+          grouping_keys: Properties (or
+              [computed properties](../guides/extensibility/advanced-metrics#computed-properties))
+              used to group the underlying billable metric
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        if not price_id:
+            raise ValueError(f"Expected a non-empty value for `price_id` but received {price_id!r}")
+        return self._post(
+            f"/prices/{price_id}/evaluate",
+            body=maybe_transform(
+                {
+                    "timeframe_end": timeframe_end,
+                    "timeframe_start": timeframe_start,
+                    "customer_id": customer_id,
+                    "external_customer_id": external_customer_id,
+                    "filter": filter,
+                    "grouping_keys": grouping_keys,
+                },
+                price_evaluate_params.PriceEvaluateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=PriceEvaluateResponse,
+        )
+
     def fetch(
         self,
         price_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -1318,14 +1538,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["unit"],
         name: str,
         unit_config: price_create_params.NewFloatingUnitPriceUnitConfig,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1357,14 +1578,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1388,14 +1611,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["package"],
         name: str,
         package_config: price_create_params.NewFloatingPackagePricePackageConfig,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1427,14 +1651,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1458,14 +1684,15 @@
         currency: str,
         item_id: str,
         matrix_config: price_create_params.NewFloatingMatrixPriceMatrixConfig,
         model_type: Literal["matrix"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1497,14 +1724,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1528,14 +1757,15 @@
         currency: str,
         item_id: str,
         matrix_with_allocation_config: price_create_params.NewFloatingMatrixWithAllocationPriceMatrixWithAllocationConfig,
         model_type: Literal["matrix_with_allocation"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1567,14 +1797,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1598,14 +1830,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered"],
         name: str,
         tiered_config: price_create_params.NewFloatingTieredPriceTieredConfig,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1637,14 +1870,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1668,14 +1903,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered_bps"],
         name: str,
         tiered_bps_config: price_create_params.NewFloatingTieredBpsPriceTieredBpsConfig,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1707,14 +1943,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1738,14 +1976,15 @@
         cadence: Literal["annual", "monthly", "quarterly", "one_time"],
         currency: str,
         item_id: str,
         model_type: Literal["bps"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1777,14 +2016,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1808,14 +2049,15 @@
         cadence: Literal["annual", "monthly", "quarterly", "one_time"],
         currency: str,
         item_id: str,
         model_type: Literal["bulk_bps"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1847,14 +2089,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1878,14 +2122,15 @@
         cadence: Literal["annual", "monthly", "quarterly", "one_time"],
         currency: str,
         item_id: str,
         model_type: Literal["bulk"],
         name: str,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1917,14 +2162,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -1948,14 +2195,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["threshold_total_amount"],
         name: str,
         threshold_total_amount_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -1987,14 +2235,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -2018,14 +2268,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered_package"],
         name: str,
         tiered_package_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -2057,14 +2308,89 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
+          external_price_id: An alias for the price.
+
+          fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
+              applied.
+
+          invoice_grouping_key: The property used to group this price on an invoice
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        ...
+
+    @overload
+    async def create(
+        self,
+        *,
+        cadence: Literal["annual", "monthly", "quarterly", "one_time"],
+        currency: str,
+        grouped_tiered_config: Dict[str, object],
+        item_id: str,
+        model_type: Literal["grouped_tiered"],
+        name: str,
+        billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
+        billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
+        external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
+        fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
+        invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Price:
+        """This endpoint is used to create a [price](../reference/price).
+
+        A price created
+        using this endpoint is always an add-on, meaning that it’s not associated with a
+        specific plan and can instead be individually added to subscriptions, including
+        subscriptions on different plans.
+
+        An `external_price_id` can be optionally specified as an alias to allow
+        ergonomic interaction with prices in the Orb API.
+
+        See the [Price resource](../reference/price) for the specification of different
+        price model configurations possible in this endpoint.
+
+        Args:
+          cadence: The cadence to bill for this price on.
+
+          currency: An ISO 4217 currency string for which this price is billed in.
+
+          item_id: The id of the item the plan will be associated with.
+
+          name: The name of the price.
+
+          billable_metric_id: The id of the billable metric for the price. Only needed if the price is
+              usage-based.
+
+          billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
+              this is true, and in-arrears if this is false.
+
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -2088,14 +2414,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered_with_minimum"],
         name: str,
         tiered_with_minimum_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -2127,14 +2454,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -2158,14 +2487,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["package_with_allocation"],
         name: str,
         package_with_allocation_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -2197,14 +2527,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -2228,14 +2560,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["tiered_package_with_minimum"],
         name: str,
         tiered_package_with_minimum_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -2267,14 +2600,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -2298,14 +2633,15 @@
         currency: str,
         item_id: str,
         model_type: Literal["unit_with_percent"],
         name: str,
         unit_with_percent_config: Dict[str, object],
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -2337,14 +2673,16 @@
 
           billable_metric_id: The id of the billable metric for the price. Only needed if the price is
               usage-based.
 
           billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
               this is true, and in-arrears if this is false.
 
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
           external_price_id: An alias for the price.
 
           fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
               applied.
 
           invoice_grouping_key: The property used to group this price on an invoice
 
@@ -2368,14 +2706,15 @@
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_bps_config"],
         ["bps_config", "cadence", "currency", "item_id", "model_type", "name"],
         ["bulk_bps_config", "cadence", "currency", "item_id", "model_type", "name"],
         ["bulk_config", "cadence", "currency", "item_id", "model_type", "name"],
         ["cadence", "currency", "item_id", "model_type", "name", "threshold_total_amount_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_package_config"],
+        ["cadence", "currency", "grouped_tiered_config", "item_id", "model_type", "name"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_with_minimum_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "package_with_allocation_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_package_with_minimum_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "unit_with_percent_config"],
     )
     async def create(
         self,
@@ -2390,36 +2729,39 @@
         | Literal["tiered"]
         | Literal["tiered_bps"]
         | Literal["bps"]
         | Literal["bulk_bps"]
         | Literal["bulk"]
         | Literal["threshold_total_amount"]
         | Literal["tiered_package"]
+        | Literal["grouped_tiered"]
         | Literal["tiered_with_minimum"]
         | Literal["package_with_allocation"]
         | Literal["tiered_package_with_minimum"]
         | Literal["unit_with_percent"],
         name: str,
         unit_config: price_create_params.NewFloatingUnitPriceUnitConfig | NotGiven = NOT_GIVEN,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
         invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
         package_config: price_create_params.NewFloatingPackagePricePackageConfig | NotGiven = NOT_GIVEN,
         matrix_config: price_create_params.NewFloatingMatrixPriceMatrixConfig | NotGiven = NOT_GIVEN,
         matrix_with_allocation_config: price_create_params.NewFloatingMatrixWithAllocationPriceMatrixWithAllocationConfig
         | NotGiven = NOT_GIVEN,
         tiered_config: price_create_params.NewFloatingTieredPriceTieredConfig | NotGiven = NOT_GIVEN,
         tiered_bps_config: price_create_params.NewFloatingTieredBpsPriceTieredBpsConfig | NotGiven = NOT_GIVEN,
         bps_config: price_create_params.NewFloatingBpsPriceBpsConfig | NotGiven = NOT_GIVEN,
         bulk_bps_config: price_create_params.NewFloatingBulkBpsPriceBulkBpsConfig | NotGiven = NOT_GIVEN,
         bulk_config: price_create_params.NewFloatingBulkPriceBulkConfig | NotGiven = NOT_GIVEN,
         threshold_total_amount_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_package_config: Dict[str, object] | NotGiven = NOT_GIVEN,
+        grouped_tiered_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_with_minimum_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         package_with_allocation_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_package_with_minimum_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         unit_with_percent_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -2438,27 +2780,29 @@
                         "currency": currency,
                         "item_id": item_id,
                         "model_type": model_type,
                         "name": name,
                         "unit_config": unit_config,
                         "billable_metric_id": billable_metric_id,
                         "billed_in_advance": billed_in_advance,
+                        "conversion_rate": conversion_rate,
                         "external_price_id": external_price_id,
                         "fixed_price_quantity": fixed_price_quantity,
                         "invoice_grouping_key": invoice_grouping_key,
                         "package_config": package_config,
                         "matrix_config": matrix_config,
                         "matrix_with_allocation_config": matrix_with_allocation_config,
                         "tiered_config": tiered_config,
                         "tiered_bps_config": tiered_bps_config,
                         "bps_config": bps_config,
                         "bulk_bps_config": bulk_bps_config,
                         "bulk_config": bulk_config,
                         "threshold_total_amount_config": threshold_total_amount_config,
                         "tiered_package_config": tiered_package_config,
+                        "grouped_tiered_config": grouped_tiered_config,
                         "tiered_with_minimum_config": tiered_with_minimum_config,
                         "package_with_allocation_config": package_with_allocation_config,
                         "tiered_package_with_minimum_config": tiered_package_with_minimum_config,
                         "unit_with_percent_config": unit_with_percent_config,
                     },
                     price_create_params.PriceCreateParams,
                 ),
@@ -2518,14 +2862,107 @@
                     },
                     price_list_params.PriceListParams,
                 ),
             ),
             model=cast(Any, Price),  # Union types cannot be passed in as arguments in the type system
         )
 
+    async def evaluate(
+        self,
+        price_id: str,
+        *,
+        timeframe_end: Union[str, datetime],
+        timeframe_start: Union[str, datetime],
+        customer_id: Optional[str] | NotGiven = NOT_GIVEN,
+        external_customer_id: Optional[str] | NotGiven = NOT_GIVEN,
+        filter: Optional[str] | NotGiven = NOT_GIVEN,
+        grouping_keys: List[str] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> PriceEvaluateResponse:
+        """
+        This endpoint is used to evaluate the output of a price for a given customer and
+        time range. It enables filtering and grouping the output using
+        [computed properties](../guides/extensibility/advanced-metrics#computed-properties),
+        supporting the following workflows:
+
+        1. Showing detailed usage and costs to the end customer.
+        2. Auditing subtotals on invoice line items.
+
+        For these workflows, the expressiveness of computed properties in both the
+        filters and grouping is critical. For example, if you'd like to show your
+        customer their usage grouped by hour and another property, you can do so with
+        the following `grouping_keys`:
+        `["hour_floor_timestamp_millis(timestamp_millis)", "my_property"]`. If you'd
+        like to examine a customer's usage for a specific property value, you can do so
+        with the following `filter`:
+        `my_property = 'foo' AND my_other_property = 'bar'`.
+
+        By default, the start of the time range must be no more than 100 days ago and
+        the length of the results must be no greater than 1000. Note that this is a POST
+        endpoint rather than a GET endpoint because it employs a JSON body rather than
+        query parameters.
+
+        Args:
+          timeframe_end: The exclusive upper bound for event timestamps
+
+          timeframe_start: The inclusive lower bound for event timestamps
+
+          customer_id: The ID of the customer to which this evaluation is scoped.
+
+          external_customer_id: The external customer ID of the customer to which this evaluation is scoped.
+
+          filter: A boolean
+              [computed property](../guides/extensibility/advanced-metrics#computed-properties)
+              used to filter the underlying billable metric
+
+          grouping_keys: Properties (or
+              [computed properties](../guides/extensibility/advanced-metrics#computed-properties))
+              used to group the underlying billable metric
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        if not price_id:
+            raise ValueError(f"Expected a non-empty value for `price_id` but received {price_id!r}")
+        return await self._post(
+            f"/prices/{price_id}/evaluate",
+            body=await async_maybe_transform(
+                {
+                    "timeframe_end": timeframe_end,
+                    "timeframe_start": timeframe_start,
+                    "customer_id": customer_id,
+                    "external_customer_id": external_customer_id,
+                    "filter": filter,
+                    "grouping_keys": grouping_keys,
+                },
+                price_evaluate_params.PriceEvaluateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=PriceEvaluateResponse,
+        )
+
     async def fetch(
         self,
         price_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -2565,14 +3002,17 @@
 
         self.create = _legacy_response.to_raw_response_wrapper(
             prices.create,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
             prices.list,
         )
+        self.evaluate = _legacy_response.to_raw_response_wrapper(
+            prices.evaluate,
+        )
         self.fetch = _legacy_response.to_raw_response_wrapper(
             prices.fetch,
         )
 
     @cached_property
     def external_price_id(self) -> ExternalPriceIDWithRawResponse:
         return ExternalPriceIDWithRawResponse(self._prices.external_price_id)
@@ -2584,14 +3024,17 @@
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
             prices.create,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
             prices.list,
         )
+        self.evaluate = _legacy_response.async_to_raw_response_wrapper(
+            prices.evaluate,
+        )
         self.fetch = _legacy_response.async_to_raw_response_wrapper(
             prices.fetch,
         )
 
     @cached_property
     def external_price_id(self) -> AsyncExternalPriceIDWithRawResponse:
         return AsyncExternalPriceIDWithRawResponse(self._prices.external_price_id)
@@ -2603,14 +3046,17 @@
 
         self.create = to_streamed_response_wrapper(
             prices.create,
         )
         self.list = to_streamed_response_wrapper(
             prices.list,
         )
+        self.evaluate = to_streamed_response_wrapper(
+            prices.evaluate,
+        )
         self.fetch = to_streamed_response_wrapper(
             prices.fetch,
         )
 
     @cached_property
     def external_price_id(self) -> ExternalPriceIDWithStreamingResponse:
         return ExternalPriceIDWithStreamingResponse(self._prices.external_price_id)
@@ -2622,14 +3068,17 @@
 
         self.create = async_to_streamed_response_wrapper(
             prices.create,
         )
         self.list = async_to_streamed_response_wrapper(
             prices.list,
         )
+        self.evaluate = async_to_streamed_response_wrapper(
+            prices.evaluate,
+        )
         self.fetch = async_to_streamed_response_wrapper(
             prices.fetch,
         )
 
     @cached_property
     def external_price_id(self) -> AsyncExternalPriceIDWithStreamingResponse:
         return AsyncExternalPriceIDWithStreamingResponse(self._prices.external_price_id)
```

### Comparing `orb_billing-1.47.1/src/orb/types/__init__.py` & `orb_billing-1.48.0/src/orb/types/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 from __future__ import annotations
 
 from .item import Item as Item
 from .plan import Plan as Plan
 from .price import Price as Price
 from .coupon import Coupon as Coupon
-from .shared import Discount as Discount
+from .shared import (
+    Discount as Discount,
+    PaginationMetadata as PaginationMetadata,
+    BillingCycleRelativeDate as BillingCycleRelativeDate,
+)
 from .invoice import Invoice as Invoice
 from .customer import Customer as Customer
 from .credit_note import CreditNote as CreditNote
 from .subscription import Subscription as Subscription
 from .subscriptions import Subscriptions as Subscriptions
 from .item_list_params import ItemListParams as ItemListParams
 from .plan_list_params import PlanListParams as PlanListParams
@@ -24,31 +28,35 @@
 from .event_ingest_params import EventIngestParams as EventIngestParams
 from .event_search_params import EventSearchParams as EventSearchParams
 from .event_update_params import EventUpdateParams as EventUpdateParams
 from .invoice_list_params import InvoiceListParams as InvoiceListParams
 from .price_create_params import PriceCreateParams as PriceCreateParams
 from .coupon_create_params import CouponCreateParams as CouponCreateParams
 from .customer_list_params import CustomerListParams as CustomerListParams
+from .evaluate_price_group import EvaluatePriceGroup as EvaluatePriceGroup
 from .metric_create_params import MetricCreateParams as MetricCreateParams
 from .metric_list_response import MetricListResponse as MetricListResponse
 from .event_ingest_response import EventIngestResponse as EventIngestResponse
 from .event_search_response import EventSearchResponse as EventSearchResponse
 from .event_update_response import EventUpdateResponse as EventUpdateResponse
 from .invoice_create_params import InvoiceCreateParams as InvoiceCreateParams
 from .metric_fetch_response import MetricFetchResponse as MetricFetchResponse
+from .price_evaluate_params import PriceEvaluateParams as PriceEvaluateParams
 from .customer_create_params import CustomerCreateParams as CustomerCreateParams
 from .customer_update_params import CustomerUpdateParams as CustomerUpdateParams
 from .metric_create_response import MetricCreateResponse as MetricCreateResponse
 from .credit_note_list_params import CreditNoteListParams as CreditNoteListParams
+from .price_evaluate_response import PriceEvaluateResponse as PriceEvaluateResponse
 from .top_level_ping_response import TopLevelPingResponse as TopLevelPingResponse
 from .event_deprecate_response import EventDeprecateResponse as EventDeprecateResponse
 from .invoice_mark_paid_params import InvoiceMarkPaidParams as InvoiceMarkPaidParams
 from .subscription_list_params import SubscriptionListParams as SubscriptionListParams
 from .subscription_cancel_params import SubscriptionCancelParams as SubscriptionCancelParams
 from .subscription_create_params import SubscriptionCreateParams as SubscriptionCreateParams
+from .subscription_update_params import SubscriptionUpdateParams as SubscriptionUpdateParams
 from .invoice_fetch_upcoming_params import InvoiceFetchUpcomingParams as InvoiceFetchUpcomingParams
 from .invoice_fetch_upcoming_response import InvoiceFetchUpcomingResponse as InvoiceFetchUpcomingResponse
 from .invoice_line_item_create_params import InvoiceLineItemCreateParams as InvoiceLineItemCreateParams
 from .subscription_fetch_costs_params import SubscriptionFetchCostsParams as SubscriptionFetchCostsParams
 from .subscription_fetch_usage_params import SubscriptionFetchUsageParams as SubscriptionFetchUsageParams
 from .invoice_line_item_create_response import InvoiceLineItemCreateResponse as InvoiceLineItemCreateResponse
 from .subscription_fetch_costs_response import SubscriptionFetchCostsResponse as SubscriptionFetchCostsResponse
```

### Comparing `orb_billing-1.47.1/src/orb/types/coupon.py` & `orb_billing-1.48.0/src/orb/types/coupon.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/coupon_create_params.py` & `orb_billing-1.48.0/src/orb/types/coupon_create_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import List, Union, Optional
+from typing import Union, Optional
 from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["CouponCreateParams", "Discount", "DiscountPercentageDiscount", "DiscountAmountDiscount"]
+__all__ = ["CouponCreateParams", "Discount", "DiscountNewCouponPercentageDiscount", "DiscountNewCouponAmountDiscount"]
 
 
 class CouponCreateParams(TypedDict, total=False):
     discount: Required[Discount]
 
     redemption_code: Required[str]
     """This string can be used to redeem this coupon for a given subscription."""
@@ -23,41 +23,20 @@
     max_redemptions: Optional[int]
     """
     The maximum number of redemptions allowed for this coupon before it is
     exhausted;`null` here means "unlimited".
     """
 
 
-class DiscountPercentageDiscount(TypedDict, total=False):
-    applies_to_price_ids: Required[List[str]]
-    """List of price_ids that this discount applies to.
-
-    For plan/plan phase discounts, this can be a subset of prices.
-    """
-
+class DiscountNewCouponPercentageDiscount(TypedDict, total=False):
     discount_type: Required[Literal["percentage"]]
 
     percentage_discount: Required[float]
-    """Only available if discount_type is `percentage`.
-
-    This is a number between 0 and 1.
-    """
 
-    reason: Optional[str]
 
-
-class DiscountAmountDiscount(TypedDict, total=False):
+class DiscountNewCouponAmountDiscount(TypedDict, total=False):
     amount_discount: Required[str]
-    """Only available if discount_type is `amount`."""
-
-    applies_to_price_ids: Required[List[str]]
-    """List of price_ids that this discount applies to.
-
-    For plan/plan phase discounts, this can be a subset of prices.
-    """
 
     discount_type: Required[Literal["amount"]]
 
-    reason: Optional[str]
-
 
-Discount = Union[DiscountPercentageDiscount, DiscountAmountDiscount]
+Discount = Union[DiscountNewCouponPercentageDiscount, DiscountNewCouponAmountDiscount]
```

### Comparing `orb_billing-1.47.1/src/orb/types/coupon_list_params.py` & `orb_billing-1.48.0/src/orb/types/coupon_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/credit_note.py` & `orb_billing-1.48.0/src/orb/types/credit_note.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customer.py` & `orb_billing-1.48.0/src/orb/types/customer.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customer_create_params.py` & `orb_billing-1.48.0/src/orb/types/customer_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customer_list_params.py` & `orb_billing-1.48.0/src/orb/types/customer_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customer_update_by_external_id_params.py` & `orb_billing-1.48.0/src/orb/types/customer_update_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customer_update_params.py` & `orb_billing-1.48.0/src/orb/types/customer_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/event_ingest_params.py` & `orb_billing-1.48.0/src/orb/types/event_ingest_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/event_ingest_response.py` & `orb_billing-1.48.0/src/orb/types/event_ingest_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/event_search_params.py` & `orb_billing-1.48.0/src/orb/types/event_search_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/event_search_response.py` & `orb_billing-1.48.0/src/orb/types/event_search_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/event_update_params.py` & `orb_billing-1.48.0/src/orb/types/event_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/invoice.py` & `orb_billing-1.48.0/src/orb/types/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, List, Union, Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from .price import Price
-from .shared import Discount
 from .._models import BaseModel
+from .shared.discount import Discount
 
 __all__ = [
     "Invoice",
     "AutoCollection",
     "BillingAddress",
     "CreditNote",
     "Customer",
@@ -859,14 +859,16 @@
     Invoice numbers have a prefix such as `RFOBWG`. These can be sequential per
     account or customer.
     """
 
     invoice_pdf: Optional[str] = None
     """The link to download the PDF representation of the `Invoice`."""
 
+    invoice_source: Literal["subscription", "partial", "one_off"]
+
     issue_failed_at: Optional[datetime] = None
     """
     If the invoice failed to issue, this will be the last time it failed to issue
     (even if it is now in a different state.)
     """
 
     issued_at: Optional[datetime] = None
```

### Comparing `orb_billing-1.47.1/src/orb/types/invoice_create_params.py` & `orb_billing-1.48.0/src/orb/types/invoice_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/invoice_fetch_upcoming_response.py` & `orb_billing-1.48.0/src/orb/types/invoice_fetch_upcoming_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, List, Union, Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from .price import Price
-from .shared import Discount
 from .._models import BaseModel
+from .shared.discount import Discount
 
 __all__ = [
     "InvoiceFetchUpcomingResponse",
     "AutoCollection",
     "BillingAddress",
     "CreditNote",
     "Customer",
@@ -856,14 +856,16 @@
     Invoice numbers have a prefix such as `RFOBWG`. These can be sequential per
     account or customer.
     """
 
     invoice_pdf: Optional[str] = None
     """The link to download the PDF representation of the `Invoice`."""
 
+    invoice_source: Literal["subscription", "partial", "one_off"]
+
     issue_failed_at: Optional[datetime] = None
     """
     If the invoice failed to issue, this will be the last time it failed to issue
     (even if it is now in a different state.)
     """
 
     issued_at: Optional[datetime] = None
```

### Comparing `orb_billing-1.47.1/src/orb/types/invoice_line_item_create_params.py` & `orb_billing-1.48.0/src/orb/types/invoice_line_item_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/invoice_line_item_create_response.py` & `orb_billing-1.48.0/src/orb/types/invoice_line_item_create_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import List, Union, Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from .price import Price
-from .shared import Discount
 from .._models import BaseModel
+from .shared.discount import Discount
 
 __all__ = [
     "InvoiceLineItemCreateResponse",
     "Maximum",
     "Minimum",
     "SubLineItem",
     "SubLineItemMatrixSubLineItem",
```

### Comparing `orb_billing-1.47.1/src/orb/types/invoice_list_params.py` & `orb_billing-1.48.0/src/orb/types/invoice_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/invoice_mark_paid_params.py` & `orb_billing-1.48.0/src/orb/types/invoice_mark_paid_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/item.py` & `orb_billing-1.48.0/src/orb/types/item.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/metric_create_params.py` & `orb_billing-1.48.0/src/orb/types/metric_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/metric_create_response.py` & `orb_billing-1.48.0/src/orb/types/metric_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/metric_fetch_response.py` & `orb_billing-1.48.0/src/orb/types/metric_fetch_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/metric_list_params.py` & `orb_billing-1.48.0/src/orb/types/metric_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/metric_list_response.py` & `orb_billing-1.48.0/src/orb/types/metric_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/plan.py` & `orb_billing-1.48.0/src/orb/types/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, List, Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from .price import Price
-from .shared import Discount
 from .._models import BaseModel
+from .shared.discount import Discount
 
 __all__ = [
     "Plan",
     "BasePlan",
     "Maximum",
     "Minimum",
     "PlanPhase",
```

### Comparing `orb_billing-1.47.1/src/orb/types/plan_create_params.py` & `orb_billing-1.48.0/src/orb/types/plan_create_params.py`

 * *Files 19% similar despite different names*

```diff
@@ -101,14 +101,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -118,15 +127,15 @@
     """The property used to group this price on an invoice"""
 
 
 class PriceNewPlanPackagePricePackageConfig(TypedDict, total=False):
     package_amount: Required[str]
     """A currency amount to rate usage by"""
 
-    package_size: Optional[int]
+    package_size: Required[int]
     """An integer amount to represent package size.
 
     For example, 1000 here would divide usage by 1000 before multiplying by
     package_amount in rating
     """
 
 
@@ -152,14 +161,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -214,14 +232,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -269,14 +296,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -330,14 +366,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -377,14 +422,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -435,14 +489,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -487,14 +550,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -526,14 +598,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -565,14 +646,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -604,14 +694,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -643,14 +742,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -682,14 +790,23 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
```

### Comparing `orb_billing-1.47.1/src/orb/types/plan_list_params.py` & `orb_billing-1.48.0/src/orb/types/plan_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/plan_update_params.py` & `orb_billing-1.48.0/src/orb/types/plan_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/price.py` & `orb_billing-1.48.0/src/orb/types/price.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,111 +2,143 @@
 
 from typing import Dict, List, Union, Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from pydantic import Field as FieldInfo
 
-from .shared import Discount
 from .._models import BaseModel
+from .shared.discount import Discount
 
 __all__ = [
     "Price",
     "UnitPrice",
     "UnitPriceBillableMetric",
+    "UnitPriceCreditAllocation",
     "UnitPriceItem",
     "UnitPriceMaximum",
     "UnitPriceMinimum",
     "UnitPriceUnitConfig",
     "PackagePrice",
     "PackagePriceBillableMetric",
+    "PackagePriceCreditAllocation",
     "PackagePriceItem",
     "PackagePriceMaximum",
     "PackagePriceMinimum",
     "PackagePricePackageConfig",
     "MatrixPrice",
     "MatrixPriceBillableMetric",
+    "MatrixPriceCreditAllocation",
     "MatrixPriceItem",
     "MatrixPriceMatrixConfig",
     "MatrixPriceMatrixConfigMatrixValue",
     "MatrixPriceMaximum",
     "MatrixPriceMinimum",
     "TieredPrice",
     "TieredPriceBillableMetric",
+    "TieredPriceCreditAllocation",
     "TieredPriceItem",
     "TieredPriceMaximum",
     "TieredPriceMinimum",
     "TieredPriceTieredConfig",
     "TieredPriceTieredConfigTier",
     "TieredBpsPrice",
     "TieredBpsPriceBillableMetric",
+    "TieredBpsPriceCreditAllocation",
     "TieredBpsPriceItem",
     "TieredBpsPriceMaximum",
     "TieredBpsPriceMinimum",
     "TieredBpsPriceTieredBpsConfig",
     "TieredBpsPriceTieredBpsConfigTier",
     "BpsPrice",
     "BpsPriceBillableMetric",
     "BpsPriceBpsConfig",
+    "BpsPriceCreditAllocation",
     "BpsPriceItem",
     "BpsPriceMaximum",
     "BpsPriceMinimum",
     "BulkBpsPrice",
     "BulkBpsPriceBillableMetric",
     "BulkBpsPriceBulkBpsConfig",
     "BulkBpsPriceBulkBpsConfigTier",
+    "BulkBpsPriceCreditAllocation",
     "BulkBpsPriceItem",
     "BulkBpsPriceMaximum",
     "BulkBpsPriceMinimum",
     "BulkPrice",
     "BulkPriceBillableMetric",
     "BulkPriceBulkConfig",
     "BulkPriceBulkConfigTier",
+    "BulkPriceCreditAllocation",
     "BulkPriceItem",
     "BulkPriceMaximum",
     "BulkPriceMinimum",
     "ThresholdTotalAmountPrice",
     "ThresholdTotalAmountPriceBillableMetric",
+    "ThresholdTotalAmountPriceCreditAllocation",
     "ThresholdTotalAmountPriceItem",
     "ThresholdTotalAmountPriceMaximum",
     "ThresholdTotalAmountPriceMinimum",
     "TieredPackagePrice",
     "TieredPackagePriceBillableMetric",
+    "TieredPackagePriceCreditAllocation",
     "TieredPackagePriceItem",
     "TieredPackagePriceMaximum",
     "TieredPackagePriceMinimum",
+    "GroupedTieredPrice",
+    "GroupedTieredPriceBillableMetric",
+    "GroupedTieredPriceCreditAllocation",
+    "GroupedTieredPriceItem",
+    "GroupedTieredPriceMaximum",
+    "GroupedTieredPriceMinimum",
     "TieredWithMinimumPrice",
     "TieredWithMinimumPriceBillableMetric",
+    "TieredWithMinimumPriceCreditAllocation",
     "TieredWithMinimumPriceItem",
     "TieredWithMinimumPriceMaximum",
     "TieredWithMinimumPriceMinimum",
+    "TieredPackageWithMinimumPrice",
+    "TieredPackageWithMinimumPriceBillableMetric",
+    "TieredPackageWithMinimumPriceCreditAllocation",
+    "TieredPackageWithMinimumPriceItem",
+    "TieredPackageWithMinimumPriceMaximum",
+    "TieredPackageWithMinimumPriceMinimum",
     "PackageWithAllocationPrice",
     "PackageWithAllocationPriceBillableMetric",
+    "PackageWithAllocationPriceCreditAllocation",
     "PackageWithAllocationPriceItem",
     "PackageWithAllocationPriceMaximum",
     "PackageWithAllocationPriceMinimum",
     "UnitWithPercentPrice",
     "UnitWithPercentPriceBillableMetric",
+    "UnitWithPercentPriceCreditAllocation",
     "UnitWithPercentPriceItem",
     "UnitWithPercentPriceMaximum",
     "UnitWithPercentPriceMinimum",
     "MatrixWithAllocationPrice",
     "MatrixWithAllocationPriceBillableMetric",
+    "MatrixWithAllocationPriceCreditAllocation",
     "MatrixWithAllocationPriceItem",
     "MatrixWithAllocationPriceMatrixWithAllocationConfig",
     "MatrixWithAllocationPriceMatrixWithAllocationConfigMatrixValue",
     "MatrixWithAllocationPriceMaximum",
     "MatrixWithAllocationPriceMinimum",
 ]
 
 
 class UnitPriceBillableMetric(BaseModel):
     id: str
 
 
+class UnitPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class UnitPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class UnitPriceMaximum(BaseModel):
@@ -139,16 +171,20 @@
 class UnitPrice(BaseModel):
     id: str
 
     billable_metric: Optional[UnitPriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[UnitPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -174,14 +210,20 @@
     unit_config: UnitPriceUnitConfig
 
 
 class PackagePriceBillableMetric(BaseModel):
     id: str
 
 
+class PackagePriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class PackagePriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class PackagePriceMaximum(BaseModel):
@@ -206,31 +248,35 @@
     """Minimum amount applied"""
 
 
 class PackagePricePackageConfig(BaseModel):
     package_amount: str
     """A currency amount to rate usage by"""
 
-    package_size: Optional[int] = None
+    package_size: int
     """An integer amount to represent package size.
 
     For example, 1000 here would divide usage by 1000 before multiplying by
     package_amount in rating
     """
 
 
 class PackagePrice(BaseModel):
     id: str
 
     billable_metric: Optional[PackagePriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[PackagePriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -256,14 +302,20 @@
     price_type: Literal["usage_price", "fixed_price"]
 
 
 class MatrixPriceBillableMetric(BaseModel):
     id: str
 
 
+class MatrixPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class MatrixPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class MatrixPriceMatrixConfigMatrixValue(BaseModel):
@@ -314,16 +366,20 @@
 class MatrixPrice(BaseModel):
     id: str
 
     billable_metric: Optional[MatrixPriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[MatrixPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -349,14 +405,20 @@
     price_type: Literal["usage_price", "fixed_price"]
 
 
 class TieredPriceBillableMetric(BaseModel):
     id: str
 
 
+class TieredPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class TieredPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class TieredPriceMaximum(BaseModel):
@@ -400,16 +462,20 @@
 class TieredPrice(BaseModel):
     id: str
 
     billable_metric: Optional[TieredPriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[TieredPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -435,14 +501,20 @@
     tiered_config: TieredPriceTieredConfig
 
 
 class TieredBpsPriceBillableMetric(BaseModel):
     id: str
 
 
+class TieredBpsPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class TieredBpsPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class TieredBpsPriceMaximum(BaseModel):
@@ -492,16 +564,20 @@
 class TieredBpsPrice(BaseModel):
     id: str
 
     billable_metric: Optional[TieredBpsPriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[TieredBpsPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -535,14 +611,20 @@
     bps: float
     """Basis point take rate per event"""
 
     per_unit_maximum: Optional[str] = None
     """Optional currency amount maximum to cap spend per event"""
 
 
+class BpsPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class BpsPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class BpsPriceMaximum(BaseModel):
@@ -572,16 +654,20 @@
 
     billable_metric: Optional[BpsPriceBillableMetric] = None
 
     bps_config: BpsPriceBpsConfig
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[BpsPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -624,14 +710,20 @@
     tiers: List[BulkBpsPriceBulkBpsConfigTier]
     """
     Tiers for a bulk BPS pricing model where all usage is aggregated to a single
     tier based on total volume
     """
 
 
+class BulkBpsPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class BulkBpsPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class BulkBpsPriceMaximum(BaseModel):
@@ -661,16 +753,20 @@
 
     billable_metric: Optional[BulkBpsPriceBillableMetric] = None
 
     bulk_bps_config: BulkBpsPriceBulkBpsConfig
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[BulkBpsPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -707,14 +803,20 @@
 
 
 class BulkPriceBulkConfig(BaseModel):
     tiers: List[BulkPriceBulkConfigTier]
     """Bulk tiers for rating based on total usage volume"""
 
 
+class BulkPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class BulkPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class BulkPriceMaximum(BaseModel):
@@ -744,16 +846,20 @@
 
     billable_metric: Optional[BulkPriceBillableMetric] = None
 
     bulk_config: BulkPriceBulkConfig
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[BulkPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -777,14 +883,20 @@
     price_type: Literal["usage_price", "fixed_price"]
 
 
 class ThresholdTotalAmountPriceBillableMetric(BaseModel):
     id: str
 
 
+class ThresholdTotalAmountPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class ThresholdTotalAmountPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class ThresholdTotalAmountPriceMaximum(BaseModel):
@@ -812,16 +924,20 @@
 class ThresholdTotalAmountPrice(BaseModel):
     id: str
 
     billable_metric: Optional[ThresholdTotalAmountPriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[ThresholdTotalAmountPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -847,14 +963,20 @@
     threshold_total_amount_config: Dict[str, object]
 
 
 class TieredPackagePriceBillableMetric(BaseModel):
     id: str
 
 
+class TieredPackagePriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class TieredPackagePriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class TieredPackagePriceMaximum(BaseModel):
@@ -882,16 +1004,20 @@
 class TieredPackagePrice(BaseModel):
     id: str
 
     billable_metric: Optional[TieredPackagePriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[TieredPackagePriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -913,18 +1039,104 @@
     plan_phase_order: Optional[int] = None
 
     price_type: Literal["usage_price", "fixed_price"]
 
     tiered_package_config: Dict[str, object]
 
 
+class GroupedTieredPriceBillableMetric(BaseModel):
+    id: str
+
+
+class GroupedTieredPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
+class GroupedTieredPriceItem(BaseModel):
+    id: str
+
+    name: str
+
+
+class GroupedTieredPriceMaximum(BaseModel):
+    applies_to_price_ids: List[str]
+    """List of price_ids that this maximum amount applies to.
+
+    For plan/plan phase maximums, this can be a subset of prices.
+    """
+
+    maximum_amount: str
+    """Maximum amount applied"""
+
+
+class GroupedTieredPriceMinimum(BaseModel):
+    applies_to_price_ids: List[str]
+    """List of price_ids that this minimum amount applies to.
+
+    For plan/plan phase minimums, this can be a subset of prices.
+    """
+
+    minimum_amount: str
+    """Minimum amount applied"""
+
+
+class GroupedTieredPrice(BaseModel):
+    id: str
+
+    billable_metric: Optional[GroupedTieredPriceBillableMetric] = None
+
+    cadence: Literal["one_time", "monthly", "quarterly", "annual"]
+
+    conversion_rate: Optional[float] = None
+
+    created_at: datetime
+
+    credit_allocation: Optional[GroupedTieredPriceCreditAllocation] = None
+
+    currency: str
+
+    discount: Optional[Discount] = None
+
+    external_price_id: Optional[str] = None
+
+    fixed_price_quantity: Optional[float] = None
+
+    grouped_tiered_config: Dict[str, object]
+
+    item: GroupedTieredPriceItem
+
+    maximum: Optional[GroupedTieredPriceMaximum] = None
+
+    maximum_amount: Optional[str] = None
+
+    minimum: Optional[GroupedTieredPriceMinimum] = None
+
+    minimum_amount: Optional[str] = None
+
+    price_model_type: Literal["grouped_tiered"] = FieldInfo(alias="model_type")
+
+    name: str
+
+    plan_phase_order: Optional[int] = None
+
+    price_type: Literal["usage_price", "fixed_price"]
+
+
 class TieredWithMinimumPriceBillableMetric(BaseModel):
     id: str
 
 
+class TieredWithMinimumPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class TieredWithMinimumPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class TieredWithMinimumPriceMaximum(BaseModel):
@@ -952,16 +1164,20 @@
 class TieredWithMinimumPrice(BaseModel):
     id: str
 
     billable_metric: Optional[TieredWithMinimumPriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[TieredWithMinimumPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -983,18 +1199,104 @@
     plan_phase_order: Optional[int] = None
 
     price_type: Literal["usage_price", "fixed_price"]
 
     tiered_with_minimum_config: Dict[str, object]
 
 
+class TieredPackageWithMinimumPriceBillableMetric(BaseModel):
+    id: str
+
+
+class TieredPackageWithMinimumPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
+class TieredPackageWithMinimumPriceItem(BaseModel):
+    id: str
+
+    name: str
+
+
+class TieredPackageWithMinimumPriceMaximum(BaseModel):
+    applies_to_price_ids: List[str]
+    """List of price_ids that this maximum amount applies to.
+
+    For plan/plan phase maximums, this can be a subset of prices.
+    """
+
+    maximum_amount: str
+    """Maximum amount applied"""
+
+
+class TieredPackageWithMinimumPriceMinimum(BaseModel):
+    applies_to_price_ids: List[str]
+    """List of price_ids that this minimum amount applies to.
+
+    For plan/plan phase minimums, this can be a subset of prices.
+    """
+
+    minimum_amount: str
+    """Minimum amount applied"""
+
+
+class TieredPackageWithMinimumPrice(BaseModel):
+    id: str
+
+    billable_metric: Optional[TieredPackageWithMinimumPriceBillableMetric] = None
+
+    cadence: Literal["one_time", "monthly", "quarterly", "annual"]
+
+    conversion_rate: Optional[float] = None
+
+    created_at: datetime
+
+    credit_allocation: Optional[TieredPackageWithMinimumPriceCreditAllocation] = None
+
+    currency: str
+
+    discount: Optional[Discount] = None
+
+    external_price_id: Optional[str] = None
+
+    fixed_price_quantity: Optional[float] = None
+
+    item: TieredPackageWithMinimumPriceItem
+
+    maximum: Optional[TieredPackageWithMinimumPriceMaximum] = None
+
+    maximum_amount: Optional[str] = None
+
+    minimum: Optional[TieredPackageWithMinimumPriceMinimum] = None
+
+    minimum_amount: Optional[str] = None
+
+    price_model_type: Literal["tiered_package_with_minimum"] = FieldInfo(alias="model_type")
+
+    name: str
+
+    plan_phase_order: Optional[int] = None
+
+    price_type: Literal["usage_price", "fixed_price"]
+
+    tiered_package_with_minimum_config: Dict[str, object]
+
+
 class PackageWithAllocationPriceBillableMetric(BaseModel):
     id: str
 
 
+class PackageWithAllocationPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class PackageWithAllocationPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class PackageWithAllocationPriceMaximum(BaseModel):
@@ -1022,16 +1324,20 @@
 class PackageWithAllocationPrice(BaseModel):
     id: str
 
     billable_metric: Optional[PackageWithAllocationPriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[PackageWithAllocationPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -1057,14 +1363,20 @@
     price_type: Literal["usage_price", "fixed_price"]
 
 
 class UnitWithPercentPriceBillableMetric(BaseModel):
     id: str
 
 
+class UnitWithPercentPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class UnitWithPercentPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class UnitWithPercentPriceMaximum(BaseModel):
@@ -1092,16 +1404,20 @@
 class UnitWithPercentPrice(BaseModel):
     id: str
 
     billable_metric: Optional[UnitWithPercentPriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[UnitWithPercentPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -1127,14 +1443,20 @@
     unit_with_percent_config: Dict[str, object]
 
 
 class MatrixWithAllocationPriceBillableMetric(BaseModel):
     id: str
 
 
+class MatrixWithAllocationPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
 class MatrixWithAllocationPriceItem(BaseModel):
     id: str
 
     name: str
 
 
 class MatrixWithAllocationPriceMatrixWithAllocationConfigMatrixValue(BaseModel):
@@ -1188,16 +1510,20 @@
 class MatrixWithAllocationPrice(BaseModel):
     id: str
 
     billable_metric: Optional[MatrixWithAllocationPriceBillableMetric] = None
 
     cadence: Literal["one_time", "monthly", "quarterly", "annual"]
 
+    conversion_rate: Optional[float] = None
+
     created_at: datetime
 
+    credit_allocation: Optional[MatrixWithAllocationPriceCreditAllocation] = None
+
     currency: str
 
     discount: Optional[Discount] = None
 
     external_price_id: Optional[str] = None
 
     fixed_price_quantity: Optional[float] = None
@@ -1230,12 +1556,14 @@
     TieredPrice,
     TieredBpsPrice,
     BpsPrice,
     BulkBpsPrice,
     BulkPrice,
     ThresholdTotalAmountPrice,
     TieredPackagePrice,
+    GroupedTieredPrice,
     TieredWithMinimumPrice,
+    TieredPackageWithMinimumPrice,
     PackageWithAllocationPrice,
     UnitWithPercentPrice,
     MatrixWithAllocationPrice,
 ]
```

### Comparing `orb_billing-1.47.1/src/orb/types/price_create_params.py` & `orb_billing-1.48.0/src/orb/types/price_create_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "NewFloatingBulkBpsPriceBulkBpsConfig",
     "NewFloatingBulkBpsPriceBulkBpsConfigTier",
     "NewFloatingBulkPrice",
     "NewFloatingBulkPriceBulkConfig",
     "NewFloatingBulkPriceBulkConfigTier",
     "NewFloatingThresholdTotalAmountPrice",
     "NewFloatingTieredPackagePrice",
+    "NewFloatingGroupedTieredPrice",
     "NewFloatingTieredWithMinimumPrice",
     "NewFloatingPackageWithAllocationPrice",
     "NewFloatingTieredPackageWithMinimumPrice",
     "NewFloatingUnitWithPercentPrice",
 ]
 
 
@@ -65,14 +66,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -112,14 +116,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -129,15 +136,15 @@
     """The property used to group this price on an invoice"""
 
 
 class NewFloatingPackagePricePackageConfig(TypedDict, total=False):
     package_amount: Required[str]
     """A currency amount to rate usage by"""
 
-    package_size: Optional[int]
+    package_size: Required[int]
     """An integer amount to represent package size.
 
     For example, 1000 here would divide usage by 1000 before multiplying by
     package_amount in rating
     """
 
 
@@ -166,14 +173,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -231,14 +241,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -299,14 +312,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -357,14 +373,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -421,14 +440,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -471,14 +493,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -532,14 +557,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -587,14 +615,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -629,14 +660,62 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    external_price_id: Optional[str]
+    """An alias for the price."""
+
+    fixed_price_quantity: Optional[float]
+    """
+    If the Price represents a fixed cost, this represents the quantity of units
+    applied.
+    """
+
+    invoice_grouping_key: Optional[str]
+    """The property used to group this price on an invoice"""
+
+
+class NewFloatingGroupedTieredPrice(TypedDict, total=False):
+    cadence: Required[Literal["annual", "monthly", "quarterly", "one_time"]]
+    """The cadence to bill for this price on."""
+
+    currency: Required[str]
+    """An ISO 4217 currency string for which this price is billed in."""
+
+    grouped_tiered_config: Required[Dict[str, object]]
+
+    item_id: Required[str]
+    """The id of the item the plan will be associated with."""
+
+    model_type: Required[Literal["grouped_tiered"]]
+
+    name: Required[str]
+    """The name of the price."""
+
+    billable_metric_id: Optional[str]
+    """The id of the billable metric for the price.
+
+    Only needed if the price is usage-based.
+    """
+
+    billed_in_advance: Optional[bool]
+    """
+    If the Price represents a fixed cost, the price will be billed in-advance if
+    this is true, and in-arrears if this is false.
+    """
+
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -671,14 +750,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -713,14 +795,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -755,14 +840,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -797,14 +885,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -822,12 +913,13 @@
     NewFloatingTieredPrice,
     NewFloatingTieredBpsPrice,
     NewFloatingBpsPrice,
     NewFloatingBulkBpsPrice,
     NewFloatingBulkPrice,
     NewFloatingThresholdTotalAmountPrice,
     NewFloatingTieredPackagePrice,
+    NewFloatingGroupedTieredPrice,
     NewFloatingTieredWithMinimumPrice,
     NewFloatingPackageWithAllocationPrice,
     NewFloatingTieredPackageWithMinimumPrice,
     NewFloatingUnitWithPercentPrice,
 ]
```

### Comparing `orb_billing-1.47.1/src/orb/types/subscription.py` & `orb_billing-1.48.0/src/orb/types/subscription.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_cancel_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_cancel_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_create_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_create_params.py`

 * *Files 20% similar despite different names*

```diff
@@ -145,14 +145,23 @@
 class PriceOverrideOverrideUnitPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["unit"]]
 
     unit_config: Required[PriceOverrideOverrideUnitPriceUnitConfig]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideUnitPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -162,15 +171,15 @@
     """The subscription's override minimum amount for the plan."""
 
 
 class PriceOverrideOverridePackagePricePackageConfig(TypedDict, total=False):
     package_amount: Required[str]
     """A currency amount to rate usage by"""
 
-    package_size: Optional[int]
+    package_size: Required[int]
     """An integer amount to represent package size.
 
     For example, 1000 here would divide usage by 1000 before multiplying by
     package_amount in rating
     """
 
 
@@ -205,14 +214,23 @@
 class PriceOverrideOverridePackagePrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["package"]]
 
     package_config: Required[PriceOverrideOverridePackagePricePackageConfig]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverridePackagePriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -276,14 +294,23 @@
 class PriceOverrideOverrideMatrixPrice(TypedDict, total=False):
     id: Required[str]
 
     matrix_config: Required[PriceOverrideOverrideMatrixPriceMatrixConfig]
 
     model_type: Required[Literal["matrix"]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideMatrixPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -340,14 +367,23 @@
 class PriceOverrideOverrideTieredPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["tiered"]]
 
     tiered_config: Required[PriceOverrideOverrideTieredPriceTieredConfig]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideTieredPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -410,14 +446,23 @@
 class PriceOverrideOverrideTieredBpsPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["tiered_bps"]]
 
     tiered_bps_config: Required[PriceOverrideOverrideTieredBpsPriceTieredBpsConfig]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideTieredBpsPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -466,14 +511,23 @@
 class PriceOverrideOverrideBpsPrice(TypedDict, total=False):
     id: Required[str]
 
     bps_config: Required[PriceOverrideOverrideBpsPriceBpsConfig]
 
     model_type: Required[Literal["bps"]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideBpsPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -533,14 +587,23 @@
 class PriceOverrideOverrideBulkBpsPrice(TypedDict, total=False):
     id: Required[str]
 
     bulk_bps_config: Required[PriceOverrideOverrideBulkBpsPriceBulkBpsConfig]
 
     model_type: Required[Literal["bulk_bps"]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideBulkBpsPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -594,14 +657,23 @@
 class PriceOverrideOverrideBulkPrice(TypedDict, total=False):
     id: Required[str]
 
     bulk_config: Required[PriceOverrideOverrideBulkPriceBulkConfig]
 
     model_type: Required[Literal["bulk"]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideBulkPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -642,14 +714,23 @@
 class PriceOverrideOverrideThresholdTotalAmountPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["threshold_total_amount"]]
 
     threshold_total_amount_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideThresholdTotalAmountPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -690,14 +771,23 @@
 class PriceOverrideOverrideTieredPackagePrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["tiered_package"]]
 
     tiered_package_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideTieredPackagePriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -738,14 +828,23 @@
 class PriceOverrideOverrideTieredWithMinimumPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["tiered_with_minimum"]]
 
     tiered_with_minimum_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideTieredWithMinimumPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -786,14 +885,23 @@
 class PriceOverrideOverridePackageWithAllocationPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["package_with_allocation"]]
 
     package_with_allocation_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverridePackageWithAllocationPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -834,14 +942,23 @@
 class PriceOverrideOverrideUnitWithPercentPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["unit_with_percent"]]
 
     unit_with_percent_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideUnitWithPercentPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
```

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_fetch_costs_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_fetch_costs_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_fetch_costs_response.py` & `orb_billing-1.48.0/src/orb/types/subscription_fetch_costs_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_fetch_schedule_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_fetch_schedule_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_fetch_schedule_response.py` & `orb_billing-1.48.0/src/orb/types/subscription_fetch_schedule_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_fetch_usage_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_fetch_usage_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_list_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_price_intervals_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_price_intervals_params.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 from typing import Dict, List, Union, Iterable, Optional
 from datetime import datetime
 from typing_extensions import Literal, Required, Annotated, TypedDict
 
 from .._utils import PropertyInfo
+from .shared.billing_cycle_relative_date import BillingCycleRelativeDate
 
 __all__ = [
     "SubscriptionPriceIntervalsParams",
     "Add",
     "AddDiscount",
     "AddDiscountAmountDiscountCreationParams",
     "AddDiscountPercentageDiscountCreationParams",
@@ -39,14 +40,15 @@
     "AddPriceNewFloatingBulkBpsPriceBulkBpsConfig",
     "AddPriceNewFloatingBulkBpsPriceBulkBpsConfigTier",
     "AddPriceNewFloatingBulkPrice",
     "AddPriceNewFloatingBulkPriceBulkConfig",
     "AddPriceNewFloatingBulkPriceBulkConfigTier",
     "AddPriceNewFloatingThresholdTotalAmountPrice",
     "AddPriceNewFloatingTieredPackagePrice",
+    "AddPriceNewFloatingGroupedTieredPrice",
     "AddPriceNewFloatingTieredWithMinimumPrice",
     "AddPriceNewFloatingPackageWithAllocationPrice",
     "AddPriceNewFloatingTieredPackageWithMinimumPrice",
     "AddPriceNewFloatingUnitWithPercentPrice",
     "Edit",
     "EditFixedFeeQuantityTransition",
 ]
@@ -132,14 +134,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -149,15 +154,15 @@
     """The property used to group this price on an invoice"""
 
 
 class AddPriceNewFloatingPackagePricePackageConfig(TypedDict, total=False):
     package_amount: Required[str]
     """A currency amount to rate usage by"""
 
-    package_size: Optional[int]
+    package_size: Required[int]
     """An integer amount to represent package size.
 
     For example, 1000 here would divide usage by 1000 before multiplying by
     package_amount in rating
     """
 
 
@@ -186,14 +191,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -251,14 +259,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -319,14 +330,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -377,14 +391,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -441,14 +458,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -491,14 +511,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -552,14 +575,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -607,14 +633,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -649,14 +678,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -691,14 +723,62 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    external_price_id: Optional[str]
+    """An alias for the price."""
+
+    fixed_price_quantity: Optional[float]
+    """
+    If the Price represents a fixed cost, this represents the quantity of units
+    applied.
+    """
+
+    invoice_grouping_key: Optional[str]
+    """The property used to group this price on an invoice"""
+
+
+class AddPriceNewFloatingGroupedTieredPrice(TypedDict, total=False):
+    cadence: Required[Literal["annual", "monthly", "quarterly", "one_time"]]
+    """The cadence to bill for this price on."""
+
+    currency: Required[str]
+    """An ISO 4217 currency string for which this price is billed in."""
+
+    grouped_tiered_config: Required[Dict[str, object]]
+
+    item_id: Required[str]
+    """The id of the item the plan will be associated with."""
+
+    model_type: Required[Literal["grouped_tiered"]]
+
+    name: Required[str]
+    """The name of the price."""
+
+    billable_metric_id: Optional[str]
+    """The id of the billable metric for the price.
+
+    Only needed if the price is usage-based.
+    """
+
+    billed_in_advance: Optional[bool]
+    """
+    If the Price represents a fixed cost, the price will be billed in-advance if
+    this is true, and in-arrears if this is false.
+    """
+
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -733,14 +813,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -775,14 +858,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -817,14 +903,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -859,14 +948,17 @@
 
     billed_in_advance: Optional[bool]
     """
     If the Price represents a fixed cost, the price will be billed in-advance if
     this is true, and in-arrears if this is false.
     """
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
     external_price_id: Optional[str]
     """An alias for the price."""
 
     fixed_price_quantity: Optional[float]
     """
     If the Price represents a fixed cost, this represents the quantity of units
     applied.
@@ -884,36 +976,35 @@
     AddPriceNewFloatingTieredPrice,
     AddPriceNewFloatingTieredBpsPrice,
     AddPriceNewFloatingBpsPrice,
     AddPriceNewFloatingBulkBpsPrice,
     AddPriceNewFloatingBulkPrice,
     AddPriceNewFloatingThresholdTotalAmountPrice,
     AddPriceNewFloatingTieredPackagePrice,
+    AddPriceNewFloatingGroupedTieredPrice,
     AddPriceNewFloatingTieredWithMinimumPrice,
     AddPriceNewFloatingPackageWithAllocationPrice,
     AddPriceNewFloatingTieredPackageWithMinimumPrice,
     AddPriceNewFloatingUnitWithPercentPrice,
 ]
 
 
 class Add(TypedDict, total=False):
     start_date: Required[
-        Annotated[Union[Union[str, datetime], Literal["start_of_term", "end_of_term"]], PropertyInfo(format="iso8601")]
+        Annotated[Union[Union[str, datetime], BillingCycleRelativeDate], PropertyInfo(format="iso8601")]
     ]
     """The start date of the price interval.
 
     This is the date that the price will start billing on the subscription.
     """
 
     discounts: Optional[Iterable[AddDiscount]]
     """A list of discounts to initialize on the price interval."""
 
-    end_date: Annotated[
-        Union[Union[str, datetime], Literal["start_of_term", "end_of_term"], None], PropertyInfo(format="iso8601")
-    ]
+    end_date: Annotated[Union[Union[str, datetime], BillingCycleRelativeDate, None], PropertyInfo(format="iso8601")]
     """The end date of the price interval.
 
     This is the date that the price will stop billing on the subscription.
     """
 
     external_price_id: Optional[str]
     """The external price id of the price to add to the subscription."""
@@ -955,29 +1046,25 @@
     billing_cycle_day: Optional[int]
     """The updated billing cycle day for this price interval.
 
     If not specified, the billing cycle day will not be updated. Note that
     overlapping price intervals must have the same billing cycle day.
     """
 
-    end_date: Annotated[
-        Union[Union[str, datetime], Literal["start_of_term", "end_of_term"], None], PropertyInfo(format="iso8601")
-    ]
+    end_date: Annotated[Union[Union[str, datetime], BillingCycleRelativeDate, None], PropertyInfo(format="iso8601")]
     """The updated end date of this price interval.
 
     If not specified, the start date will not be updated.
     """
 
     fixed_fee_quantity_transitions: Optional[Iterable[EditFixedFeeQuantityTransition]]
     """A list of fixed fee quantity transitions to use for this price interval.
 
     Note that this list will overwrite all existing fixed fee quantity transitions
     on the price interval.
     """
 
-    start_date: Annotated[
-        Union[Union[str, datetime], Literal["start_of_term", "end_of_term"]], PropertyInfo(format="iso8601")
-    ]
+    start_date: Annotated[Union[Union[str, datetime], BillingCycleRelativeDate], PropertyInfo(format="iso8601")]
     """The updated start date of this price interval.
 
     If not specified, the start date will not be updated.
     """
```

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_schedule_plan_change_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_schedule_plan_change_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -145,14 +145,23 @@
 class PriceOverrideOverrideUnitPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["unit"]]
 
     unit_config: Required[PriceOverrideOverrideUnitPriceUnitConfig]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideUnitPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -162,15 +171,15 @@
     """The subscription's override minimum amount for the plan."""
 
 
 class PriceOverrideOverridePackagePricePackageConfig(TypedDict, total=False):
     package_amount: Required[str]
     """A currency amount to rate usage by"""
 
-    package_size: Optional[int]
+    package_size: Required[int]
     """An integer amount to represent package size.
 
     For example, 1000 here would divide usage by 1000 before multiplying by
     package_amount in rating
     """
 
 
@@ -205,14 +214,23 @@
 class PriceOverrideOverridePackagePrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["package"]]
 
     package_config: Required[PriceOverrideOverridePackagePricePackageConfig]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverridePackagePriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -276,14 +294,23 @@
 class PriceOverrideOverrideMatrixPrice(TypedDict, total=False):
     id: Required[str]
 
     matrix_config: Required[PriceOverrideOverrideMatrixPriceMatrixConfig]
 
     model_type: Required[Literal["matrix"]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideMatrixPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -340,14 +367,23 @@
 class PriceOverrideOverrideTieredPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["tiered"]]
 
     tiered_config: Required[PriceOverrideOverrideTieredPriceTieredConfig]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideTieredPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -410,14 +446,23 @@
 class PriceOverrideOverrideTieredBpsPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["tiered_bps"]]
 
     tiered_bps_config: Required[PriceOverrideOverrideTieredBpsPriceTieredBpsConfig]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideTieredBpsPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -466,14 +511,23 @@
 class PriceOverrideOverrideBpsPrice(TypedDict, total=False):
     id: Required[str]
 
     bps_config: Required[PriceOverrideOverrideBpsPriceBpsConfig]
 
     model_type: Required[Literal["bps"]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideBpsPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -533,14 +587,23 @@
 class PriceOverrideOverrideBulkBpsPrice(TypedDict, total=False):
     id: Required[str]
 
     bulk_bps_config: Required[PriceOverrideOverrideBulkBpsPriceBulkBpsConfig]
 
     model_type: Required[Literal["bulk_bps"]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideBulkBpsPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -594,14 +657,23 @@
 class PriceOverrideOverrideBulkPrice(TypedDict, total=False):
     id: Required[str]
 
     bulk_config: Required[PriceOverrideOverrideBulkPriceBulkConfig]
 
     model_type: Required[Literal["bulk"]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideBulkPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -642,14 +714,23 @@
 class PriceOverrideOverrideThresholdTotalAmountPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["threshold_total_amount"]]
 
     threshold_total_amount_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideThresholdTotalAmountPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -690,14 +771,23 @@
 class PriceOverrideOverrideTieredPackagePrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["tiered_package"]]
 
     tiered_package_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideTieredPackagePriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -738,14 +828,23 @@
 class PriceOverrideOverrideTieredWithMinimumPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["tiered_with_minimum"]]
 
     tiered_with_minimum_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideTieredWithMinimumPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -786,14 +885,23 @@
 class PriceOverrideOverridePackageWithAllocationPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["package_with_allocation"]]
 
     package_with_allocation_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverridePackageWithAllocationPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
@@ -834,14 +942,23 @@
 class PriceOverrideOverrideUnitWithPercentPrice(TypedDict, total=False):
     id: Required[str]
 
     model_type: Required[Literal["unit_with_percent"]]
 
     unit_with_percent_config: Required[Dict[str, object]]
 
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """The currency of the price.
+
+    If not provided, the currency of the plan will be used.
+    """
+
     discount: Optional[PriceOverrideOverrideUnitWithPercentPriceDiscount]
     """The subscription's override discount for the plan."""
 
     fixed_price_quantity: Optional[float]
     """The starting quantity of the price, if the price is a fixed price."""
 
     maximum_amount: Optional[str]
```

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_trigger_phase_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_trigger_phase_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_update_fixed_fee_quantity_params.py` & `orb_billing-1.48.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/subscription_usage.py` & `orb_billing-1.48.0/src/orb/types/subscription_usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import List, Union, Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
+from .shared.pagination_metadata import PaginationMetadata
 
 __all__ = [
     "SubscriptionUsage",
     "UngroupedSubscriptionUsage",
     "UngroupedSubscriptionUsageData",
     "UngroupedSubscriptionUsageDataBillableMetric",
     "UngroupedSubscriptionUsageDataUsage",
     "GroupedSubscriptionUsage",
     "GroupedSubscriptionUsageData",
     "GroupedSubscriptionUsageDataBillableMetric",
     "GroupedSubscriptionUsageDataMetricGroup",
     "GroupedSubscriptionUsageDataUsage",
-    "GroupedSubscriptionUsagePaginationMetadata",
 ]
 
 
 class UngroupedSubscriptionUsageDataBillableMetric(BaseModel):
     id: str
 
     name: str
@@ -73,20 +73,14 @@
     metric_group: GroupedSubscriptionUsageDataMetricGroup
 
     usage: List[GroupedSubscriptionUsageDataUsage]
 
     view_mode: Literal["periodic", "cumulative"]
 
 
-class GroupedSubscriptionUsagePaginationMetadata(BaseModel):
-    has_more: bool
-
-    next_cursor: Optional[str] = None
-
-
 class GroupedSubscriptionUsage(BaseModel):
     data: List[GroupedSubscriptionUsageData]
 
-    pagination_metadata: Optional[GroupedSubscriptionUsagePaginationMetadata] = None
+    pagination_metadata: Optional[PaginationMetadata] = None
 
 
 SubscriptionUsage = Union[UngroupedSubscriptionUsage, GroupedSubscriptionUsage]
```

### Comparing `orb_billing-1.47.1/src/orb/types/beta/price_evaluate_params.py` & `orb_billing-1.48.0/src/orb/types/beta/price_evaluate_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/coupons/subscription_list_params.py` & `orb_billing-1.48.0/src/orb/types/coupons/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/__init__.py` & `orb_billing-1.48.0/src/orb/types/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/balance_transaction_create_response.py` & `orb_billing-1.48.0/src/orb/types/customers/balance_transaction_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/balance_transaction_list_params.py` & `orb_billing-1.48.0/src/orb/types/customers/balance_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/balance_transaction_list_response.py` & `orb_billing-1.48.0/src/orb/types/customers/balance_transaction_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/cost_list_by_external_id_params.py` & `orb_billing-1.48.0/src/orb/types/customers/cost_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/cost_list_by_external_id_response.py` & `orb_billing-1.48.0/src/orb/types/customers/cost_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/cost_list_params.py` & `orb_billing-1.48.0/src/orb/types/customers/cost_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/cost_list_response.py` & `orb_billing-1.48.0/src/orb/types/customers/cost_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credit_list_by_external_id_params.py` & `orb_billing-1.48.0/src/orb/types/customers/credit_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credit_list_params.py` & `orb_billing-1.48.0/src/orb/types/customers/credit_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/usage_update_by_external_id_params.py` & `orb_billing-1.48.0/src/orb/types/customers/usage_update_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/usage_update_by_external_id_response.py` & `orb_billing-1.48.0/src/orb/types/customers/usage_update_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/usage_update_params.py` & `orb_billing-1.48.0/src/orb/types/customers/usage_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/__init__.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     Individual keys can be removed by setting the value to `null`, and the entire
     metadata mapping can be cleared by setting `metadata` to `null`.
     """
 
     per_unit_cost_basis: Optional[str]
     """Can only be specified when entry_type=increment.
 
-    How much, in USD, a customer paid for a single credit in this block
+    How much, in the customer's currency, a customer paid for a single credit in
+    this block
     """
 
 
 class AddIncrementCreditLedgerEntryRequestParamsInvoiceSettings(TypedDict, total=False):
     auto_collection: Required[bool]
     """
     Whether the credits purchase invoice should auto collect with the customer's
@@ -86,14 +87,20 @@
     date for the invoice. If you intend the invoice to be due on issue, set this
     to 0.
     """
 
     memo: Optional[str]
     """An optional memo to display on the invoice."""
 
+    require_successful_payment: bool
+    """
+    If true, the new credit block will require that the corresponding invoice is
+    paid before it can be drawn down from.
+    """
+
 
 class AddDecrementCreditLedgerEntryRequestParams(TypedDict, total=False):
     amount: Required[float]
     """The number of credits to effect.
 
     Note that this is required for increment, decrement, void, or undo operations.
     """
```

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/ledger_create_entry_params.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     Individual keys can be removed by setting the value to `null`, and the entire
     metadata mapping can be cleared by setting `metadata` to `null`.
     """
 
     per_unit_cost_basis: Optional[str]
     """Can only be specified when entry_type=increment.
 
-    How much, in USD, a customer paid for a single credit in this block
+    How much, in the customer's currency, a customer paid for a single credit in
+    this block
     """
 
 
 class AddIncrementCreditLedgerEntryRequestParamsInvoiceSettings(TypedDict, total=False):
     auto_collection: Required[bool]
     """
     Whether the credits purchase invoice should auto collect with the customer's
@@ -86,14 +87,20 @@
     date for the invoice. If you intend the invoice to be due on issue, set this
     to 0.
     """
 
     memo: Optional[str]
     """An optional memo to display on the invoice."""
 
+    require_successful_payment: bool
+    """
+    If true, the new credit block will require that the corresponding invoice is
+    paid before it can be drawn down from.
+    """
+
 
 class AddDecrementCreditLedgerEntryRequestParams(TypedDict, total=False):
     amount: Required[float]
     """The number of credits to effect.
 
     Note that this is required for increment, decrement, void, or undo operations.
     """
```

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/ledger_create_entry_response.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/ledger_list_by_external_id_params.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/ledger_list_by_external_id_response.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/ledger_list_params.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/ledger_list_response.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/top_up_create_by_external_id_params.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,7 +53,13 @@
     The net terms determines the difference between the invoice date and the issue
     date for the invoice. If you intend the invoice to be due on issue, set this
     to 0.
     """
 
     memo: Optional[str]
     """An optional memo to display on the invoice."""
+
+    require_successful_payment: bool
+    """
+    If true, new credit blocks created by this top-up will require that the
+    corresponding invoice is paid before they can be drawn down from.
+    """
```

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/top_up_create_by_external_id_response.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Optional
 from typing_extensions import Literal
 
 from ...._models import BaseModel
 
-__all__ = ["TopUpCreateByExternalIDResponse", "InvoiceSettings"]
+__all__ = ["TopUpListByExternalIDResponse", "InvoiceSettings"]
 
 
 class InvoiceSettings(BaseModel):
     auto_collection: bool
     """
     Whether the credits purchase invoice should auto collect with the customer's
     saved payment method.
@@ -21,16 +21,22 @@
     date for the invoice. If you intend the invoice to be due on issue, set this
     to 0.
     """
 
     memo: Optional[str] = None
     """An optional memo to display on the invoice."""
 
+    require_successful_payment: Optional[bool] = None
+    """
+    If true, new credit blocks created by this top-up will require that the
+    corresponding invoice is paid before they can be drawn down from.
+    """
+
 
-class TopUpCreateByExternalIDResponse(BaseModel):
+class TopUpListByExternalIDResponse(BaseModel):
     id: str
 
     amount: str
     """The amount to increment when the threshold is reached."""
 
     currency: str
     """The currency or custom pricing unit to use for this top-up.
```

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/top_up_create_params.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,7 +53,13 @@
     The net terms determines the difference between the invoice date and the issue
     date for the invoice. If you intend the invoice to be due on issue, set this
     to 0.
     """
 
     memo: Optional[str]
     """An optional memo to display on the invoice."""
+
+    require_successful_payment: bool
+    """
+    If true, new credit blocks created by this top-up will require that the
+    corresponding invoice is paid before they can be drawn down from.
+    """
```

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/top_up_create_response.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Optional
 from typing_extensions import Literal
 
 from ...._models import BaseModel
 
-__all__ = ["TopUpCreateResponse", "InvoiceSettings"]
+__all__ = ["TopUpListResponse", "InvoiceSettings"]
 
 
 class InvoiceSettings(BaseModel):
     auto_collection: bool
     """
     Whether the credits purchase invoice should auto collect with the customer's
     saved payment method.
@@ -21,16 +21,22 @@
     date for the invoice. If you intend the invoice to be due on issue, set this
     to 0.
     """
 
     memo: Optional[str] = None
     """An optional memo to display on the invoice."""
 
+    require_successful_payment: Optional[bool] = None
+    """
+    If true, new credit blocks created by this top-up will require that the
+    corresponding invoice is paid before they can be drawn down from.
+    """
+
 
-class TopUpCreateResponse(BaseModel):
+class TopUpListResponse(BaseModel):
     id: str
 
     amount: str
     """The amount to increment when the threshold is reached."""
 
     currency: str
     """The currency or custom pricing unit to use for this top-up.
```

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/top_up_list_by_external_id_params.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/customers/credits/top_up_list_by_external_id_response.py` & `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Optional
 from typing_extensions import Literal
 
 from ...._models import BaseModel
 
-__all__ = ["TopUpListByExternalIDResponse", "InvoiceSettings"]
+__all__ = ["TopUpCreateResponse", "InvoiceSettings"]
 
 
 class InvoiceSettings(BaseModel):
     auto_collection: bool
     """
     Whether the credits purchase invoice should auto collect with the customer's
     saved payment method.
@@ -21,16 +21,22 @@
     date for the invoice. If you intend the invoice to be due on issue, set this
     to 0.
     """
 
     memo: Optional[str] = None
     """An optional memo to display on the invoice."""
 
+    require_successful_payment: Optional[bool] = None
+    """
+    If true, new credit blocks created by this top-up will require that the
+    corresponding invoice is paid before they can be drawn down from.
+    """
+
 
-class TopUpListByExternalIDResponse(BaseModel):
+class TopUpCreateResponse(BaseModel):
     id: str
 
     amount: str
     """The amount to increment when the threshold is reached."""
 
     currency: str
     """The currency or custom pricing unit to use for this top-up.
```

### Comparing `orb_billing-1.47.1/src/orb/types/events/__init__.py` & `orb_billing-1.48.0/src/orb/types/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/events/backfill_close_response.py` & `orb_billing-1.48.0/src/orb/types/events/backfill_create_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from typing import Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from ..._models import BaseModel
 
-__all__ = ["BackfillCloseResponse"]
+__all__ = ["BackfillCreateResponse"]
 
 
-class BackfillCloseResponse(BaseModel):
+class BackfillCreateResponse(BaseModel):
     id: str
 
     close_time: Optional[datetime] = None
     """If in the future, the time at which the backfill will automatically close.
 
     If in the past, the time at which the backfill was closed.
     """
@@ -22,14 +22,17 @@
 
     customer_id: Optional[str] = None
     """The customer ID this backfill is scoped to.
 
     If null, this backfill is not scoped to a single customer.
     """
 
+    events_ingested: int
+    """The number of events ingested in this backfill."""
+
     reverted_at: Optional[datetime] = None
     """The time at which this backfill was reverted."""
 
     status: Literal["pending", "reflected", "pending_revert", "reverted"]
     """The status of the backfill."""
 
     timeframe_end: datetime
```

### Comparing `orb_billing-1.47.1/src/orb/types/events/backfill_create_params.py` & `orb_billing-1.48.0/src/orb/types/events/backfill_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/events/backfill_create_response.py` & `orb_billing-1.48.0/src/orb/types/events/backfill_revert_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from typing import Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from ..._models import BaseModel
 
-__all__ = ["BackfillCreateResponse"]
+__all__ = ["BackfillRevertResponse"]
 
 
-class BackfillCreateResponse(BaseModel):
+class BackfillRevertResponse(BaseModel):
     id: str
 
     close_time: Optional[datetime] = None
     """If in the future, the time at which the backfill will automatically close.
 
     If in the past, the time at which the backfill was closed.
     """
@@ -22,14 +22,17 @@
 
     customer_id: Optional[str] = None
     """The customer ID this backfill is scoped to.
 
     If null, this backfill is not scoped to a single customer.
     """
 
+    events_ingested: int
+    """The number of events ingested in this backfill."""
+
     reverted_at: Optional[datetime] = None
     """The time at which this backfill was reverted."""
 
     status: Literal["pending", "reflected", "pending_revert", "reverted"]
     """The status of the backfill."""
 
     timeframe_end: datetime
```

### Comparing `orb_billing-1.47.1/src/orb/types/events/backfill_fetch_response.py` & `orb_billing-1.48.0/src/orb/types/events/backfill_fetch_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
     customer_id: Optional[str] = None
     """The customer ID this backfill is scoped to.
 
     If null, this backfill is not scoped to a single customer.
     """
 
+    events_ingested: int
+    """The number of events ingested in this backfill."""
+
     reverted_at: Optional[datetime] = None
     """The time at which this backfill was reverted."""
 
     status: Literal["pending", "reflected", "pending_revert", "reverted"]
     """The status of the backfill."""
 
     timeframe_end: datetime
```

### Comparing `orb_billing-1.47.1/src/orb/types/events/backfill_list_response.py` & `orb_billing-1.48.0/src/orb/types/events/backfill_list_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
     customer_id: Optional[str] = None
     """The customer ID this backfill is scoped to.
 
     If null, this backfill is not scoped to a single customer.
     """
 
+    events_ingested: int
+    """The number of events ingested in this backfill."""
+
     reverted_at: Optional[datetime] = None
     """The time at which this backfill was reverted."""
 
     status: Literal["pending", "reflected", "pending_revert", "reverted"]
     """The status of the backfill."""
 
     timeframe_end: datetime
```

### Comparing `orb_billing-1.47.1/src/orb/types/events/backfill_revert_response.py` & `orb_billing-1.48.0/src/orb/types/events/backfill_close_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from typing import Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from ..._models import BaseModel
 
-__all__ = ["BackfillRevertResponse"]
+__all__ = ["BackfillCloseResponse"]
 
 
-class BackfillRevertResponse(BaseModel):
+class BackfillCloseResponse(BaseModel):
     id: str
 
     close_time: Optional[datetime] = None
     """If in the future, the time at which the backfill will automatically close.
 
     If in the past, the time at which the backfill was closed.
     """
@@ -22,14 +22,17 @@
 
     customer_id: Optional[str] = None
     """The customer ID this backfill is scoped to.
 
     If null, this backfill is not scoped to a single customer.
     """
 
+    events_ingested: int
+    """The number of events ingested in this backfill."""
+
     reverted_at: Optional[datetime] = None
     """The time at which this backfill was reverted."""
 
     status: Literal["pending", "reflected", "pending_revert", "reverted"]
     """The status of the backfill."""
 
     timeframe_end: datetime
```

### Comparing `orb_billing-1.47.1/src/orb/types/plans/external_plan_id_update_params.py` & `orb_billing-1.48.0/src/orb/types/plans/external_plan_id_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/src/orb/types/shared/discount.py` & `orb_billing-1.48.0/src/orb/types/shared/discount.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/LICENSE` & `orb_billing-1.48.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orb_billing-1.47.1/pyproject.toml` & `orb_billing-1.48.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "orb-billing"
-version = "1.47.1"
+version = "1.48.0"
 description = "The official Python library for the orb API"
-readme = "README.md"
+dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Orb", email = "team@withorb.com" },
 ]
 dependencies = [
     "httpx>=0.23.0, <1",
     "pydantic>=1.9.0, <3",
@@ -44,15 +44,15 @@
 
 
 
 [tool.rye]
 managed = true
 # version pins are in requirements-dev.lock
 dev-dependencies = [
-    "pyright",
+    "pyright>=1.1.359",
     "mypy",
     "respx",
     "pytest",
     "pytest-asyncio",
     "ruff",
     "time-machine",
     "nox",
@@ -64,15 +64,15 @@
 [tool.rye.scripts]
 format = { chain = [
   "format:ruff",
   "format:docs",
   "fix:ruff",
 ]}
 "format:black" = "black ."
-"format:docs" = "python bin/ruffen-docs.py README.md api.md"
+"format:docs" = "python scripts/utils/ruffen-docs.py README.md api.md"
 "format:ruff" = "ruff format"
 "format:isort" = "isort ."
 
 "lint" = { chain = [
   "check:ruff",
   "typecheck",
 ]}
@@ -84,25 +84,36 @@
   "typecheck:mypy"
 ]}
 "typecheck:pyright" = "pyright"
 "typecheck:verify-types" = "pyright --verifytypes orb --ignoreexternal"
 "typecheck:mypy" = "mypy ."
 
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
   "src/*"
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/orb"]
 
+[tool.hatch.metadata.hooks.fancy-pypi-readme]
+content-type = "text/markdown"
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
+path = "README.md"
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
+# replace relative links with absolute links
+pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
+replacement = '[\1](https://github.com/orbcorp/orb-python/tree/main/\g<2>)'
+
 [tool.black]
 line-length = 120
 target-version = ["py37"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--tb=short"
@@ -146,15 +157,17 @@
   "E722",
   # unused arguments
   "ARG",
   # print statements
   "T201",
   "T203",
   # misuse of typing.TYPE_CHECKING
-  "TCH004"
+  "TCH004",
+  # import rules
+  "TID251",
 ]
 ignore = [
   # mutable defaults
   "B006",
 ]
 unfixable = [
   # disable auto fix for print statements
@@ -162,18 +175,22 @@
   "T203",
 ]
 ignore-init-module-imports = true
 
 [tool.ruff.format]
 docstring-code-format = true
 
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
+"functools.lru_cache".msg = "This function does not retain type information for the wrapped function's arguments; The `lru_cache` function from `_utils` should be used instead"
+
 [tool.ruff.lint.isort]
 length-sort = true
 length-sort-straight = true
 combine-as-imports = true
 extra-standard-library = ["typing_extensions"]
 known-first-party = ["orb", "tests"]
 
 [tool.ruff.per-file-ignores]
 "bin/**.py" = ["T201", "T203"]
+"scripts/**.py" = ["T201", "T203"]
 "tests/**.py" = ["T201", "T203"]
 "examples/**.py" = ["T201", "T203"]
```

### Comparing `orb_billing-1.47.1/PKG-INFO` & `orb_billing-1.48.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: orb-billing
-Version: 1.47.1
+Version: 1.48.0
 Summary: The official Python library for the orb API
 Project-URL: Homepage, https://github.com/orbcorp/orb-python
 Project-URL: Repository, https://github.com/orbcorp/orb-python
 Author-email: Orb <team@withorb.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -38,26 +38,26 @@
 
 The Orb Python library provides convenient access to the Orb REST API from any Python 3.7+
 application. The library includes type definitions for all request params and response fields,
 and offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).
 
 ## Documentation
 
-The REST API documentation can be found [on docs.withorb.com](https://docs.withorb.com/reference/api-reference). The full API of this library can be found in [api.md](api.md).
+The REST API documentation can be found [on docs.withorb.com](https://docs.withorb.com/reference/api-reference). The full API of this library can be found in [api.md](https://github.com/orbcorp/orb-python/tree/main/api.md).
 
 ## Installation
 
 ```sh
 # install from PyPI
 pip install orb-billing
 ```
 
 ## Usage
 
-The full API of this library can be found in [api.md](api.md).
+The full API of this library can be found in [api.md](https://github.com/orbcorp/orb-python/tree/main/api.md).
 
 ```python
 import os
 from orb import Orb
 
 client = Orb(
     # This is the default and can be omitted
@@ -102,18 +102,18 @@
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
 ## Using types
 
-Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict). Responses are [Pydantic models](https://docs.pydantic.dev), which provide helper methods for things like:
+Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict). Responses are [Pydantic models](https://docs.pydantic.dev) which also provide helper methods for things like:
 
-- Serializing back into JSON, `model.model_dump_json(indent=2, exclude_unset=True)`
-- Converting to a dictionary, `model.model_dump(exclude_unset=True)`
+- Serializing back into JSON, `model.to_json()`
+- Converting to a dictionary, `model.to_dict()`
 
 Typed requests and responses provide autocomplete and documentation within your editor. If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `basic`.
 
 ## Pagination
 
 List methods in the Orb API are paginated.
 
@@ -195,14 +195,37 @@
         "country": "USA",
         "line1": "123 Example Street",
     },
 )
 print(customer.id)
 ```
 
+## Webhook Verification
+
+We provide helper methods for verifying that a webhook request came from Orb, and not a malicious third party.
+
+You can use `orb.webhooks.verify_signature(body: string, headers, secret?) -> None` or `orb.webhooks.unwrap(body: string, headers, secret?) -> Payload`,
+both of which will raise an error if the signature is invalid.
+
+Note that the "body" parameter must be the raw JSON string sent from the server (do not parse it first).
+The `.unwrap()` method can parse this JSON for you into a `Payload` object.
+
+For example, in [FastAPI](https://fastapi.tiangolo.com/):
+
+```py
+@app.post('/my-webhook-handler')
+async def handler(request: Request):
+    body = await request.body()
+    secret = os.environ['ORB_WEBHOOK_SECRET']  # env var or client arg used by default; explicit here.
+    payload = client.webhooks.unwrap(body, request.headers, secret)
+    print(payload)
+
+    return {'ok': True}
+```
+
 ## Handling errors
 
 When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `orb.APIConnectionError` is raised.
 
 When the API returns a non-success status code (that is, 4xx or 5xx
 response), a subclass of `orb.APIStatusError` is raised, containing `status_code` and `response` properties.
 
@@ -283,23 +306,23 @@
 
 # More granular control:
 client = Orb(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-client.with_options(timeout=5 * 1000).customers.create(
+client.with_options(timeout=5.0).customers.create(
     email="example-customer@withorb.com",
     name="My Customer",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
-Note that requests that time out are [retried twice by default](#retries).
+Note that requests that time out are [retried twice by default](https://github.com/orbcorp/orb-python/tree/main/#retries).
 
 ## Advanced
 
 ### Logging
 
 We use the standard library [`logging`](https://docs.python.org/3/library/logging.html) module.
 
@@ -367,15 +390,15 @@
         print(line)
 ```
 
 The context manager is required so that the response will reliably be closed.
 
 ### Making custom/undocumented requests
 
-This library is typed for convenient access the documented API.
+This library is typed for convenient access to the documented API.
 
 If you need to access undocumented endpoints, params, or response properties, the library can still be used.
 
 #### Undocumented endpoints
 
 To make requests to undocumented endpoints, you can make requests using `client.get`, `client.post`, and other
 http verbs. Options on the client will be respected (such as retries) will be respected when making this
@@ -409,21 +432,20 @@
 You can directly override the [httpx client](https://www.python-httpx.org/api/#client) to customize it for your use case, including:
 
 - Support for proxies
 - Custom transports
 - Additional [advanced](https://www.python-httpx.org/advanced/#client-instances) functionality
 
 ```python
-import httpx
-from orb import Orb
+from orb import Orb, DefaultHttpxClient
 
 client = Orb(
     # Or use the `ORB_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
-    http_client=httpx.Client(
+    http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
 )
 ```
 
 ### Managing HTTP resources
```

