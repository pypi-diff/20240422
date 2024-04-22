# Comparing `tmp/cognite_power_ops-0.94.0.tar.gz` & `tmp/cognite_power_ops-0.94.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.94.0.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.94.1.tar", max compression
```

## Comparing `cognite_power_ops-0.94.0.tar` & `cognite_power_ops-0.94.1.tar`

### file list

```diff
@@ -1,673 +1,672 @@
--rw-r--r--   0        0        0    10758 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/LICENSE
--rw-r--r--   0        0        0     3322 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/README.md
--rw-r--r--   0        0        0      150 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/__init__.py
--rw-r--r--   0        0        0       23 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/_version.py
--rw-r--r--   0        0        0     5273 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/cdf_labels.py
--rw-r--r--   0        0        0     8779 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/cli.py
--rw-r--r--   0        0        0       74 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0      105 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/__init__.py
--rw-r--r--   0        0        0    32135 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/_core.py
--rw-r--r--   0        0        0    26235 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/alert.py
--rw-r--r--   0        0        0     1492 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py
--rw-r--r--   0        0        0    27110 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py
--rw-r--r--   0        0        0     2041 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py
--rw-r--r--   0        0        0     2039 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py
--rw-r--r--   0        0        0    11759 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py
--rw-r--r--   0        0        0    16844 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py
--rw-r--r--   0        0        0     1513 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py
--rw-r--r--   0        0        0    27874 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py
--rw-r--r--   0        0        0     1971 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py
--rw-r--r--   0        0        0     8302 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py
--rw-r--r--   0        0        0    16131 2024-04-16 14:12:07.405355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py
--rw-r--r--   0        0        0    25401 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py
--rw-r--r--   0        0        0    25313 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py
--rw-r--r--   0        0        0    25313 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py
--rw-r--r--   0        0        0    25195 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py
--rw-r--r--   0        0        0    25692 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    25604 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py
--rw-r--r--   0        0        0     1513 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py
--rw-r--r--   0        0        0    25330 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py
--rw-r--r--   0        0        0    25780 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    25692 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py
--rw-r--r--   0        0        0     9211 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api_client.py
--rw-r--r--   0        0        0     2654 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py
--rw-r--r--   0        0        0    16179 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py
--rw-r--r--   0        0        0    19431 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py
--rw-r--r--   0        0        0     8148 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py
--rw-r--r--   0        0        0    23764 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py
--rw-r--r--   0        0        0    22916 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py
--rw-r--r--   0        0        0     9015 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py
--rw-r--r--   0        0        0      109 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/__init__.py
--rw-r--r--   0        0        0    32350 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/_core.py
--rw-r--r--   0        0        0    16860 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/bid_method.py
--rw-r--r--   0        0        0     1511 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/bid_method_query.py
--rw-r--r--   0        0        0    26226 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator.py
--rw-r--r--   0        0        0    15705 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py
--rw-r--r--   0        0        0     1625 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py
--rw-r--r--   0        0        0    28005 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py
--rw-r--r--   0        0        0     5828 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_query.py
--rw-r--r--   0        0        0    27596 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py
--rw-r--r--   0        0        0     2197 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py
--rw-r--r--   0        0        0    32967 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant.py
--rw-r--r--   0        0        0    30394 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py
--rw-r--r--   0        0        0     1998 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_generators.py
--rw-r--r--   0        0        0    30394 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py
--rw-r--r--   0        0        0    30394 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py
--rw-r--r--   0        0        0    30438 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py
--rw-r--r--   0        0        0    30100 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py
--rw-r--r--   0        0        0    30100 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py
--rw-r--r--   0        0        0     8084 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_query.py
--rw-r--r--   0        0        0    30394 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py
--rw-r--r--   0        0        0    27060 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area.py
--rw-r--r--   0        0        0    27668 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py
--rw-r--r--   0        0        0    27580 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py
--rw-r--r--   0        0        0    27580 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py
--rw-r--r--   0        0        0    27462 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py
--rw-r--r--   0        0        0    27374 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py
--rw-r--r--   0        0        0    27739 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py
--rw-r--r--   0        0        0    27959 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    27871 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py
--rw-r--r--   0        0        0     2011 2024-04-16 14:12:07.409355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_plants.py
--rw-r--r--   0        0        0    11709 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_query.py
--rw-r--r--   0        0        0    27597 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py
--rw-r--r--   0        0        0    28047 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    27959 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py
--rw-r--r--   0        0        0     2095 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py
--rw-r--r--   0        0        0    20054 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/reservoir.py
--rw-r--r--   0        0        0     1510 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/reservoir_query.py
--rw-r--r--   0        0        0    15561 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py
--rw-r--r--   0        0        0     1615 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py
--rw-r--r--   0        0        0    22125 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/watercourse.py
--rw-r--r--   0        0        0     2026 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py
--rw-r--r--   0        0        0    26508 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py
--rw-r--r--   0        0        0     6635 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/watercourse_query.py
--rw-r--r--   0        0        0    10150 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api_client.py
--rw-r--r--   0        0        0     4810 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/__init__.py
--rw-r--r--   0        0        0     8028 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py
--rw-r--r--   0        0        0    22916 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_core.py
--rw-r--r--   0        0        0    19888 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_generator.py
--rw-r--r--   0        0        0     9775 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py
--rw-r--r--   0        0        0    32088 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_plant.py
--rw-r--r--   0        0        0    33431 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_price_area.py
--rw-r--r--   0        0        0    10116 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py
--rw-r--r--   0        0        0     9645 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py
--rw-r--r--   0        0        0    13820 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py
--rw-r--r--   0        0        0      113 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/__init__.py
--rw-r--r--   0        0        0     8201 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/_core.py
--rw-r--r--   0        0        0    14521 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/case.py
--rw-r--r--   0        0        0     7486 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py
--rw-r--r--   0        0        0     9780 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py
--rw-r--r--   0        0        0    15960 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/mapping.py
--rw-r--r--   0        0        0    17869 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/model_template.py
--rw-r--r--   0        0        0    11367 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py
--rw-r--r--   0        0        0    19744 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/scenario.py
--rw-r--r--   0        0        0    10871 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/transformation.py
--rw-r--r--   0        0        0     3003 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api_client.py
--rw-r--r--   0        0        0     2524 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py
--rw-r--r--   0        0        0     4596 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py
--rw-r--r--   0        0        0     2226 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py
--rw-r--r--   0        0        0     5824 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py
--rw-r--r--   0        0        0     2393 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py
--rw-r--r--   0        0        0     4586 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py
--rw-r--r--   0        0        0     5174 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py
--rw-r--r--   0        0        0     2819 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py
--rw-r--r--   0        0        0     6951 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py
--rw-r--r--   0        0        0     2621 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py
--rw-r--r--   0        0        0      118 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/__init__.py
--rw-r--r--   0        0        0    32598 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py
--rw-r--r--   0        0        0    26333 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py
--rw-r--r--   0        0        0     1497 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py
--rw-r--r--   0        0        0    23471 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py
--rw-r--r--   0        0        0     2115 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py
--rw-r--r--   0        0        0     7177 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py
--rw-r--r--   0        0        0    29138 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py
--rw-r--r--   0        0        0     2059 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py
--rw-r--r--   0        0        0     2106 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py
--rw-r--r--   0        0        0    13622 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py
--rw-r--r--   0        0        0    22831 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py
--rw-r--r--   0        0        0     2032 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py
--rw-r--r--   0        0        0     7128 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py
--rw-r--r--   0        0        0    16942 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py
--rw-r--r--   0        0        0     1518 2024-04-16 14:12:07.413355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py
--rw-r--r--   0        0        0    24946 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py
--rw-r--r--   0        0        0     2185 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py
--rw-r--r--   0        0        0    10308 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py
--rw-r--r--   0        0        0     2410 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py
--rw-r--r--   0        0        0    19843 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py
--rw-r--r--   0        0        0    25798 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py
--rw-r--r--   0        0        0    25883 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py
--rw-r--r--   0        0        0     2613 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py
--rw-r--r--   0        0        0    20327 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py
--rw-r--r--   0        0        0     2415 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py
--rw-r--r--   0        0        0     4483 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py
--rw-r--r--   0        0        0    18030 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py
--rw-r--r--   0        0        0    24799 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py
--rw-r--r--   0        0        0     1559 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py
--rw-r--r--   0        0        0    15855 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py
--rw-r--r--   0        0        0    24935 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py
--rw-r--r--   0        0        0    25177 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py
--rw-r--r--   0        0        0     2777 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py
--rw-r--r--   0        0        0    18424 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py
--rw-r--r--   0        0        0     1618 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py
--rw-r--r--   0        0        0    11242 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py
--rw-r--r--   0        0        0     7397 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py
--rw-r--r--   0        0        0    16179 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py
--rw-r--r--   0        0        0    14604 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py
--rw-r--r--   0        0        0    24068 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py
--rw-r--r--   0        0        0    14962 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py
--rw-r--r--   0        0        0     8042 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py
--rw-r--r--   0        0        0    22916 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py
--rw-r--r--   0        0        0    17010 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py
--rw-r--r--   0        0        0    14696 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py
--rw-r--r--   0        0        0    11922 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py
--rw-r--r--   0        0        0     9353 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py
--rw-r--r--   0        0        0    13242 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py
--rw-r--r--   0        0        0     8909 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py
--rw-r--r--   0        0        0      123 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/__init__.py
--rw-r--r--   0        0        0    41803 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/_core.py
--rw-r--r--   0        0        0    28392 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/alert.py
--rw-r--r--   0        0        0     1486 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/alert_query.py
--rw-r--r--   0        0        0    24852 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py
--rw-r--r--   0        0        0     2445 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py
--rw-r--r--   0        0        0     7859 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py
--rw-r--r--   0        0        0    27557 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document.py
--rw-r--r--   0        0        0    29838 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py
--rw-r--r--   0        0        0     2125 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py
--rw-r--r--   0        0        0     2123 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py
--rw-r--r--   0        0        0    11654 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py
--rw-r--r--   0        0        0     2056 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py
--rw-r--r--   0        0        0    31537 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py
--rw-r--r--   0        0        0     2194 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py
--rw-r--r--   0        0        0     2399 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py
--rw-r--r--   0        0        0    13156 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py
--rw-r--r--   0        0        0     6256 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_query.py
--rw-r--r--   0        0        0    16995 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix.py
--rw-r--r--   0        0        0    20707 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py
--rw-r--r--   0        0        0     2194 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py
--rw-r--r--   0        0        0     2352 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py
--rw-r--r--   0        0        0     9120 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py
--rw-r--r--   0        0        0     1507 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py
--rw-r--r--   0        0        0    24990 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_row.py
--rw-r--r--   0        0        0     1986 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py
--rw-r--r--   0        0        0     8727 2024-04-16 14:12:07.417355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_row_query.py
--rw-r--r--   0        0        0    23488 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_input.py
--rw-r--r--   0        0        0     1527 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_input_query.py
--rw-r--r--   0        0        0    26010 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_output.py
--rw-r--r--   0        0        0     2098 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py
--rw-r--r--   0        0        0     7530 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_output_query.py
--rw-r--r--   0        0        0    30503 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator.py
--rw-r--r--   0        0        0    29640 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py
--rw-r--r--   0        0        0    14623 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py
--rw-r--r--   0        0        0     1621 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py
--rw-r--r--   0        0        0     5996 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_query.py
--rw-r--r--   0        0        0    29214 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py
--rw-r--r--   0        0        0     2275 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py
--rw-r--r--   0        0        0    30967 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/market_configuration.py
--rw-r--r--   0        0        0     1557 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py
--rw-r--r--   0        0        0    21738 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py
--rw-r--r--   0        0        0     2719 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py
--rw-r--r--   0        0        0    30364 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     4187 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    31040 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0     2403 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py
--rw-r--r--   0        0        0    10702 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py
--rw-r--r--   0        0        0    26004 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py
--rw-r--r--   0        0        0     2305 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py
--rw-r--r--   0        0        0     2463 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py
--rw-r--r--   0        0        0    12658 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py
--rw-r--r--   0        0        0    29102 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py
--rw-r--r--   0        0        0     2502 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py
--rw-r--r--   0        0        0     2660 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py
--rw-r--r--   0        0        0     2676 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py
--rw-r--r--   0        0        0    16509 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py
--rw-r--r--   0        0        0    21267 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant.py
--rw-r--r--   0        0        0    34870 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information.py
--rw-r--r--   0        0        0    31031 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py
--rw-r--r--   0        0        0     2177 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py
--rw-r--r--   0        0        0    31031 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py
--rw-r--r--   0        0        0    31031 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py
--rw-r--r--   0        0        0    31075 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py
--rw-r--r--   0        0        0    31163 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py
--rw-r--r--   0        0        0    31163 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py
--rw-r--r--   0        0        0     6307 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_query.py
--rw-r--r--   0        0        0    31031 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py
--rw-r--r--   0        0        0     1486 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_query.py
--rw-r--r--   0        0        0    35566 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py
--rw-r--r--   0        0        0    31218 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py
--rw-r--r--   0        0        0     2260 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py
--rw-r--r--   0        0        0    31218 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py
--rw-r--r--   0        0        0    31218 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py
--rw-r--r--   0        0        0    31262 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py
--rw-r--r--   0        0        0    31350 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py
--rw-r--r--   0        0        0    31350 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py
--rw-r--r--   0        0        0     6373 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py
--rw-r--r--   0        0        0    31218 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py
--rw-r--r--   0        0        0    21879 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/power_asset.py
--rw-r--r--   0        0        0     1512 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/power_asset_query.py
--rw-r--r--   0        0        0    21768 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area.py
--rw-r--r--   0        0        0    23928 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py
--rw-r--r--   0        0        0    27423 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py
--rw-r--r--   0        0        0    27335 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py
--rw-r--r--   0        0        0    27335 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py
--rw-r--r--   0        0        0    27217 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py
--rw-r--r--   0        0        0    27714 2024-04-16 14:12:07.421355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    27626 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py
--rw-r--r--   0        0        0     1528 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py
--rw-r--r--   0        0        0    27352 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py
--rw-r--r--   0        0        0    27802 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    27714 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py
--rw-r--r--   0        0        0    24500 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py
--rw-r--r--   0        0        0    27713 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py
--rw-r--r--   0        0        0    27521 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py
--rw-r--r--   0        0        0     2794 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py
--rw-r--r--   0        0        0    26627 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information.py
--rw-r--r--   0        0        0    28169 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py
--rw-r--r--   0        0        0    28081 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py
--rw-r--r--   0        0        0    28081 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py
--rw-r--r--   0        0        0    27963 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py
--rw-r--r--   0        0        0    28081 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py
--rw-r--r--   0        0        0    28460 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    28372 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py
--rw-r--r--   0        0        0    27889 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py
--rw-r--r--   0        0        0     2851 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py
--rw-r--r--   0        0        0    28098 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py
--rw-r--r--   0        0        0    28548 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    28460 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py
--rw-r--r--   0        0        0     1507 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_query.py
--rw-r--r--   0        0        0    18930 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_production.py
--rw-r--r--   0        0        0    25079 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_production_price.py
--rw-r--r--   0        0        0    25321 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_production_production.py
--rw-r--r--   0        0        0     2623 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_production_query.py
--rw-r--r--   0        0        0    25220 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py
--rw-r--r--   0        0        0     1601 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py
--rw-r--r--   0        0        0    27660 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py
--rw-r--r--   0        0        0    24151 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py
--rw-r--r--   0        0        0     3878 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py
--rw-r--r--   0        0        0    18438 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_case.py
--rw-r--r--   0        0        0     6064 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_case_query.py
--rw-r--r--   0        0        0     2071 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py
--rw-r--r--   0        0        0    17214 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_commands.py
--rw-r--r--   0        0        0     1521 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py
--rw-r--r--   0        0        0    20249 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_file.py
--rw-r--r--   0        0        0     1502 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_file_query.py
--rw-r--r--   0        0        0    23570 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_model.py
--rw-r--r--   0        0        0     2279 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py
--rw-r--r--   0        0        0     5631 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_model_query.py
--rw-r--r--   0        0        0    32763 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     2608 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py
--rw-r--r--   0        0        0     7877 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    29852 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py
--rw-r--r--   0        0        0     1548 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py
--rw-r--r--   0        0        0    29105 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py
--rw-r--r--   0        0        0     2688 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py
--rw-r--r--   0        0        0    27944 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py
--rw-r--r--   0        0        0     2223 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py
--rw-r--r--   0        0        0     8858 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py
--rw-r--r--   0        0        0    16377 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_result.py
--rw-r--r--   0        0        0     2042 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py
--rw-r--r--   0        0        0     2214 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py
--rw-r--r--   0        0        0    11103 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_result_query.py
--rw-r--r--   0        0        0    22289 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario.py
--rw-r--r--   0        0        0     2338 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py
--rw-r--r--   0        0        0     8104 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py
--rw-r--r--   0        0        0    23085 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py
--rw-r--r--   0        0        0     4851 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py
--rw-r--r--   0        0        0     2216 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py
--rw-r--r--   0        0        0    21375 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_time_series.py
--rw-r--r--   0        0        0     1533 2024-04-16 14:12:07.425355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py
--rw-r--r--   0        0        0    26338 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py
--rw-r--r--   0        0        0    27685 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py
--rw-r--r--   0        0        0     3695 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py
--rw-r--r--   0        0        0    27490 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py
--rw-r--r--   0        0        0     2153 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py
--rw-r--r--   0        0        0     8841 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py
--rw-r--r--   0        0        0    27145 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py
--rw-r--r--   0        0        0     2743 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py
--rw-r--r--   0        0        0    27652 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py
--rw-r--r--   0        0        0     2195 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py
--rw-r--r--   0        0        0     2330 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py
--rw-r--r--   0        0        0    11719 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py
--rw-r--r--   0        0        0    30353 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     2477 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py
--rw-r--r--   0        0        0     5956 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    29442 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0     2375 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py
--rw-r--r--   0        0        0     9141 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py
--rw-r--r--   0        0        0    15615 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py
--rw-r--r--   0        0        0     1611 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py
--rw-r--r--   0        0        0    24038 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py
--rw-r--r--   0        0        0     2906 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py
--rw-r--r--   0        0        0    32573 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     4476 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    21933 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/watercourse.py
--rw-r--r--   0        0        0     1516 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/watercourse_query.py
--rw-r--r--   0        0        0    44629 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api_client.py
--rw-r--r--   0        0        0    37530 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/__init__.py
--rw-r--r--   0        0        0    17724 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_alert.py
--rw-r--r--   0        0        0    19045 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py
--rw-r--r--   0        0        0    17003 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py
--rw-r--r--   0        0        0    20325 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py
--rw-r--r--   0        0        0    24038 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py
--rw-r--r--   0        0        0     8675 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py
--rw-r--r--   0        0        0    13297 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py
--rw-r--r--   0        0        0    21939 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py
--rw-r--r--   0        0        0    22919 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_core.py
--rw-r--r--   0        0        0    12436 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_function_input.py
--rw-r--r--   0        0        0    16494 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_function_output.py
--rw-r--r--   0        0        0    23043 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_generator.py
--rw-r--r--   0        0        0     9182 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py
--rw-r--r--   0        0        0    16689 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py
--rw-r--r--   0        0        0    13527 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py
--rw-r--r--   0        0        0    21898 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    23503 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0    20860 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py
--rw-r--r--   0        0        0    23349 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py
--rw-r--r--   0        0        0    10500 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_plant.py
--rw-r--r--   0        0        0    26506 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py
--rw-r--r--   0        0        0    29307 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py
--rw-r--r--   0        0        0    11193 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py
--rw-r--r--   0        0        0    10749 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_area.py
--rw-r--r--   0        0        0    23293 2024-04-16 14:12:07.429355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py
--rw-r--r--   0        0        0    17874 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py
--rw-r--r--   0        0        0    27975 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py
--rw-r--r--   0        0        0    13124 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_production.py
--rw-r--r--   0        0        0    15360 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py
--rw-r--r--   0        0        0    16791 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py
--rw-r--r--   0        0        0    14456 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py
--rw-r--r--   0        0        0     8881 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py
--rw-r--r--   0        0        0    11080 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py
--rw-r--r--   0        0        0    16536 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py
--rw-r--r--   0        0        0    23998 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    18119 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py
--rw-r--r--   0        0        0    17739 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py
--rw-r--r--   0        0        0    18550 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py
--rw-r--r--   0        0        0    16368 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py
--rw-r--r--   0        0        0    16997 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py
--rw-r--r--   0        0        0    13212 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py
--rw-r--r--   0        0        0    12493 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py
--rw-r--r--   0        0        0    19542 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py
--rw-r--r--   0        0        0    18640 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py
--rw-r--r--   0        0        0    17220 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py
--rw-r--r--   0        0        0    18291 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py
--rw-r--r--   0        0        0    20082 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    19880 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0     9657 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py
--rw-r--r--   0        0        0    14420 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py
--rw-r--r--   0        0        0    22515 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    10848 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py
--rw-r--r--   0        0        0     1301 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/_logger.py
--rw-r--r--   0        0        0      139 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/data_classes.py
--rw-r--r--   0        0        0     1322 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/data_set_api.py
--rw-r--r--   0        0        0     6750 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0       62 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/__init__.py
--rw-r--r--   0        0        0      885 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/_api_client.py
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/api/__init__.py
--rw-r--r--   0        0        0     8367 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/api/dayahead_trigger_api.py
--rw-r--r--   0        0        0     4797 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/api/shop_result_files_api.py
--rw-r--r--   0        0        0     4432 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/api/shop_results_api.py
--rw-r--r--   0        0        0     9593 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/api/shop_run_api.py
--rw-r--r--   0        0        0      600 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/__init__.py
--rw-r--r--   0        0        0     4114 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/case.py
--rw-r--r--   0        0        0     9057 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/dayahead_trigger.py
--rw-r--r--   0        0        0     2720 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/helpers.py
--rw-r--r--   0        0        0      603 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/plotting.py
--rw-r--r--   0        0        0     6164 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_result_files.py
--rw-r--r--   0        0        0     6607 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_results.py
--rw-r--r--   0        0        0    10210 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_results_compare.py
--rw-r--r--   0        0        0     3021 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_run.py
--rw-r--r--   0        0        0     3743 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_run_event.py
--rw-r--r--   0        0        0     4374 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_case.py
--rw-r--r--   0        0        0     1101 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_file_reference.py
--rw-r--r--   0        0        0    13466 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_run.py
--rw-r--r--   0        0        0    15419 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_run_api.py
--rw-r--r--   0        0        0     3885 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_run_filter.py
--rw-r--r--   0        0        0      563 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/client/shop/utils.py
--rw-r--r--   0        0        0      947 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/cognite_modules/_system.yaml
--rw-r--r--   0        0        0     1941 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/config.dev.yaml
--rw-r--r--   0        0        0      729 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml
--rw-r--r--   0        0        0     1095 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml
--rw-r--r--   0        0        0     1680 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml
--rw-r--r--   0        0        0      100 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/affr_space.space.yaml
--rw-r--r--   0        0        0       92 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/asset.space.yaml
--rw-r--r--   0        0        0      367 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidMethod.container.yaml
--rw-r--r--   0        0        0     2102 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml
--rw-r--r--   0        0        0      750 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml
--rw-r--r--   0        0        0     1380 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml
--rw-r--r--   0        0        0      857 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml
--rw-r--r--   0        0        0     1038 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml
--rw-r--r--   0        0        0      502 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidMethod.container.yaml
--rw-r--r--   0        0        0     1408 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml
--rw-r--r--   0        0        0     2281 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml
--rw-r--r--   0        0        0     2375 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml
--rw-r--r--   0        0        0      556 2024-04-16 14:12:07.433355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml
--rw-r--r--   0        0        0      466 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidDocument.container.yaml
--rw-r--r--   0        0        0      767 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml
--rw-r--r--   0        0        0      371 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMethod.container.yaml
--rw-r--r--   0        0        0      532 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml
--rw-r--r--   0        0        0      618 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml
--rw-r--r--   0        0        0      416 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenario.container.yaml
--rw-r--r--   0        0        0      490 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenarioResults.container.yaml
--rw-r--r--   0        0        0      113 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/dayahead_space.space.yaml
--rw-r--r--   0        0        0      118 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/instance.space.yaml
--rw-r--r--   0        0        0     1515 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml
--rw-r--r--   0        0        0      116 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/shared.space.yaml
--rw-r--r--   0        0        0       81 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/types.space.yaml
--rw-r--r--   0        0        0     1379 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml
--rw-r--r--   0        0        0      606 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml
--rw-r--r--   0        0        0     3917 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml
--rw-r--r--   0        0        0     2786 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml
--rw-r--r--   0        0        0     2618 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml
--rw-r--r--   0        0        0     1138 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml
--rw-r--r--   0        0        0     5199 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml
--rw-r--r--   0        0        0     5204 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml
--rw-r--r--   0        0        0     1060 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml
--rw-r--r--   0        0        0     1121 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml
--rw-r--r--   0        0        0     1887 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml
--rw-r--r--   0        0        0     2558 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml
--rw-r--r--   0        0        0     2374 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml
--rw-r--r--   0        0        0      858 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml
--rw-r--r--   0        0        0      579 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml
--rw-r--r--   0        0        0     1945 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml
--rw-r--r--   0        0        0     1845 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml
--rw-r--r--   0        0        0      723 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml
--rw-r--r--   0        0        0      700 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml
--rw-r--r--   0        0        0      711 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml
--rw-r--r--   0        0        0     1015 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml
--rw-r--r--   0        0        0     1479 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml
--rw-r--r--   0        0        0     1312 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml
--rw-r--r--   0        0        0      666 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml
--rw-r--r--   0        0        0     1230 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml
--rw-r--r--   0        0        0      605 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml
--rw-r--r--   0        0        0     4964 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml
--rw-r--r--   0        0        0     6519 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml
--rw-r--r--   0        0        0     2052 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml
--rw-r--r--   0        0        0     3499 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml
--rw-r--r--   0        0        0     2918 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml
--rw-r--r--   0        0        0     2575 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml
--rw-r--r--   0        0        0     2276 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml
--rw-r--r--   0        0        0     2163 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml
--rw-r--r--   0        0        0     1748 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml
--rw-r--r--   0        0        0      814 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml
--rw-r--r--   0        0        0     1292 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml
--rw-r--r--   0        0        0      496 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocumentDayAhead.container.yaml
--rw-r--r--   0        0        0      772 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml
--rw-r--r--   0        0        0     1659 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml
--rw-r--r--   0        0        0      755 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml
--rw-r--r--   0        0        0     2426 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml
--rw-r--r--   0        0        0     1379 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionMetadata.container.yaml
--rw-r--r--   0        0        0     1040 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml
--rw-r--r--   0        0        0     2082 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml
--rw-r--r--   0        0        0      756 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml
--rw-r--r--   0        0        0     2425 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml
--rw-r--r--   0        0        0     1076 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml
--rw-r--r--   0        0        0     1628 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml
--rw-r--r--   0        0        0      689 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml
--rw-r--r--   0        0        0      712 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml
--rw-r--r--   0        0        0      504 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPObjectiveValue.container.yaml
--rw-r--r--   0        0        0     1074 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml
--rw-r--r--   0        0        0     1106 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml
--rw-r--r--   0        0        0     1462 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml
--rw-r--r--   0        0        0      634 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml
--rw-r--r--   0        0        0      464 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCommands.container.yaml
--rw-r--r--   0        0        0     1128 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml
--rw-r--r--   0        0        0     1446 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml
--rw-r--r--   0        0        0      280 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopPartialBidConfiguration.container.yaml
--rw-r--r--   0        0        0      978 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml
--rw-r--r--   0        0        0      690 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml
--rw-r--r--   0        0        0      869 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml
--rw-r--r--   0        0        0     1789 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml
--rw-r--r--   0        0        0     2661 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml
--rw-r--r--   0        0        0      118 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/instance.space.yaml
--rw-r--r--   0        0        0      104 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/models.space.yaml
--rw-r--r--   0        0        0     5275 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml
--rw-r--r--   0        0        0      854 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml
--rw-r--r--   0        0        0       91 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/type.space.yaml
--rw-r--r--   0        0        0     3704 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml
--rw-r--r--   0        0        0     2834 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml
--rw-r--r--   0        0        0     2983 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml
--rw-r--r--   0        0        0      871 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml
--rw-r--r--   0        0        0     1283 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml
--rw-r--r--   0        0        0     2330 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml
--rw-r--r--   0        0        0     1073 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml
--rw-r--r--   0        0        0     1260 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml
--rw-r--r--   0        0        0      535 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml
--rw-r--r--   0        0        0      599 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml
--rw-r--r--   0        0        0     4498 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml
--rw-r--r--   0        0        0      512 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml
--rw-r--r--   0        0        0     2932 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml
--rw-r--r--   0        0        0     1659 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml
--rw-r--r--   0        0        0      596 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml
--rw-r--r--   0        0        0      543 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml
--rw-r--r--   0        0        0     1476 2024-04-16 14:12:07.437355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml
--rw-r--r--   0        0        0     2264 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml
--rw-r--r--   0        0        0     1059 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml
--rw-r--r--   0        0        0     1184 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml
--rw-r--r--   0        0        0     2520 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml
--rw-r--r--   0        0        0     1450 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml
--rw-r--r--   0        0        0     1726 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml
--rw-r--r--   0        0        0     1564 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml
--rw-r--r--   0        0        0      701 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml
--rw-r--r--   0        0        0     1225 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml
--rw-r--r--   0        0        0     1349 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml
--rw-r--r--   0        0        0      890 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml
--rw-r--r--   0        0        0     2331 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml
--rw-r--r--   0        0        0     1840 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml
--rw-r--r--   0        0        0     1027 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml
--rw-r--r--   0        0        0     1705 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml
--rw-r--r--   0        0        0     2573 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml
--rw-r--r--   0        0        0     1965 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml
--rw-r--r--   0        0        0     1535 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml
--rw-r--r--   0        0        0     1977 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml
--rw-r--r--   0        0        0     1797 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     1053 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml
--rw-r--r--   0        0        0     1750 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     1522 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml
--rw-r--r--   0        0        0     1660 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml
--rw-r--r--   0        0        0     1069 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml
--rw-r--r--   0        0        0     1249 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml
--rw-r--r--   0        0        0     1680 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     1336 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     2513 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml
--rw-r--r--   0        0        0      985 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml
--rw-r--r--   0        0        0     1761 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml
--rw-r--r--   0        0        0     1359 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml
--rw-r--r--   0        0        0     1430 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml
--rw-r--r--   0        0        0     1014 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml
--rw-r--r--   0        0        0     1382 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml
--rw-r--r--   0        0        0     1438 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml
--rw-r--r--   0        0        0     1392 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml
--rw-r--r--   0        0        0     2707 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml
--rw-r--r--   0        0        0     1587 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml
--rw-r--r--   0        0        0     1114 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/prerun_transformations/__init__.py
--rw-r--r--   0        0        0    34098 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/prerun_transformations/transformations.py
--rw-r--r--   0        0        0      278 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/__init__.py
--rw-r--r--   0        0        0     1792 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/__init__.py
--rw-r--r--   0        0        0    12764 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/_main.py
--rw-r--r--   0        0        0      595 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/_settings.py
--rw-r--r--   0        0        0    12408 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/_shared.py
--rw-r--r--   0        0        0       75 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/cogshop/__init__.py
--rw-r--r--   0        0        0      720 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/cogshop/shop_file_config.py
--rw-r--r--   0        0        0      815 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/__init__.py
--rw-r--r--   0        0        0     5486 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/_core.py
--rw-r--r--   0        0        0     2106 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/benchmarking.py
--rw-r--r--   0        0        0     2105 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/dayahead.py
--rw-r--r--   0        0        0      961 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/market.py
--rw-r--r--   0        0        0    10827 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/rkom.py
--rw-r--r--   0        0        0      417 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/production/__init__.py
--rw-r--r--   0        0        0      830 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/production/connections.py
--rw-r--r--   0        0        0     1414 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/production/generator.py
--rw-r--r--   0        0        0     5675 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/production/plant.py
--rw-r--r--   0        0        0     2868 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/config/production/watercourse.py
--rw-r--r--   0        0        0      244 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/core/__init__.py
--rw-r--r--   0        0        0     9185 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/core/cdf.py
--rw-r--r--   0        0        0      442 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/core/echo.py
--rw-r--r--   0        0        0    27692 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/core/main.py
--rw-r--r--   0        0        0     2563 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/core/transform.py
--rw-r--r--   0        0        0     2161 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/core/validation.py
--rw-r--r--   0        0        0      474 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/diff/__init__.py
--rw-r--r--   0        0        0     6774 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/diff/core.py
--rw-r--r--   0        0        0    12631 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/diff/data_classes.py
--rw-r--r--   0        0        0      424 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/__init__.py
--rw-r--r--   0        0        0       82 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/_shared_v1_v2/__init__.py
--rw-r--r--   0        0        0      811 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py
--rw-r--r--   0        0        0    10495 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py
--rw-r--r--   0        0        0     1143 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/_shared_v1_v2/market_model.py
--rw-r--r--   0        0        0     8337 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/_shared_v1_v2/production_model.py
--rw-r--r--   0        0        0      788 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/__init__.py
--rw-r--r--   0        0        0    11195 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/asset_model.py
--rw-r--r--   0        0        0     9602 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/asset_type.py
--rw-r--r--   0        0        0     5251 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/cdf_resources.py
--rw-r--r--   0        0        0    11641 2024-04-16 14:12:07.441355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/data_model.py
--rw-r--r--   0        0        0     1896 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/dms_models.py
--rw-r--r--   0        0        0      592 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/graph_ql.py
--rw-r--r--   0        0        0      148 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/helpers.py
--rw-r--r--   0        0        0     6668 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/model.py
--rw-r--r--   0        0        0     1705 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/resource_type.py
--rw-r--r--   0        0        0     1302 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/__init__.py
--rw-r--r--   0        0        0     8141 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/cogshop.py
--rw-r--r--   0        0        0      243 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/config_to_model/__init__.py
--rw-r--r--   0        0        0     8940 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py
--rw-r--r--   0        0        0    15631 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py
--rw-r--r--   0        0        0     9726 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py
--rw-r--r--   0        0        0      491 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/graphql_schemas/__init__.py
--rw-r--r--   0        0        0      832 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql
--rw-r--r--   0        0        0     3499 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/base.py
--rw-r--r--   0        0        0     3184 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/benchmark.py
--rw-r--r--   0        0        0     2405 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/dayahead.py
--rw-r--r--   0        0        0     2797 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/rkom.py
--rw-r--r--   0        0        0     7801 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/production.py
--rw-r--r--   0        0        0      395 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v2/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v2/config_to_model/__init__.py
--rw-r--r--   0        0        0     8873 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py
--rw-r--r--   0        0        0    27181 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v2/powerops_models.py
--rw-r--r--   0        0        0     7631 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/models/v2/production_dm.py
--rw-r--r--   0        0        0      150 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/time_series_mapping/__init__.py
--rw-r--r--   0        0        0     2149 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/time_series_mapping/mapping.py
--rw-r--r--   0        0        0     2456 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/time_series_mapping/static_mapping.py
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/v2/__init__.py
--rw-r--r--   0        0        0      238 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/v2/main.py
--rw-r--r--   0        0        0     7548 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/v2/shop_to_assets.py
--rw-r--r--   0        0        0     4524 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/resync/validation.py
--rw-r--r--   0        0        0        0 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0      160 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/__init__.py
--rw-r--r--   0        0        0     1389 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/_cdf_auth.py
--rw-r--r--   0        0        0     3169 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/_settings.py
--rw-r--r--   0        0        0     7517 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/calls.py
--rw-r--r--   0        0        0    10874 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/extraction_pipelines.py
--rw-r--r--   0        0        0      970 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/resource_creation.py
--rw-r--r--   0        0        0     2540 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/lookup.py
--rw-r--r--   0        0        0     1097 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/navigation.py
--rw-r--r--   0        0        0      514 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/require.py
--rw-r--r--   0        0        0      227 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/retry/__init__.py
--rw-r--r--   0        0        0     5619 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/retry/api.py
--rw-r--r--   0        0        0     7828 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/serialization.py
--rw-r--r--   0        0        0     3667 2024-04-16 14:12:07.445355 cognite_power_ops-0.94.0/cognite/powerops/utils/time.py
--rw-r--r--   0        0        0     3775 2024-04-16 14:12:07.449355 cognite_power_ops-0.94.0/pyproject.toml
--rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 cognite_power_ops-0.94.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/LICENSE
+-rw-r--r--   0        0        0     3322 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/README.md
+-rw-r--r--   0        0        0      150 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/_version.py
+-rw-r--r--   0        0        0     5273 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/cdf_labels.py
+-rw-r--r--   0        0        0     8779 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/cli.py
+-rw-r--r--   0        0        0       74 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0      105 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/__init__.py
+-rw-r--r--   0        0        0    32135 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/_core.py
+-rw-r--r--   0        0        0    26235 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/alert.py
+-rw-r--r--   0        0        0     1492 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py
+-rw-r--r--   0        0        0    27110 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py
+-rw-r--r--   0        0        0     2041 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py
+-rw-r--r--   0        0        0     2039 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py
+-rw-r--r--   0        0        0    11759 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py
+-rw-r--r--   0        0        0    16844 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py
+-rw-r--r--   0        0        0     1513 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py
+-rw-r--r--   0        0        0    27874 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py
+-rw-r--r--   0        0        0     1971 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py
+-rw-r--r--   0        0        0     8302 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py
+-rw-r--r--   0        0        0    16131 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py
+-rw-r--r--   0        0        0    25401 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py
+-rw-r--r--   0        0        0    25313 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py
+-rw-r--r--   0        0        0    25313 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py
+-rw-r--r--   0        0        0    25195 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py
+-rw-r--r--   0        0        0    25692 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    25604 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0     1513 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py
+-rw-r--r--   0        0        0    25330 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py
+-rw-r--r--   0        0        0    25780 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    25692 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0     9211 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api_client.py
+-rw-r--r--   0        0        0     2654 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py
+-rw-r--r--   0        0        0    16179 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py
+-rw-r--r--   0        0        0    19431 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py
+-rw-r--r--   0        0        0     8148 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py
+-rw-r--r--   0        0        0    23764 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py
+-rw-r--r--   0        0        0    22916 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py
+-rw-r--r--   0        0        0     9015 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py
+-rw-r--r--   0        0        0      109 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/__init__.py
+-rw-r--r--   0        0        0    32350 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/_core.py
+-rw-r--r--   0        0        0    16860 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/bid_method.py
+-rw-r--r--   0        0        0     1511 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/bid_method_query.py
+-rw-r--r--   0        0        0    26226 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator.py
+-rw-r--r--   0        0        0    15705 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py
+-rw-r--r--   0        0        0     1625 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py
+-rw-r--r--   0        0        0    28005 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py
+-rw-r--r--   0        0        0     5828 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_query.py
+-rw-r--r--   0        0        0    27596 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py
+-rw-r--r--   0        0        0     2197 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py
+-rw-r--r--   0        0        0    32967 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant.py
+-rw-r--r--   0        0        0    30394 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py
+-rw-r--r--   0        0        0     1998 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_generators.py
+-rw-r--r--   0        0        0    30394 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py
+-rw-r--r--   0        0        0    30394 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py
+-rw-r--r--   0        0        0    30438 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py
+-rw-r--r--   0        0        0    30100 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py
+-rw-r--r--   0        0        0    30100 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py
+-rw-r--r--   0        0        0     8084 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_query.py
+-rw-r--r--   0        0        0    30394 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py
+-rw-r--r--   0        0        0    27060 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area.py
+-rw-r--r--   0        0        0    27668 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py
+-rw-r--r--   0        0        0    27580 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py
+-rw-r--r--   0        0        0    27580 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py
+-rw-r--r--   0        0        0    27462 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py
+-rw-r--r--   0        0        0    27374 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py
+-rw-r--r--   0        0        0    27739 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py
+-rw-r--r--   0        0        0    27959 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27871 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0     2011 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_plants.py
+-rw-r--r--   0        0        0    11709 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_query.py
+-rw-r--r--   0        0        0    27597 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py
+-rw-r--r--   0        0        0    28047 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27959 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0     2095 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py
+-rw-r--r--   0        0        0    20054 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/reservoir.py
+-rw-r--r--   0        0        0     1510 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/reservoir_query.py
+-rw-r--r--   0        0        0    15561 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py
+-rw-r--r--   0        0        0     1615 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py
+-rw-r--r--   0        0        0    22125 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse.py
+-rw-r--r--   0        0        0     2026 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py
+-rw-r--r--   0        0        0    26508 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py
+-rw-r--r--   0        0        0     6635 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_query.py
+-rw-r--r--   0        0        0    10150 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api_client.py
+-rw-r--r--   0        0        0     4810 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/__init__.py
+-rw-r--r--   0        0        0     8028 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py
+-rw-r--r--   0        0        0    22916 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_core.py
+-rw-r--r--   0        0        0    19888 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_generator.py
+-rw-r--r--   0        0        0     9775 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py
+-rw-r--r--   0        0        0    32088 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_plant.py
+-rw-r--r--   0        0        0    33431 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_price_area.py
+-rw-r--r--   0        0        0    10116 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py
+-rw-r--r--   0        0        0     9645 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py
+-rw-r--r--   0        0        0    13820 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py
+-rw-r--r--   0        0        0      113 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/__init__.py
+-rw-r--r--   0        0        0     8201 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/_core.py
+-rw-r--r--   0        0        0    14521 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/case.py
+-rw-r--r--   0        0        0     7486 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py
+-rw-r--r--   0        0        0     9780 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py
+-rw-r--r--   0        0        0    15960 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/mapping.py
+-rw-r--r--   0        0        0    17869 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/model_template.py
+-rw-r--r--   0        0        0    11367 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py
+-rw-r--r--   0        0        0    19744 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/scenario.py
+-rw-r--r--   0        0        0    10871 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/transformation.py
+-rw-r--r--   0        0        0     3003 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api_client.py
+-rw-r--r--   0        0        0     2524 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py
+-rw-r--r--   0        0        0     4596 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py
+-rw-r--r--   0        0        0     2226 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py
+-rw-r--r--   0        0        0     5824 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py
+-rw-r--r--   0        0        0     2393 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py
+-rw-r--r--   0        0        0     4586 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py
+-rw-r--r--   0        0        0     5174 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py
+-rw-r--r--   0        0        0     2819 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py
+-rw-r--r--   0        0        0     6951 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py
+-rw-r--r--   0        0        0     2621 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py
+-rw-r--r--   0        0        0      118 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/__init__.py
+-rw-r--r--   0        0        0    32598 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py
+-rw-r--r--   0        0        0    26333 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py
+-rw-r--r--   0        0        0     1497 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py
+-rw-r--r--   0        0        0    23471 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py
+-rw-r--r--   0        0        0     2115 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py
+-rw-r--r--   0        0        0     7177 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py
+-rw-r--r--   0        0        0    29138 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py
+-rw-r--r--   0        0        0     2059 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py
+-rw-r--r--   0        0        0     2106 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py
+-rw-r--r--   0        0        0    13622 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py
+-rw-r--r--   0        0        0    22831 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py
+-rw-r--r--   0        0        0     2032 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py
+-rw-r--r--   0        0        0     7128 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py
+-rw-r--r--   0        0        0    16942 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py
+-rw-r--r--   0        0        0     1518 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py
+-rw-r--r--   0        0        0    24946 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py
+-rw-r--r--   0        0        0     2185 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py
+-rw-r--r--   0        0        0    10308 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py
+-rw-r--r--   0        0        0     2410 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py
+-rw-r--r--   0        0        0    19843 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py
+-rw-r--r--   0        0        0    25798 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py
+-rw-r--r--   0        0        0    25883 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py
+-rw-r--r--   0        0        0     2613 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py
+-rw-r--r--   0        0        0    20327 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py
+-rw-r--r--   0        0        0     2415 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py
+-rw-r--r--   0        0        0     4483 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py
+-rw-r--r--   0        0        0    18030 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py
+-rw-r--r--   0        0        0    24799 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py
+-rw-r--r--   0        0        0     1559 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py
+-rw-r--r--   0        0        0    15855 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py
+-rw-r--r--   0        0        0    24935 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py
+-rw-r--r--   0        0        0    25177 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py
+-rw-r--r--   0        0        0     2777 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py
+-rw-r--r--   0        0        0    18424 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py
+-rw-r--r--   0        0        0     1618 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py
+-rw-r--r--   0        0        0    11242 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py
+-rw-r--r--   0        0        0     7397 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py
+-rw-r--r--   0        0        0    16179 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py
+-rw-r--r--   0        0        0    14604 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py
+-rw-r--r--   0        0        0    24068 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py
+-rw-r--r--   0        0        0    14962 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py
+-rw-r--r--   0        0        0     8042 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py
+-rw-r--r--   0        0        0    22916 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py
+-rw-r--r--   0        0        0    17010 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py
+-rw-r--r--   0        0        0    14696 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py
+-rw-r--r--   0        0        0    11922 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py
+-rw-r--r--   0        0        0     9353 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py
+-rw-r--r--   0        0        0    13242 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py
+-rw-r--r--   0        0        0     8909 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py
+-rw-r--r--   0        0        0      123 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/__init__.py
+-rw-r--r--   0        0        0    41803 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/_core.py
+-rw-r--r--   0        0        0    28392 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/alert.py
+-rw-r--r--   0        0        0     1486 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/alert_query.py
+-rw-r--r--   0        0        0    24852 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py
+-rw-r--r--   0        0        0     2445 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py
+-rw-r--r--   0        0        0     7859 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py
+-rw-r--r--   0        0        0    27557 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document.py
+-rw-r--r--   0        0        0    29838 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py
+-rw-r--r--   0        0        0     2125 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py
+-rw-r--r--   0        0        0     2123 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py
+-rw-r--r--   0        0        0    11654 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py
+-rw-r--r--   0        0        0     2056 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py
+-rw-r--r--   0        0        0    31537 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py
+-rw-r--r--   0        0        0     2194 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py
+-rw-r--r--   0        0        0     2399 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py
+-rw-r--r--   0        0        0    13156 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py
+-rw-r--r--   0        0        0     6256 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_query.py
+-rw-r--r--   0        0        0    16995 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix.py
+-rw-r--r--   0        0        0    20707 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py
+-rw-r--r--   0        0        0     2194 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py
+-rw-r--r--   0        0        0     2352 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py
+-rw-r--r--   0        0        0     9120 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py
+-rw-r--r--   0        0        0     1507 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py
+-rw-r--r--   0        0        0    24990 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row.py
+-rw-r--r--   0        0        0     1986 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py
+-rw-r--r--   0        0        0     8727 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row_query.py
+-rw-r--r--   0        0        0    23488 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_input.py
+-rw-r--r--   0        0        0     1527 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_input_query.py
+-rw-r--r--   0        0        0    26010 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output.py
+-rw-r--r--   0        0        0     2098 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py
+-rw-r--r--   0        0        0     7530 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output_query.py
+-rw-r--r--   0        0        0    30503 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator.py
+-rw-r--r--   0        0        0    29640 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py
+-rw-r--r--   0        0        0    14623 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py
+-rw-r--r--   0        0        0     1621 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py
+-rw-r--r--   0        0        0     5996 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_query.py
+-rw-r--r--   0        0        0    29214 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py
+-rw-r--r--   0        0        0     2275 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py
+-rw-r--r--   0        0        0    30967 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/market_configuration.py
+-rw-r--r--   0        0        0     1557 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py
+-rw-r--r--   0        0        0    21738 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py
+-rw-r--r--   0        0        0     2719 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py
+-rw-r--r--   0        0        0    30364 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     4187 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    31040 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0     2403 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py
+-rw-r--r--   0        0        0    10702 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py
+-rw-r--r--   0        0        0    26004 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py
+-rw-r--r--   0        0        0     2305 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py
+-rw-r--r--   0        0        0     2463 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py
+-rw-r--r--   0        0        0    12658 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py
+-rw-r--r--   0        0        0    29102 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py
+-rw-r--r--   0        0        0     2502 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py
+-rw-r--r--   0        0        0     2660 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py
+-rw-r--r--   0        0        0     2676 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py
+-rw-r--r--   0        0        0    16509 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py
+-rw-r--r--   0        0        0    21267 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant.py
+-rw-r--r--   0        0        0    34870 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information.py
+-rw-r--r--   0        0        0    31031 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py
+-rw-r--r--   0        0        0     2177 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py
+-rw-r--r--   0        0        0    31031 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py
+-rw-r--r--   0        0        0    31031 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py
+-rw-r--r--   0        0        0    31075 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py
+-rw-r--r--   0        0        0    31163 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py
+-rw-r--r--   0        0        0    31163 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py
+-rw-r--r--   0        0        0     6307 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_query.py
+-rw-r--r--   0        0        0    31031 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py
+-rw-r--r--   0        0        0     1486 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_query.py
+-rw-r--r--   0        0        0    35566 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py
+-rw-r--r--   0        0        0    31218 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py
+-rw-r--r--   0        0        0     2260 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py
+-rw-r--r--   0        0        0    31218 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py
+-rw-r--r--   0        0        0    31218 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py
+-rw-r--r--   0        0        0    31262 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py
+-rw-r--r--   0        0        0    31350 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py
+-rw-r--r--   0        0        0    31350 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py
+-rw-r--r--   0        0        0     6373 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py
+-rw-r--r--   0        0        0    31218 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py
+-rw-r--r--   0        0        0    21879 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/power_asset.py
+-rw-r--r--   0        0        0     1512 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/power_asset_query.py
+-rw-r--r--   0        0        0    21768 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area.py
+-rw-r--r--   0        0        0    23928 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py
+-rw-r--r--   0        0        0    27423 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py
+-rw-r--r--   0        0        0    27335 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py
+-rw-r--r--   0        0        0    27335 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py
+-rw-r--r--   0        0        0    27217 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py
+-rw-r--r--   0        0        0    27714 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27626 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0     1528 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py
+-rw-r--r--   0        0        0    27352 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py
+-rw-r--r--   0        0        0    27802 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27714 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0    24500 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py
+-rw-r--r--   0        0        0    27713 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py
+-rw-r--r--   0        0        0    27521 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py
+-rw-r--r--   0        0        0     2794 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py
+-rw-r--r--   0        0        0    26627 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information.py
+-rw-r--r--   0        0        0    28169 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py
+-rw-r--r--   0        0        0    28081 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py
+-rw-r--r--   0        0        0    28081 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py
+-rw-r--r--   0        0        0    27963 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py
+-rw-r--r--   0        0        0    28081 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py
+-rw-r--r--   0        0        0    28460 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    28372 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0    27889 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py
+-rw-r--r--   0        0        0     2851 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py
+-rw-r--r--   0        0        0    28098 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py
+-rw-r--r--   0        0        0    28548 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    28460 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0     1507 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_query.py
+-rw-r--r--   0        0        0    18930 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production.py
+-rw-r--r--   0        0        0    25079 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_price.py
+-rw-r--r--   0        0        0    25321 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_production.py
+-rw-r--r--   0        0        0     2623 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_query.py
+-rw-r--r--   0        0        0    25220 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py
+-rw-r--r--   0        0        0     1601 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py
+-rw-r--r--   0        0        0    27660 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py
+-rw-r--r--   0        0        0    24151 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0     3878 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py
+-rw-r--r--   0        0        0    18438 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case.py
+-rw-r--r--   0        0        0     6064 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case_query.py
+-rw-r--r--   0        0        0     2071 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py
+-rw-r--r--   0        0        0    17214 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_commands.py
+-rw-r--r--   0        0        0     1521 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py
+-rw-r--r--   0        0        0    20249 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_file.py
+-rw-r--r--   0        0        0     1502 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_file_query.py
+-rw-r--r--   0        0        0    23570 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model.py
+-rw-r--r--   0        0        0     2279 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py
+-rw-r--r--   0        0        0     5631 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model_query.py
+-rw-r--r--   0        0        0    32763 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     2608 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py
+-rw-r--r--   0        0        0     7877 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    29852 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py
+-rw-r--r--   0        0        0     1548 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py
+-rw-r--r--   0        0        0    29105 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py
+-rw-r--r--   0        0        0     2688 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py
+-rw-r--r--   0        0        0    27944 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py
+-rw-r--r--   0        0        0     2223 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py
+-rw-r--r--   0        0        0     8858 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py
+-rw-r--r--   0        0        0    16377 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result.py
+-rw-r--r--   0        0        0     2042 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py
+-rw-r--r--   0        0        0     2214 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py
+-rw-r--r--   0        0        0    11103 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_query.py
+-rw-r--r--   0        0        0    22289 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario.py
+-rw-r--r--   0        0        0     2338 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py
+-rw-r--r--   0        0        0     8104 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py
+-rw-r--r--   0        0        0    23085 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py
+-rw-r--r--   0        0        0     4851 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py
+-rw-r--r--   0        0        0     2216 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py
+-rw-r--r--   0        0        0    21375 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series.py
+-rw-r--r--   0        0        0     1533 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py
+-rw-r--r--   0        0        0    26338 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py
+-rw-r--r--   0        0        0    27685 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py
+-rw-r--r--   0        0        0     3695 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py
+-rw-r--r--   0        0        0    27490 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py
+-rw-r--r--   0        0        0     2153 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py
+-rw-r--r--   0        0        0     8841 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py
+-rw-r--r--   0        0        0    27145 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py
+-rw-r--r--   0        0        0     2743 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py
+-rw-r--r--   0        0        0    27652 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py
+-rw-r--r--   0        0        0     2195 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py
+-rw-r--r--   0        0        0     2330 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py
+-rw-r--r--   0        0        0    11719 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py
+-rw-r--r--   0        0        0    30353 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     2477 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py
+-rw-r--r--   0        0        0     5956 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    29442 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0     2375 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py
+-rw-r--r--   0        0        0     9141 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py
+-rw-r--r--   0        0        0    15615 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py
+-rw-r--r--   0        0        0     1611 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py
+-rw-r--r--   0        0        0    24038 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0     2906 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py
+-rw-r--r--   0        0        0    32573 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     4476 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    21933 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/watercourse.py
+-rw-r--r--   0        0        0     1516 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/watercourse_query.py
+-rw-r--r--   0        0        0    44629 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api_client.py
+-rw-r--r--   0        0        0    37530 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/__init__.py
+-rw-r--r--   0        0        0    17724 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_alert.py
+-rw-r--r--   0        0        0    19045 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py
+-rw-r--r--   0        0        0    17003 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py
+-rw-r--r--   0        0        0    20325 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py
+-rw-r--r--   0        0        0    24038 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py
+-rw-r--r--   0        0        0     8689 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py
+-rw-r--r--   0        0        0    13311 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py
+-rw-r--r--   0        0        0    21939 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py
+-rw-r--r--   0        0        0    22919 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_core.py
+-rw-r--r--   0        0        0    12436 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_function_input.py
+-rw-r--r--   0        0        0    16494 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_function_output.py
+-rw-r--r--   0        0        0    23071 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_generator.py
+-rw-r--r--   0        0        0     9182 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py
+-rw-r--r--   0        0        0    16689 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py
+-rw-r--r--   0        0        0    13527 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py
+-rw-r--r--   0        0        0    21898 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    23503 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0    20874 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py
+-rw-r--r--   0        0        0    23363 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py
+-rw-r--r--   0        0        0    10500 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant.py
+-rw-r--r--   0        0        0    26506 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py
+-rw-r--r--   0        0        0    29307 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py
+-rw-r--r--   0        0        0    11193 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py
+-rw-r--r--   0        0        0    10749 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area.py
+-rw-r--r--   0        0        0    23293 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py
+-rw-r--r--   0        0        0    17874 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py
+-rw-r--r--   0        0        0    27975 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py
+-rw-r--r--   0        0        0    13152 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_production.py
+-rw-r--r--   0        0        0    15360 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py
+-rw-r--r--   0        0        0    16791 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0    14456 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py
+-rw-r--r--   0        0        0     8881 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py
+-rw-r--r--   0        0        0    11080 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py
+-rw-r--r--   0        0        0    16536 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py
+-rw-r--r--   0        0        0    23998 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    18119 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py
+-rw-r--r--   0        0        0    17739 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py
+-rw-r--r--   0        0        0    18550 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py
+-rw-r--r--   0        0        0    16368 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py
+-rw-r--r--   0        0        0    16997 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py
+-rw-r--r--   0        0        0    13212 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py
+-rw-r--r--   0        0        0    12493 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py
+-rw-r--r--   0        0        0    19542 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py
+-rw-r--r--   0        0        0    18640 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py
+-rw-r--r--   0        0        0    17220 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py
+-rw-r--r--   0        0        0    18291 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py
+-rw-r--r--   0        0        0    20082 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    19880 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0     9657 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py
+-rw-r--r--   0        0        0    14420 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0    22515 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    10848 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py
+-rw-r--r--   0        0        0     1301 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_logger.py
+-rw-r--r--   0        0        0      139 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/data_classes.py
+-rw-r--r--   0        0        0     1322 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/data_set_api.py
+-rw-r--r--   0        0        0     6750 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0       62 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/_api_client.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/__init__.py
+-rw-r--r--   0        0        0     8367 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/dayahead_trigger_api.py
+-rw-r--r--   0        0        0     4797 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_result_files_api.py
+-rw-r--r--   0        0        0     4432 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_results_api.py
+-rw-r--r--   0        0        0     9593 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_run_api.py
+-rw-r--r--   0        0        0      600 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/__init__.py
+-rw-r--r--   0        0        0     4114 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/case.py
+-rw-r--r--   0        0        0     9057 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/dayahead_trigger.py
+-rw-r--r--   0        0        0     2720 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/helpers.py
+-rw-r--r--   0        0        0      603 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/plotting.py
+-rw-r--r--   0        0        0     6164 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_result_files.py
+-rw-r--r--   0        0        0     6607 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_results.py
+-rw-r--r--   0        0        0    10210 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_results_compare.py
+-rw-r--r--   0        0        0     3021 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_run.py
+-rw-r--r--   0        0        0     3743 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_run_event.py
+-rw-r--r--   0        0        0     4374 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_case.py
+-rw-r--r--   0        0        0     1101 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_file_reference.py
+-rw-r--r--   0        0        0    13466 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run.py
+-rw-r--r--   0        0        0    15419 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run_api.py
+-rw-r--r--   0        0        0     3885 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run_filter.py
+-rw-r--r--   0        0        0      563 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/utils.py
+-rw-r--r--   0        0        0      947 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/cognite_modules/_system.yaml
+-rw-r--r--   0        0        0     1941 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/config.dev.yaml
+-rw-r--r--   0        0        0      729 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml
+-rw-r--r--   0        0        0     1095 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml
+-rw-r--r--   0        0        0     1680 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml
+-rw-r--r--   0        0        0      100 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/affr_space.space.yaml
+-rw-r--r--   0        0        0       92 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/asset.space.yaml
+-rw-r--r--   0        0        0      367 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidMethod.container.yaml
+-rw-r--r--   0        0        0     2102 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml
+-rw-r--r--   0        0        0      750 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml
+-rw-r--r--   0        0        0     1380 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml
+-rw-r--r--   0        0        0      857 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml
+-rw-r--r--   0        0        0     1038 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml
+-rw-r--r--   0        0        0      502 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidMethod.container.yaml
+-rw-r--r--   0        0        0     1408 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml
+-rw-r--r--   0        0        0     2281 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml
+-rw-r--r--   0        0        0     2375 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml
+-rw-r--r--   0        0        0      556 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml
+-rw-r--r--   0        0        0      466 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidDocument.container.yaml
+-rw-r--r--   0        0        0      767 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml
+-rw-r--r--   0        0        0      371 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMethod.container.yaml
+-rw-r--r--   0        0        0      532 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml
+-rw-r--r--   0        0        0      618 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml
+-rw-r--r--   0        0        0      416 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenario.container.yaml
+-rw-r--r--   0        0        0      490 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenarioResults.container.yaml
+-rw-r--r--   0        0        0      113 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/dayahead_space.space.yaml
+-rw-r--r--   0        0        0      118 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/instance.space.yaml
+-rw-r--r--   0        0        0     1515 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml
+-rw-r--r--   0        0        0      116 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/shared.space.yaml
+-rw-r--r--   0        0        0       81 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/types.space.yaml
+-rw-r--r--   0        0        0     1379 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml
+-rw-r--r--   0        0        0      606 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml
+-rw-r--r--   0        0        0     3917 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml
+-rw-r--r--   0        0        0     2786 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml
+-rw-r--r--   0        0        0     2618 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml
+-rw-r--r--   0        0        0     1138 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml
+-rw-r--r--   0        0        0     5199 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml
+-rw-r--r--   0        0        0     5204 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml
+-rw-r--r--   0        0        0     1060 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml
+-rw-r--r--   0        0        0     1121 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml
+-rw-r--r--   0        0        0     1887 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml
+-rw-r--r--   0        0        0     2558 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml
+-rw-r--r--   0        0        0     2374 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml
+-rw-r--r--   0        0        0      858 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml
+-rw-r--r--   0        0        0      579 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml
+-rw-r--r--   0        0        0     1945 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml
+-rw-r--r--   0        0        0     1845 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml
+-rw-r--r--   0        0        0      723 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml
+-rw-r--r--   0        0        0      700 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml
+-rw-r--r--   0        0        0      711 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml
+-rw-r--r--   0        0        0     1015 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml
+-rw-r--r--   0        0        0     1479 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml
+-rw-r--r--   0        0        0     1312 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml
+-rw-r--r--   0        0        0      666 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml
+-rw-r--r--   0        0        0     1230 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml
+-rw-r--r--   0        0        0      605 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml
+-rw-r--r--   0        0        0     4964 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml
+-rw-r--r--   0        0        0     6519 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml
+-rw-r--r--   0        0        0     2052 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml
+-rw-r--r--   0        0        0     3499 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml
+-rw-r--r--   0        0        0     2918 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml
+-rw-r--r--   0        0        0     2575 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml
+-rw-r--r--   0        0        0     2276 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml
+-rw-r--r--   0        0        0     2163 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml
+-rw-r--r--   0        0        0     1748 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml
+-rw-r--r--   0        0        0      814 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml
+-rw-r--r--   0        0        0     1292 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml
+-rw-r--r--   0        0        0      496 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocumentDayAhead.container.yaml
+-rw-r--r--   0        0        0      771 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml
+-rw-r--r--   0        0        0     1659 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml
+-rw-r--r--   0        0        0      755 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml
+-rw-r--r--   0        0        0     3521 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml
+-rw-r--r--   0        0        0     1038 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml
+-rw-r--r--   0        0        0     2082 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml
+-rw-r--r--   0        0        0      756 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml
+-rw-r--r--   0        0        0     2425 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml
+-rw-r--r--   0        0        0     1076 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml
+-rw-r--r--   0        0        0     1628 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml
+-rw-r--r--   0        0        0      689 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml
+-rw-r--r--   0        0        0      710 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml
+-rw-r--r--   0        0        0      504 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPObjectiveValue.container.yaml
+-rw-r--r--   0        0        0     1074 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml
+-rw-r--r--   0        0        0     1106 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml
+-rw-r--r--   0        0        0     1462 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml
+-rw-r--r--   0        0        0      634 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml
+-rw-r--r--   0        0        0      464 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCommands.container.yaml
+-rw-r--r--   0        0        0     1128 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml
+-rw-r--r--   0        0        0     1446 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml
+-rw-r--r--   0        0        0      280 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopPartialBidConfiguration.container.yaml
+-rw-r--r--   0        0        0      978 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml
+-rw-r--r--   0        0        0      690 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml
+-rw-r--r--   0        0        0      869 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml
+-rw-r--r--   0        0        0     1789 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml
+-rw-r--r--   0        0        0     2661 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml
+-rw-r--r--   0        0        0      118 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/instance.space.yaml
+-rw-r--r--   0        0        0      104 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/models.space.yaml
+-rw-r--r--   0        0        0     5275 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml
+-rw-r--r--   0        0        0      854 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml
+-rw-r--r--   0        0        0       91 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/type.space.yaml
+-rw-r--r--   0        0        0     3704 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml
+-rw-r--r--   0        0        0     2834 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml
+-rw-r--r--   0        0        0     2983 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml
+-rw-r--r--   0        0        0      871 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml
+-rw-r--r--   0        0        0     1283 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml
+-rw-r--r--   0        0        0     2330 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml
+-rw-r--r--   0        0        0     1073 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml
+-rw-r--r--   0        0        0     1260 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml
+-rw-r--r--   0        0        0      535 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml
+-rw-r--r--   0        0        0      599 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml
+-rw-r--r--   0        0        0     4498 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml
+-rw-r--r--   0        0        0      512 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml
+-rw-r--r--   0        0        0     2932 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml
+-rw-r--r--   0        0        0     1659 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml
+-rw-r--r--   0        0        0      596 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml
+-rw-r--r--   0        0        0      543 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml
+-rw-r--r--   0        0        0     1476 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml
+-rw-r--r--   0        0        0     2264 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml
+-rw-r--r--   0        0        0     1059 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml
+-rw-r--r--   0        0        0     1184 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml
+-rw-r--r--   0        0        0     2520 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml
+-rw-r--r--   0        0        0     1450 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml
+-rw-r--r--   0        0        0     1726 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml
+-rw-r--r--   0        0        0     1564 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml
+-rw-r--r--   0        0        0      701 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml
+-rw-r--r--   0        0        0     1225 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml
+-rw-r--r--   0        0        0     1349 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml
+-rw-r--r--   0        0        0      890 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml
+-rw-r--r--   0        0        0     2331 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml
+-rw-r--r--   0        0        0     1840 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml
+-rw-r--r--   0        0        0     1027 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml
+-rw-r--r--   0        0        0     1705 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml
+-rw-r--r--   0        0        0     2573 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml
+-rw-r--r--   0        0        0     1965 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml
+-rw-r--r--   0        0        0     1535 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml
+-rw-r--r--   0        0        0     1399 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml
+-rw-r--r--   0        0        0     1797 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     1053 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml
+-rw-r--r--   0        0        0     1750 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     1522 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml
+-rw-r--r--   0        0        0     1660 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml
+-rw-r--r--   0        0        0     1069 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml
+-rw-r--r--   0        0        0     1249 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml
+-rw-r--r--   0        0        0     1680 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     1336 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     2119 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml
+-rw-r--r--   0        0        0      981 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml
+-rw-r--r--   0        0        0     1757 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml
+-rw-r--r--   0        0        0     1355 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml
+-rw-r--r--   0        0        0     1426 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml
+-rw-r--r--   0        0        0     1010 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml
+-rw-r--r--   0        0        0     1378 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml
+-rw-r--r--   0        0        0     1434 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml
+-rw-r--r--   0        0        0     1392 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml
+-rw-r--r--   0        0        0     2707 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml
+-rw-r--r--   0        0        0     1587 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml
+-rw-r--r--   0        0        0     1114 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/prerun_transformations/__init__.py
+-rw-r--r--   0        0        0    34098 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/prerun_transformations/transformations.py
+-rw-r--r--   0        0        0      278 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/__init__.py
+-rw-r--r--   0        0        0     1792 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/__init__.py
+-rw-r--r--   0        0        0    12764 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/_main.py
+-rw-r--r--   0        0        0      595 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/_settings.py
+-rw-r--r--   0        0        0    12408 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/_shared.py
+-rw-r--r--   0        0        0       75 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/cogshop/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/cogshop/shop_file_config.py
+-rw-r--r--   0        0        0      815 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/__init__.py
+-rw-r--r--   0        0        0     5486 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/_core.py
+-rw-r--r--   0        0        0     2106 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/benchmarking.py
+-rw-r--r--   0        0        0     2105 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/dayahead.py
+-rw-r--r--   0        0        0      961 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/market.py
+-rw-r--r--   0        0        0    10827 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/rkom.py
+-rw-r--r--   0        0        0      417 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/__init__.py
+-rw-r--r--   0        0        0      830 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/connections.py
+-rw-r--r--   0        0        0     1414 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/generator.py
+-rw-r--r--   0        0        0     5675 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/plant.py
+-rw-r--r--   0        0        0     2868 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/watercourse.py
+-rw-r--r--   0        0        0      244 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/__init__.py
+-rw-r--r--   0        0        0     9185 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/cdf.py
+-rw-r--r--   0        0        0      442 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/echo.py
+-rw-r--r--   0        0        0    27692 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/main.py
+-rw-r--r--   0        0        0     2563 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/transform.py
+-rw-r--r--   0        0        0     2161 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/validation.py
+-rw-r--r--   0        0        0      474 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/diff/__init__.py
+-rw-r--r--   0        0        0     6774 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/diff/core.py
+-rw-r--r--   0        0        0    12631 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/diff/data_classes.py
+-rw-r--r--   0        0        0      424 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/__init__.py
+-rw-r--r--   0        0        0       82 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/__init__.py
+-rw-r--r--   0        0        0      811 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py
+-rw-r--r--   0        0        0    10495 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py
+-rw-r--r--   0        0        0     1143 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/market_model.py
+-rw-r--r--   0        0        0     8337 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/production_model.py
+-rw-r--r--   0        0        0      788 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/__init__.py
+-rw-r--r--   0        0        0    11195 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/asset_model.py
+-rw-r--r--   0        0        0     9602 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/asset_type.py
+-rw-r--r--   0        0        0     5251 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/cdf_resources.py
+-rw-r--r--   0        0        0    11641 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/data_model.py
+-rw-r--r--   0        0        0     1896 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/dms_models.py
+-rw-r--r--   0        0        0      592 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/graph_ql.py
+-rw-r--r--   0        0        0      148 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/helpers.py
+-rw-r--r--   0        0        0     6668 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/model.py
+-rw-r--r--   0        0        0     1705 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/resource_type.py
+-rw-r--r--   0        0        0     1302 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/__init__.py
+-rw-r--r--   0        0        0     8141 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/cogshop.py
+-rw-r--r--   0        0        0      243 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/__init__.py
+-rw-r--r--   0        0        0     8940 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py
+-rw-r--r--   0        0        0    15631 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py
+-rw-r--r--   0        0        0     9726 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py
+-rw-r--r--   0        0        0      491 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/graphql_schemas/__init__.py
+-rw-r--r--   0        0        0      832 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql
+-rw-r--r--   0        0        0     3499 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/base.py
+-rw-r--r--   0        0        0     3184 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/benchmark.py
+-rw-r--r--   0        0        0     2405 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/dayahead.py
+-rw-r--r--   0        0        0     2797 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/rkom.py
+-rw-r--r--   0        0        0     7801 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/production.py
+-rw-r--r--   0        0        0      395 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/config_to_model/__init__.py
+-rw-r--r--   0        0        0     8873 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py
+-rw-r--r--   0        0        0    27181 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/powerops_models.py
+-rw-r--r--   0        0        0     7631 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/production_dm.py
+-rw-r--r--   0        0        0      150 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/__init__.py
+-rw-r--r--   0        0        0     2149 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/mapping.py
+-rw-r--r--   0        0        0     2456 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/static_mapping.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/v2/__init__.py
+-rw-r--r--   0        0        0      238 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/v2/main.py
+-rw-r--r--   0        0        0     7548 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/v2/shop_to_assets.py
+-rw-r--r--   0        0        0     4524 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/validation.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/__init__.py
+-rw-r--r--   0        0        0     1389 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/_cdf_auth.py
+-rw-r--r--   0        0        0     3169 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/_settings.py
+-rw-r--r--   0        0        0     7517 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/calls.py
+-rw-r--r--   0        0        0    10874 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/extraction_pipelines.py
+-rw-r--r--   0        0        0      970 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/resource_creation.py
+-rw-r--r--   0        0        0     2540 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/lookup.py
+-rw-r--r--   0        0        0     1097 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/navigation.py
+-rw-r--r--   0        0        0      514 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/require.py
+-rw-r--r--   0        0        0      227 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/retry/__init__.py
+-rw-r--r--   0        0        0     5619 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/retry/api.py
+-rw-r--r--   0        0        0     7828 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/serialization.py
+-rw-r--r--   0        0        0     3667 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/time.py
+-rw-r--r--   0        0        0     3775 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/pyproject.toml
+-rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 cognite_power_ops-0.94.1/PKG-INFO
```

### Comparing `cognite_power_ops-0.94.0/LICENSE` & `cognite_power_ops-0.94.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/README.md` & `cognite_power_ops-0.94.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/cdf_labels.py` & `cognite_power_ops-0.94.1/cognite/powerops/cdf_labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/cli.py` & `cognite_power_ops-0.94.1/cognite/powerops/cli.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/alert.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/_api_client.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/bid_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/bid_method_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/bid_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_generators.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_generators.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_plants.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_plants.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/reservoir.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/reservoir.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/reservoir_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/reservoir_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/watercourse.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api/watercourse_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/_api_client.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_generator.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_plant.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_price_area.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/case.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/mapping.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/model_template.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/model_template.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/scenario.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api/transformation.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/_api_client.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/alert.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/alert_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/alert_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_document_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_row.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/bid_row_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_input_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/function_output_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/market_configuration.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/market_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/power_asset.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/power_asset.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/power_asset_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/power_asset_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_area_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_production.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_production_price.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_production_production.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/price_production_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_case.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_case_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_commands.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_commands.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_file.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_file.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_file_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_file_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_model_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_result.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_result_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/watercourse.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api/watercourse_query.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/watercourse_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/_api_client.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_alert.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         write_view = (view_by_read_class or {}).get(BidMatrix, dm.ViewId("sp_power_ops_models", "BidMatrix", "1"))
 
         properties: dict[str, Any] = {}
 
         if self.state is not None:
             properties["state"] = self.state
 
