# Comparing `tmp/circuitcalculator-0.2.4.tar.gz` & `tmp/circuitcalculator-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitcalculator-0.2.4.tar", last modified: Sat Apr 13 15:13:23 2024, max compression
+gzip compressed data, was "circuitcalculator-0.2.5.tar", last modified: Fri May  3 19:29:03 2024, max compression
```

## Comparing `circuitcalculator-0.2.4.tar` & `circuitcalculator-0.2.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.768934 circuitcalculator-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.768934 circuitcalculator-0.2.4/src/CircuitCalculator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.772934 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/impedance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.772934 circuitcalculator-0.2.4/src/CircuitCalculator/Network/
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/NodalAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/equivalent_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/labelmapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/supernodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/PlottingTemplates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.776934 circuitcalculator-0.2.4/src/CircuitCalculator/SignalProcessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SignalProcessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SignalProcessing/periodic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SignalProcessing/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.776934 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/plot_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.776934 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramSolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/Display.py
--rw-r--r--   0 runner    (1001) docker     (127)    27291 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/Elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/LampLighter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.776934 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/style.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/styling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17548 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.017192 circuitcalculator-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-03 19:29:03.017192 circuitcalculator-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:29:03.017192 circuitcalculator-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.005192 circuitcalculator-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.009193 circuitcalculator-0.2.5/src/CircuitCalculator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.009193 circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/impedance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.013193 circuitcalculator-0.2.5/src/CircuitCalculator/Network/
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Network/NodalAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Network/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Network/equivalent_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Network/labelmapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Network/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Network/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Network/supernodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Network/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/PlottingTemplates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.013193 circuitcalculator-0.2.5/src/CircuitCalculator/SignalProcessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SignalProcessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SignalProcessing/periodic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SignalProcessing/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.013193 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/plot_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.017192 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/DiagramParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/DiagramSolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/Display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25892 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/Elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/LampLighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.017192 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/styles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.017192 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/styles/DIN/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/styles/DIN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/styles/DIN/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/styles/styling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/src/CircuitCalculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.017192 circuitcalculator-0.2.5/src/CircuitCalculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-03 19:29:02.000000 circuitcalculator-0.2.5/src/CircuitCalculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-03 19:29:03.000000 circuitcalculator-0.2.5/src/CircuitCalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:29:02.000000 circuitcalculator-0.2.5/src/CircuitCalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 19:29:02.000000 circuitcalculator-0.2.5/src/CircuitCalculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 19:29:02.000000 circuitcalculator-0.2.5/src/CircuitCalculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:03.017192 circuitcalculator-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17548 2024-05-03 19:28:56.000000 circuitcalculator-0.2.5/tests/test_integration.py
```

### Comparing `circuitcalculator-0.2.4/LICENSE` & `circuitcalculator-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/PKG-INFO` & `circuitcalculator-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: CircuitCalculator
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library for analysing and calculating electric networks.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: matplotlib==3.5.2
-Requires-Dist: schemdraw==0.18
+Requires-Dist: schemdraw==0.19
 
 # CircuitCalculator
 
 This project is a simple calculator for electrical circuits. It allows users to input the values of various components in a circuit (such as resistors, capacitors, and voltage sources) and will then calculate various properties of the circuit, such as the current and voltage at different points.
 
 ## Usage
```

### Comparing `circuitcalculator-0.2.4/README.md` & `circuitcalculator-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/circuit.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/circuit.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/components.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/components.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/impedance.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/impedance.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/serializers.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/serializers.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/solution.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/solution.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/transformers.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Circuit/transformers.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Network/NodalAnalysis.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Network/NodalAnalysis.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Network/elements.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Network/elements.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Network/equivalent_sources.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Network/equivalent_sources.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Network/loaders.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Network/loaders.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Network/network.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Network/network.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Network/supernodes.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Network/supernodes.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Network/transformers.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Network/transformers.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/PlottingTemplates.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/PlottingTemplates.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SignalProcessing/periodic_functions.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SignalProcessing/periodic_functions.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/TimeSeries.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/layout.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/layout.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/plot_elements.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleAnalysis/plot_elements.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramParser.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/DiagramParser.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramSolution.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/DiagramSolution.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/Display.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/Display.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/Elements.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/Elements.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from . import schemdraw_element_extension as extension
 
 from . import Display as dsp
 
 import numpy as np
 
 from typing import Any
+from collections import ChainMap
 from enum import Enum
 from abc import ABC
 
 def round_node(node: schemdraw.util.Point) -> schemdraw.util.Point:
     def local_round(x):
         return round(x, ndigits=2)
     return schemdraw.util.Point((local_round(node.x), local_round(node.y)))
