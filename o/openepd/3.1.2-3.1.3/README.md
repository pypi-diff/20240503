# Comparing `tmp/openepd-3.1.2.tar.gz` & `tmp/openepd-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-3.1.2.tar", max compression
+gzip compressed data, was "openepd-3.1.3.tar", max compression
```

## Comparing `openepd-3.1.2.tar` & `openepd-3.1.3.tar`

### file list

```diff
@@ -1,95 +1,92 @@
--rw-r--r--   0        0        0    11357 2024-04-23 17:16:43.101493 openepd-3.1.2/LICENSE
--rw-r--r--   0        0        0     6786 2024-04-23 17:16:43.101493 openepd-3.1.2/README.md
--rw-r--r--   0        0        0     3147 2024-04-23 17:16:43.105493 openepd-3.1.2/pyproject.toml
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/__init__.py
--rw-r--r--   0        0        0    21142 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/base_sync_client.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/category/__init__.py
--rw-r--r--   0        0        0     1067 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/category/dto.py
--rw-r--r--   0        0        0     1588 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/category/sync_api.py
--rw-r--r--   0        0        0     8681 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/common.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/base.py
--rw-r--r--   0        0        0     4705 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/common.py
--rw-r--r--   0        0        0     2377 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/meta.py
--rw-r--r--   0        0        0     2211 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/mf.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/params.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/epd/__init__.py
--rw-r--r--   0        0        0     5091 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/epd/dto.py
--rw-r--r--   0        0        0     4391 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/epd/sync_api.py
--rw-r--r--   0        0        0     2376 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/errors.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/pcr/__init__.py
--rw-r--r--   0        0        0     1649 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/pcr/dto.py
--rw-r--r--   0        0        0     1805 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/pcr/sync_api.py
--rw-r--r--   0        0        0     2504 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/sync_client.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/test/__init__.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/bundle/__init__.py
--rw-r--r--   0        0        0     7086 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/bundle/base.py
--rw-r--r--   0        0        0     2663 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/bundle/model.py
--rw-r--r--   0        0        0     6904 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/bundle/reader.py
--rw-r--r--   0        0        0     8353 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/bundle/writer.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/compat/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/compat/pydantic.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     9154 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/base.py
--rw-r--r--   0        0        0     1856 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/category.py
--rw-r--r--   0        0        0     5659 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/common.py
--rw-r--r--   0        0        0    14299 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/epd.py
--rw-r--r--   0        0        0     1918 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/factory.py
--rw-r--r--   0        0        0    17165 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     4013 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/org.py
--rw-r--r--   0        0        0     4620 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/pcr.py
--rw-r--r--   0        0        0      862 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/README.md
--rw-r--r--   0        0        0     5176 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     2271 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/aluminium.py
--rw-r--r--   0        0        0     3549 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/asphalt.py
--rw-r--r--   0        0        0     2697 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/base.py
--rw-r--r--   0        0        0    15961 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1934 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/accessories.py
--rw-r--r--   0        0        0     3161 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/aggregates.py
--rw-r--r--   0        0        0     2440 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/aluminium.py
--rw-r--r--   0        0        0     3837 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/asphalt.py
--rw-r--r--   0        0        0     1034 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/bulk_materials.py
--rw-r--r--   0        0        0     1058 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
--rw-r--r--   0        0        0     6939 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/cladding.py
--rw-r--r--   0        0        0     2324 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/cmu.py
--rw-r--r--   0        0        0     1117 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/common.py
--rw-r--r--   0        0        0     8324 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/concrete.py
--rw-r--r--   0        0        0     2422 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/conveying_equipment.py
--rw-r--r--   0        0        0    10457 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/electrical.py
--rw-r--r--   0        0        0     2117 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
--rw-r--r--   0        0        0     1029 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/electricity.py
--rw-r--r--   0        0        0    58482 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/enums.py
--rw-r--r--   0        0        0    22337 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/finishes.py
--rw-r--r--   0        0        0     2801 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/fire_and_smoke_protection.py
--rw-r--r--   0        0        0     3076 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/furnishings.py
--rw-r--r--   0        0        0     1023 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/grouting.py
--rw-r--r--   0        0        0     4599 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/manufacturing_inputs.py
--rw-r--r--   0        0        0     3177 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/masonry.py
--rw-r--r--   0        0        0     1225 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/material_handling.py
--rw-r--r--   0        0        0    11561 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/mechanical.py
--rw-r--r--   0        0        0     1900 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/mechanical_insulation.py
--rw-r--r--   0        0        0     8644 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/network_infrastructure.py
--rw-r--r--   0        0        0    19729 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/openings.py
--rw-r--r--   0        0        0     1057 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/other_electrical_equipment.py
--rw-r--r--   0        0        0     3453 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/other_materials.py
--rw-r--r--   0        0        0     5439 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/plumbing.py
--rw-r--r--   0        0        0     2690 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/precast_concrete.py
--rw-r--r--   0        0        0     3516 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/sheathing.py
--rw-r--r--   0        0        0    10255 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/steel.py
--rw-r--r--   0        0        0     7963 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/thermal_moisture_protection.py
--rw-r--r--   0        0        0     2768 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/utility_piping.py
--rw-r--r--   0        0        0     6199 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/wood.py
--rw-r--r--   0        0        0     1880 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/wood_joists.py
--rw-r--r--   0        0        0    13664 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/glass.py
--rw-r--r--   0        0        0     6367 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/steel.py
--rw-r--r--   0        0        0     5144 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/wood.py
--rw-r--r--   0        0        0     1535 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/standard.py
--rw-r--r--   0        0        0      837 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/validation/__init__.py
--rw-r--r--   0        0        0     2652 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/validation/common.py
--rw-r--r--   0        0        0     1105 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/validation/numbers.py
--rw-r--r--   0        0        0     5287 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/validation/quantity.py
--rw-r--r--   0        0        0     4690 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/versioning.py
--rw-r--r--   0        0        0        0 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/py.typed
--rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 openepd-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-03 17:44:36.520837 openepd-3.1.3/LICENSE
+-rw-r--r--   0        0        0     6786 2024-05-03 17:44:36.520837 openepd-3.1.3/README.md
+-rw-r--r--   0        0        0     3147 2024-05-03 17:44:36.524837 openepd-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/__init__.py
+-rw-r--r--   0        0        0    21142 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/base_sync_client.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/category/__init__.py
+-rw-r--r--   0        0        0     1067 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/category/dto.py
+-rw-r--r--   0        0        0     1588 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/category/sync_api.py
+-rw-r--r--   0        0        0     8681 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/common.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/dto/__init__.py
+-rw-r--r--   0        0        0     1250 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/dto/base.py
+-rw-r--r--   0        0        0     4705 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/dto/common.py
+-rw-r--r--   0        0        0     2377 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/dto/meta.py
+-rw-r--r--   0        0        0     2211 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/dto/mf.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/dto/params.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/epd/__init__.py
+-rw-r--r--   0        0        0     5091 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/epd/dto.py
+-rw-r--r--   0        0        0     4391 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/epd/sync_api.py
+-rw-r--r--   0        0        0     2376 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/errors.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/pcr/__init__.py
+-rw-r--r--   0        0        0     1649 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/pcr/dto.py
+-rw-r--r--   0        0        0     1805 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/pcr/sync_api.py
+-rw-r--r--   0        0        0     2504 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/sync_client.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/api/test/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/bundle/__init__.py
+-rw-r--r--   0        0        0     7086 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/bundle/base.py
+-rw-r--r--   0        0        0     2663 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/bundle/model.py
+-rw-r--r--   0        0        0     6904 2024-05-03 17:44:36.524837 openepd-3.1.3/src/openepd/bundle/reader.py
+-rw-r--r--   0        0        0     8353 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/bundle/writer.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/compat/__init__.py
+-rw-r--r--   0        0        0     1051 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/compat/compat_functional_validators.py
+-rw-r--r--   0        0        0     1363 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/compat/pydantic.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     9154 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/base.py
+-rw-r--r--   0        0        0     1856 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/category.py
+-rw-r--r--   0        0        0     5659 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/common.py
+-rw-r--r--   0        0        0    14299 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     1918 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/factory.py
+-rw-r--r--   0        0        0    17165 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     4013 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/org.py
+-rw-r--r--   0        0        0     4620 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0      862 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/README.md
+-rw-r--r--   0        0        0     5176 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3549 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/asphalt.py
+-rw-r--r--   0        0        0     2697 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/base.py
+-rw-r--r--   0        0        0     9810 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1934 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/accessories.py
+-rw-r--r--   0        0        0     3161 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/aggregates.py
+-rw-r--r--   0        0        0     2440 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/aluminium.py
+-rw-r--r--   0        0        0     3365 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/asphalt.py
+-rw-r--r--   0        0        0     1034 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/bulk_materials.py
+-rw-r--r--   0        0        0     1058 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
+-rw-r--r--   0        0        0     6475 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/cladding.py
+-rw-r--r--   0        0        0     2000 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/cmu.py
+-rw-r--r--   0        0        0     1117 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/common.py
+-rw-r--r--   0        0        0     7204 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/concrete.py
+-rw-r--r--   0        0        0     1986 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/conveying_equipment.py
+-rw-r--r--   0        0        0     9996 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/electrical.py
+-rw-r--r--   0        0        0     2117 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
+-rw-r--r--   0        0        0     1029 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/electricity.py
+-rw-r--r--   0        0        0    58482 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/enums.py
+-rw-r--r--   0        0        0    20292 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/finishes.py
+-rw-r--r--   0        0        0     2665 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/fire_and_smoke_protection.py
+-rw-r--r--   0        0        0     2940 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/furnishings.py
+-rw-r--r--   0        0        0     1023 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/grouting.py
+-rw-r--r--   0        0        0     4599 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/manufacturing_inputs.py
+-rw-r--r--   0        0        0     3216 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/masonry.py
+-rw-r--r--   0        0        0     1225 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/material_handling.py
+-rw-r--r--   0        0        0     8388 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/mechanical.py
+-rw-r--r--   0        0        0     1714 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/mechanical_insulation.py
+-rw-r--r--   0        0        0     7924 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/network_infrastructure.py
+-rw-r--r--   0        0        0    19035 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/openings.py
+-rw-r--r--   0        0        0     1057 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/other_electrical_equipment.py
+-rw-r--r--   0        0        0     3453 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/other_materials.py
+-rw-r--r--   0        0        0     4652 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/plumbing.py
+-rw-r--r--   0        0        0     2490 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/precast_concrete.py
+-rw-r--r--   0        0        0     3516 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/sheathing.py
+-rw-r--r--   0        0        0    10119 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/steel.py
+-rw-r--r--   0        0        0     7368 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/thermal_moisture_protection.py
+-rw-r--r--   0        0        0     2372 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/utility_piping.py
+-rw-r--r--   0        0        0     6027 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/wood.py
+-rw-r--r--   0        0        0     1880 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/specs/generated/wood_joists.py
+-rw-r--r--   0        0        0     1535 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/standard.py
+-rw-r--r--   0        0        0      837 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/validation/__init__.py
+-rw-r--r--   0        0        0     2652 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/validation/common.py
+-rw-r--r--   0        0        0     1105 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/validation/numbers.py
+-rw-r--r--   0        0        0     7411 2024-05-03 17:44:36.528837 openepd-3.1.3/src/openepd/model/validation/quantity.py
+-rw-r--r--   0        0        0     4690 2024-05-03 17:44:36.532837 openepd-3.1.3/src/openepd/model/versioning.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:44:36.532837 openepd-3.1.3/src/openepd/py.typed
+-rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 openepd-3.1.3/PKG-INFO
```

### Comparing `openepd-3.1.2/LICENSE` & `openepd-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/README.md` & `openepd-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/pyproject.toml` & `openepd-3.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "3.1.2"
+version = "3.1.3"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
```

### Comparing `openepd-3.1.2/src/openepd/__init__.py` & `openepd-3.1.3/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/__version__.py` & `openepd-3.1.3/src/openepd/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "3.1.2"
+VERSION = "3.1.3"
```

### Comparing `openepd-3.1.2/src/openepd/api/__init__.py` & `openepd-3.1.3/src/openepd/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/base_sync_client.py` & `openepd-3.1.3/src/openepd/api/base_sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/category/__init__.py` & `openepd-3.1.3/src/openepd/api/category/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/category/dto.py` & `openepd-3.1.3/src/openepd/api/category/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/category/sync_api.py` & `openepd-3.1.3/src/openepd/api/category/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/common.py` & `openepd-3.1.3/src/openepd/api/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/dto/__init__.py` & `openepd-3.1.3/src/openepd/api/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/dto/base.py` & `openepd-3.1.3/src/openepd/api/dto/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/dto/common.py` & `openepd-3.1.3/src/openepd/api/dto/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/dto/meta.py` & `openepd-3.1.3/src/openepd/api/dto/meta.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/dto/mf.py` & `openepd-3.1.3/src/openepd/api/dto/mf.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/dto/params.py` & `openepd-3.1.3/src/openepd/api/dto/params.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/epd/__init__.py` & `openepd-3.1.3/src/openepd/api/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/epd/dto.py` & `openepd-3.1.3/src/openepd/api/epd/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/epd/sync_api.py` & `openepd-3.1.3/src/openepd/api/epd/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/errors.py` & `openepd-3.1.3/src/openepd/api/errors.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/pcr/__init__.py` & `openepd-3.1.3/src/openepd/api/pcr/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/pcr/dto.py` & `openepd-3.1.3/src/openepd/api/pcr/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/pcr/sync_api.py` & `openepd-3.1.3/src/openepd/api/pcr/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/sync_client.py` & `openepd-3.1.3/src/openepd/api/sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/api/test/__init__.py` & `openepd-3.1.3/src/openepd/api/test/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/bundle/__init__.py` & `openepd-3.1.3/src/openepd/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/bundle/base.py` & `openepd-3.1.3/src/openepd/bundle/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/bundle/model.py` & `openepd-3.1.3/src/openepd/bundle/model.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/bundle/reader.py` & `openepd-3.1.3/src/openepd/bundle/reader.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/bundle/writer.py` & `openepd-3.1.3/src/openepd/bundle/writer.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/compat/__init__.py` & `openepd-3.1.3/src/openepd/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/compat/pydantic.py` & `openepd-3.1.3/src/openepd/model/validation/numbers.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-try:
-    from pydantic import v1 as pyd  # type: ignore
-    from pydantic.v1 import generics as pyd_generics  # type: ignore
-except ImportError:
-    import pydantic as pyd  # type: ignore[no-redef]
-    from pydantic import generics as pyd_generics  # type: ignore[no-redef]
+from typing import Annotated
 