-        if self.bid_matrix is not None:
+        if self.bid_matrix is not None or write_none:
             properties["bidMatrix"] = self.bid_matrix
 
         if properties:
             this_node = dm.NodeApply(
                 space=self.space,
                 external_id=self.external_id,
                 existing_version=None if allow_version_increase else self.data_record.existing_version,
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         )
 
         properties: dict[str, Any] = {}
 
         if self.state is not None:
             properties["state"] = self.state
 
-        if self.bid_matrix is not None:
+        if self.bid_matrix is not None or write_none:
             properties["bidMatrix"] = self.bid_matrix
 
         if properties:
             this_node = dm.NodeApply(
                 space=self.space,
                 external_id=self.external_id,
                 existing_version=None if allow_version_increase else self.data_record.existing_version,
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_function_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_function_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_function_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_function_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_generator.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,21 +344,21 @@
 
         if self.penstock_number is not None:
             properties["penstockNumber"] = self.penstock_number
 
         if self.start_cost is not None:
             properties["startCost"] = self.start_cost
 
-        if self.start_stop_cost is not None:
+        if self.start_stop_cost is not None or write_none:
             if isinstance(self.start_stop_cost, str) or self.start_stop_cost is None:
                 properties["startStopCost"] = self.start_stop_cost
             else:
                 properties["startStopCost"] = self.start_stop_cost.external_id
 
-        if self.availability_time_series is not None:
+        if self.availability_time_series is not None or write_none:
             if isinstance(self.availability_time_series, str) or self.availability_time_series is None:
                 properties["availabilityTimeSeries"] = self.availability_time_series
             else:
                 properties["availabilityTimeSeries"] = self.availability_time_series.external_id
 
         if self.generator_efficiency_curve is not None:
             properties["generatorEfficiencyCurve"] = {
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         )
 
         properties: dict[str, Any] = {}
 
         if self.state is not None:
             properties["state"] = self.state
 
-        if self.bid_matrix is not None:
+        if self.bid_matrix is not None or write_none:
             properties["bidMatrix"] = self.bid_matrix
 
         if self.power_asset is not None:
             properties["powerAsset"] = {
                 "space": self.space if isinstance(self.power_asset, str) else self.power_asset.space,
                 "externalId": self.power_asset if isinstance(self.power_asset, str) else self.power_asset.external_id,
             }
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
         )
 
         properties: dict[str, Any] = {}
 
         if self.state is not None:
             properties["state"] = self.state
 