@@ -446,33 +447,36 @@
     def L(self) -> float:
         return self._L
 
     @property
     def type(self) -> str:
         return 'inductor'
 
-class RealCurrentSource(schemdraw.elements.Element2Term, SimpleCircuitElement):
-    def __init__(self, current_source: CurrentSource, resistor: Resistor, *args, zoom_resistor: float = 0.7, name: str = '', reverse: bool = False, **kwargs):
-        if current_source.is_reverse:
-            reverse = not reverse
-        super().__init__(*args, reverse=reverse, **kwargs)
-        SimpleCircuitElement.__init__(self, name=current_source.name, reverse=reverse)
-        self.segments += segments_of(current_source)
-        transform = schemdraw.transform.Transform(theta = 0, globalshift=((1-zoom_resistor)/2,-1.5), localshift=(0, 0), zoom=zoom_resistor)
-        self.segments += [s.xform(transform) for s in segments_of(resistor)]
-        left_line = schemdraw.Segment([(-1, 0), (-1, -1.5), ((1-zoom_resistor)/2, -1.5)])
-        right_line = schemdraw.Segment([(2, 0), (2, -1.5), ((1+zoom_resistor)/2, -1.5)])
-        self.segments += [left_line, right_line]
-        self.anchors['value_label'] = (0.5, -1.2)
-        self.anchors['i_label'] = current_source.anchors['i_label']
-        self.anchors['v_label'] = (0.5, -2.4)
-        self._userlabels += current_source._userlabels
-        self._userlabels += resistor._userlabels
-        self._I = current_source.I
-        self._R = resistor.R
+@extension.linear_current_source
+@simple_circuit_element
+class RealCurrentSource(schemdraw.elements.compound.ElementCompound):
+    def __init__(self, name: str, I: float, R: float, *args, **kwargs):
+        self._I = I
+        self._R = R
+        self._name = name
+        super().__init__(*args, **kwargs)
+
+    def setup(self):
+        zoom_resistor = 0.7
+        cs = CurrentSource(I=self._I, name=self._name, d='r')
+        res = Resistor(R=self._R, name='R', l=zoom_resistor, d='r')
+        transform = schemdraw.transform.Transform(theta = 0, globalshift=(((-3-zoom_resistor)/2,-1.5)), localshift=(0, 0), zoom=zoom_resistor)
+        res.segments = [s.xform(transform) for s in res.segments]
+        res.anchors['value_label'] = (-1.5, -2.5)
+        self.add(cs)
+        self.add(res)
+        self.add(l_up:=schemdraw.elements.Line(d='r', l=1).at(res.end))
+        self.add(l_down:=schemdraw.elements.Line(d='l', l=1).at(res.start))
+        self.add(schemdraw.elements.Line(d='u', l=1.5).at(l_up.end))
+        self.add(schemdraw.elements.Line(d='u', l=1.5).at(l_down.end))
 
     @property
     def I(self) -> complex:
         return self._I
 
     @property
     def R(self) -> float:
@@ -482,45 +486,33 @@
     def G(self) -> float:
         return 1/self._R
 
     @property
     def type(self) -> str:
         return 'real_current_source'
 