-pydantic = pyd
+from openepd.compat.pydantic import pyd
 
-__all__ = ["pyd", "pydantic", "pyd_generics"]
+# todo when move to pydantic 2, check that validators are being enforced.
+RatioFloat = Annotated[float, pyd.Field(ge=0, le=1, example=0.5)]
+PositiveInt = Annotated[int, pyd.Field(ge=0, example=1)]
```

### Comparing `openepd-3.1.2/src/openepd/model/__init__.py` & `openepd-3.1.3/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/base.py` & `openepd-3.1.3/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/category.py` & `openepd-3.1.3/src/openepd/model/category.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/common.py` & `openepd-3.1.3/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/epd.py` & `openepd-3.1.3/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/factory.py` & `openepd-3.1.3/src/openepd/model/factory.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/lcia.py` & `openepd-3.1.3/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/org.py` & `openepd-3.1.3/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/pcr.py` & `openepd-3.1.3/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/README.md` & `openepd-3.1.3/src/openepd/model/specs/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/__init__.py` & `openepd-3.1.3/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/asphalt.py` & `openepd-3.1.3/src/openepd/model/specs/asphalt.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/base.py` & `openepd-3.1.3/src/openepd/model/specs/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/concrete.py` & `openepd-3.1.3/src/openepd/model/specs/generated/openings.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,349 +13,529 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from enum import StrEnum
-from typing import Literal
 
 from openepd.compat.pydantic import pyd
 from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.common import OpenEPDUnit
-from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec, BaseOpenEpdSpec
-from openepd.model.specs.generated.enums import AciExposureClass, CsaExposureClass, EnExposureClass
-from openepd.model.validation.common import together_validator
+from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
+from openepd.model.specs.generated.enums import (
+    FlatGlassPanesThickness,
+    FrameMaterial,
+    HardwareFunction,
+    NAFSPerformanceGrade,
+    Spacer,
+    ThermalSeparation,
+)
 from openepd.model.validation.numbers import RatioFloat
-from openepd.model.validation.quantity import LengthMmStr, PressureMPaStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr, PressureMPaStr, SpeedStr, validate_unit_factory
 
 
-class CmuWeightClassification(StrEnum):
-    """Concrete Masonry Unit weight classification."""
+class GlazingIntendedApplication(BaseOpenEpdSchema):
+    """Glass intended application mixin."""
 