-        if self.bid_matrix is not None:
+        if self.bid_matrix is not None or write_none:
             properties["bidMatrix"] = self.bid_matrix
 
         if self.power_asset is not None:
             properties["powerAsset"] = {
                 "space": self.space if isinstance(self.power_asset, str) else self.power_asset.space,
                 "externalId": self.power_asset if isinstance(self.power_asset, str) else self.power_asset.external_id,
             }
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_plant.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_area.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_price_production.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_production.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,21 +208,21 @@
         )
 
         properties: dict[str, Any] = {}
 
         if self.name is not None:
             properties["name"] = self.name
 
-        if self.price is not None:
+        if self.price is not None or write_none:
             if isinstance(self.price, str) or self.price is None:
                 properties["price"] = self.price
             else:
                 properties["price"] = self.price.external_id
 
-        if self.production is not None:
+        if self.production is not None or write_none:
             if isinstance(self.production, str) or self.production is None:
                 properties["production"] = self.production
             else:
                 properties["production"] = self.production.external_id
 
         if self.shop_result is not None:
             properties["shopResult"] = {
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/_logger.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/_logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/data_set_api.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/data_set_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/powerops_client.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/powerops_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/_api_client.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/api/dayahead_trigger_api.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/dayahead_trigger_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/api/shop_result_files_api.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_result_files_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/api/shop_results_api.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_results_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/api/shop_run_api.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_run_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/case.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/dayahead_trigger.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/dayahead_trigger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/helpers.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/plotting.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/plotting.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_result_files.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_result_files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_results.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_results.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_results_compare.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_results_compare.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_run.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_run.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/data_classes/shop_run_event.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_run_event.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_case.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_file_reference.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_file_reference.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_run.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_run_api.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/shop_run_filter.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run_filter.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/client/shop/utils.py` & `cognite_power_ops-0.94.1/cognite/powerops/client/shop/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/cognite_modules/_system.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/cognite_modules/_system.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/config.dev.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/config.dev.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     nullable: false
     autoIncrement: false
     name: state
   bidMatrix:
     type:
       list: false
       type: sequence
-    nullable: false
+    nullable: true
     autoIncrement: false
     name: bidMatrix
   powerAsset:
     type:
       list: false
       type: direct
     nullable: true
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,55 @@
 space: "{{power_ops_models}}"
 externalId: FunctionData
 name: FunctionData
 usedFor: node
 properties:
+  functionName:
+    type:
+      list: false
+      collation: ucs_basic
+      type: text
+    nullable: false
+    autoIncrement: false
+    name: functionName
+    description: The name of the function
+  functionCallId:
+    type:
+      list: false
+      collation: ucs_basic
+      type: text
+    nullable: false
+    autoIncrement: false
+    name: functionCallId
+    description: The function call id
+  workflowExecutionId:
+    type:
+      list: false
+      collation: ucs_basic
+      type: text
+    nullable: false
+    autoIncrement: false
+    name: workflowExecutionId
+    description: The process id
+  workflowStep:
+    type:
+      list: false
+      type: int32
+    nullable: false
+    autoIncrement: false
+    name: workflowStep
+    description: The process step
+  linkedStep:
+    type:
+      list: false
+      type: direct
+    nullable: true
+    autoIncrement: false
+    name: linkedStep
+    description: Typically the input to the function
   direct1:
     type:
       list: false
       type: direct
     nullable: true
     autoIncrement: false
     name: direct1
@@ -124,14 +167,23 @@
     name: sequence
   flag:
     type:
       type: boolean
     nullable: true
     autoIncrement: false
     name: flag
-constraints:
-  requiredFunctionMetadata:
-    require:
-      space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
-      type: container
-    constraintType: requires
+indexes:
+  functionNameIndex:
+    properties:
+      - functionName
+    indexType: btree
+    cursorable: false
+  functionCallIdIndex:
+    properties:
+      - functionCallId
+    indexType: btree
+    cursorable: false
+  workflowExecutionIdIndex:
+    properties:
+      - workflowExecutionId
+    indexType: btree
+    cursorable: false
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionMetadata.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,50 @@
 space: "{{power_ops_models}}"
-externalId: FunctionMetadata
-name: FunctionMetadata
+externalId: ShopScenario
+name: ShopScenario
 usedFor: node
 properties:
-  functionName:
+  name:
     type:
       list: false
       collation: ucs_basic
       type: text
     nullable: false
     autoIncrement: false
-    name: functionName
-    description: The name of the function
-  functionCallId:
+    name: name
+    description: The name of the Shop Scenario
+  model:
     type:
       list: false
-      collation: ucs_basic
-      type: text
-    nullable: false
-    autoIncrement: false
-    name: functionCallId
-    description: The function call id
-  workflowExecutionId:
-    type:
-      list: false
-      collation: ucs_basic
-      type: text
-    nullable: false
+      type: direct
+    nullable: true
     autoIncrement: false
-    name: workflowExecutionId
-    description: The process id
-  workflowStep:
+    name: model
+    description: The model template
+  commands:
     type:
       list: false
-      type: int32
-    nullable: false
+      type: direct
+    nullable: true
     autoIncrement: false
-    name: workflowStep
-    description: The process step
-  linkedStep:
+    name: commands
+    description: The commands to run shop with
+  source:
     type:
       list: false
-      type: direct
+      collation: ucs_basic
+      type: text
     nullable: true
     autoIncrement: false
-    name: linkedStep
-    description: Typically the input to the function
+    name: source
+    description: The source of the scenario
 indexes:
-  functionNameIndex:
-    properties:
-      - functionName
-    indexType: btree
-    cursorable: false
-  functionCallIdIndex:
+  nameIndex:
     properties:
-      - functionCallId
+      - name
     indexType: btree
     cursorable: false
-  workflowExecutionIdIndex:
+  sourceIndex:
     properties:
-      - workflowExecutionId
+      - source
     indexType: btree
     cursorable: false
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,22 +24,22 @@
     nullable: false
     autoIncrement: false
     name: startCost
   startStopCost:
     type:
       type: timeseries
       list: false
-    nullable: false
+    nullable: true
     autoIncrement: false
     name: startStopCost
   availabilityTimeSeries:
     type:
       type: timeseries
       list: false
-    nullable: false
+    nullable: true
     autoIncrement: false
     name: availabilityTimeSeries
   generatorEfficiencyCurve:
     type:
       type: direct
       list: false
     nullable: true
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     autoIncrement: false
     name: name
     description: TODO
   price:
     type:
       list: false
       type: timeseries
-    nullable: false
+    nullable: true
     autoIncrement: false
     name: price
     description: TODO
   production:
     type:
       list: false
       type: timeseries
-    nullable: false
+    nullable: true
     autoIncrement: false
     name: production
     description: TODO
   shopResult:
     type:
       list: false
       type: direct
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,78 @@
 space: "{{power_ops_models}}"
-externalId: FunctionInput
-name: FunctionInput
+externalId: FunctionOutput
+name: FunctionOutput
 description: Base class for all function inputs
 filter:
   and:
     - hasData:
         - type: container
           space: "{{power_ops_models}}"
-          externalId: FunctionMetadata
+          externalId: FunctionData
     - equals:
         property:
           - node
           - space
         value: "{{power_ops_instance_space}}"
-        # - not:
-        #     hasData:
-        #       - type: view
-        #         space: "{{power_ops_models}}"
-        #         externalId: FunctionOutput
-        #         version: "{{version}}"
-        # - equals:
+        # - exists:
         #     property:
-        #       - node
-        #       - type
-        #     value:
-        #       externalId: FunctionInput
-        #       space: "{{power_ops_type_space}}"
-        # - not:
-        #     in:
-        #       property:
-        #         - node
-        #         - type
-        #       values: [FunctionOutput]
+        #       - input
 implements: []
 version: "{{version}}"
 properties:
   workflowExecutionId:
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: workflowExecutionId
     name: workflowExecutionId
     description: The process associated with the function execution
   workflowStep:
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: workflowStep
     name: workflowStep
     description: This is the step in the process.
   functionName:
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: functionName
     name: functionName
     description: The name of the function
   functionCallId:
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: functionCallId
     name: functionCallId
     description: The function call id
+  input:
+    container:
+      space: "{{power_ops_models}}"
+      externalId: FunctionData
+      type: container
+    containerPropertyIdentifier: linkedStep
+    name: input
+    source:
+      space: "{{power_ops_models}}"
+      externalId: FunctionInput
+      version: "{{version}}"
+      type: view
+  alerts:
+    type:
+      space: "{{power_ops_type_space}}"
+      externalId: calculationIssue
+    source:
+      space: "{{power_ops_models}}"
+      externalId: Alert
+      version: "{{version}}"
+      type: view
+    direction: outwards
+    name: alerts
+    description: An array of calculation level Alerts.
+    connectionType: multi_edge_connection
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,91 @@
 space: "{{power_ops_models}}"
-externalId: FunctionOutput
-name: FunctionOutput
-description: Base class for all function inputs
+externalId: ShopResult
+name: ShopResult
+description: A generic shop result type that collects all time series outputs from SHOP. This type replaces the POWEROPS_SHOP_RUN event in cdf today
 filter:
   and:
     - hasData:
         - type: container
           space: "{{power_ops_models}}"
-          externalId: FunctionMetadata
+          externalId: ShopResult
     - equals:
         property:
           - node
           - space
         value: "{{power_ops_instance_space}}"
-        # - not:
-        #     equals:
-        #       property:
-        #         - node
-        #         - type
-        #       value: {
-        #           "space": "{{power_ops_instance_space}}",
-        #           "externalId": "FunctionInput",
-        #         } #FunctionInput
-        # - not:
-        #     in:
-        #       property:
-        #         - node
-        #         - type
-        #       values: [FunctionInput]
 implements: []
 version: "{{version}}"
 properties:
-  workflowExecutionId:
+  case:
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: ShopResult
       type: container
-    containerPropertyIdentifier: workflowExecutionId
-    name: workflowExecutionId
-    description: The process associated with the function execution
-  workflowStep:
+    containerPropertyIdentifier: case
+    name: case
+    description: The case that was used to produce this result
+    source:
+      space: "{{power_ops_models}}"
+      externalId: ShopCase
+      version: "{{version}}"
+      type: view
+  objectiveSequence:
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: ShopResult
       type: container
-    containerPropertyIdentifier: workflowStep
-    name: workflowStep
-    description: This is the step in the process.
-  functionName:
+    containerPropertyIdentifier: objectiveSequence
+    name: objectiveSequence
+    description: The sequence of the objective function
+  preRun:
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: ShopResult
       type: container
-    containerPropertyIdentifier: functionName
-    name: functionName
-    description: The name of the function
-  functionCallId:
+    containerPropertyIdentifier: preRun
+    name: preRun
+    description: The pre-run data for the SHOP run
+  postRun:
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: ShopResult
       type: container
-    containerPropertyIdentifier: functionCallId
-    name: functionCallId
-    description: The function call id
-  input:
+    containerPropertyIdentifier: postRun
+    name: postRun
+    description: The post-run data for the SHOP run
+  messages:
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: ShopResult
       type: container
-    containerPropertyIdentifier: linkedStep
-    name: input
+    containerPropertyIdentifier: messages
+    name: messages
+    description: The messages from the SHOP run
+  cplexLogs:
+    container:
+      space: "{{power_ops_models}}"
+      externalId: ShopResult
+      type: container
+    containerPropertyIdentifier: cplexLogs
+    name: cplexLogs
+    description: The logs from CPLEX
+  outputTimeSeries:
+    type:
+      space: "{{power_ops_type_space}}"
+      externalId: ShopResult.outputTimeSeries
     source:
       space: "{{power_ops_models}}"
-      externalId: FunctionInput
+      externalId: ShopTimeSeries
       version: "{{version}}"
       type: view
+    direction: outwards
+    name: outputTimeSeries
+    description: TODO
+    connectionType: multi_edge_connection
   alerts:
     type:
       space: "{{power_ops_type_space}}"
       externalId: calculationIssue
     source:
       space: "{{power_ops_models}}"
       externalId: Alert
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     version: "{{version}}"
     type: view
 version: "{{version}}"
 properties:
   input: # Overrides the view type from the FunctionOutput view
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: linkedStep
     name: input
     source:
       space: "{{power_ops_models}}"
       externalId: BenchmarkingCollectorInput
       version: "{{version}}"
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     version: "{{version}}"
     type: view
 version: "{{version}}"
 properties:
   input: # Overrides the view type from the FunctionOutput view
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: linkedStep
     name: input
     source:
       space: "{{power_ops_models}}"
       externalId: PartialBidMatrixCalculationInput
       version: "{{version}}"
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     version: "{{version}}"
     type: view
 version: "{{version}}"
 properties:
   input: # Overrides the view type from the FunctionOutput view
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: linkedStep
     name: input
     source:
       space: "{{power_ops_models}}"
       externalId: ShopTriggerInput
       version: "{{version}}"
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     version: "{{version}}"
     type: view
 version: "{{version}}"
 properties:
   input: # Overrides the view type from the FunctionOutput view
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: linkedStep
     name: input
     source:
       space: "{{power_ops_models}}"
       externalId: ShopPreprocessorInput
       version: "{{version}}"
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     version: "{{version}}"
     type: view
 version: "{{version}}"
 properties:
   input: # Overrides the view type from the FunctionOutput view
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: linkedStep
     name: input
     source:
       space: "{{power_ops_models}}"
       externalId: TaskDispatcherBenchmarkingInput
       version: "{{version}}"
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     version: "{{version}}"
     type: view
 version: "{{version}}"
 properties:
   input: # Overrides the view type from the FunctionOutput view
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: linkedStep
     name: input
     source:
       space: "{{power_ops_models}}"
       externalId: TaskDispatcherInput
       version: "{{version}}"
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     version: "{{version}}"
     type: view
 version: "{{version}}"
 properties:
   input: # Overrides the view type from the FunctionOutput view
     container:
       space: "{{power_ops_models}}"
-      externalId: FunctionMetadata
+      externalId: FunctionData
       type: container
     containerPropertyIdentifier: linkedStep
     name: input
     source:
       space: "{{power_ops_models}}"
       externalId: TotalBidMatrixCalculationInput
       version: "{{version}}"
```

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml` & `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/prerun_transformations/transformations.py` & `cognite_power_ops-0.94.1/cognite/powerops/prerun_transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/_main.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/_main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/_settings.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/_settings.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/_shared.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/_shared.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/cogshop/shop_file_config.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/cogshop/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/_core.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/benchmarking.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/benchmarking.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/dayahead.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/dayahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/market.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/market.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/market/rkom.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/rkom.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/production/connections.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/connections.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/production/generator.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/production/plant.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/config/production/watercourse.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/core/cdf.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/core/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/core/main.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/core/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/core/transform.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/core/transform.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/core/validation.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/core/validation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/diff/core.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/diff/core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/diff/data_classes.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/diff/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/_shared_v1_v2/market_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/market_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/_shared_v1_v2/production_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/production_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/asset_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/asset_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/asset_type.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/asset_type.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/cdf_resources.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/cdf_resources.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/data_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/data_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/dms_models.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/dms_models.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/graph_ql.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/graph_ql.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/base/resource_type.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/resource_type.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/cogshop.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/cogshop.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/__init__.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/base.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/base.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/benchmark.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/benchmark.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/dayahead.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/dayahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/market/rkom.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/rkom.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v1/production.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v2/powerops_models.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/powerops_models.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/models/v2/production_dm.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/production_dm.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/time_series_mapping/mapping.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/time_series_mapping/static_mapping.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/v2/shop_to_assets.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/v2/shop_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/resync/validation.py` & `cognite_power_ops-0.94.1/cognite/powerops/resync/validation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/_cdf_auth.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/_cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/_settings.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/_settings.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/calls.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/calls.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/extraction_pipelines.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/extraction_pipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/cdf/resource_creation.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/resource_creation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/lookup.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/navigation.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/navigation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/require.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/require.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/retry/api.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/retry/api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/serialization.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/cognite/powerops/utils/time.py` & `cognite_power_ops-0.94.1/cognite/powerops/utils/time.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.0/pyproject.toml` & `cognite_power_ops-0.94.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.94.0"
+version = "0.94.1"
 description = "SDK for power markets operations on Cognite Data Fusion"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 documentation = "https://cognite-power-ops-sdk.readthedocs-hosted.com/en/latest/"
 homepage = "https://cognite-power-ops-sdk.readthedocs-hosted.com/en/latest/"
 repository = "https://github.com/cognitedata/power-ops-sdk"
```

### Comparing `cognite_power_ops-0.94.0/PKG-INFO` & `cognite_power_ops-0.94.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.94.0
+Version: 0.94.1
 Summary: SDK for power markets operations on Cognite Data Fusion
 Home-page: https://cognite-power-ops-sdk.readthedocs-hosted.com/en/latest/
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
```