-class RealVoltageSource(schemdraw.elements.Element2Term, SimpleCircuitElement):
-    def __init__(self, voltage_source: VoltageSource, resistor: Resistor, *args, reverse: bool = False, **kwargs):
-        reverse_voltage_source = not voltage_source.is_reverse
-        if reverse_voltage_source:
-            reverse = not reverse
-        schemdraw.elements.Element2Term.__init__(self, *args, reverse=reverse_voltage_source, **kwargs)
-        SimpleCircuitElement.__init__(self, name=voltage_source.name, reverse=reverse_voltage_source)
-        transform_resistor = schemdraw.transform.Transform(theta = 0, globalshift=(0, 0))
-        transform_voltage_source = schemdraw.transform.Transform(theta = 0, globalshift=(3, 0))
-        if reverse:
-            transform_resistor, transform_voltage_source = transform_voltage_source, transform_resistor
-        self.segments.append(schemdraw.segments.Segment([(0, 0), (0, 0), schemdraw.elements.elements.gap, (1, 0), (3, 0), schemdraw.elements.elements.gap, (4, 0), (4, 0)]))
-        self.segments.extend([s.xform(transform_resistor) for s in segments_of(resistor)])
-        self.segments.extend([s.xform(transform_voltage_source) for s in segments_of(voltage_source)])
-        for a, p in voltage_source.anchors.items():
-            self.anchors[a+'_vs'] = transform_voltage_source.transform(p)
-        for a, p in resistor.anchors.items():
-            self.anchors[a+'_res'] = transform_resistor.transform(p)
-        voltage_source_labels = [l for l in voltage_source._userlabels]
-        resistor_labels = [l for l in resistor._userlabels]
-        for l in voltage_source_labels:
-            if type(l.loc) == str:
-                l.loc += '_vs'
-        for l in resistor_labels:
-            if type(l.loc) == str:
-                l.loc += '_res'
-        self._userlabels += voltage_source._userlabels
-        self._userlabels += resistor._userlabels
-        self._V = -voltage_source.V
-        self._R = resistor.R
-        self.anchors['v_label'] = (2, -1.5)
+@extension.linear_voltage_source
+@simple_circuit_element
+class RealVoltageSource(schemdraw.elements.compound.ElementCompound):
+    def __init__(self, name: str, V: float, R: float, *args, **kwargs):
+        self._V = V
+        self._R = R
+        self._name = name
+        super().__init__(*args, **kwargs)
+
+    def setup(self):
+        zoom_resistor = 1 
+        vs = VoltageSource(V=self._V, name=self._name, d='l')
+        res = Resistor(R=self._R, name='R', l=zoom_resistor, d='l')
+        transform_resistor = schemdraw.transform.Transform(theta = 0, globalshift=(0, 0), zoom=zoom_resistor)
+        res.segments = [s.xform(transform_resistor) for s in res.segments]
+        res.anchors['value_label'] = (0.5, -0.8)
+        self.add(L:=schemdraw.elements.Line(d='l', l=1))
+        self.add(res.at(L.end))
+        self.add(vs)
 
     @property
     def V(self) -> complex:
         return self._V
 
     @property
     def R(self) -> float:
@@ -704,18 +696,16 @@
     def left(self) -> schemdraw.elements.Element:
         return super().down()
 
     def right(self) -> schemdraw.elements.Element:
         return super().up()
 
 class VoltageLabel(schemdraw.elements.CurrentLabel):
-    def __init__(self, at: schemdraw.elements.Element, vlabel: str = '', label_loc: str = 'bottom', reverse: bool = False, **kwargs):
-        kwargs.update({'color': kwargs.get('color', dsp.blue)})
-        kwargs.update({'headlength': kwargs.get('headlength', 0.4)})
-        kwargs.update({'headwidth': kwargs.get('headwidth', 0.3)})
+    def __init__(self, at: schemdraw.elements.Element, vlabel: str = '', label_loc: str = 'bottom', reverse: bool = False, color: str | tuple[float, float, float] = dsp.blue, **kwargs):
+        self.params = ChainMap({'headwidth': 0.3, 'headlength': 0.4, 'color': color}, self.params)
         if isinstance(at, RealVoltageSource):
             kwargs.update({'length': kwargs.get('length', 4)})
         super().__init__(reverse=reverse, **kwargs)
         try:
             self.at(at.v_label)
             self.theta(at.transform.theta)
         except AttributeError:
```

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/LampLighter.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/LampLighter.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             self.anchors['value_label'] = (0.5, -0.9)
             self.anchors['v_label'] = (0.5, 0.3)
             self.anchors['s_label'] = (0.5, -1.2)
             return super().left()
 
         def _place_label(self, label: schemdraw.elements.elements.Label, theta: float = 0):
             delta = self.end-self.start
-            if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
+            if abs(delta[1]) > abs(delta[0]): # portrait placing
                 if delta[1] < 0:
                     theta = 90
             super()._place_label(label=label, theta=theta)
     
     return extended_resistor
 
 def source(element: Type[schemdraw.elements.Element]) -> Type[schemdraw.elements.Element]:
@@ -69,15 +69,15 @@
             self.anchors['value_label'] = (0.0, -0.6)
             self.anchors['s_label'] = (0.0, -1.1)
             self.anchors['v_label'] = (0.0, 0.3)
             return super().left()
 
         def _place_label(self, label: schemdraw.elements.elements.Label, theta: float = 0):
             delta = self.end-self.start
-            if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
+            if abs(delta[1]) > abs(delta[0]): # portrait placing
                 if delta[1] < 0:
                     theta = 90
             super()._place_label(label=label, theta=theta)
 
     return extended_inductor
 
 def inductor(element: Type[schemdraw.elements.Element]) -> Type[schemdraw.elements.Element]:
@@ -98,21 +98,53 @@
             self.anchors['value_label'] = (0.5, -0.6)
             self.anchors['v_label'] = (0.5, 0.2)
             self.anchors['s_label'] = (0.5, -1.2)
             return super().left()
 
         def _place_label(self, label: schemdraw.elements.elements.Label, theta: float = 0):
             delta = self.end-self.start
-            if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
+            if abs(delta[1]) > abs(delta[0]): # portrait placing
                 if delta[1] < 0:
                     theta = 90
             super()._place_label(label=label, theta=theta)
 
     return extended_inductor
 
+def linear_current_source(element: Type[schemdraw.elements.Element]) -> Type[schemdraw.elements.Element]:
+    class extended_linear_source(element):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.anchors['value_label'] = (0.5, -1.2)
+            self.anchors['start'] = (0, 0)
+            self.anchors['center'] = (0, 1.5)
+            self.anchors['end'] = (3, 0)
+
+        def up(self) -> schemdraw.elements.Element:
+            self.anchors['value_label'] = (0.5, -0.6)
+            self.anchors['v_label'] = (1.5, -2.5)
+            self.anchors['s_label'] = (0.5, -1.2)
+            return super().up()
+
+    return extended_linear_source
+
+def linear_voltage_source(element: Type[schemdraw.elements.Element]) -> Type[schemdraw.elements.Element]:
+    class extended_linear_source(element):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.anchors['v_label'] = (2, -1.5)
+            self.anchors['start'] = (-5, 0)
+            self.anchors['center'] = (0, 1.5)
+            self.anchors['end'] = (0, 0)
+
+        def up(self) -> schemdraw.elements.Element:
+            self.anchors['v_label'] = (-1.5, -2.5)
+            return super().up()
+
+    return extended_linear_source
+
 def lamp(element: Type[schemdraw.elements.Element]) -> Type[schemdraw.elements.Element]:
     class extended_lamp(element):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             self.anchors['value_label'] = (0.5, 0.8)
             self.anchors['v_label'] = (0.5, -1.1)
             self.anchors['i_label'] = (1.2, 0.3)
```

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/serializer.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     str: lambda x: x,
     int: lambda x: x,
     float: lambda x: x,
     bool: lambda x: x,
     dict: lambda x: {k: serialize_schemdraw_element(v) for k, v in x.items()},
     list: lambda x: [serialize_schemdraw_element(e) for e in x],
     tuple: lambda x: [serialize_schemdraw_element(e) for e in x],
-    ChainMap: lambda x: dict(x),
+    ChainMap: lambda x: {k: serialize_schemdraw_element(v) for k, v in x.items()},
     schemdraw.util.Point: lambda x: schemdraw_object_properties(x, listify_point),
     schemdraw.segments.Segment: lambda x: schemdraw_object_properties(x, dictify_segment),
     schemdraw.segments.SegmentText: lambda x: schemdraw_object_properties(x, dictify_segment_text),
     schemdraw.segments.SegmentCircle: lambda x: schemdraw_object_properties(x, dictify_segment_circle),
     schemdraw.transform.Transform: lambda x: schemdraw_object_properties(x, dictify_transform)
 }
```

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from schemdraw.elements.twoterm import ResistorIEC
 from schemdraw.elements.sources import Source
 from schemdraw.transform import Transform
-from schemdraw.segments import Segment, SegmentArrow
+from schemdraw.segments import Segment
 
 class InductorDIN(ResistorIEC):
     def __init__(self, *d, **kwargs):
         super().__init__(*d, **kwargs)
         self.segments = [self.segments[0].xform(Transform(theta=0, globalshift=(0,0)), fill='black')]
 
 class SourceUDIN(Source):
@@ -17,8 +17,8 @@
     def __init__(self, *d, **kwargs):
         super().__init__(*d, **kwargs)
         self.segments.append(Segment([(0.5, -0.5), (0.5, 0.5)]))
 
 class SourceIDIN2(SourceIDIN):
     def __init__(self, *d, **kwargs):
         super().__init__(*d, **kwargs)
-        self.segments.append(SegmentArrow((1.2, 0.2), (1.7, 0.2)))
+        self.segments.append(Segment((1.2, 0.2), (1.7, 0.2), arrow='>'))
```

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator/Utils.py` & `circuitcalculator-0.2.5/src/CircuitCalculator/Utils.py`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/PKG-INFO` & `circuitcalculator-0.2.5/src/CircuitCalculator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: CircuitCalculator
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library for analysing and calculating electric networks.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: matplotlib==3.5.2
-Requires-Dist: schemdraw==0.18
+Requires-Dist: schemdraw==0.19
 
 # CircuitCalculator
 
 This project is a simple calculator for electrical circuits. It allows users to input the values of various components in a circuit (such as resistors, capacitors, and voltage sources) and will then calculate various properties of the circuit, such as the current and voltage at different points.
 
 ## Usage
```

### Comparing `circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/SOURCES.txt` & `circuitcalculator-0.2.5/src/CircuitCalculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitcalculator-0.2.4/tests/test_integration.py` & `circuitcalculator-0.2.5/tests/test_integration.py`

 * *Files identical despite different names*