-    Normal = "Normal"
-    """Normal weight CMU has a density of 125 lbs/cu. ft."""
-    Medium = "Medium"
-    """Medium weight CMU has a density of 105-125 lbs/cu. ft."""
-    Light = "Light"
-    """Lightweight CMU has a density less than 105 lbs/cu. ft."""
-
-
-class CmuOptions(BaseOpenEpdSchema):
-    """Concrete Masonry Unit options."""
-
-    load_bearing: bool | None = pyd.Field(
-        description="Load-Bearing. CMUs intended to be loadbearing, rather than simply cosmetic",
-        example=True,
+    curtain_wall: bool | None = pyd.Field(default=None, description="Intended for curtain walls. Relevant for IGUs.")
+    r_windows: bool | None = pyd.Field(
         default=None,
+        description="Intended for residential (NAFS 'R') and similar windows, doors, or skylights. Relevant for IGUs.",
     )
-    aerated_concrete: bool | None = pyd.Field(
-        description="AAC Aerated Concrete. Aerated Autoclaved Concrete, a foam concrete.", example=True, default=None
-    )
-    insulated: bool | None = pyd.Field(
-        description="Insulated. CMUs with integral insulation", example=True, default=None
-    )
-    sound_absorbing: bool | None = pyd.Field(
-        description="Sound Absorbing. CMUs structured for sound absorbtion", example=True, default=None
+    lc_windows: bool | None = pyd.Field(
+        default=None, description="Intended for light commercial (NAFS 'LC') and similar windows. Relevant for IGUs."
     )
-    white: bool | None = pyd.Field(
-        description="White. CMU using white cement and light-colored aggregate", example=True, default=None
+    cw_windows: bool | None = pyd.Field(
+        default=None, description="Intended for commercial (NAFS 'CW') and similar windows. Relevant for IGUs."
     )
-    recycled_aggregate: bool | None = pyd.Field(
-        description="Recycled aggregate. CMU using primarily reycled aggregates", example=True, default=None
+    aw_windows: bool | None = pyd.Field(
+        default=None, description="Intended for architectural (NAFS 'AW') and similar windows. Relevant for IGUs."
     )
-    groundface: bool | None = pyd.Field(
-        description="Ground Face. Ground or Honed facing, typically for improved appearance", example=True, default=None
+    storefronts: bool | None = pyd.Field(
+        default=None, description="Intended for Storefronts and similar applications. Relevant for IGUs."
     )
-    splitface: bool | None = pyd.Field(
-        description="Splitface. Rough surface texture via splitting; aggregate can be seen", example=True, default=None
+    glazed_doors: bool | None = pyd.Field(
+        default=None, description="Intended for Glazed Doors and similar applications. Relevant for IGUs."
     )
-    smoothface: bool | None = pyd.Field(
-        description="Smooth Face. Standard smooth-faced blocks", example=True, default=None
+    unit_skylights: bool | None = pyd.Field(
+        default=None, description="Intended for Unit Skylights and similar applications. Relevant for IGUs."
     )
-    slumpstone: bool | None = pyd.Field(
-        description="Slumpstone. A slightly rounded, random distortion with the look of rustic adobe.",
-        example=True,
+    sloped_skylights: bool | None = pyd.Field(
         default=None,
+        description="Intended for sloped glazing, and architectural skylights, and similar. Relevant for IGUs.",
+    )
+    other: bool | None = pyd.Field(
+        default=None, description="Intended for other application not listed. Relevant for IGUs."
     )
 
 
-class ConcreteTypicalApplication(BaseOpenEpdSpec):
-    """Typical Application for Concrete."""
+class GlazingOptionsMixin(BaseOpenEpdSchema):
+    """Common glazing options."""
 
-    fnd: bool | None = pyd.Field(
-        description="Foundation. Typically used in direct contact with soil, e.g. footings, piles, mass concrete, "
-        "mat foundations, and similar applications.",
-        example=True,
+    low_emissivity: bool | None = pyd.Field(default=None, description="Low Emissivity coatings", example=True)
+    electrochromic: bool | None = pyd.Field(
         default=None,
-    )
-    sog: bool | None = pyd.Field(
-        description="Slab on Grade. Typically used in continuously supported horizontal "
-        "applications e.g. slab on grade, topping slabs, sidewalks, and roadways.",
+        description="Glazing with an electrically controllable solar heat gain and/or other properties.",
         example=True,
-        default=None,
     )
-    hrz: bool | None = pyd.Field(
-        description="Elevated Horizontal. Typically used in elevated horizontal applications, either on metal deck or "
-        "where soffit formwork must be removed, e.g. post-tension plates, rebar plates, beams and slabs, "
-        "waffle slabs.",
-        example=True,
-        default=None,
+    acid_etched: bool | None = pyd.Field(
+        default=None, description="Flat glass that has undergone a chemical etching process.", example=True
     )
-    vrt_wall: bool | None = pyd.Field(description="Vertical Wall.", example=True, default=None)
-    vrt_column: bool | None = pyd.Field(description="Vertical Column.", example=True, default=None)
-    vrt_other: bool | None = pyd.Field(
-        description="Vertical Other. Typically used in vertical applications other than "
-        "walls or columns, e.g. sloped surfaces where formwork is required "
-        "on multiple faces.",
-        example=True,
+    tempered: bool | None = pyd.Field(
         default=None,
-    )
-    sht: bool | None = pyd.Field(
-        description="Shotcrete. Pneumatically applied, without formwork on all sides.", example=True, default=None
-    )
-    cdf: bool | None = pyd.Field(
-        description="Flowable Fill (CDF). Typically used to fill voids, backfill retaining "
-        "walls, as a sub-base, and similar applications. Also called Controlled "
-        "Density Fill (CDF) or Controlled Low Strength Materials (CLSM).",
+        description="Consists of a single pane that has been heat-treated to give the glass increased impact "
+        "resistance. Standard typically used in North America.",
         example=True,
-        default=None,
     )
-    sac: bool | None = pyd.Field(
-        description="Typically used in concrete sidewalks and barrier curbs.", example=True, default=None
+    toughened: bool | None = pyd.Field(
+        default=None,
+        description="Consists of a single pane that has been specially heat-treated to give the glass increased impact "
+        "resistance. Standard typically used in Europe.",
+        example=True,
     )
-    pav: bool | None = pyd.Field(description="Typically used in pervious concrete", example=True, default=None)
-    oil: bool | None = pyd.Field(
-        description="Concretes for use in creation, maintenance, and decommissioning of "
-        "petroleum extraction wells and similar applications. Includes foamed "
-        "cement; often called cement in the drilling industry. Differs from "
-        "flowable fill and grout in that it contains no sand or other aggregates.",
+    laminated: bool | None = pyd.Field(
+        default=None,
+        description="Consists of at least two glass panes lying one on top of the other, with one or several layers of "
+        "a tear-resistant, viscoelastic film positioned between the panes, which consist of polyvinyl "
+        "butyral (PVB)",
         example=True,
+    )
+    fire_resistant: bool | None = pyd.Field(default=None, example=True)
+    fire_protection: bool | None = pyd.Field(
         default=None,
+        description="Specifically tested for its ability to block flames and smoke, but not radiant heat. Ranges from"
+        " specialty tempered products rated for ~20 minutes to glass ceramics rated up to 3 hours.",
+        example=True,
     )
-    grt: bool | None = pyd.Field(
-        description="Cement grouting is a slurry that is placed as a flowable liquid. It is "
-        "an effective material for filling and strengthening granular soils, "
-        "voids in rocks, foundation underpinnings, and other underground voids. "
-        "Also called structural grout, these materials typically impart"
-        " significant strength to the system",
+    pyrolytic_coated: bool | None = pyd.Field(
+        default=None,
+        description="At least one coating is applied in a pyrolytic process, typically during float glass production.",
         example=True,
+    )
+    sputter_coat: bool | None = pyd.Field(
         default=None,
+        description="At least one coating is applied using sputter (vacuum deposition) coating.",
+        example=True,
     )
-    ota: bool | None = pyd.Field(
-        description="Typical application not covered by other values.", example=True, default=None
+    solar_heat_gain: RatioFloat | None = pyd.Field(
+        default=None,
+        description="Solar heat gain, measured at a certain level of Differential Pressure. Range is 0 to 1.",
+        example=0.5,
+        ge=0,
+        le=1,
     )
 
 
-class CmuSpec(BaseOpenEpdSpec):
-    """Standardized Concrete Masonry Unit-specific extension for OpenEPD."""
+class PanelDoorsV1(BaseOpenEpdHierarchicalSpec):
+    """Panel doors performance specification."""
 
-    strength: str = pyd.Field(description="Compressive strength", example="4000 psi")
-    options: CmuOptions = pyd.Field(
-        description="Options for CMU. List of true/false properties", default_factory=CmuOptions
-    )
+    _EXT_VERSION = "1.0"
 
 
-class Cementitious(BaseOpenEpdSchema):
-    """List of cementitious materials, and proportion by mass."""
+class PressureResistantDoorsV1(BaseOpenEpdHierarchicalSpec):
+    """Pressure-Resistant Doors."""
+
+    _EXT_VERSION = "1.0"
+
+
+class SpecialFunctionDoorsV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Special function doors.
+
+    Includes doors for e.g., cold storage, hangars, lightproof applications,
+    security, sound control, vaults, etc.
+    """
+
+    _EXT_VERSION = "1.0"
+
+    # Nested specs:
+    PanelDoors: PanelDoorsV1 | None = None
+    PressureResistantDoors: PressureResistantDoorsV1 | None = None
 
-    opc: RatioFloat | None = pyd.Field(
-        default=None, description="Ordinary Gray Portland Cement", example=0.5, ge=0, le=1
-    )
-    wht: RatioFloat | None = pyd.Field(default=None, description="White Portland Cement", example=0.5, ge=0, le=1)
-    ggbs: RatioFloat | None = pyd.Field(
-        default=None, description="Ground Granulated Blast Furnace Slag", example=0.5, ge=0, le=1
-    )
-    flyAsh: RatioFloat | None = pyd.Field(
-        default=None, description="Fly Ash, including types F, CL, and CH", example=0.5, ge=0, le=1
-    )
-    siFume: RatioFloat | None = pyd.Field(default=None, description="Silica Fume", example=0.5, ge=0, le=1)
-    gg45: RatioFloat | None = pyd.Field(
-        default=None, description="Ground Glass, 45um or smaller", example=0.5, ge=0, le=1
-    )
-    natPoz: RatioFloat | None = pyd.Field(default=None, description="Natural pozzolan", example=0.5, ge=0, le=1)
-    mk: RatioFloat | None = pyd.Field(default=None, description="Metakaolin", example=0.5, ge=0, le=1)
-    CaCO3: RatioFloat | None = pyd.Field(default=None, description="Limestone", example=0.5, ge=0, le=1)
-    other: RatioFloat | None = pyd.Field(default=None, description="Other SCMs", example=0.5, ge=0, le=1)
 
+class SlidingGlassDoorsV1(BaseOpenEpdHierarchicalSpec):
+    """Sliding glass doors performance specification."""
 
-class TypicalApplication(BaseOpenEpdSchema):
-    """Concrete typical application."""
+    _EXT_VERSION = "1.0"
+
+
+class FenestrationAccessoriesV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Fenestration accessories.
+
+    Gaskets, seals, fasteners, and other low-mass items which may be useful in calculating the impact of a
+    fenestration system.
+    """
+
+    _EXT_VERSION = "1.0"
+
+
+class FenestrationFramingV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Fenestration Framing.
+
+    Lineal elements ("sticks") for use in fenestration, including frames, sashes, and mullions.
+    """
+
+    _EXT_VERSION = "1.0"
+
+    # Own fields:
+    thermal_separation: ThermalSeparation | None = pyd.Field(default=None, example="Aluminium")
+    material: FrameMaterial | None = pyd.Field(default=None, example="Vinyl")
+
+
+class FenestrationHardwareV1(BaseOpenEpdHierarchicalSpec):
+    """Locks, operation hardware, and other substantial items declared on a per-piece basis."""
+
+    _EXT_VERSION = "1.0"
+
+    # Own fields:
+    function: HardwareFunction | None = pyd.Field(default=None, description="", example="Lock")
 
-    fnd: bool | None = pyd.Field(description="Foundation", default=None)
-    sog: bool | None = pyd.Field(description="Slab on Grade", default=None)
-    hrz: bool | None = pyd.Field(description="Elevated Horizontal", default=None)
-    vrt_wall: bool | None = pyd.Field(description="Vertical Wall", default=None)
-    vrt_column: bool | None = pyd.Field(description="Vertical Column", default=None)
-    vrt_other: bool | None = pyd.Field(description="Vertical Other", default=None)
-    sht: bool | None = pyd.Field(description="Shotcrete", default=None)
-    cdf: bool | None = pyd.Field(description="Flowable Fill (CDF,default=None)", default=None)
-    sac: bool | None = pyd.Field(description="Sidewalk and Curb", default=None)
-    pav: bool | None = pyd.Field(description="Paving", default=None)
-    oil: bool | None = pyd.Field(description="Oil Patch", default=None)
-    grt: bool | None = pyd.Field(description="Cement Grout", default=None)
-    ota: bool | None = pyd.Field(description="Other", default=None)
 
+class FlatGlassPanesV1(BaseOpenEpdHierarchicalSpec):
+    """Monolithic, uncoated flat glass panes that are not substantially processed."""
 
-class ConcreteV1Options(BaseOpenEpdSchema):
-    """Concrete options."""
+    _EXT_VERSION = "1.0"
+
+    # Own fields:
+    thickness: FlatGlassPanesThickness | None = pyd.Field(default=None, example="12 mm")
+
+    _flat_glass_panes_thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(
+        validate_unit_factory("m")
+    )
 
-    lightweight: bool | None = pyd.Field(description="Lightweight", default=None)
-    plc: bool | None = pyd.Field(description="Portland Limestone Cement", default=None)
-    scc: bool | None = pyd.Field(description="Self Compacting", default=None)
-    finishable: bool | None = pyd.Field(description="Finishable", default=None)
-    air: bool | None = pyd.Field(description="Air Entrainment", default=None)
-    co2: bool | None = pyd.Field(description="CO2 Curing", default=None)
-    white: bool | None = pyd.Field(description="White Cement", default=None)
-    fiber_reinforced: bool | None = pyd.Field(description="Fiber reinforced", default=None)
 
+class ProcessedNonInsulatingGlassPanesV1(BaseOpenEpdHierarchicalSpec, GlazingOptionsMixin):
+    """
+    Solid glass panes without internal gaps which have been heat-treated or otherwise substantially processed.
 
-class ReadyMixV1(BaseOpenEpdHierarchicalSpec):
-    """Concretes to be mixed and then poured on-site."""
+    Includes:
+    1. Coatings including low-e and other coatings (see PCR)
+    2. laminating (fire-rated, glass clad polycarbonate, interlayers
+    3. Heat treated (heat strengthened, tempered, fire-rated)
+    4. Mechanically or chemically processed or fabricated
+    (edging, bending, etching, drilling, notching, cutting, polishing, etc)
+    5. combined products of processing in 1-5.
+    """
 
     _EXT_VERSION = "1.0"
 
 
-class FlowableFillV1(BaseOpenEpdHierarchicalSpec):
+class GlazedDoorsV1(BaseOpenEpdHierarchicalSpec):
     """
-    Flowable fill is a slurry that is placed as a flowable liquid (high slump) and sets with no compaction.
+    Factory assembled door which is at least 50% glass by area.
 
-    It is often used in tight or restricted access areas where placing and compacting
-    fill is difficult. Applications include filling large voids such as abandoned underground storage
-    tanks, basements, tunnels, mines, and sewers. It can also be used as paving sub-base, bridge
-    abutment, and retaining wall backfill. Also called Controlled Density Fill (CDF) or Controlled
-    Low Strength Materials (CLSMs). These materials typically have compressive strengths
-    under 1200 psi.
+    Includes sliding patio doors and hinged doors.
     """
 
     _EXT_VERSION = "1.0"
 
 
-class OilPatchV1(BaseOpenEpdHierarchicalSpec):
+class UnitSkylightsV1(BaseOpenEpdHierarchicalSpec):
     """
-    Concretes for use in petroleum extraction wells and similar applications.
+    Unit skylights performance specification.
 
-    Includes foamed cement; often called cement in the drilling industry. Differs from
-    flowable fill and grout in that it contains no sand or other aggregates.
+    A factory assembled fenestration unit for installation on the roof of a structure to provide interior
+    building spaces with natural daylight, warmth, and ventilation; generally not operable
+    by hand (cf. roof window). Includes frame(s) and possibly operating hardware.
     """
 
     _EXT_VERSION = "1.0"
 
 
-class ConcretePavingV1(BaseOpenEpdHierarchicalSpec):
-    """Concrete paving."""
+class WindowsV1(BaseOpenEpdHierarchicalSpec):
+    """Windows including glazing and frame material."""
 
     _EXT_VERSION = "1.0"
 
 
-class ShotcreteV1(BaseOpenEpdHierarchicalSpec):
-    """Concretes sprayed on a target."""
+class IntegratedDoorsOpeningAssembliesV1(BaseOpenEpdHierarchicalSpec):
+    """Pre-installed unit that includes door, frame, and hardware."""
 
     _EXT_VERSION = "1.0"
 
 
-class CementGroutV1(BaseOpenEpdHierarchicalSpec):
+class MetalDoorAndFramesV1(BaseOpenEpdHierarchicalSpec):
+    """Metal doors and frames."""
+
+    _EXT_VERSION = "1.0"
+
+
+class SpecialtyDoorsAndFramesV1(BaseOpenEpdHierarchicalSpec):
     """
-    Cement grouting is a slurry that is placed as a flowable liquid.
+    Specialty doors and frames.
 
-    It is an effective material for filling and
-    strengthening granular soils, voids in rocks, foundation underpinnings, and other underground voids. Also called
-    structural grout, these materials typically impart significant compressive strength to the system.
+    Includes e.g., access doors and panels, sliding glass doors, coiling doors, special function doors,
+    folding doors, etc.
+    """
+
+    _EXT_VERSION = "1.0"
+
+    # Nested specs:
+    SpecialFunctionDoors: SpecialFunctionDoorsV1 | None = None
+    SlidingGlassDoors: SlidingGlassDoorsV1 | None = None
+
+
+class WoodDoorsV1(BaseOpenEpdHierarchicalSpec):
+    """Wood doors performance specification."""
+
+    _EXT_VERSION = "1.0"
+
+
+class FenestrationPartsV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Fenestration Parts.
 
+    Parts and assemblies for integration into building fenestration such as windows, curtain walls,
+    and storefronts.
     """
 
     _EXT_VERSION = "1.0"
 
+    # Own fields:
+    intended_application: GlazingIntendedApplication | None = pyd.Field(
+        default=None, description="Intended application."
+    )
+
+    # Nested specs:
+    FenestrationAccessories: FenestrationAccessoriesV1 | None = None
+    FenestrationFraming: FenestrationFramingV1 | None = None
+    FenestrationHardware: FenestrationHardwareV1 | None = None
+
 
-class ConcreteV1(BaseOpenEpdHierarchicalSpec):
-    """Concrete spec."""
+class GlassPanesV1(BaseOpenEpdHierarchicalSpec):
+    """Flat glass panes."""
 
     _EXT_VERSION = "1.0"
 
-    strength_28d: PressureMPaStr | None = pyd.Field(
-        default=None, example="30 MPa", description="Concrete strength after 28 days"
+    # Nested specs:
+    FlatGlassPanes: FlatGlassPanesV1 | None = None
+    ProcessedNonInsulatingGlassPanes: ProcessedNonInsulatingGlassPanesV1 | None = None
+
+
+class NAFSPerformanceClass(BaseOpenEpdSchema):
+    """NAFS Performance class."""
+
+    r: bool | None = pyd.Field(
+        default=None, description="Residential; commonly used in one- and two-family dwellings.", example=True
     )
-    strength_early: PressureMPaStr | None = pyd.Field(
+    lc: bool | None = pyd.Field(
         default=None,
-        example="30 MPa",
-        description="A strength spec which is to be reached earlier than 28 days (e.g. 3d)",
+        description="Light Commercial: commonly used in low-rise and mid-rise multi-family dwellings and other "
+        "buildings where larger sizes and higher loading requirements are expected.",
+        example=True,
     )
-    strength_early_d: Literal[3, 7, 14] | None = pyd.Field(default=None, description="Test Day for the Early Strength")
-    strength_late: PressureMPaStr | None = pyd.Field(
+    cw: bool | None = pyd.Field(
         default=None,
-        example="30 MPa",
-        description="A strength spec which is to be reached later than 28 days (e.g. 42d)",
+        description="Commercial Window: commonly used in low-rise and mid-rise buildings where larger sizes, higher "
+        "loading requirements, limits on deflection, and heavy use are expected.",
+        example=True,
     )
-    strength_late_d: Literal[42, 56, 72, 96, 120] | None = pyd.Field(
-        default=None, description="Test Day for the Late Strength"
+    aw: bool | None = pyd.Field(
+        default=None,
+        description="Architectural Window: commonly used in high-rise and mid-rise buildings to meet increased "
+        "loading requirements and limits on deflection, and in buildings where frequent and extreme use "
+        "of the fenestration products is expected.",
+        example=True,
     )
-    slump: LengthMmStr | None = pyd.Field(description="Minimum test slump", example="40 mm", default=None)
-    w_c_ratio: RatioFloat | None = pyd.Field(description="Ratio of water to cement", example=0.3, default=None)
-    aci_exposure_classes: list[AciExposureClass] = pyd.Field(
-        description=(AciExposureClass.__doc__ or "").lstrip(), default_factory=list
+
+
+class NAFSFenestrationV1(BaseOpenEpdHierarchicalSpec, GlazingOptionsMixin):
+    """Factory assembled fenestration units compliant to the North American Fenestration Standard."""
+
+    _EXT_VERSION = "1.0"
+
+    # Own fields:
+    hurricane_resistant: bool | None = pyd.Field(
+        default=None, description="The product has been designed to resist windborne debris.", example=True
     )
-    csa_exposure_classes: list[CsaExposureClass] = pyd.Field(
-        description=(CsaExposureClass.__doc__ or "").lstrip(), default_factory=list
+
+    assembly_u_factor: str | None = pyd.Field(
+        default=None,
+        description="Weighted average conductance of heat across assembly (including frame).",
+        example="1 USI",
     )
-    en_exposure_classes: list[EnExposureClass] = pyd.Field(
-        description=(EnExposureClass.__doc__ or "").lstrip(), default_factory=list
+    air_infiltration: SpeedStr | None = pyd.Field(
+        default=None,
+        description="Air infiltration, measured at a certain level of Differential Pressure.",
+        example="1 m3 / m2 / s",
     )
-    cementitious: Cementitious | None = pyd.Field(
+
+    thermal_separation: ThermalSeparation | None = pyd.Field(default=None, example="Aluminium")
+    dp_rating: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
+    glass_panes: int | None = pyd.Field(
         default=None,
-        description="List of cementitious materials, and proportion by mass. Each field is 0 to 1.",
+        description="Number of panes, each separated by a cavity. A 3 pane unit has 2 cavities. example: 3",
+        example=3,
     )
-    application: TypicalApplication | None = pyd.Field(description="Typical Application", default=None)
-    options: ConcreteV1Options | None = pyd.Field(description="Concrete options", default=None)
 
-    # Nested specs
-    ReadyMix: ReadyMixV1 | None = None
-    FlowableFill: FlowableFillV1 | None = None
-    OilPatch: OilPatchV1 | None = None
-    ConcretePaving: ConcretePavingV1 | None = None
-    Shotcrete: ShotcreteV1 | None = None
-    CementGrout: CementGroutV1 | None = None
+    performance_class: NAFSPerformanceClass | None = pyd.Field(
+        default=None, description="Performance class according to NAFS."
+    )
 
-    _compressive_strength_unit_validator = pyd.validator("strength_28d", allow_reuse=True, check_fields=False)(
-        validate_unit_factory(OpenEPDUnit.MPa)
+    performance_grade: NAFSPerformanceGrade | None = pyd.Field(
+        default=None,
+        description="NAFS Performance Grade. The NAFS Performance Grade is a number that represents the performance "
+        "of the glazing product. The higher the number, the better the performance. The NAFS Performance "
+        "Grade is calculated using the NAFS Performance Class, the NAFS Performance Index, and the NAFS "
+        "Performance Factor. While it is expressed as pressure, there are specific values which are "
+        "allowed. The values are listed in the enum.",
+        example="95 psf",
     )
-    _strength_early_unit_validator = pyd.validator("strength_early", allow_reuse=True)(
-        validate_unit_factory(OpenEPDUnit.MPa)
+
+    _assembly_u_factor_is_quantity_validator = pyd.validator("assembly_u_factor", allow_reuse=True)(
+        validate_unit_factory("USI")
     )
-    _strength_late_unit_validator = pyd.validator("strength_late", allow_reuse=True)(
-        validate_unit_factory(OpenEPDUnit.MPa)
+    _nafs_performance_grade_is_quantity_validator = pyd.validator("performance_grade", allow_reuse=True)(
+        validate_unit_factory("psf")
     )
 
-    @pyd.root_validator
-    def _late_validator(cls, values):
-        together_validator("strength_late", "strength_late_d", values)
-        return values
-
-    @pyd.root_validator
-    def _early_validator(cls, values):
-        together_validator("strength_early", "strength_early_d", values)
-        return values
+    # Nested specs:
+    GlazedDoors: GlazedDoorsV1 | None = None
+    UnitSkylights: UnitSkylightsV1 | None = None
+    Windows: WindowsV1 | None = None
 
 
-class PrecastConcreteV1(BaseOpenEpdHierarchicalSpec):
-    """Precast Concrete spec."""
+class InsulatingGlazingUnitsV1(BaseOpenEpdHierarchicalSpec, GlazingOptionsMixin):
+    """Insulating glazing units performance specification."""
 
     _EXT_VERSION = "1.0"
 
-    strength_28d: PressureMPaStr | None = pyd.Field(
-        default=None, example="30 MPa", description="Concrete strength after 28 days"
+    # Own fields:
+    intended_application: GlazingIntendedApplication | None = pyd.Field(
+        default=None, description="Intended application for IGUs."
     )
 
-    lightweight: bool | None = pyd.Field(description="Lightweight", default=None)
-    steel_mass_percentage: RatioFloat | None = pyd.Field(
+    hurricane_resistant: bool | None = pyd.Field(default=None, example=True)
+
+    dp_rating: PressureMPaStr | None = pyd.Field(
+        default=None, description="Maximum Differential Pressure, a measure of wind tolerance.", example="1 MPa"
+    )
+    air_infiltration: SpeedStr | None = pyd.Field(
+        default=None,
+        description="Air infiltration, measured at a certain level of Differential Pressure.",
+        example="1 m3 / m2 / s",
+    )
+    glass_panes: int | None = pyd.Field(
         default=None,
-        description="Percent of total mass that is steel reinforcement. Steel reinforcement "
-        "substantially changes functional performance and usually adds substantial GWP "
-        "per declared unit.",
+        description="Number of panes, each separated by a cavity. A 3 pane unit has 2 cavities. example: 3",
+        example=3,
+    )
+    cog_u_factor: str | None = pyd.Field(
+        default=None, description="Conductance of heat at center of glass.", example="1 USI"
+    )
+    spacer: Spacer | None = pyd.Field(
+        default=None, description="Spacer material for Integrated Glass Unit.", example="Aluminium"
     )
 
-    insulated: bool | None = pyd.Field(description="Insulated", default=None)
-    gfrc: bool | None = pyd.Field(description="Glass Fiber Reinforced Concrete", default=None)
+    _dp_rating_is_quantity_validator = pyd.validator("dp_rating", allow_reuse=True)(validate_unit_factory("MPa"))
+    _cog_u_factor_is_quantity_validator = pyd.validator("cog_u_factor", allow_reuse=True)(validate_unit_factory("USI"))
 
-    _compressive_strength_unit_validator = pyd.validator("strength_28d", allow_reuse=True)(
-        validate_unit_factory(OpenEPDUnit.MPa)
-    )
+
+class CurtainWallsV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Curtain Walls.
+
+    Exterior skin of building where walls are non-structural and are outboard of the floor slabs,
+    often as system of aluminum framing with vision glass and opaque panels of glass, metal, or other
+    materials.
+
+    Can be 'unitized' (prefabricated off-site) or 'stick' (fabricated on site).
+    """
+
+    _EXT_VERSION = "1.0"
+
+
+class DoorsAndFramesV1(BaseOpenEpdHierarchicalSpec):
+    """Doors (the operable part) and frames (what holds the door proper)."""
+
+    _EXT_VERSION = "1.0"
+
+    # Own fields:
+    height: LengthMmStr | None = pyd.Field(default=None, example="1200 mm")
+    width: LengthMmStr | None = pyd.Field(default=None, example="600 mm")
+
+    # Nested specs:
+    IntegratedDoorsOpeningAssemblies: IntegratedDoorsOpeningAssembliesV1 | None = None
+    MetalDoorAndFrames: MetalDoorAndFramesV1 | None = None
+    SpecialtyDoorsAndFrames: SpecialtyDoorsAndFramesV1 | None = None
+    WoodDoors: WoodDoorsV1 | None = None
+
+
+class EntrancesV1(BaseOpenEpdHierarchicalSpec):
+    """Building entrances (distinct from the door proper)."""
+
+    _EXT_VERSION = "1.0"
+
+
+class GlazingV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Glazing performance specification.
+
+    Broad category of glass-based products, accessories, and assemblies ranging from
+    glass panes and framing to curtain walls.
+    """
+
+    _EXT_VERSION = "1.0"
+
+    # Nested specs:
+    FenestrationParts: FenestrationPartsV1 | None = None
+    GlassPanes: GlassPanesV1 | None = None
+    NAFSFenestration: NAFSFenestrationV1 | None = None
+    InsulatingGlazingUnits: InsulatingGlazingUnitsV1 | None = None
+
+
+class StorefrontsV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Storefronts.
+
+    Fabricated building facades commonly used in retail applications, typically one or two stories
+    tall and using metal framing and glass.
+    """
+
+    _EXT_VERSION = "1.0"
+
+
+class TranslucentWallAndRoofAssembliesV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Translucent wall and roof assemblies.
+
+    Includes structured polycarbonate panel and fiberglass sandwich panel assemblies.
+    """
+
+    _EXT_VERSION = "1.0"
+
+
+class WindowWallAssembliesV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Window Wall Assemblies.
+
+    Exterior skin of building where walls are non-structural and sit between floor slabs, often as
+    system of aluminum framing with vision glass and opaque panels of glass, metal,
+    or other materials.
+    """
+
+    _EXT_VERSION = "1.0"
+
+
+class OpeningsV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Openings performance specification.
+
+    General category that includes windows, storefronts, window walls, curtain walls,
+    doors, entrances, etc.
+    """
+
+    _EXT_VERSION = "1.0"
+
+    # Own fields:
+    thickness: LengthMmStr | None = pyd.Field(default=None, example="80 mm")
+
+    # Nested specs:
+    CurtainWalls: CurtainWallsV1 | None = None
+    DoorsAndFrames: DoorsAndFramesV1 | None = None
+    Entrances: EntrancesV1 | None = None
+    Glazing: GlazingV1 | None = None
+    Storefronts: StorefrontsV1 | None = None
+    TranslucentWallAndRoofAssemblies: TranslucentWallAndRoofAssembliesV1 | None = None
+    WindowWallAssemblies: WindowWallAssembliesV1 | None = None
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/accessories.py` & `openepd-3.1.3/src/openepd/model/specs/generated/accessories.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/aggregates.py` & `openepd-3.1.3/src/openepd/model/specs/generated/aggregates.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/aluminium.py` & `openepd-3.1.3/src/openepd/model/specs/generated/aluminium.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/asphalt.py` & `openepd-3.1.3/src/openepd/model/specs/generated/asphalt.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import AsphaltGradation, AsphaltMixType
 from openepd.model.validation.numbers import RatioFloat
-from openepd.model.validation.quantity import LengthMmStr, TemperatureCStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr, TemperatureCStr
 
 
 class AsphaltV1(BaseOpenEpdHierarchicalSpec):
     """Asphalt performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -70,17 +70,7 @@
     gradation: AsphaltGradation | None = pyd.Field(default=None, description="Asphalt gradation", example="Gap-graded")
 
     sbr: bool | None = pyd.Field(default=None, description="Styrene-butadiene rubber (SBR)", example=True)
     sbs: bool | None = pyd.Field(default=None, description="Styrene-butadiene-styrene (SBS)", example=True)
     ppa: bool | None = pyd.Field(default=None, description="Polyphosphoric acid (PPA)", example=True)
     gtr: bool | None = pyd.Field(default=None, description="Ground tire rubber (GTR)", example=True)
     pmb: bool | None = pyd.Field(default=None, description="Polymer modified bitumen (PMB)", example=True)
-
-    _asphalt_aggregate_size_max_is_quantity_validator = pyd.validator("aggregate_size_max", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-    _asphalt_max_temperature_is_quantity_validator = pyd.validator("max_temperature", allow_reuse=True)(
-        validate_unit_factory("°C")
-    )
-    _asphalt_min_temperature_is_quantity_validator = pyd.validator("min_temperature", allow_reuse=True)(
-        validate_unit_factory("°C")
-    )
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/bulk_materials.py` & `openepd-3.1.3/src/openepd/model/specs/generated/bulk_materials.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/cast_decks_and_underlayment.py` & `openepd-3.1.3/src/openepd/model/specs/generated/cast_decks_and_underlayment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/cladding.py` & `openepd-3.1.3/src/openepd/model/specs/generated/cladding.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import CladdingFacingMaterial, CladdingInsulatingMaterial, SidingFormFactor
-from openepd.model.validation.quantity import LengthMmStr, LengthMStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr, LengthMStr, RValueStr, validate_unit_factory
 
 
 class AluminiumSidingV1(BaseOpenEpdHierarchicalSpec):
     """Aluminium siding performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -122,21 +122,17 @@
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     insulated: bool | None = pyd.Field(default=None, description="", example=True)
     ventilated: bool | None = pyd.Field(default=None, description="", example=True)
     paint_or_stain_required: bool | None = pyd.Field(default=None, description="", example=True)
-    r_value: str | None = pyd.Field(default=None, description="", example="1 K * m2 / W")
+    r_value: RValueStr | None = pyd.Field(default=None, description="")
     form_factor: SidingFormFactor | None = pyd.Field(default=None, description="", example="Lap")
 
-    _siding_r_value_is_quantity_validator = pyd.validator("r_value", allow_reuse=True)(
-        validate_unit_factory("K * m2 / W")
-    )
-
     # Nested specs:
     MetalSiding: MetalSidingV1 | None = None
     CompositionSiding: CompositionSidingV1 | None = None
     FiberCementSiding: FiberCementSidingV1 | None = None
     InsulatedVinylSiding: InsulatedVinylSidingV1 | None = None
     PlywoodSiding: PlywoodSidingV1 | None = None
     PolypropyleneSiding: PolypropyleneSidingV1 | None = None
@@ -146,39 +142,31 @@
 
 class InsulatedRoofPanelsV1(BaseOpenEpdHierarchicalSpec):
     """Insulated roof panels performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    r_value: str | None = pyd.Field(default=None, description="", example="1 K * m2 / W")
+    r_value: RValueStr | None = pyd.Field(default=None, description="")
     insulating_material: CladdingInsulatingMaterial | None = pyd.Field(
         default=None, description="", example="No Insulation"
     )
 
-    _cladding_r_value_is_quantity_validator = pyd.validator("r_value", allow_reuse=True)(
-        validate_unit_factory("K * m2 / W")
-    )
-
 
 class InsulatedWallPanelsV1(BaseOpenEpdHierarchicalSpec):
     """Insulated wall panels performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    r_value: str | None = pyd.Field(default=None, description="", example="1 K * m2 / W")
+    r_value: RValueStr | None = pyd.Field(default=None, description="")
     insulating_material: CladdingInsulatingMaterial | None = pyd.Field(
         default=None, description="", example="No Insulation"
     )
 
-    _cladding_r_value_is_quantity_validator = pyd.validator("r_value", allow_reuse=True)(
-        validate_unit_factory("K * m2 / W")
-    )
-
 
 class RoofPanelsV1(BaseOpenEpdHierarchicalSpec):
     """Roof panels performance specification."""
 
     _EXT_VERSION = "1.0"
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/cmu.py` & `openepd-3.1.3/src/openepd/model/specs/generated/cmu.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import CmuBlockType, CmuWeightClassification
-from openepd.model.validation.quantity import GwpKgCo2eStr, PressureMPaStr, validate_unit_factory
+from openepd.model.validation.quantity import GwpKgCo2eStr, PressureMPaStr
 
 
 class CMUV1(BaseOpenEpdHierarchicalSpec):
     """CMU performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -33,14 +33,7 @@
     strength_28d: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
     weight_classification: CmuWeightClassification | None = pyd.Field(default=None, description="", example="Normal")
     block_type: CmuBlockType | None = pyd.Field(default=None, description="", example="Gray")
     insulated: bool | None = pyd.Field(default=None, description="", example=True)
     sound_performance: bool | None = pyd.Field(default=None, description="", example=True)
     b1_recarbonation: GwpKgCo2eStr | None = pyd.Field(default=None, description="", example="1 kgCO2e")
     b1_recarbonation_z: float | None = pyd.Field(default=None, description="", example=2.3)
-
-    _concrete_compressive_strength_28d_is_quantity_validator = pyd.validator("strength_28d", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
-    _b1_recarbonation_is_quantity_validator = pyd.validator("b1_recarbonation", allow_reuse=True)(
-        validate_unit_factory("kgCO2e")
-    )
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/common.py` & `openepd-3.1.3/src/openepd/model/specs/generated/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/concrete.py` & `openepd-3.1.3/src/openepd/model/specs/generated/concrete.py`

 * *Files 17% similar despite different names*

```diff
@@ -164,33 +164,14 @@
         default=None, description="List of CSA exposure classes", example=["csa.C-2"]
     )
     en_exposure_classes: list[EnExposureClass] | None = pyd.Field(
         default=None, description="List of EN exposure classes", example=["en206.X0"]
     )
     typical_application: ConcreteTypicalApplication | None = pyd.Field(default=None, description="Typical Application")
 
-    _concrete_compressive_strength_28d_is_quantity_validator = pyd.validator("strength_28d", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
-    _concrete_compressive_strength_other_is_quantity_validator = pyd.validator("strength_other", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
-    _concrete_slump_is_quantity_validator = pyd.validator("slump", allow_reuse=True)(validate_unit_factory("m"))
-    _concrete_min_slump_is_quantity_validator = pyd.validator("min_slump", allow_reuse=True)(validate_unit_factory("m"))
-    _concrete_max_slump_is_quantity_validator = pyd.validator("max_slump", allow_reuse=True)(validate_unit_factory("m"))
-    _concrete_min_pipeline_size_is_quantity_validator = pyd.validator("min_pipeline_size", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-    _concrete_aggregate_size_max_is_quantity_validator = pyd.validator("aggregate_size_max", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-    _concrete_cement_content_is_quantity_validator = pyd.validator("cement_content", allow_reuse=True)(
-        validate_unit_factory("kg")
-    )
-
     # Nested specs:
     CementGrout: CementGroutV1 | None = None
     ConcretePaving: ConcretePavingV1 | None = None
     FlowableFill: FlowableFillV1 | None = None
     OilPatch: OilPatchV1 | None = None
     ReadyMix: ReadyMixV1 | None = None
     Shotcrete: ShotcreteV1 | None = None
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/conveying_equipment.py` & `openepd-3.1.3/src/openepd/model/specs/generated/conveying_equipment.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,41 +16,31 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import ElevatorsBuildingRise, ElevatorsUsageIntensity
-from openepd.model.validation.quantity import LengthMStr, MassKgStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMStr, MassKgStr, SpeedStr
 
 
 class ElevatorsV1(BaseOpenEpdHierarchicalSpec):
     """Elevators performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     usage_intensity: list[ElevatorsUsageIntensity] | None = pyd.Field(
         default=None, description="", example=["Very low"]
     )
     travel_length: LengthMStr | None = pyd.Field(default=None, description="", example="1 m")
     rated_load: MassKgStr | None = pyd.Field(default=None, description="", example="1 kg")
-    rated_speed: str | None = pyd.Field(default=None, description="", example="1 m / s")
+    rated_speed: SpeedStr | None = pyd.Field(default=None, description="", example="1 m / s")
     building_rise: ElevatorsBuildingRise | None = pyd.Field(default=None, description="", example="Low-rise")
 
-    _elevators_travel_length_is_quantity_validator = pyd.validator("travel_length", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-    _elevators_rated_load_is_quantity_validator = pyd.validator("rated_load", allow_reuse=True)(
-        validate_unit_factory("kg")
-    )
-    _elevators_rated_speed_is_quantity_validator = pyd.validator("rated_speed", allow_reuse=True)(
-        validate_unit_factory("m / s")
-    )
-
 
 class ConveyingEquipmentV1(BaseOpenEpdHierarchicalSpec):
     """Conveying equipment performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/electrical.py` & `openepd-3.1.3/src/openepd/model/specs/generated/electrical.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import CableTraysMaterial, EnergySource, RacewaysMaterial
 from openepd.model.validation.quantity import (
+    ColorTemperatureStr,
     LengthMmStr,
     LengthMStr,
+    LuminosityStr,
     MassKgStr,
-    TemperatureCStr,
+    PowerStr,
     validate_quantity_ge_factory,
     validate_quantity_le_factory,
     validate_unit_factory,
 )
 
 
 class LowVoltBusesV1(BaseOpenEpdHierarchicalSpec):
@@ -66,19 +68,14 @@
     depth: LengthMmStr | None = pyd.Field(default=None, description="", example="100 mm")
     static_load: MassKgStr | None = pyd.Field(default=None, description="", example="1 kg")
     ventilated: bool | None = pyd.Field(
         default=None, description="At least 40% of the tray base is open to air flow", example=True
     )
     cable_trays_material: CableTraysMaterial | None = pyd.Field(default=None, description="", example="Stainless Steel")
 
-    _height_is_quantity_validator = pyd.validator("height", allow_reuse=True)(validate_unit_factory("m"))
-    _width_is_quantity_validator = pyd.validator("width", allow_reuse=True)(validate_unit_factory("m"))
-    _depth_is_quantity_validator = pyd.validator("depth", allow_reuse=True)(validate_unit_factory("m"))
-    _static_load_is_quantity_validator = pyd.validator("static_load", allow_reuse=True)(validate_unit_factory("kg"))
-
 
 class ElectricalBusesV1(BaseOpenEpdHierarchicalSpec):
     """Electrical buses performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
@@ -106,17 +103,14 @@
     # Own fields:
     width: LengthMStr | None = pyd.Field(default=None, description="", example="100 mm")
     depth: LengthMStr | None = pyd.Field(default=None, description="", example="100 mm")
     painted: bool | None = pyd.Field(default=None, description="", example=True)
     divided: bool | None = pyd.Field(default=None, description="", example=True)
     raceways_material: RacewaysMaterial | None = pyd.Field(default=None, description="", example="Aluminum")
 
-    _width_is_quantity_validator = pyd.validator("width", allow_reuse=True)(validate_unit_factory("m"))
-    _depth_is_quantity_validator = pyd.validator("depth", allow_reuse=True)(validate_unit_factory("m"))
-
 
 class FueledElectricalGeneratorsV1(BaseOpenEpdHierarchicalSpec):
     """Fueled electrical generators performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
@@ -246,27 +240,30 @@
 
 class LightingV1(BaseOpenEpdHierarchicalSpec):
     """Lighting performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    color_temperature: TemperatureCStr | None = pyd.Field(default=None, description="", example="1 K")
+    color_temperature: ColorTemperatureStr | None = pyd.Field(default=None, description="", example="1 K")
     typical_utilization: str | None = pyd.Field(default=None, description="", example="1 h / yr")
-    luminosity: str | None = pyd.Field(default=None, description="", example="1 lumen")
-    wattage: str | None = pyd.Field(default=None, description="", example="1000.0 W")
+    luminosity: LuminosityStr | None = pyd.Field(default=None, description="", example="1 lumen")
+    wattage: PowerStr | None = pyd.Field(default=None, description="")
     color_rendering_index: float | None = pyd.Field(default=None, description="", example=2.3)
     dimmable: bool | None = pyd.Field(default=None, description="", example=True)
 
     _color_temperature_quantity_ge_validator = pyd.validator("color_temperature", allow_reuse=True)(
         validate_quantity_ge_factory("1E+03 K")
     )
     _color_temperature_quantity_le_validator = pyd.validator("color_temperature", allow_reuse=True)(
         validate_quantity_le_factory("1E+04 K")
     )
+    _typical_utilization_unit_validator = pyd.validator("typical_utilization", allow_reuse=True)(
+        validate_unit_factory("h / yr")
+    )
     _typical_utilization_quantity_ge_validator = pyd.validator("typical_utilization", allow_reuse=True)(
         validate_quantity_ge_factory("25 h / yr")
     )
     _luminosity_quantity_ge_validator = pyd.validator("luminosity", allow_reuse=True)(
         validate_quantity_ge_factory("450 lumen")
     )
     _luminosity_quantity_le_validator = pyd.validator("luminosity", allow_reuse=True)(
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py` & `openepd-3.1.3/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/electricity.py` & `openepd-3.1.3/src/openepd/model/specs/generated/electricity.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/enums.py` & `openepd-3.1.3/src/openepd/model/specs/generated/enums.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/finishes.py` & `openepd-3.1.3/src/openepd/model/specs/generated/finishes.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,26 +77,14 @@
     finished_floor_height: LengthMmStr | None = pyd.Field(default=None, description="", example="1 m")
     panel_thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="1 m")
     concentrated_load: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
     uniform_load: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
     rolling_load_10_pass: str | None = pyd.Field(default=None, description="", example="1 N")
     rolling_load_10000_pass: str | None = pyd.Field(default=None, description="", example="1 N")
 
-    _access_flooring_finished_floor_height_is_quantity_validator = pyd.validator(
-        "finished_floor_height", allow_reuse=True
-    )(validate_unit_factory("m"))
-    _access_flooring_panel_thickness_is_quantity_validator = pyd.validator("panel_thickness", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-    _access_flooring_concentrated_load_is_quantity_validator = pyd.validator("concentrated_load", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
-    _access_flooring_uniform_load_is_quantity_validator = pyd.validator("uniform_load", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
     _access_flooring_rolling_load_10_pass_is_quantity_validator = pyd.validator(
         "rolling_load_10_pass", allow_reuse=True
     )(validate_unit_factory("N"))
     _access_flooring_rolling_load_10000_pass_is_quantity_validator = pyd.validator(
         "rolling_load_10000_pass", allow_reuse=True
     )(validate_unit_factory("N"))
 
@@ -120,23 +108,16 @@
     fire_smoke_density_rating_astme648: str | None = pyd.Field(default=None, description="")
     voc_emissions: str | None = pyd.Field(default=None, description="", example="test_valueValidatedStringProperty")
     cushioned: bool | None = pyd.Field(default=None, description="", example=True)
     bleachable: bool | None = pyd.Field(default=None, description="", example=True)
     gwp_factor_base: GwpKgCo2eStr | None = pyd.Field(default=None, description="", example="1 kgCO2e")
     gwp_factor_yarn: GwpKgCo2eStr | None = pyd.Field(default=None, description="", example="1 kgCO2e")
 
-    _length_is_quantity_validator = pyd.validator("length", allow_reuse=True)(validate_unit_factory("m"))
-    _width_is_quantity_validator = pyd.validator("width", allow_reuse=True)(validate_unit_factory("m"))
     _yarn_weight_is_quantity_validator = pyd.validator("yarn_weight", allow_reuse=True)(validate_unit_factory("g / m2"))
-    _gwp_factor_base_is_quantity_validator = pyd.validator("gwp_factor_base", allow_reuse=True)(
-        validate_unit_factory("kgCO2e")
-    )
-    _gwp_factor_yarn_is_quantity_validator = pyd.validator("gwp_factor_yarn", allow_reuse=True)(
-        validate_unit_factory("kgCO2e")
-    )
+    _yarn_weight_ge_validator = pyd.validator("yarn_weight", allow_reuse=True)(validate_quantity_ge_factory("0 g / m2"))
 
 
 class LaminateV1(BaseOpenEpdHierarchicalSpec):
     """Laminate performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -163,20 +144,14 @@
     thickness: ResilientFlooringThickness | None = pyd.Field(default=None, description="", example="≤ 2mm")
     sport_flooring: bool | None = pyd.Field(default=None, description="", example=True)
     conductive_flooring: bool | None = pyd.Field(default=None, description="", example=True)
     zwtl: bool | None = pyd.Field(default=None, description="", example=True)
     floor_score: bool | None = pyd.Field(default=None, description="", example=True)
     nsf332: bool | None = pyd.Field(default=None, description="", example=True)
 
-    _length_is_quantity_validator = pyd.validator("length", allow_reuse=True)(validate_unit_factory("m"))
-    _width_is_quantity_validator = pyd.validator("width", allow_reuse=True)(validate_unit_factory("m"))
-    _resilient_flooring_wear_layer_is_quantity_validator = pyd.validator("wear_layer", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-
 
 class WallBaseV1(BaseOpenEpdHierarchicalSpec):
     """Wall base performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
@@ -190,27 +165,23 @@
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
     timber_species: WoodFlooringTimberSpecies | None = pyd.Field(default=None, description="", example="Oak")
     fabrication: WoodFlooringFabrication | None = pyd.Field(default=None, description="", example="Solid hardwood")
     forest_practices_certifiers: list[OrgRef] | None = pyd.Field(default=None, description="")
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-
 
 class AcousticalCeilingsV1(BaseOpenEpdHierarchicalSpec):
     """Acoustical ceilings performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-
 
 class CeramicTileV1(BaseOpenEpdHierarchicalSpec):
     """Ceramic tile performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
@@ -369,15 +340,15 @@
 
 class TilingV1(BaseOpenEpdHierarchicalSpec):
     """Tiling performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    thickness: LengthMStr | None = pyd.Field(default=None, description="", example="1 m")
+    thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="9 mm")
     flooring: bool | None = pyd.Field(default=None, description="Tiling intended for walking.", example=True)
     wall_finish: bool | None = pyd.Field(
         default=None,
         description="A decorative tile designed for use on vertical surfaces such as walls or backsplashes.",
         example=True,
     )
     cladding: bool | None = pyd.Field(
@@ -414,16 +385,14 @@
         default=None,
         description="Proportion of this product that is sourced from post-consumer recycled content, by mass.",
         example=0.5,
         ge=0,
         le=1,
     )
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-    _thickness_min_validator = pyd.validator("thickness", allow_reuse=True)(validate_quantity_ge_factory("0 mm"))
     _thickness_max_validator = pyd.validator("thickness", allow_reuse=True)(validate_quantity_le_factory("50 mm"))
 
     # Nested specs:
     CeramicTile: CeramicTileV1 | None = None
     GaugedTile: GaugedTileV1 | None = None
     GlassTile: GlassTileV1 | None = None
 
@@ -466,15 +435,14 @@
     soft_body_impact_e695: int | None = pyd.Field(default=None, description="", example=3)
     hard_body_impact_c1929: int | None = pyd.Field(default=None, description="", example=3)
     mold_resistant: bool | None = pyd.Field(default=None, description="", example=True)
     foil_backing: bool | None = pyd.Field(default=None, description="", example=True)
     moisture_resistant: bool | None = pyd.Field(default=None, description="", example=True)
     abuse_resistant: bool | None = pyd.Field(default=None, description="", example=True)
 
-    _gypsum_thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
     _gypsum_r_factor_is_quantity_validator = pyd.validator("r_factor", allow_reuse=True)(validate_unit_factory("RSI"))
 
     # Nested specs:
     GypsumSupports: GypsumSupportsV1 | None = None
 
 
 class MirrorsV1(BaseOpenEpdHierarchicalSpec):
@@ -493,16 +461,14 @@
     """Wall finishes performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-
 
 class FinishesV1(BaseOpenEpdHierarchicalSpec):
     """Finishes performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/fire_and_smoke_protection.py` & `openepd-3.1.3/src/openepd/model/specs/generated/fire_and_smoke_protection.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import (
     IntumescentFireproofingMaterialType,
     SprayFireproofingDensity,
     SprayFireproofingMaterialType,
 )
-from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr
 
 
 class IntumescentFireproofingV1(BaseOpenEpdHierarchicalSpec):
     """Intumescent fireproofing performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -52,16 +52,14 @@
     """Applied fireproofing performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-
     # Nested specs:
     IntumescentFireproofing: IntumescentFireproofingV1 | None = None
     SprayFireproofing: SprayFireproofingV1 | None = None
 
 
 class FirestoppingV1(BaseOpenEpdHierarchicalSpec):
     """Firestopping performance specification."""
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/furnishings.py` & `openepd-3.1.3/src/openepd/model/specs/generated/furnishings.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import CountertopMaterial
-from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr
 
 
 class DemountablePartitionTrackV1(BaseOpenEpdHierarchicalSpec):
     """Demountable partition track performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -40,16 +40,14 @@
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="30 mm")
     countertop_material: CountertopMaterial | None = pyd.Field(default=None, description="", example="Stone")
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-
 
 class DemountablePartitionsV1(BaseOpenEpdHierarchicalSpec):
     """Demountable partitions performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/grouting.py` & `openepd-3.1.3/src/openepd/model/specs/generated/grouting.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/manufacturing_inputs.py` & `openepd-3.1.3/src/openepd/model/specs/generated/manufacturing_inputs.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/masonry.py` & `openepd-3.1.3/src/openepd/model/specs/generated/masonry.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
-from openepd.model.validation.quantity import PressureMPaStr, validate_unit_factory
+from openepd.model.validation.quantity import PressureMPaStr, validate_quantity_ge_factory, validate_unit_factory
 
 
 class GMUV1(BaseOpenEpdHierarchicalSpec):
     """Glass Masonry Unit performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -34,21 +34,22 @@
     _EXT_VERSION = "1.0"
 
     # Own fields:
     strength_28d: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
     thermal_conductivity: str | None = pyd.Field(default=None, description="", example="1 W / (m * K)")
     white: bool | None = pyd.Field(default=None, description="", example=True)
 
-    _concrete_compressive_strength_28d_is_quantity_validator = pyd.validator("strength_28d", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
     _aac_thermal_conductivity_is_quantity_validator = pyd.validator("thermal_conductivity", allow_reuse=True)(
         validate_unit_factory("W / (m * K)")
     )
 
+    _aac_thermal_conductivity_min_validator = pyd.validator("thermal_conductivity", allow_reuse=True)(
+        validate_quantity_ge_factory("0 W / (m * K)")
+    )
+
 
 class BrickV1(BaseOpenEpdHierarchicalSpec):
     """Brick performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/material_handling.py` & `openepd-3.1.3/src/openepd/model/specs/generated/material_handling.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/mechanical_insulation.py` & `openepd-3.1.3/src/openepd/model/specs/generated/mechanical_insulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,22 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import InsulatingMaterial, InsulationIntendedApplication
-from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr
 
 
 class MechanicalInsulationV1(BaseOpenEpdHierarchicalSpec):
     """Mechanical insulation performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     r_value: float | None = pyd.Field(default=None, description="", example=2.3)
     material: InsulatingMaterial | None = pyd.Field(default=None, description="", example="Mineral Wool")
     intended_application: list[InsulationIntendedApplication] | None = pyd.Field(
         default=None, description="", example=["Wall & General"]
     )
     thickness_per_declared_unit: LengthMmStr | None = pyd.Field(default=None, description="", example="20 mm")
-
-    _thickness_per_declared_unit_is_quantity_validator = pyd.validator("thickness_per_declared_unit", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/network_infrastructure.py` & `openepd-3.1.3/src/openepd/model/specs/generated/network_infrastructure.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     FloorBoxCoverMaterial,
     FloorBoxFloorMaterial,
     FloorBoxMaterial,
     PduTechnology,
     RacewaysMaterial,
     RackType,
 )
-from openepd.model.validation.quantity import LengthMmStr, MassKgStr, validate_unit_factory
+from openepd.model.validation.quantity import ElectricalCurrentStr, LengthMmStr, MassKgStr, validate_unit_factory
 
 
 class PDUV1(BaseOpenEpdHierarchicalSpec):
     """P d u performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    amperage: str | None = pyd.Field(default=None, description="", example="1 A")
+    amperage: ElectricalCurrentStr | None = pyd.Field(default=None, description="", example="1 A")
     outlet_level_metering: bool | None = pyd.Field(default=None, description="", example=True)
     outlet_level_switching: bool | None = pyd.Field(default=None, description="", example=True)
     pdu_technology: PduTechnology | None = pyd.Field(default=None, description="", example="Basic")
     pdu_outlets: int | None = pyd.Field(default=None, description="", example=3, le=200)
 
     _amperage_is_quantity_validator = pyd.validator("amperage", allow_reuse=True)(validate_unit_factory("A"))
 
@@ -55,16 +55,14 @@
     _EXT_VERSION = "1.0"
 
     # Own fields:
     static_load: MassKgStr | None = pyd.Field(default=None, description="", example="1 kg")
     total_racking_units: int | None = pyd.Field(default=None, description="", example=3)
     rack_type: RackType | None = pyd.Field(default=None, description="", example="Cabinet")
 
-    _static_load_is_quantity_validator = pyd.validator("static_load", allow_reuse=True)(validate_unit_factory("kg"))
-
 
 class DataCablingV1(BaseOpenEpdHierarchicalSpec):
     """Data cabling performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
@@ -137,19 +135,14 @@
     depth: LengthMmStr | None = pyd.Field(default=None, description="Depth of enclosure system", example="1 m")
     static_load: MassKgStr | None = pyd.Field(default=None, description="Mass that the unit can hold", example="1 kg")
     ventilated: bool | None = pyd.Field(
         default=None, description="At least 40% of the tray base is open to air flow", example=True
     )
     material: CableTraysMaterial | None = pyd.Field(default=None, description="", example="Stainless Steel")
 
-    _height_is_quantity_validator = pyd.validator("height", allow_reuse=True)(validate_unit_factory("m"))
-    _width_is_quantity_validator = pyd.validator("width", allow_reuse=True)(validate_unit_factory("m"))
-    _depth_is_quantity_validator = pyd.validator("depth", allow_reuse=True)(validate_unit_factory("m"))
-    _static_load_is_quantity_validator = pyd.validator("static_load", allow_reuse=True)(validate_unit_factory("kg"))
-
 
 class NetworkingRacewaysV1(BaseOpenEpdHierarchicalSpec):
     """Networking raceways performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
@@ -159,17 +152,14 @@
     divided: bool | None = pyd.Field(
         default=None,
         description="Dual service raceway for high and low voltage data and power applications",
         example=True,
     )
     raceways_material: RacewaysMaterial | None = pyd.Field(default=None, description="", example="Aluminum")
 
-    _width_is_quantity_validator = pyd.validator("width", allow_reuse=True)(validate_unit_factory("m"))
-    _depth_is_quantity_validator = pyd.validator("depth", allow_reuse=True)(validate_unit_factory("m"))
-
 
 class NetworkInfrastructureV1(BaseOpenEpdHierarchicalSpec):
     """Network infrastructure performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/other_electrical_equipment.py` & `openepd-3.1.3/src/openepd/model/specs/generated/other_electrical_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/other_materials.py` & `openepd-3.1.3/src/openepd/model/specs/generated/other_materials.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/plumbing.py` & `openepd-3.1.3/src/openepd/model/specs/generated/plumbing.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import FireProtectionPipingMaterial, PipingAnsiSchedule, PlumbingPipingMaterial
-from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr, MassPerLengthStr
 
 
 class BathtubsV1(BaseOpenEpdHierarchicalSpec):
     """Bathtubs performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -51,28 +51,20 @@
     """Fire protection piping performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="6 mm")
     piping_diameter: LengthMmStr | None = pyd.Field(default=None, description="", example="120 mm")
-    mass_per_unit_length: str | None = pyd.Field(default=None, description="", example="1 kg / m")
+    mass_per_unit_length: MassPerLengthStr | None = pyd.Field(default=None, description="", example="1 kg / m")
     piping_ansi_schedule: PipingAnsiSchedule | None = pyd.Field(default=None, description="", example="5")
     fire_protection_piping_material: FireProtectionPipingMaterial | None = pyd.Field(
         default=None, description="", example="PVC"
     )
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-    _piping_diameter_is_quantity_validator = pyd.validator("piping_diameter", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-    _mass_per_unit_length_is_quantity_validator = pyd.validator("mass_per_unit_length", allow_reuse=True)(
-        validate_unit_factory("kg / m")
-    )
-
 
 class FireSprinklersV1(BaseOpenEpdHierarchicalSpec):
     """Fire sprinklers performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
@@ -114,26 +106,18 @@
     """Piping performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="6 mm")
     piping_diameter: LengthMmStr | None = pyd.Field(default=None, description="", example="120 mm")
-    mass_per_unit_length: str | None = pyd.Field(default=None, description="", example="1 kg / m")
+    mass_per_unit_length: MassPerLengthStr | None = pyd.Field(default=None, description="", example="1 kg / m")
     piping_ansi_schedule: PipingAnsiSchedule | None = pyd.Field(default=None, description="", example="5")
     plumbing_piping_material: PlumbingPipingMaterial | None = pyd.Field(default=None, description="", example="PVC")
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-    _piping_diameter_is_quantity_validator = pyd.validator("piping_diameter", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-    _mass_per_unit_length_is_quantity_validator = pyd.validator("mass_per_unit_length", allow_reuse=True)(
-        validate_unit_factory("kg / m")
-    )
-
 
 class PlumbingEquipmentV1(BaseOpenEpdHierarchicalSpec):
     """Plumbing equipment performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/precast_concrete.py` & `openepd-3.1.3/src/openepd/model/specs/generated/precast_concrete.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.validation.numbers import RatioFloat
-from openepd.model.validation.quantity import PressureMPaStr, validate_unit_factory
+from openepd.model.validation.quantity import PressureMPaStr
 
 
 class ArchitecturalPrecastV1(BaseOpenEpdHierarchicalSpec):
     """Architectural precast performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -54,15 +54,11 @@
         default=None,
         description="Glass Fiber Reinforced Concrete is fiber-reinforced concrete sometimes used in "
         "architectural panels",
         example=True,
     )
     steel_mass_percentage: RatioFloat | None = pyd.Field(default=None, description="", example=0.5, ge=0, le=1)
 
-    _concrete_compressive_strength_28d_is_quantity_validator = pyd.validator(
-        "concrete_compressive_strength_28d", allow_reuse=True
-    )(validate_unit_factory("MPa"))
-
     # Nested specs:
     ArchitecturalPrecast: ArchitecturalPrecastV1 | None = None
     StructuralPrecast: StructuralPrecastV1 | None = None
     UtilityUndergroundPrecast: UtilityUndergroundPrecastV1 | None = None
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/sheathing.py` & `openepd-3.1.3/src/openepd/model/specs/generated/sheathing.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/steel.py` & `openepd-3.1.3/src/openepd/model/specs/generated/steel.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,30 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
+from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec, BaseOpenEpdSpec
 from openepd.model.specs.generated.enums import SteelComposition, SteelRebarGrade
-from openepd.model.specs.steel import SteelMakingRoute
 from openepd.model.standard import Standard
 from openepd.model.validation.numbers import RatioFloat
 from openepd.model.validation.quantity import LengthMmStr, PressureMPaStr, validate_unit_factory
 
 
+class SteelMakingRoute(BaseOpenEpdSchema):
+    """Steel making route."""
+
+    bof: bool | None = pyd.Field(default=None, description="Basic oxygen furnace")
+    eaf: bool | None = pyd.Field(default=None, description="Electric arc furnace")
+    ohf: bool | None = pyd.Field(default=None, description="Open hearth furnace")
+
+
 class SteelFabricatedMixin(BaseOpenEpdSpec):
     """Class with fabricated property used in different parts of steel hierarchy."""
 
     fabricated: bool | None = pyd.Field(default=None, description="", example=True)
 
 
 class ColdFormedFramingV1(BaseOpenEpdHierarchicalSpec):
@@ -176,17 +184,14 @@
     )
     thermal_conductivity: str | None = pyd.Field(
         default=None,
         description="Thermal Conductivity, https://en.wikipedia.org/wiki/Thermal_conductivity_and_resistivity",
         example="1.45E-5 W / (m * K)",
     )
 
-    _steel_modulus_of_elasticity_is_quantity_validator = pyd.validator("modulus_of_elasticity", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
     _steel_thermal_expansion_is_quantity_validator = pyd.validator("thermal_expansion", allow_reuse=True)(
         validate_unit_factory("1 / K")
     )
     _steel_thermal_conductivity_is_quantity_validator = pyd.validator("thermal_conductivity", allow_reuse=True)(
         validate_unit_factory("W / (m * K)")
     )
 
@@ -224,18 +229,14 @@
     diameter_min: LengthMmStr | None = pyd.Field(default=None, description="Minimal diameter", example="8 mm")
     bending_pin_max: float | None = pyd.Field(default=None, example=2.3)
     ts_ys_ratio_max: float | None = pyd.Field(
         default=None, description="Max ratio of ultimate tensile to yield tensile strength", example=2.3
     )
     epoxy_coated: bool | None = pyd.Field(default=None, example=True)
 
-    _steel_rebar_diameter_min_is_quantity_validator = pyd.validator("diameter_min", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-
 
 class WireMeshSteelV1(BaseOpenEpdHierarchicalSpec, SteelFabricatedMixin):
     """Mild steel wire for reinforcement, connections, and meshes."""
 
     _EXT_VERSION = "1.0"
 
 
@@ -272,18 +273,14 @@
     galvanized: bool | None = pyd.Field(default=None, example=True)
     stainless: bool | None = pyd.Field(default=None, example=True)
     making_route: SteelMakingRoute | None = pyd.Field(default=None)
     astm_standards: list[Standard] | None = pyd.Field(default=None, description="List of ASTM standards")
     sae_standards: list[Standard] | None = pyd.Field(default=None, description="List of SAE standards")
     en_standards: list[Standard] | None = pyd.Field(default=None, description="List of EN standards")
 
-    _steel_yield_tensile_str_is_quantity_validator = pyd.validator("yield_tensile_str", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
-
     # Nested specs:
     MBQSteel: MBQSteelV1 | None = None
     CoilSteel: CoilSteelV1 | None = None
     ColdFormedSteel: ColdFormedSteelV1 | None = None
     StructuralSteel: StructuralSteelV1 | None = None
     PrefabricatedSteelAssemblies: PrefabricatedSteelAssembliesV1 | None = None
     PostTensioningSteel: PostTensioningSteelV1 | None = None
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/thermal_moisture_protection.py` & `openepd-3.1.3/src/openepd/model/specs/generated/thermal_moisture_protection.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     InsulatingMaterial,
     InsulationIntendedApplication,
     MembraneRoofingReinforcement,
     RoofCoverBoardsFacing,
     RoofCoverBoardsMaterial,
 )
 from openepd.model.validation.numbers import RatioFloat
-from openepd.model.validation.quantity import LengthMmStr, PressureMPaStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr, PressureMPaStr
 
 
 class BituminousRoofingV1(BaseOpenEpdHierarchicalSpec):
     """Bituminous roofing performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -89,18 +89,14 @@
     """Board insulation performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     compressive_strength: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
 
-    _compressive_strength_is_quantity_validator = pyd.validator("compressive_strength", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
-
 
 class FoamedInPlaceV1(BaseOpenEpdHierarchicalSpec):
     """Foamed in place performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
@@ -130,16 +126,14 @@
     total_recycled_content: RatioFloat | None = pyd.Field(default=None, description="", example=0.5, ge=0, le=1)
     post_consumer_recycled_content: RatioFloat | None = pyd.Field(default=None, description="", example=0.5, ge=0, le=1)
     reinforcement: MembraneRoofingReinforcement | None = pyd.Field(default=None, description="", example="Polyester")
     felt_backing: bool | None = pyd.Field(default=None, description="", example=True)
     nsf347: bool | None = pyd.Field(default=None, description="", example=True)
     vantage_vinyl: bool | None = pyd.Field(default=None, description="", example=True)
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-
     # Nested specs:
     BituminousRoofing: BituminousRoofingV1 | None = None
     SinglePlyEPDM: SinglePlyEPDMV1 | None = None
     SinglePlyKEE: SinglePlyKEEV1 | None = None
     SinglePlyOther: SinglePlyOtherV1 | None = None
     SinglePlyPolyurethane: SinglePlyPolyurethaneV1 | None = None
     SinglePlyPVC: SinglePlyPVCV1 | None = None
@@ -155,18 +149,14 @@
     r_value: float | None = pyd.Field(default=None, description="", example=2.3)
     material: InsulatingMaterial | None = pyd.Field(default=None, description="", example="Mineral Wool")
     intended_application: list[InsulationIntendedApplication] | None = pyd.Field(
         default=None, description="", example=["Wall & General"]
     )
     thickness_per_declared_unit: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
 
-    _thickness_per_declared_unit_is_quantity_validator = pyd.validator("thickness_per_declared_unit", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-
     # Nested specs:
     BlanketInsulation: BlanketInsulationV1 | None = None
     BlownInsulation: BlownInsulationV1 | None = None
     BoardInsulation: BoardInsulationV1 | None = None
     FoamedInPlace: FoamedInPlaceV1 | None = None
     SprayedInsulation: SprayedInsulationV1 | None = None
 
@@ -195,18 +185,14 @@
     _EXT_VERSION = "1.0"
 
     # Own fields:
     material: RoofCoverBoardsMaterial | None = pyd.Field(default=None, description="", example="Gypsum Fiber")
     facing: list[RoofCoverBoardsFacing] | None = pyd.Field(default=None, description="", example=["Paper"])
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="1 m")
 
-    _roof_cover_boards_thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-
 
 class SteepSlopeRoofingV1(BaseOpenEpdHierarchicalSpec):
     """Steep slope roofing performance specification."""
 
     _EXT_VERSION = "1.0"
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/utility_piping.py` & `openepd-3.1.3/src/openepd/model/specs/generated/utility_piping.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import BuriedPipingType, PipingAnsiSchedule, UtilityPipingMaterial
-from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr, MassPerLengthStr
 
 
 class BuildingHeatingPipingV1(BaseOpenEpdHierarchicalSpec):
     """Building heating piping performance specification."""
 
     _EXT_VERSION = "1.0"
 
@@ -44,22 +44,14 @@
     """Utility piping performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="6 m")
     piping_diameter: LengthMmStr | None = pyd.Field(default=None, description="", example="200 mm")
-    mass_per_unit_length: str | None = pyd.Field(default=None, description="", example="1 kg / m")
+    mass_per_unit_length: MassPerLengthStr | None = pyd.Field(default=None, description="", example="1 kg / m")
     piping_ansi_schedule: PipingAnsiSchedule | None = pyd.Field(default=None, description="", example="5")
     utility_piping_material: UtilityPipingMaterial | None = pyd.Field(default=None, description="", example="PVC")
 
-    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
-    _piping_diameter_is_quantity_validator = pyd.validator("piping_diameter", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-    _mass_per_unit_length_is_quantity_validator = pyd.validator("mass_per_unit_length", allow_reuse=True)(
-        validate_unit_factory("kg / m")
-    )
-
     # Nested specs:
     BuildingHeatingPiping: BuildingHeatingPipingV1 | None = None
     BuriedPiping: BuriedPipingV1 | None = None
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/wood.py` & `openepd-3.1.3/src/openepd/model/specs/generated/wood.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     CompositeLumberFabrication,
     EngineeredTimberSpecies,
     MassTimberFabrication,
     SawnTimberSpecies,
     SheathingPanelsFabrication,
 )
 from openepd.model.validation.numbers import RatioFloat
-from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
+from openepd.model.validation.quantity import LengthMmStr
 
 
 class WoodDeckingV1(BaseOpenEpdHierarchicalSpec):
     """Wood used for decking."""
 
     _EXT_VERSION = "1.0"
 
@@ -115,18 +115,14 @@
     _EXT_VERSION = "1.0"
 
     # Own fields:
     fabrication: SheathingPanelsFabrication | None = pyd.Field(default=None, description="", example="Plywood")
     wood_board_thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
     timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
 
-    _wood_board_thickness_is_quantity_validator = pyd.validator("wood_board_thickness", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
-
 
 class UnfinishedWoodV1(BaseOpenEpdHierarchicalSpec):
     """Unfinished or 'green' timber."""
 
     _EXT_VERSION = "1.0"
```

### Comparing `openepd-3.1.2/src/openepd/model/specs/generated/wood_joists.py` & `openepd-3.1.3/src/openepd/model/specs/generated/wood_joists.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/standard.py` & `openepd-3.1.3/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/validation/__init__.py` & `openepd-3.1.3/src/openepd/model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/validation/common.py` & `openepd-3.1.3/src/openepd/model/validation/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/src/openepd/model/validation/numbers.py` & `openepd-3.1.3/src/openepd/compat/compat_functional_validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import Annotated
+from typing import Any
 
-from openepd.compat.pydantic import pyd
+__all__ = ["AfterValidator"]
 
-# todo when move to pydantic 2, check that validators are being enforced.
-RatioFloat = Annotated[float, pyd.Field(ge=0, le=1, example=0.5)]
-PositiveInt = Annotated[int, pyd.Field(ge=0, example=1)]
+
+class AfterValidator:
+    """Placeholder stub for validator, unused in pydantic 1."""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        pass
```

### Comparing `openepd-3.1.2/src/openepd/model/versioning.py` & `openepd-3.1.3/src/openepd/model/versioning.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.2/PKG-INFO` & `openepd-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 3.1.2
+Version: 3.1.3
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 3.1.2 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 3.1.3 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: open-source@c-change-
 labs.com Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

