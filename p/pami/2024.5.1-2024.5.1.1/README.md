# Comparing `tmp/pami-2024.5.1.tar.gz` & `tmp/pami-2024.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2024.5.1.tar", last modified: Wed May  1 06:53:05 2024, max compression
+gzip compressed data, was "pami-2024.5.1.1.tar", last modified: Fri May  3 04:25:47 2024, max compression
```

## Comparing `pami-2024.5.1.tar` & `pami-2024.5.1.1.tar`

### file list

```diff
@@ -1,511 +1,512 @@
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.857908 pami-2024.5.1/
--rw-r--r--   0 vanithak   (502) staff       (20)    35149 2024-03-12 04:33:29.000000 pami-2024.5.1/LICENSE
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.315498 pami-2024.5.1/PAMI/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.316523 pami-2024.5.1/PAMI/AssociationRules/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.325226 pami-2024.5.1/PAMI/AssociationRules/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    13852 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14350 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14263 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19416 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6594 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)      139 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.326241 pami-2024.5.1/PAMI/correlatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.330275 pami-2024.5.1/PAMI/correlatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25689 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/correlatedPattern/basic/CoMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)    27462 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/correlatedPattern/basic/CoMinePlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6208 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.331115 pami-2024.5.1/PAMI/coveragePattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.335347 pami-2024.5.1/PAMI/coveragePattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    14643 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17200 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7155 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.344231 pami-2024.5.1/PAMI/extras/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.353515 pami-2024.5.1/PAMI/extras/DF2DB/
--rw-r--r--   0 vanithak   (502) staff       (20)     4360 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4287 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    10331 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/DF2DB/DenseFormatDF.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5413 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/DF2DB/SparseFormatDF.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3103 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6948 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    11940 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5336 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.356881 pami-2024.5.1/PAMI/extras/calculateMISValues/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6468 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6499 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/extras/calculateMISValues/usingSD.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7345 2024-04-17 06:00:20.000000 pami-2024.5.1/PAMI/extras/convertMultiTSIntoFuzzy.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.370072 pami-2024.5.1/PAMI/extras/dbStats/
--rw-r--r--   0 vanithak   (502) staff       (20)    14951 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/extras/dbStats/FuzzyDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13796 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16034 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/dbStats/SequentialDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16883 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/extras/dbStats/TemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12839 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/extras/dbStats/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15120 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    11953 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12679 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/dbStats/UtilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/dbStats/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.374748 pami-2024.5.1/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5238 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8594 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8792 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8313 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.380232 pami-2024.5.1/PAMI/extras/generateDatabase/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5685 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     9558 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5971 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5157 2024-04-10 08:52:08.000000 pami-2024.5.1/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.387990 pami-2024.5.1/PAMI/extras/graph/
--rw-r--r--   0 vanithak   (502) staff       (20)     3223 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/graph/DF2Fig.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3577 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/graph/DF2Tex.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/graph/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2750 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3599 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4465 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/graph/visualizeFuzzyPatterns.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4240 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.388961 pami-2024.5.1/PAMI/extras/image2Database/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.390625 pami-2024.5.1/PAMI/extras/imageProcessing/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6488 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.395348 pami-2024.5.1/PAMI/extras/messaging/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/messaging/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)      533 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/messaging/discord.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1575 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/messaging/gmail.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.399343 pami-2024.5.1/PAMI/extras/neighbours/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4784 2024-04-17 06:00:20.000000 pami-2024.5.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4410 2024-04-17 06:00:20.000000 pami-2024.5.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4305 2024-04-17 06:00:20.000000 pami-2024.5.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5013 2024-04-10 08:52:08.000000 pami-2024.5.1/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5183 2024-04-10 08:52:08.000000 pami-2024.5.1/PAMI/extras/plotPointOnMap_dump.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.400956 pami-2024.5.1/PAMI/extras/sampleDatasets/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/sampleDatasets/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4024 2024-04-10 08:52:08.000000 pami-2024.5.1/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.410030 pami-2024.5.1/PAMI/extras/stats/
--rw-r--r--   0 vanithak   (502) staff       (20)    12724 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/stats/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/stats/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4144 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/stats/graphDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15998 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/stats/sequentialDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16926 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/stats/temporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12692 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/extras/stats/utilityDatabase.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.439339 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/
--rw-r--r--   0 vanithak   (502) staff       (20)     7276 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6548 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2325 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2254 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2539 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1880 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1843 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2117 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2066 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2262 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/fuzzyDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1121 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1111 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1625 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1610 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3613 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3603 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/georeferencedTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/georeferencedTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4324 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3283 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4842 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3240 2024-04-10 08:52:08.000000 pami-2024.5.1/PAMI/extras/topKPatterns.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2322 2024-04-10 08:52:08.000000 pami-2024.5.1/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.441309 pami-2024.5.1/PAMI/extras/visualize/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/extras/visualize/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1897 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/extras/visualize/graphs.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.442670 pami-2024.5.1/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.452722 pami-2024.5.1/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    14510 2024-05-01 06:38:00.000000 pami-2024.5.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23166 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6856 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.454470 pami-2024.5.1/PAMI/frequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.472104 pami-2024.5.1/PAMI/frequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    13840 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5467 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/Apriori2.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13544 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/Aprioribitset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13342 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13827 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13937 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19498 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15219 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/_Apriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22703 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/_FPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6818 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.475124 pami-2024.5.1/PAMI/frequentPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    20178 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6580 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.483358 pami-2024.5.1/PAMI/frequentPattern/cuda/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5980 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13664 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14418 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13015 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14583 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14499 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17118 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14178 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.486680 pami-2024.5.1/PAMI/frequentPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    26092 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6561 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.493933 pami-2024.5.1/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5573 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15452 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12947 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17438 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.497491 pami-2024.5.1/PAMI/frequentPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)    15426 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4575 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.498463 pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.502344 pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28229 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6652 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.503409 pami-2024.5.1/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.510424 pami-2024.5.1/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    22973 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28621 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6442 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.511597 pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.516470 pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    26162 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28607 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6730 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.517593 pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.522525 pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28521 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    33585 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6623 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.523710 pami-2024.5.1/PAMI/fuzzyPartialPeriodicPatterns/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.528564 pami-2024.5.1/PAMI/fuzzyPartialPeriodicPatterns/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    22562 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyPartialPeriodicPatterns/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6469 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.529908 pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.534445 pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25786 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    27472 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6683 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.535681 pami-2024.5.1/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.538485 pami-2024.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    22107 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6791 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.539582 pami-2024.5.1/PAMI/georeferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/georeferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.546563 pami-2024.5.1/PAMI/georeferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    22965 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21152 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6697 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.547700 pami-2024.5.1/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6696 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.548714 pami-2024.5.1/PAMI/georeferencedPartialPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.552062 pami-2024.5.1/PAMI/georeferencedPartialPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    21718 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6178 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.553287 pami-2024.5.1/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.556044 pami-2024.5.1/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    38524 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6179 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.559387 pami-2024.5.1/PAMI/highUtilityGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.563106 pami-2024.5.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    42772 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6307 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.564260 pami-2024.5.1/PAMI/highUtilityPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.572558 pami-2024.5.1/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35224 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26511 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28921 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19909 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.578593 pami-2024.5.1/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17831 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.584069 pami-2024.5.1/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 vanithak   (502) staff       (20)    30022 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32848 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5193 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.586403 pami-2024.5.1/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6716 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.594624 pami-2024.5.1/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29850 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)    37379 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5934 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.599643 pami-2024.5.1/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)    37519 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.601218 pami-2024.5.1/PAMI/localPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.607770 pami-2024.5.1/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35370 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24681 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23709 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8385 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.611097 pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.616047 pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    24308 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22008 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5921 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.617479 pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.622661 pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28270 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21954 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5398 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.626027 pami-2024.5.1/PAMI/partialPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.634531 pami-2024.5.1/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    26420 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4329 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    25525 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19577 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5520 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.638550 pami-2024.5.1/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    22070 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5605 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.644525 pami-2024.5.1/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    29144 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4278 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.648144 pami-2024.5.1/PAMI/partialPeriodicPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5765 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28554 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.652976 pami-2024.5.1/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6441 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19588 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.659750 pami-2024.5.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
--rw-r--r--   0 vanithak   (502) staff       (20)    28160 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6350 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.660855 pami-2024.5.1/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.664112 pami-2024.5.1/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    27559 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6691 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.665207 pami-2024.5.1/PAMI/periodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.682575 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    17272 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21302 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26383 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18106 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 vanithak   (502) staff       (20)    36300 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17904 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/_PFECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28583 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/_PFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      726 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6549 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26643 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.687595 pami-2024.5.1/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    24417 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6539 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.692951 pami-2024.5.1/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6568 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23867 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18982 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.698907 pami-2024.5.1/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    31832 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7869 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.702417 pami-2024.5.1/PAMI/periodicFrequentPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5219 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26749 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.704239 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.710674 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 vanithak   (502) staff       (20)    19951 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6862 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.714187 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4589 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17514 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.715669 pami-2024.5.1/PAMI/recurringPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.719934 pami-2024.5.1/PAMI/recurringPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29135 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6637 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.721263 pami-2024.5.1/PAMI/relativeFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.727543 pami-2024.5.1/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30349 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4261 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.729029 pami-2024.5.1/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.732436 pami-2024.5.1/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35406 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6052 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.733838 pami-2024.5.1/PAMI/sequence/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/sequence/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.734495 pami-2024.5.1/PAMI/sequentialPatternMining/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.742926 pami-2024.5.1/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    42265 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19986 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/sequentialPatternMining/basic/SPAM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6569 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24786 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.746056 pami-2024.5.1/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6285 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.746629 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.753506 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    18431 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26770 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19807 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7271 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.758825 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 vanithak   (502) staff       (20)    27859 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7173 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.761037 pami-2024.5.1/PAMI/subgraphMining/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.773301 pami-2024.5.1/PAMI/subgraphMining/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1241 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2396 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/dfsCode.py
--rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/edge.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2616 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/extendedEdge.py
--rw-r--r--   0 vanithak   (502) staff       (20)      670 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/frequentSubgraph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4943 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/graph.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28244 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/gspan.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1748 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py
--rw-r--r--   0 vanithak   (502) staff       (20)      826 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/subgraphMining/basic/vertex.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.794423 pami-2024.5.1/PAMI/subgraphMining/topK/
--rw-r--r--   0 vanithak   (502) staff       (20)     1949 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/DFSCode.py
--rw-r--r--   0 vanithak   (502) staff       (20)      593 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/DFSThread.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1316 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/edge.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2613 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/extendedEdge.py
--rw-r--r--   0 vanithak   (502) staff       (20)      674 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/frequentSubgraph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4295 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/graph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1486 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20979 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/tkg.py
--rw-r--r--   0 vanithak   (502) staff       (20)      818 2024-03-29 21:11:29.000000 pami-2024.5.1/PAMI/subgraphMining/topK/vertex.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.797977 pami-2024.5.1/PAMI/uncertainFaultTolerantFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)    17694 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6756 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.799172 pami-2024.5.1/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.815201 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28251 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 vanithak   (502) staff       (20)    27430 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20311 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20112 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28047 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 vanithak   (502) staff       (20)    25675 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19871 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4945 2024-04-09 02:02:26.000000 pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.816487 pami-2024.5.1/PAMI/uncertainGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.821020 pami-2024.5.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30577 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4986 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.822263 pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.830065 pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    33173 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    33178 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6536 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.831283 pami-2024.5.1/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.834506 pami-2024.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29414 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6603 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.835604 pami-2024.5.1/PAMI/weightedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.839197 pami-2024.5.1/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25844 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6659 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.840540 pami-2024.5.1/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.845171 pami-2024.5.1/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29035 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7495 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.846076 pami-2024.5.1/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.848951 pami-2024.5.1/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    31245 2024-05-01 06:38:01.000000 pami-2024.5.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4771 2024-03-12 04:33:29.000000 pami-2024.5.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    71688 2024-05-01 06:53:05.856971 pami-2024.5.1/PKG-INFO
--rw-r--r--   0 vanithak   (502) staff       (20)    70199 2024-05-01 06:38:01.000000 pami-2024.5.1/README.md
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-01 06:53:05.853639 pami-2024.5.1/pami.egg-info/
--rw-r--r--   0 vanithak   (502) staff       (20)    71688 2024-05-01 06:53:05.000000 pami-2024.5.1/pami.egg-info/PKG-INFO
--rw-r--r--   0 vanithak   (502) staff       (20)    18316 2024-05-01 06:53:05.000000 pami-2024.5.1/pami.egg-info/SOURCES.txt
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-05-01 06:53:05.000000 pami-2024.5.1/pami.egg-info/dependency_links.txt
--rw-r--r--   0 vanithak   (502) staff       (20)      255 2024-05-01 06:53:05.000000 pami-2024.5.1/pami.egg-info/requires.txt
--rw-r--r--   0 vanithak   (502) staff       (20)        5 2024-05-01 06:53:05.000000 pami-2024.5.1/pami.egg-info/top_level.txt
--rw-r--r--   0 vanithak   (502) staff       (20)       38 2024-05-01 06:53:05.858117 pami-2024.5.1/setup.cfg
--rw-r--r--   0 vanithak   (502) staff       (20)     1533 2024-05-01 06:52:41.000000 pami-2024.5.1/setup.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.565535 pami-2024.5.1.1/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35149 2024-03-12 04:33:29.000000 pami-2024.5.1.1/LICENSE
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.900262 pami-2024.5.1.1/PAMI/
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.902770 pami-2024.5.1.1/PAMI/AssociationRules/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.912131 pami-2024.5.1.1/PAMI/AssociationRules/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    14350 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/AssociationRules/basic/_ARWithLeverage.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14263 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/AssociationRules/basic/_ARWithLift.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19416 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/AssociationRules/basic/_RuleMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6613 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12724 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/AssociationRules/basic/confidence.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12638 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/AssociationRules/basic/leverage.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12430 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/AssociationRules/basic/lift.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      139 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.912835 pami-2024.5.1.1/PAMI/correlatedPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.915865 pami-2024.5.1.1/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    26443 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/correlatedPattern/basic/CoMine.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    27988 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/correlatedPattern/basic/CoMinePlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6208 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.916708 pami-2024.5.1.1/PAMI/coveragePattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/coveragePattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.921434 pami-2024.5.1.1/PAMI/coveragePattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    14643 2024-05-01 06:38:00.000000 pami-2024.5.1.1/PAMI/coveragePattern/basic/CMine.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    17200 2024-05-01 06:38:00.000000 pami-2024.5.1.1/PAMI/coveragePattern/basic/CPPG.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/coveragePattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7155 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/coveragePattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.931293 pami-2024.5.1.1/PAMI/extras/
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.943878 pami-2024.5.1.1/PAMI/extras/DF2DB/
+-rw-r--r--   0 vanithak   (502) staff       (20)     4360 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4287 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    10331 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/DF2DB/DenseFormatDF.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5413 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/DF2DB/SparseFormatDF.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3103 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6948 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    11940 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5336 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.946906 pami-2024.5.1.1/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6468 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6499 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/extras/calculateMISValues/usingSD.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7345 2024-04-17 06:00:20.000000 pami-2024.5.1.1/PAMI/extras/convertMultiTSIntoFuzzy.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.960420 pami-2024.5.1.1/PAMI/extras/dbStats/
+-rw-r--r--   0 vanithak   (502) staff       (20)    14951 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/extras/dbStats/FuzzyDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    13796 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16034 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/dbStats/SequentialDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16883 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/extras/dbStats/TemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12839 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/extras/dbStats/TransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15120 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    11953 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12679 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/dbStats/UtilityDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/dbStats/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.964871 pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5238 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8594 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8792 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8313 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.969297 pami-2024.5.1.1/PAMI/extras/generateDatabase/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5685 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     9558 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5971 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5157 2024-04-10 08:52:08.000000 pami-2024.5.1.1/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.981897 pami-2024.5.1.1/PAMI/extras/graph/
+-rw-r--r--   0 vanithak   (502) staff       (20)     3223 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/graph/DF2Fig.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3577 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/graph/DF2Tex.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2750 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3599 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4465 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/graph/visualizeFuzzyPatterns.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4240 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.983074 pami-2024.5.1.1/PAMI/extras/image2Database/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.984984 pami-2024.5.1.1/PAMI/extras/imageProcessing/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6488 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.989156 pami-2024.5.1.1/PAMI/extras/messaging/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/messaging/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      533 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/messaging/discord.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1575 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/messaging/gmail.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.996932 pami-2024.5.1.1/PAMI/extras/neighbours/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4784 2024-04-17 06:00:20.000000 pami-2024.5.1.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4410 2024-04-17 06:00:20.000000 pami-2024.5.1.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4305 2024-04-17 06:00:20.000000 pami-2024.5.1.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5013 2024-04-10 08:52:08.000000 pami-2024.5.1.1/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5183 2024-04-10 08:52:08.000000 pami-2024.5.1.1/PAMI/extras/plotPointOnMap_dump.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:46.998835 pami-2024.5.1.1/PAMI/extras/sampleDatasets/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/sampleDatasets/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4024 2024-04-10 08:52:08.000000 pami-2024.5.1.1/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.006021 pami-2024.5.1.1/PAMI/extras/stats/
+-rw-r--r--   0 vanithak   (502) staff       (20)    12724 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/stats/TransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/stats/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4144 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/stats/graphDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15998 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/stats/sequentialDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16926 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/stats/temporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12692 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/extras/stats/utilityDatabase.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.036298 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/
+-rw-r--r--   0 vanithak   (502) staff       (20)     7276 2024-05-01 06:38:00.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6548 2024-05-01 06:38:00.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2325 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2254 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2539 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1880 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1843 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2117 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2066 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2262 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/fuzzyDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1121 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1111 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1625 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1610 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3613 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3603 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/georeferencedTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/georeferencedTransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4324 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3283 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4842 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3240 2024-04-10 08:52:08.000000 pami-2024.5.1.1/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2322 2024-04-10 08:52:08.000000 pami-2024.5.1.1/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.037691 pami-2024.5.1.1/PAMI/extras/visualize/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/extras/visualize/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1897 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/extras/visualize/graphs.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.038505 pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.044633 pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    14510 2024-05-01 06:38:00.000000 pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    23166 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6856 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.047017 pami-2024.5.1.1/PAMI/frequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.057684 pami-2024.5.1.1/PAMI/frequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    13840 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    13544 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/Aprioribitset.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    13631 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14033 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    13440 2024-05-03 04:25:04.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19498 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15219 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/_Apriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22703 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/_FPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6818 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.061005 pami-2024.5.1.1/PAMI/frequentPattern/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)    20178 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6580 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.114338 pami-2024.5.1.1/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5980 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    13664 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14418 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    13015 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14583 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14499 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    17118 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14178 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.118320 pami-2024.5.1.1/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 vanithak   (502) staff       (20)    26092 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6561 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.129268 pami-2024.5.1.1/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5573 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15452 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12947 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    17438 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.139405 pami-2024.5.1.1/PAMI/frequentPattern/topk/
+-rw-r--r--   0 vanithak   (502) staff       (20)    15426 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4575 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.142207 pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.150330 pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28229 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6652 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.151579 pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.161220 pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    22973 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28621 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6442 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.162295 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.166962 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    26162 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28607 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6730 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.168190 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.173289 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28521 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    33585 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6623 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.176595 pami-2024.5.1.1/PAMI/fuzzyPartialPeriodicPatterns/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.180436 pami-2024.5.1.1/PAMI/fuzzyPartialPeriodicPatterns/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    22562 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyPartialPeriodicPatterns/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6469 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.181623 pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.186737 pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    25786 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    27472 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6683 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.187614 pami-2024.5.1.1/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.190226 pami-2024.5.1.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    22107 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6791 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.191702 pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.199540 pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    22965 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    21152 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6697 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.201674 pami-2024.5.1.1/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6696 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.203094 pami-2024.5.1.1/PAMI/georeferencedPartialPeriodicPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.209815 pami-2024.5.1.1/PAMI/georeferencedPartialPeriodicPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    21718 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6178 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.211611 pami-2024.5.1.1/PAMI/highUtilityFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.217241 pami-2024.5.1.1/PAMI/highUtilityFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    38524 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6179 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.218993 pami-2024.5.1.1/PAMI/highUtilityGeoreferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.222800 pami-2024.5.1.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    42772 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6307 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.226332 pami-2024.5.1.1/PAMI/highUtilityPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.237802 pami-2024.5.1.1/PAMI/highUtilityPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35224 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/basic/EFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26511 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/basic/HMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28921 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/basic/UPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19909 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/basic/efimParallel.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.248719 pami-2024.5.1.1/PAMI/highUtilityPattern/parallel/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/parallel/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/parallel/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    17831 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilityPattern/parallel/efimparallel.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.256160 pami-2024.5.1.1/PAMI/highUtilityPatternsInStreams/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30022 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    32848 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityPatternsInStreams/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5193 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilityPatternsInStreams/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.259722 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6716 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.268318 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29850 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    37379 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5934 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.272073 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 vanithak   (502) staff       (20)    37519 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.276659 pami-2024.5.1.1/PAMI/localPeriodicPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.283854 pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35370 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    24681 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    23709 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8385 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.285057 pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.293059 pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    24308 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22008 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5921 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.294844 pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.303922 pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28270 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    21954 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5398 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.305482 pami-2024.5.1.1/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.318005 pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    26420 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4329 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    25525 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19577 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5520 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.322671 pami-2024.5.1.1/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)    22070 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5605 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.328849 pami-2024.5.1.1/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29144 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4278 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.332466 pami-2024.5.1.1/PAMI/partialPeriodicPattern/pyspark/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/pyspark/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5765 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/pyspark/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28554 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.336736 pami-2024.5.1.1/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6441 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19588 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.341676 pami-2024.5.1.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28160 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6350 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.343938 pami-2024.5.1.1/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.347486 pami-2024.5.1.1/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27559 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6691 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.348588 pami-2024.5.1.1/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.364449 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    17272 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    21302 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26383 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18106 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    36300 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    17904 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/_PFECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28583 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/_PFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      726 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6549 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26643 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.372043 pami-2024.5.1.1/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)    24417 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6539 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.379023 pami-2024.5.1.1/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6568 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    23867 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18982 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.383579 pami-2024.5.1.1/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 vanithak   (502) staff       (20)    31832 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7869 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.386434 pami-2024.5.1.1/PAMI/periodicFrequentPattern/pyspark/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5219 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26749 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.387827 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.392152 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 vanithak   (502) staff       (20)    19951 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6862 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.399767 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4589 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    17514 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.405855 pami-2024.5.1.1/PAMI/recurringPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.412363 pami-2024.5.1.1/PAMI/recurringPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29135 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6637 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.413510 pami-2024.5.1.1/PAMI/relativeFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/relativeFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.417093 pami-2024.5.1.1/PAMI/relativeFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30349 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/relativeFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4261 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/relativeFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.418088 pami-2024.5.1.1/PAMI/relativeHighUtilityPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/relativeHighUtilityPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.421027 pami-2024.5.1.1/PAMI/relativeHighUtilityPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35406 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6052 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.422233 pami-2024.5.1.1/PAMI/sequence/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/sequence/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.422744 pami-2024.5.1.1/PAMI/sequentialPatternMining/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.430979 pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    42265 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19986 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/SPAM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6569 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    24786 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.434875 pami-2024.5.1.1/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6285 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.435461 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.444946 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    18431 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26770 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19807 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7271 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.449012 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27859 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7173 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.449996 pami-2024.5.1.1/PAMI/subgraphMining/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.469965 pami-2024.5.1.1/PAMI/subgraphMining/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1241 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2396 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/dfsCode.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/edge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2616 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/extendedEdge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      670 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/frequentSubgraph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4943 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/graph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28244 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/gspan.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1748 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      826 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/basic/vertex.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.484979 pami-2024.5.1.1/PAMI/subgraphMining/topK/
+-rw-r--r--   0 vanithak   (502) staff       (20)     1949 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/DFSCode.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      593 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/DFSThread.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1316 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/edge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2613 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/extendedEdge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      674 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/frequentSubgraph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4295 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/graph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1486 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20979 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/tkg.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      818 2024-03-29 21:11:29.000000 pami-2024.5.1.1/PAMI/subgraphMining/topK/vertex.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.488521 pami-2024.5.1.1/PAMI/uncertainFaultTolerantFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)    17694 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6756 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.491600 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.514911 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28251 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    27430 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20311 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20112 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28047 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    25675 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19871 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4945 2024-04-09 02:02:26.000000 pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.516552 pami-2024.5.1.1/PAMI/uncertainGeoreferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.521296 pami-2024.5.1.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30577 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4986 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.522279 pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.531008 pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    33173 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    33178 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6536 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.532554 pami-2024.5.1.1/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.537178 pami-2024.5.1.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29414 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6603 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.538563 pami-2024.5.1.1/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.545115 pami-2024.5.1.1/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    25844 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6659 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.546617 pami-2024.5.1.1/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.549323 pami-2024.5.1.1/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29035 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7495 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.551185 pami-2024.5.1.1/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.554232 pami-2024.5.1.1/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    31245 2024-05-01 06:38:01.000000 pami-2024.5.1.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4771 2024-03-12 04:33:29.000000 pami-2024.5.1.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    71690 2024-05-03 04:25:47.564537 pami-2024.5.1.1/PKG-INFO
+-rw-r--r--   0 vanithak   (502) staff       (20)    70199 2024-05-01 06:38:01.000000 pami-2024.5.1.1/README.md
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-03 04:25:47.560733 pami-2024.5.1.1/pami.egg-info/
+-rw-r--r--   0 vanithak   (502) staff       (20)    71690 2024-05-03 04:25:46.000000 pami-2024.5.1.1/pami.egg-info/PKG-INFO
+-rw-r--r--   0 vanithak   (502) staff       (20)    18350 2024-05-03 04:25:46.000000 pami-2024.5.1.1/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-05-03 04:25:46.000000 pami-2024.5.1.1/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)      255 2024-05-03 04:25:46.000000 pami-2024.5.1.1/pami.egg-info/requires.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)        5 2024-05-03 04:25:46.000000 pami-2024.5.1.1/pami.egg-info/top_level.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)       38 2024-05-03 04:25:47.565702 pami-2024.5.1.1/setup.cfg
+-rw-r--r--   0 vanithak   (502) staff       (20)     1535 2024-05-03 04:25:29.000000 pami-2024.5.1.1/setup.py
```

### Comparing `pami-2024.5.1/LICENSE` & `pami-2024.5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2024.5.1.1/PAMI/AssociationRules/basic/_ARWithLift.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-# This code uses "confidence" metric to extract the association rules from given frequent patterns.
+# This code uses "lift" metric to extract the association rules from given frequent patterns.
 #
 # **Importing this algorithm into a python program**
-# ----------------------------------------------------
 #
-#             import PAMI.AssociationRules.basic import ARWithConfidence as alg
+#             import PAMI.AssociationRules.basic import ARWithLift as alg
 #
-#             obj = alg.ARWithConfidence(iFile, minConf)
+#             iFile = 'sampleDB.txt'
+#
+#             minConf = 0.75  # can also be specified between 0 and 1
+#
+#             obj = alg.ARWithLift(iFile, minConf)
 #
 #             obj.mine()
 #
 #             associationRules = obj.getPatterns()
 #
 #             print("Total number of Association Rules:", len(associationRules))
 #
@@ -27,15 +30,14 @@
 #
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
-
 __copyright__ = """
 Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -43,111 +45,117 @@
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-     Copyright (C)  2021 Rage Uday Kiran
-     
 """
 
 from PAMI.AssociationRules.basic import abstract as _ab
+from typing import List, Dict, Tuple, Set, Union, Any, Generator
 from deprecated import deprecated
 
-class _Confidence:
+
+class Lift:
     """
     :param  patterns: Dictionary containing patterns and its support value.
-    :type patterns: dict
+    :type  patterns: dict
     :param  singleItems: List containing all the single frequent items.
-    :type singleItems: list
+    :type  singleItems: list
     :param  minConf: Minimum confidence to mine all the satisfying association rules.
-    :type minConf: int
+    :type  minConf: int
     """
-
-    def __init__(self, patterns, singleItems, minConf):
+    
+    def __init__(self, patterns, singleItems, minConf) -> None:
         """
         :param patterns: given frequent patterns
         :type patterns: dict
         :param singleItems: one-length frequent patterns
         :type singleItems: list
         :param minConf: minimum confidence
         :type minConf: float
+        :return: None
         """
         self._frequentPatterns = patterns
         self._singleItems = singleItems
         self._minConf = minConf
         self._finalPatterns = {}
 
-    def _generation(self, prefix, suffix):
+    def _generation(self, prefix, suffix) -> None:
         """
         To generate the combinations all association rules.
 
         :param prefix: the prefix of association rule.
         :type prefix: str
         :param suffix: the suffix of association rule.
         :type suffix: str
+        :return: None
         """
         if len(suffix) == 1:
-            conf = self._generateWithConfidence(prefix, suffix[0])
+            self._generateWithLift(prefix, suffix[0])
         for i in range(len(suffix)):
             suffix1 = suffix[:i] + suffix[i + 1:]
             prefix1 = prefix + ' ' + suffix[i]
             for j in range(i + 1, len(suffix)):
-                self._generateWithConfidence(prefix + ' ' + suffix[i], suffix[j])
+                self._generateWithLift(prefix + ' ' + suffix[i], suffix[j])
                 # self._generation(prefix+ ' ' +suffix[i], suffix[i+1:])
             self._generation(prefix1, suffix1)
 
-    def _generateWithConfidence(self, lhs, rhs):
+    def _generateWithLift(self, lhs, rhs)  -> float:
         """
         To find association rules satisfying user-specified minConf
 
         :param lhs: the prefix of association rule.
         :type lhs: str
         :param rhs: the suffix of association rule.
         :type rhs: str
+        :return: the association rule
+        :rtype: float
         """
         s = lhs + '\t' + rhs
         if self._frequentPatterns.get(s) == None:
             return 0
         minimum = self._frequentPatterns[s]
         conf_lhs = minimum / self._frequentPatterns[lhs]
         conf_rhs = minimum / self._frequentPatterns[rhs]
-        if conf_lhs >= self._minConf:
+        lift_lhs = conf_lhs / self._frequentPatterns[rhs] * self._frequentPatterns[lhs]
+        right_rhs = conf_rhs / self._frequentPatterns[lhs] * self._frequentPatterns[rhs]
+        if lift_lhs >= self._minConf:
             s1 = lhs + '->' + rhs
             self._finalPatterns[s1] = conf_lhs
-        if conf_rhs >= self._minConf:
+        if right_rhs >= self._minConf:
             s1 = rhs + '->' + lhs
             self._finalPatterns[s1] = conf_rhs
 
-    def run(self):
+    def run(self) -> None:
         """
         To generate the combinations all association rules.
         """
         for i in range(len(self._singleItems)):
             suffix = self._singleItems[:i] + self._singleItems[i + 1:]
             prefix = self._singleItems[i]
             for j in range(i + 1, len(self._singleItems)):
-                self._generateWithConfidence(self._singleItems[i], self._singleItems[j])
+                self._generateWithLift(self._singleItems[i], self._singleItems[j])
             self._generation(prefix, suffix)
 
 
-class ARWithConfidence:
+class ARWithLift:
     """
     About this algorithm
     ====================
 
-    :**Description**: Association Rules are derived from frequent patterns using "confidence" metric.
+    :**Description**: Association Rules are derived from frequent patterns using "lift" metric.
 
     :**Reference**:
 
-    :**Parameters**:    - **iFile** (*str*) -- *Name of the Input file to mine complete set of association rules*
-                        - **oFile** (*str*) -- *Name of the Output file to write association rules*
-                        - **minConf** (*float*) -- *Minimum confidence to mine all the satisfying association rules. The user can specify the minConf in float between the range of 0 to 1.*
-                        - **sep** (*str*) -- *This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.*
+    :**Parameters**:    - **iFile** (*str*) -- *Name of the Input file to mine complete set of association rules.*
+                        - **oFile** (*str*) -- *Name of the output file to store complete set of association rules.*
+                        - **minConf** (*float*) -- *The user can specify the minConf in float between the range of 0 to 1.*
+                        - **sep** (*str*) --  *This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.*
 
     :**Attributes**:    - **startTime** (*float*) -- *To record the start time of the mining process.*
                         - **endTime** (*float*) -- *To record the completion time of the mining process.*
                         - **finalPatterns** (*dict*) -- *Storing the complete set of patterns in a dictionary variable.*
                         - **memoryUSS** (*float*) -- *To store the total amount of USS memory consumed by the program.*
                         - **memoryRSS** (*float*) -- *To store the total amount of RSS memory consumed by the program.*
 
@@ -157,30 +165,34 @@
 
     **Terminal command**
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 ARWithConfidence.py <inputFile> <outputFile> <minConf> <sep>
+      (.venv) $ python3 ARWithLift.py <inputFile> <outputFile> <minConf> <sep>
 
       Example Usage:
 
-      (.venv) $ python3 ARWithConfidence.py sampleDB.txt patterns.txt 0.5 ' '
+      (.venv) $ python3 ARWithLift.py sampleDB.txt patterns.txt 0.5 ' '
 
     .. note:: minConf can be specified in a value between 0 and 1.
     
     
     **Calling from a python program**
 
     .. code-block:: python
 
-            import PAMI.AssociationRules.basic import ARWithConfidence as alg
+            import PAMI.AssociationRules.basic import ARWithLift as alg
 
-            obj = alg.ARWithConfidence(iFile, minConf)
+            iFile = 'sampleDB.txt'
+
+            minConf = 0.75  # can also be specified between 0 and 1
+
+            obj = alg.ARWithLift(iFile, minConf)
 
             obj.mine()
 
             associationRules = obj.getPatterns()
 
             print("Total number of Association Rules:", len(associationRules))
 
@@ -200,45 +212,39 @@
 
             print("Total ExecutionTime in seconds:", run)
 
 
     Credits
     =======
 
-            The complete program was written by P. Likhitha  under the supervision of Professor Rage Uday Kiran.
+             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
     """
 
-    _minConf = float()
-    _startTime = float()
-    _endTime = float()
-    _iFile = " "
-    _oFile = " "
-    _Sep = " "
-    _memoryUSS = float()
-    _memoryRSS = float()
-    _frequentPatterns = {}
-
-    def __init__(self, iFile, minConf, sep):
+    def __init__(self, iFile, minConf, sep) -> None:
         """
         :param iFile: input file name or path
         :type iFile: str
         :param minConf: minimum confidence
         :type minConf: float
         :param sep: Delimiter of input file
         :type sep: str
+        :return: None
         """
         self._iFile = iFile
         self._minConf = minConf
         self._finalPatterns = {}
         self._sep = sep
 
-    def _readPatterns(self):
+    def _readPatterns(self) -> list:
         """
         Reading the input file and storing all the frequent patterns and their support respectively in a frequentPatterns variable.
+
+        :return: list of frequent patterns and their support respectively in a frequentPatterns
+        :rtype: list
         """
         self._frequentPatterns = {}
         k = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             pattern, sup = [], []
             if self._iFile.empty:
                 print("its empty..")
@@ -273,70 +279,68 @@
                             self._frequentPatterns[s.strip()] = int(line[1])
                 except IOError:
                     print("File Not Found")
                     quit()
         return k
 
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
-    def startMine(self):
+    def startMine(self) -> None:
         """
         Association rule mining process will start from here
         """
         self.mine()
 
-
-
-    def mine(self):
+    def mine(self) -> None:
         """
         Association rule mining process will start from here
         """
         self._startTime = _ab._time.time()
         k = self._readPatterns()
-        a = _Confidence(self._frequentPatterns, k, self._minConf)
+        a = Lift(self._frequentPatterns, k, self._minConf)
         a.run()
         self._finalPatterns = a._finalPatterns
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
         print("Association rules successfully  generated from frequent patterns ")
 
-    def getMemoryUSS(self):
+    def getMemoryUSS(self) -> float:
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
-    def getMemoryRSS(self):
+    def getMemoryRSS(self) -> float:
         """
         Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryRSS
 
-    def getRuntime(self):
+    def getRuntime(self) -> float:
         """
         Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self):
+    def getPatternsAsDataFrame(self) -> _ab._pd.DataFrame:
         """
         Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
@@ -344,53 +348,54 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
-    def save(self, outFile):
+    def save(self, outFile) -> None:
         """
         Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the outputfile
         :type outFile: file
+        :return: None
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self):
+    def getPatterns(self) -> dict:
         """
         Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self):
+    def printResults(self) -> None:
         """
         Function to send the result after completion of the mining process
         """
         print("Total number of Association Rules:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ARWithConfidence(_ab._sys.argv[1], float(_ab._sys.argv[3]), _ab._sys.argv[4])
+            _ap = ARWithLift(_ab._sys.argv[1], float(_ab._sys.argv[3]), _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ARWithConfidence(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = ARWithLift(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
         print("Total number of Association Rules:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
```

### Comparing `pami-2024.5.1/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2024.5.1.1/PAMI/AssociationRules/basic/_ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2024.5.1.1/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# This code uses "lift" metric to extract the association rules from given frequent patterns.
+# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
 #
-#             import PAMI.AssociationRules.basic import ARWithLift as alg
+#             import PAMI.frequentPattern.basic.ECLAT as alg
 #
 #             iFile = 'sampleDB.txt'
 #
-#             minConf = 0.75  # can also be specified between 0 and 1
+#             minSup = 10  # can also be specified between 0 and 1
 #
-#             obj = alg.ARWithLift(iFile, minConf)
+#             obj = alg.ECLAT(iFile, minSup)
 #
 #             obj.mine()
 #
-#             associationRules = obj.getPatterns()
+#             frequentPatterns = obj.getPatterns()
 #
-#             print("Total number of Association Rules:", len(associationRules))
+#             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
 #             obj.save(oFile)
 #
 #             Df = obj.getPatternInDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
@@ -47,158 +47,74 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from PAMI.AssociationRules.basic import abstract as _ab
-from typing import List, Dict, Tuple, Set, Union, Any, Generator
+from PAMI.frequentPattern.basic import abstract as _ab
 from deprecated import deprecated
 
-
-class Lift:
-    """
-    :param  patterns: Dictionary containing patterns and its support value.
-    :type  patterns: dict
-    :param  singleItems: List containing all the single frequent items.
-    :type  singleItems: list
-    :param  minConf: Minimum confidence to mine all the satisfying association rules.
-    :type  minConf: int
-    """
-    
-    def __init__(self, patterns, singleItems, minConf) -> None:
-        """
-        :param patterns: given frequent patterns
-        :type patterns: dict
-        :param singleItems: one-length frequent patterns
-        :type singleItems: list
-        :param minConf: minimum confidence
-        :type minConf: float
-        :return: None
-        """
-        self._frequentPatterns = patterns
-        self._singleItems = singleItems
-        self._minConf = minConf
-        self._finalPatterns = {}
-
-    def _generation(self, prefix, suffix) -> None:
-        """
-        To generate the combinations all association rules.
-
-        :param prefix: the prefix of association rule.
-        :type prefix: str
-        :param suffix: the suffix of association rule.
-        :type suffix: str
-        :return: None
-        """
-        if len(suffix) == 1:
-            self._generateWithLift(prefix, suffix[0])
-        for i in range(len(suffix)):
-            suffix1 = suffix[:i] + suffix[i + 1:]
-            prefix1 = prefix + ' ' + suffix[i]
-            for j in range(i + 1, len(suffix)):
-                self._generateWithLift(prefix + ' ' + suffix[i], suffix[j])
-                # self._generation(prefix+ ' ' +suffix[i], suffix[i+1:])
-            self._generation(prefix1, suffix1)
-
-    def _generateWithLift(self, lhs, rhs)  -> float:
-        """
-        To find association rules satisfying user-specified minConf
-
-        :param lhs: the prefix of association rule.
-        :type lhs: str
-        :param rhs: the suffix of association rule.
-        :type rhs: str
-        :return: the association rule
-        :rtype: float
-        """
-        s = lhs + '\t' + rhs
-        if self._frequentPatterns.get(s) == None:
-            return 0
-        minimum = self._frequentPatterns[s]
-        conf_lhs = minimum / self._frequentPatterns[lhs]
-        conf_rhs = minimum / self._frequentPatterns[rhs]
-        lift_lhs = conf_lhs / self._frequentPatterns[rhs] * self._frequentPatterns[lhs]
-        right_rhs = conf_rhs / self._frequentPatterns[lhs] * self._frequentPatterns[rhs]
-        if lift_lhs >= self._minConf:
-            s1 = lhs + '->' + rhs
-            self._finalPatterns[s1] = conf_lhs
-        if right_rhs >= self._minConf:
-            s1 = rhs + '->' + lhs
-            self._finalPatterns[s1] = conf_rhs
-
-    def run(self) -> None:
-        """
-        To generate the combinations all association rules.
-        """
-        for i in range(len(self._singleItems)):
-            suffix = self._singleItems[:i] + self._singleItems[i + 1:]
-            prefix = self._singleItems[i]
-            for j in range(i + 1, len(self._singleItems)):
-                self._generateWithLift(self._singleItems[i], self._singleItems[j])
-            self._generation(prefix, suffix)
-
-
-class ARWithLift:
+class ECLAT(_ab._frequentPatterns):
     """
     About this algorithm
     ====================
 
-    :**Description**: Association Rules are derived from frequent patterns using "lift" metric.
+    :**Description**: *ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.*
 
-    :**Reference**:
+    :**Reference**:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
+                     372-390 (2000), https://ieeexplore.ieee.org/document/846291
 
-    :**Parameters**:    - **iFile** (*str*) -- *Name of the Input file to mine complete set of association rules.*
-                        - **oFile** (*str*) -- *Name of the output file to store complete set of association rules.*
-                        - **minConf** (*float*) -- *The user can specify the minConf in float between the range of 0 to 1.*
-                        - **sep** (*str*) --  *This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.*
+    :**Parameters**:    - **iFile** (*str or URL or dataFrame*) -- *Name of the Input file to mine complete set of frequent patterns.*
+                        - **oFile** (*str*) -- *Name of the Output file to store the frequent patterns.*
+                        - **minSup** (*int or float or str*) -- The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+                        - **sep** (*str*) -- This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
     :**Attributes**:    - **startTime** (*float*) -- *To record the start time of the mining process.*
-                        - **endTime** (*float*) -- *To record the completion time of the mining process.*
+                        - **endTime** (*float*) -- *To record the end time of the mining process.*
                         - **finalPatterns** (*dict*) -- *Storing the complete set of patterns in a dictionary variable.*
                         - **memoryUSS** (*float*) -- *To store the total amount of USS memory consumed by the program.*
-                        - **memoryRSS** (*float*) -- *To store the total amount of RSS memory consumed by the program.*
-
+                        - **memoryRSS** *(float*) -- *To store the total amount of RSS memory consumed by the program.*
+                        - **Database** (*list*) -- *To store the transactions of a database in list.*
 
     Execution methods
     =================
 
     **Terminal command**
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 ARWithLift.py <inputFile> <outputFile> <minConf> <sep>
+      (.venv) $ python3 ECLAT.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 ARWithLift.py sampleDB.txt patterns.txt 0.5 ' '
+      (.venv) $ python3 ECLAT.py sampleDB.txt patterns.txt 10.0
+
+    .. note:: minSup can be specified  in support count or a value between 0 and 1.
+
 
-    .. note:: minConf can be specified in a value between 0 and 1.
-    
-    
     **Calling from a python program**
 
     .. code-block:: python
 
-            import PAMI.AssociationRules.basic import ARWithLift as alg
+            import PAMI.frequentPattern.basic.ECLAT as alg
 
             iFile = 'sampleDB.txt'
 
-            minConf = 0.75  # can also be specified between 0 and 1
+            minSup = 10  # can also be specified between 0 and 1
 
-            obj = alg.ARWithLift(iFile, minConf)
+            obj = alg.ECLAT(iFile, minSup)
 
             obj.mine()
 
-            associationRules = obj.getPatterns()
+            frequentPatterns = obj.getPatterns()
 
-            print("Total number of Association Rules:", len(associationRules))
+            print("Total number of Frequent Patterns:", len(frequentPatterns))
 
             obj.save(oFile)
 
             Df = obj.getPatternInDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
@@ -209,119 +125,187 @@
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
 
-    Credits
-    =======
+    Credits:
+    ========
 
-             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+    The complete program was written by Kundai and revised by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
-    def __init__(self, iFile, minConf, sep) -> None:
-        """
-        :param iFile: input file name or path
-        :type iFile: str
-        :param minConf: minimum confidence
-        :type minConf: float
-        :param sep: Delimiter of input file
-        :type sep: str
-        :return: None
-        """
-        self._iFile = iFile
-        self._minConf = minConf
-        self._finalPatterns = {}
-        self._sep = sep
+    _minSup = float()
+    _startTime = float()
+    _endTime = float()
+    _finalPatterns = {}
+    _iFile = " "
+    _oFile = " "
+    _sep = " "
+    _memoryUSS = float()
+    _memoryRSS = float()
+    _Database = []
 
-    def _readPatterns(self) -> list:
+    def _creatingItemSets(self) -> float:
         """
-        Reading the input file and storing all the frequent patterns and their support respectively in a frequentPatterns variable.
 
-        :return: list of frequent patterns and their support respectively in a frequentPatterns
-        :rtype: list
+        Storing the complete transactions of the database/input file in a database variable
+
+        :return: the complete transactions of the database/input file in a database variable
+        :rtype: float
         """
-        self._frequentPatterns = {}
-        k = []
+        self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            pattern, sup = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
-            if 'pattern' in i:
-                pattern = self._iFile['pattern'].tolist()
-            if 'support' in i:
-                support = self._iFile['support'].tolist()
-            for i in range(len(pattern)):
-                s = '\t'.join(pattern[i])
-                self._frequentPattern[s] = support[i]
+            if 'Transactions' in i:
+                self._Database = self._iFile['Transactions'].tolist()
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
-                    line = line.strip()
-                    line = line.split(':')
-                    s = line[0].split(self._sep)
-                    s = '\t'.join(s)
-                    self._frequentPatterns[s.strip()] = int(line[1])
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
-                            line = line.strip()
-                            line = line.split(':')
-                            s = line[0].split(self._sep)
-                            for j in s:
-                                if j not in k:
-                                    k.append(j)
-                            s = '\t'.join(s)
-                            self._frequentPatterns[s.strip()] = int(line[1])
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
-        return k
+
+    def _getUniqueItemList(self) -> list:
+        """
+
+        Generating one frequent patterns
+
+        :return: list of unique patterns
+        :rtype: list
+        """
+        self._finalPatterns = {}
+        candidate = {}
+        uniqueItem = []
+        for i in range(len(self._Database)):
+            for j in range(len(self._Database[i])):
+                if self._Database[i][j] not in candidate:
+                    candidate[self._Database[i][j]] = {i}
+                else:
+                    candidate[self._Database[i][j]].add(i)
+        for key, value in candidate.items():
+            supp = len(value)
+            if supp >= self._minSup:
+                self._finalPatterns[key] = [value]
+                uniqueItem.append(key)
+        uniqueItem.sort()
+        return uniqueItem
+
+    def _generateFrequentPatterns(self, candidateFrequent: list) -> None:
+        """
+
+        It will generate the combinations of frequent items
+
+        :param candidateFrequent :it represents the items with their respective transaction identifiers
+        :type candidateFrequent: list
+        :return: None
+        """
+        new_freqList = []
+        for i in range(0, len(candidateFrequent)):
+            item1 = candidateFrequent[i]
+            i1_list = item1.split()
+            for j in range(i + 1, len(candidateFrequent)):
+                item2 = candidateFrequent[j]
+                i2_list = item2.split()
+                if i1_list[:-1] == i2_list[:-1]:
+                    interSet = self._finalPatterns[item1][0].intersection(self._finalPatterns[item2][0])
+                    if len(interSet) >= self._minSup:
+                        newKey = item1 + "\t" + i2_list[-1]
+                        self._finalPatterns[newKey] = [interSet]
+                        new_freqList.append(newKey)
+                else: break
+
+        if len(new_freqList) > 0:
+                self._generateFrequentPatterns(new_freqList)
+
+    def _convert(self, value) -> float:
+        """
+
+        To convert the user specified minSup value
+
+        :param value: user specified minSup value
+        :return: converted type
+        :rtype: float
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
 
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
-        Association rule mining process will start from here
+        Frequent pattern mining process will start from here
         """
+
         self.mine()
 
     def mine(self) -> None:
         """
-        Association rule mining process will start from here
+        Frequent pattern mining process will start from here
         """
+
         self._startTime = _ab._time.time()
-        k = self._readPatterns()
-        a = Lift(self._frequentPatterns, k, self._minConf)
-        a.run()
-        self._finalPatterns = a._finalPatterns
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
+        self._creatingItemSets()
+        self._minSup = self._convert(self._minSup)
+        uniqueItemList = self._getUniqueItemList()
+        self._generateFrequentPatterns(uniqueItemList)
+        for x, y in self._finalPatterns.items():
+            self._finalPatterns[x] = len(y[0])
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Association rules successfully  generated from frequent patterns ")
+        print("Frequent patterns were generated successfully using ECLAT algorithm")
 
     def getMemoryUSS(self) -> float:
         """
+
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self) -> float:
         """
+
         Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryRSS
@@ -334,70 +318,73 @@
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self) -> _ab._pd.DataFrame:
         """
+
         Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
-    def save(self, outFile) -> None:
+    def save(self, outFile: str) -> None:
         """
+
         Complete set of frequent patterns will be loaded in to an output file
 
-        :param outFile: name of the outputfile
-        :type outFile: file
+        :param outFile: name of the output file
+        :type outFile: csvfile
         :return: None
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
-            writer.write("%s \n" % s1)
+            patternsAndSupport = x.strip() + ":" + str(y)
+            writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self) -> dict:
         """
+
         Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self) -> None:
         """
-        Function to send the result after completion of the mining process
+        Function used to print the results
         """
-        print("Total number of Association Rules:", len(self.getPatterns()))
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ARWithLift(_ab._sys.argv[1], float(_ab._sys.argv[3]), _ab._sys.argv[4])
+            _ap = ECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ARWithLift(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = ECLAT(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
-        print("Total number of Association Rules:", len(_ap.getPatterns()))
+        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print(_ap.getPatternsAsDataFrame())
+        print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.5.1/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2024.5.1.1/PAMI/AssociationRules/basic/_RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/AssociationRules/basic/abstract.py` & `pami-2024.5.1.1/PAMI/AssociationRules/basic/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minConf = minConf
-        self._finalPatterns = {}
+        self._associationRules = {}
         self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
 
     @_abstractmethod
@@ -122,15 +122,15 @@
         """
         Code for the mining process will start from this function
         """
 
         pass
 
     @_abstractmethod
-    def getPatterns(self):
+    def getAssociationRules(self):
         """
         Complete set of frequent patterns generated will be retrieved from this function
         """
 
         pass
 
     @_abstractmethod
@@ -140,15 +140,15 @@
         :param oFile: Name of the output file
         :type oFile: csv file
         """
 
         pass
 
     @_abstractmethod
-    def getPatternsAsDataFrame(self):
+    def getAssociationRulesAsDataFrame(self):
         """
         Complete set of frequent patterns will be loaded in to data frame from this function
         """
 
         pass
 
     @_abstractmethod
```

### Comparing `pami-2024.5.1/PAMI/correlatedPattern/__init__.py` & `pami-2024.5.1.1/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/correlatedPattern/basic/CoMine.py` & `pami-2024.5.1.1/PAMI/correlatedPattern/basic/CoMinePlus.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-# CoMine is one of the fundamental algorithm to discover correlated patterns in a transactional database.
+# CPGrowthPlus is one of the efficient algorithm to discover Correlated patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
-# --------------------------------------------------------
+# -----------------------------------------------
 #
+#             from PAMI.correlatedPattern.basic import CoMinePlus as alg
 #
-#             from PAMI.correlatedPattern.basic import CoMine as alg
+#             iFile = 'sampleTDB.txt'
 #
-#             obj = alg.CoMine(iFile, minSup, minAllConf, sep)
+#             minSup = 0.25 # can be specified between 0 and 1
+#
+#             minAllConf = 0.2 # can  be specified between 0 and 1
+#
+#             obj = alg.CoMinePlus(iFile, minSup, minAllConf, sep)
 #
 #             obj.mine()
 #
-#             Rules = obj.getPatterns()
+#             correlatedPattern = obj.getPatterns()
 #
-#             print("Total number of  Patterns:", len(Patterns))
+#             print("Total number of correlated Patterns:", len(correlatedPattern))
 #
 #             obj.save(oFile)
 #
 #             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
@@ -28,16 +33,14 @@
 #
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
-
-
 __copyright__ = """
 Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -46,83 +49,73 @@
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
-
 """
 
 from PAMI.correlatedPattern.basic import abstract as _ab
 import pandas as _pd
-from typing import List, Dict, Tuple, Union
+from typing import List, Dict, Tuple, Set, Union, Any, Optional, Generator
 from deprecated import deprecated
 
+
 class _Node:
     """
     A class used to represent the node of correlatedPatternTree
 
+    :**Attributes**:    **itemId** (*int) -- *storing item of a node*
+                        **counter** (*int*) -- **To maintain the support of node**
+                        **parent** (*node) -- **To maintain the parent of every node**
+                        **child** (*list*) -- **To maintain the children of node**
+                        **nodeLink** (*node*) -- **Points to the node with same itemId**
 
-    :Attributes:
-
-        itemId : int
-            storing item of a node
-        counter : int
-            To maintain the support of node
-        parent : node
-            To maintain the parent of every node
-        child : list
-            To maintain the children of node
-        nodeLink : node
-            Points to the node with same itemId
-
-    :Methods:
+    :**Methods**:
 
         getChild(itemName)
             returns the node with same itemName from correlatedPatternTree
     """
 
     def __init__(self) -> None:
+
         self.itemId = -1
         self.counter = 1
         self.parent = None
         self.child = []
         self.nodeLink = None
 
-    def getChild(self, id1) -> Union[None, '_Node']:
+    def getChild(self, itemName: int) -> Union['_Node', None]:
         """
-        :param id1: give item id as input
-        :type id1: int
-        :return: the node with same itemId
-        :rtype: _Node
+        Retrieving the child from the tree
+
+        :param itemName: name of the child
+        :type itemName: list
+        :return: returns the node with same itemName from correlatedPatternTree
+        :rtype: list
         """
         for i in self.child:
-            if i.itemId == id1:
+            if i.itemId == itemName:
                 return i
         return None
 
 
 class _Tree:
     """
     A class used to represent the correlatedPatternGrowth tree structure
 
     :Attributes:
 
-        headerList : list
-            storing the list of items in tree sorted in ascending of their supports
-        mapItemNodes : dictionary
-            storing the nodes with same item name
-        mapItemLastNodes : dictionary
-            representing the map that indicates the last node for each item
-        root : Node
-            representing the root Node in a tree
+        **headerList** (*list*) -- **storing the list of items in tree sorted in ascending of their supports**
+        **mapItemNodes** (*dictionary*) -- **storing the nodes with same item name**
+        **mapItemLastNodes** (*dictionary*) -- **representing the map that indicates the last node for each item**
+        **root** (*Node*) -- **representing the root Node in a tree**
 
-
-    :Methods:
+    :**Methods**:
 
         createHeaderList(items,minSup)
             takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
             creating transaction as a branch in correlatedPatternTree
         fixNodeLinks(item,newNode)
             To create the link for nodes with same item
@@ -136,201 +129,184 @@
         self.headerList = []
         self.mapItemNodes = {}
         self.mapItemLastNodes = {}
         self.root = _Node()
 
     def addTransaction(self, transaction: List[int]) -> None:
         """
-        Adding transaction into tree
+        Adding a transaction into a tree
 
-        :param transaction : it represents a single transaction in a database
-        :type transaction : list
+        :param transaction: it represents a transaction in a database
+        :type transaction: list
         :return: None
         """
 
+        # This method taken a transaction as input and returns the tree
         current = self.root
         for i in transaction:
             child = current.getChild(i)
-            if child is None:
+            if not child:
                 newNode = _Node()
                 newNode.itemId = i
                 newNode.parent = current
                 current.child.append(newNode)
                 self.fixNodeLinks(i, newNode)
                 current = newNode
             else:
                 child.counter += 1
                 current = child
 
-    def fixNodeLinks(self, item: int, newNode: '_Node') -> None:
+    def fixNodeLinks(self, item: int, newNode: _Node) -> None:
         """
         Fixing node link for the newNode that inserted into correlatedPatternTree
 
         :param item: it represents the item of newNode
-        :type item : int
-        :param newNode : it represents the newNode that inserted in correlatedPatternTree
-        :type newNode : Node
+        :type item: int
+        :param newNode: it represents the newNode that inserted in correlatedPatternTree
+        :type newNode: Node
         :return: None
         """
         if item in self.mapItemLastNodes.keys():
             lastNode = self.mapItemLastNodes[item]
             lastNode.nodeLink = newNode
         self.mapItemLastNodes[item] = newNode
         if item not in self.mapItemNodes.keys():
             self.mapItemNodes[item] = newNode
 
-    def printTree(self, root: '_Node') -> None:
+    def printTree(self, root: _Node) -> None:
         """
-        This method is to find the details of parent, children, and support of a Node
+        Print the details of Node in correlatedPatternTree
 
         :param root: it represents the Node in correlatedPatternTree
         :type root: Node
         :return: None
         """
-
-        if root.child is None:
+        # this method is used print the details of tree
+        if not root.child:
             return
         else:
             for i in root.child:
                 print(i.itemId, i.counter, i.parent.itemId)
                 self.printTree(i)
 
     def createHeaderList(self, mapSupport: Dict[int, int], minSup: int) -> None:
         """
         To create the headerList
 
-        :param mapSupport : it represents the items with their supports
-        :type mapSupport : dictionary
-        :param minSup : it represents the minSup
-        :param minSup : float
+        :param mapSupport: it represents the items with their supports
+        :type mapSupport: dictionary
+        :param minSup: it represents the minSup
+        :type minSup: float
         :return: None
         """
-        
+        # the correlatedPatternTree always maintains the header table to start the mining from leaf nodes
         t1 = []
         for x, y in mapSupport.items():
             if y >= minSup:
                 t1.append(x)
-        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda val: val[1], reverse=True)]
         self.headerList = [i for i in t1 if i in itemSetBuffer]
 
-    def addPrefixPath(self, prefix: List['_Node'], mapSupportBeta, minSup) -> None:
+    def addPrefixPath(self, prefix: List[_Node], mapSupportBeta: Dict[int, int], minSup: int) -> None:
         """
         To construct the conditional tree with prefix paths of a node in correlatedPatternTree
 
-        :param prefix : it represents the prefix items of a Node
-        :type prefix : list
-        :param mapSupportBeta : it represents the items with their supports
-        :param mapSupportBeta : dictionary
-        :param minSup : to check the item meets with minSup
-        :param minSup : float
+        :param prefix: it represents the prefix items of a Node
+        :type prefix: list
+        :param mapSupportBeta: it represents the items with their supports
+        :type mapSupportBeta: dictionary
+        :param minSup: to check the item meets with minSup
+        :type minSup: float
         :return: None
         """
+        # this method is used to add prefix paths in conditional trees of correlatedPatternTree
         pathCount = prefix[0].counter
         current = self.root
         prefix.reverse()
         for i in range(0, len(prefix) - 1):
             pathItem = prefix[i]
             if mapSupportBeta.get(pathItem.itemId) >= minSup:
                 child = current.getChild(pathItem.itemId)
-                if child is None:
+                if not child:
                     newNode = _Node()
                     newNode.itemId = pathItem.itemId
                     newNode.parent = current
                     newNode.counter = pathCount
                     current.child.append(newNode)
                     current = newNode
                     self.fixNodeLinks(pathItem.itemId, newNode)
                 else:
                     child.counter += pathCount
                     current = child
 
 
-class CoMine(_ab._correlatedPatterns):
+class CoMinePlus(_ab._correlatedPatterns):
     """
     About this algorithm
     ====================
 
-    :Description: CoMine is one of the fundamental algorithm to discover correlated  patterns in a transactional database. It is based on the traditional FP-Growth algorithm. This algorithm uses depth-first search technique to find all correlated patterns in a transactional database.
-
-    :Reference: Lee, Y.K., Kim, W.Y., Cao, D., Han, J. (2003). CoMine: efficient mining of correlated patterns. In ICDM (pp. 581–584).
+    :**Description**:   CoMinePlus is one of the efficient algorithm to discover correlated patterns in a transactional database. Using Item Support Intervals technique which is generating correlated patterns of higher order by combining only with items that have support within specified interval.
 
-    :param  iFile: str :
-                   Name of the Input file to mine complete set of correlated patterns
-    :param  oFile: str :
-                   Name of the output file to store complete set of correlated patterns
-    :param  minSup: int or float or str :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
-    :param minAllConf: float :
-                    The user can specify minAllConf values within the range (0, 1).
-    :param  sep: str :
-                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-
-    :Attributes:
-
-        memoryUSS : float
-            To store the total amount of USS memory consumed by the program
-        memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
-        startTime:float
-            To record the start time of the mining process
-        endTime:float
-            To record the completion time of the mining process
-        minSup : int
-            The user given minSup
-        minAllConf: float
-            The user given minimum all confidence Ratio(should be in range of 0 to 1)
-        Database : list
-            To store the transactions of a database in list
-        mapSupport : Dictionary
-            To maintain the information of item and their frequency
-        lno : int
-            it represents the total no of transactions
-        tree : class
-            it represents the Tree class
-        itemSetCount : int
-            it represents the total no of patterns
-        finalPatterns : dict
-            it represents to store the patterns
-        itemSetBuffer : list
-            it represents the store the items in mining
-        maxPatternLength : int
-           it represents the constraint for pattern length
+    :**Reference**:     Uday Kiran R., Kitsuregawa M. (2012) Efficient Discovery of Correlated Patterns in Transactional Databases Using Items’ Support Intervals.
+        In: Liddle S.W., Schewe KD., Tjoa A.M., Zhou X. (eds) Database and Expert Systems Applications. DEXA 2012. Lecture Notes in Computer Science, vol 7446. Springer, Berlin, Heidelberg.
+        https://doi.org/10.1007/978-3-642-32600-4_18
+
+    :**parameters**     **iFile** (*str*) -- **Name of the Input file to mine complete set of correlated patterns**
+                        :**oFile** (*str*) -- **Name of the output file to store complete set of correlated patterns**
+                        :**minSup** (*int or float or str*) -- **The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.**
+                        :**minAllConf** (*str*) -- **Name of Neighbourhood file name**
+                        :**sep** (*str*) -- **This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.**
+
+    :**Attributes**:    **memoryUSS** (*float*) -- **To store the total amount of USS memory consumed by the program**
+                        **memoryRSS** (*float*) -- **To store the total amount of RSS memory consumed by the program**
+                        **startTime** (*float*) -- **To record the start time of the mining process**
+                        **endTime** (*float*) -- **To record the completion time of the mining process**
+                        **minSup** (*float*) -- **The user given minSup**
+                        **minAllConf** (*float*) -- **The user given minimum all confidence Ratio (should be in range of 0 to 1)**
+                        **Database** (*list*) -- **To store the transactions of a database in list**
+                        **mapSupport** (*Dictionary*) -- **To maintain the information of item and their frequency**
+                        **lno** (*int*) -- **it represents the total no of transactions**
+                        **tree** (*class*) -- **it represents the Tree class**
+                        **itemSetCount** (*int*) -- **it represents the total no of patterns**
+                        **finalPatterns** (*dict*) -- **it represents to store the patterns**
+                        **itemSetBuffer** (*list*) -- **it represents the store the items in mining**
+                        **maxPatternLength** (*int*) -- **it represents the constraint for pattern length**
 
     Execution methods
     =================
 
     **Terminal command**
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 CoMine.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
+      (.venv) $ python3 CoMinePlus.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
 
       Example Usage:
 
-      (.venv) $ python3 CoMine.py sampleTDB.txt output.txt 0.25 0.2
+      (.venv) $ python3 CoMinePlus.py sampleTDB.txt patterns.txt 0.4 0.5 ','
 
     .. note:: minSup can be specified in support count or a value between 0 and 1.
 
     **Calling from a python program**
 
     .. code-block:: python
 
-            from PAMI.correlatedPattern.basic import CoMine as alg
+            from PAMI.correlatedPattern.basic import CoMinePlus as alg
 
-            obj = alg.CoMine(iFile, minSup, minAllConf,sep)
+            obj = alg.CoMinePlus(iFile, minSup, minAllConf, sep)
 
             obj.mine()
 
-            patterns = obj.getPatterns()
+            correlatedPatterns = obj.getPatterns()
 
-            print("Total number of  Patterns:", len(patterns))
+            print("Total number of correlated patterns:", len(correlatedPatterns))
 
-            obj.savePatterns(oFile)
+            obj.save(oFile)
 
             df = obj.getPatternsAsDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
@@ -338,50 +314,52 @@
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
+
     Credits
     =======
 
              The complete program was written by B.Sai Chitra under the supervision of Professor Rage Uday Kiran.
 
-    """
+        """
 
     _startTime = float()
     _endTime = float()
-    _minSup = float()
+    _minSup = str()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
+    _minAllConf = 0.0
     _memoryUSS = float()
     _memoryRSS = float()
-    _minAllConf = 0.0
     _Database = []
     _mapSupport = {}
     _lno = 0
     _tree = str()
     _itemSetBuffer = None
     _fpNodeTempBuffer = []
     _itemSetCount = 0
     _maxPatternLength = 1000
     _sep = "\t"
 
-    def __init__(self, iFile: Union[str, _pd.DataFrame], minSup: Union[int, float, str], minAllConf: float, sep: str="\t") ->None:
+    def __init__(self, iFile: Union[str, _pd.DataFrame], minSup: Union[int, float, str], minAllConf: str, sep: str="\t") -> None:
         """
-        param iFile: give the input file
+        param iFile: input file name
         type iFile: str or DataFrame or url
-        param minSup: minimum support
-        type minSup:   int or float
-        param sep: Delimiter of input file
-        type sep: str
+        param minSup: user-specified minimum support
+        type minSup: int or float
+        param minAllConf: user-specified minimum all confidence
+        type minAllConf: float
+        param sep: delimiter of input file
+        type sep : str
         """
-
         super().__init__(iFile, minSup, minAllConf, sep)
 
     def _creatingItemSets(self) -> None:
         """
         Storing the complete transactions of the database/input file in a database variable
         """
         self._Database = []
@@ -408,128 +386,90 @@
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _getRatio(self, prefix: List[int], prefixLength: int, s: int) -> float:
-        """
-        A Function to get itemSet Ratio
-
-        :param prefix:the path
-        :type prefix: list
-        :param prefixLength: length
-        :type prefixLength:int
-        :s :current ratio
-        :type s:float
-        :return: minAllConf of prefix
-        :rtype:float
-        """
-        maximums = 0
-        for ele in range(prefixLength):
-            i = prefix[ele]
-            if maximums < self._mapSupport.get(i):
-                maximums = self._mapSupport.get(i)
-        return s / maximums
-
     def _correlatedOneItem(self) -> None:
         """
-        Generating One correlated item
+        Generating One correlated items sets
         """
         self._mapSupport = {}
         for i in self._Database:
             for j in i:
                 if j not in self._mapSupport:
                     self._mapSupport[j] = 1
                 else:
                     self._mapSupport[j] += 1
 
-    def _saveItemSet(self, prefix, prefixLength, support) -> None:
+    def _saveItemSet(self, prefix: List[_Node], prefixLength: int, support: int, ratio: float) -> None:
         """
         To save the correlated patterns mined form correlatedPatternTree
 
         :param prefix: the correlated pattern
         :type prefix: list
-        :param prefixLength : the length of a correlated pattern
-        :type prefixLength : int
+        :param prefixLength: the length of a correlated pattern
+        :type prefixLength: int
         :param support: the support of a pattern
-        :type support :  int
+        :type support:  int
+        :param ratio: float
         :return: None
-
-        The correlated patterns were stored in a global variable finalPatterns
         """
-        all_conf = self._getRatio(prefix, prefixLength, support)
-        if all_conf < self._minAllConf:
-            return
-        l = []
+
+        sample = []
         for i in range(prefixLength):
-            l.append(prefix[i])
+            sample.append(prefix[i])
         self._itemSetCount += 1
-        self._finalPatterns[tuple(l)] = [support, all_conf]
-    
-    def _convert(self, value: Union[int, float, str]) -> None:
-        """
-        To convert the type of user specified minSup value
+        self._finalPatterns[tuple(sample)] = [support, ratio]
 
-        :param value: user specified minSup value
-        :return: None
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
-
-    def _saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength) -> None:
+    def _saveAllCombinations(self, tempBuffer: List[_Node], s: int, position: int, prefix: List[_Node], prefixLength: int) -> None:
         """
         Generating all the combinations for items in single branch in correlatedPatternTree
 
         :param tempBuffer: items in a single branch
         :type tempBuffer: list
-        :param s : support at leaf node of a branch
-        :param position : the length of a tempBuffer
-        :type position : int
-        :param prefix : it represents the list of leaf node
-        :type prefix : list
-        :param prefixLength : the length of prefix
-        :type prefixLength :int
+        :param s: support at leaf node of a branch
+        :type s: int
+        :param position: the length of a tempBuffer
+        :type position: int
+        :param prefix: it represents the list of leaf node
+        :type prefix: list
+        :param prefixLength: the length of prefix
+        :type prefixLength: int
         :return: None
         """
         max1 = 1 << position
         for i in range(1, max1):
             newPrefixLength = prefixLength
             for j in range(position):
                 isSet = i & (1 << j)
                 if isSet > 0:
                     prefix.insert(newPrefixLength, tempBuffer[j].itemId)
                     newPrefixLength += 1
-            self._saveItemSet(prefix, newPrefixLength, s)
+            ratio = s/self._mapSupport[self._getMaxItem(prefix, newPrefixLength)]
+            if ratio >= self._minAllConf:
+                self._saveItemSet(prefix, newPrefixLength, s, ratio)
 
-    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree, prefix, prefixLength, mapSupport) -> None:
+    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree: _Tree, prefix: List[_Node], prefixLength: int, mapSupport: Dict[int, int], minConf: float)  -> None:
         """
         Mining the fp tree
 
         :param correlatedPatternTree: it represents the correlatedPatternTree
         :type correlatedPatternTree: class Tree
-        :param prefix : it represents an empty list and store the patterns that are mined
-        :type prefix : list
-        :param prefixLength : the length of prefix
-        :type prefixLength :int
+        :param prefix: it represents an empty list and store the patterns that are mined
+        :type prefix: list
+        :param param prefixLength: the length of prefix
+        :type prefixLength: int
         :param mapSupport : it represents the support of item
         :type mapSupport : dictionary
+        :param minConf: representing the minimum confidence
+        :type minConf: float
         :return: None
         """
-
         singlePath = True
         position = 0
         s = 0
         if len(correlatedPatternTree.root.child) > 1:
             singlePath = False
         else:
             currentNode = correlatedPatternTree.root.child[0]
@@ -545,80 +485,112 @@
                 currentNode = currentNode.child[0]
         if singlePath is True:
             self._saveAllCombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
         else:
             for i in reversed(correlatedPatternTree.headerList):
                 item = i
                 support = mapSupport[i]
+                low = max(int(_ab._math.floor(mapSupport[i]*self._minAllConf)), self._minSup)
+                high = max(int(_ab._math.floor(mapSupport[i]/minConf)), self._minSup)
                 betaSupport = support
                 prefix.insert(prefixLength, item)
-                self._saveItemSet(prefix, prefixLength + 1, betaSupport)
+                max1 = self._getMaxItem(prefix, prefixLength)
+                if self._mapSupport[max1] < self._mapSupport[item]:
+                    max1 = item
+                ratio = support / self._mapSupport[max1]
+                if ratio >= self._minAllConf:
+                    self._saveItemSet(prefix, prefixLength + 1, betaSupport, ratio)
                 if prefixLength + 1 < self._maxPatternLength:
                     prefixPaths = []
                     path = correlatedPatternTree.mapItemNodes.get(item)
                     mapSupportBeta = {}
                     while path is not None:
                         if path.parent.itemId != -1:
-                            prefixPath = []
-                            prefixPath.append(path)
+                            prefixPath = [path]
                             pathCount = path.counter
                             parent1 = path.parent
-                            while parent1.itemId != -1:
-                                prefixPath.append(parent1)
-                                if mapSupportBeta.get(parent1.itemId) is None:
-                                    mapSupportBeta[parent1.itemId] = pathCount
-                                else:
-                                    mapSupportBeta[parent1.itemId] = mapSupportBeta[parent1.itemId] + pathCount
-                                parent1 = parent1.parent
-                            prefixPaths.append(prefixPath)
+                            if mapSupport.get(parent1.itemId) >= low and mapSupport.get(parent1.itemId) <= high:
+                                while parent1.itemId != -1:
+                                    all_conf = int(support/max(mapSupport.get(parent1.itemId), support))
+                                    if mapSupport.get(parent1.itemId) >= all_conf:
+                                        prefixPath.append(parent1)
+                                        if mapSupportBeta.get(parent1.itemId) is None:
+                                            mapSupportBeta[parent1.itemId] = pathCount
+                                        else:
+                                            mapSupportBeta[parent1.itemId] = mapSupportBeta[parent1.itemId] + pathCount
+                                        parent1 = parent1.parent
+                                    else:
+                                        break
+                                prefixPaths.append(prefixPath)
                         path = path.nodeLink
                     treeBeta = _Tree()
                     for k in prefixPaths:
                         treeBeta.addPrefixPath(k, mapSupportBeta, self._minSup)
                     if len(treeBeta.root.child) > 0:
                         treeBeta.createHeaderList(mapSupportBeta, self._minSup)
-                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta)
+                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta, minConf)
+
+    def _convert(self, value: Union[int, float, str]) -> Union[int, float]:
+        """
+        To convert the type of user specified minSup value
+
+        :param value: user specified minSup value
+        :return: converted type
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
 
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
-        main method to start
+        Main program to start the operation
         """
         self.mine()
 
     def mine(self) -> None:
         """
-        main method to start
+        Main program to start the operation
         """
+
         self._startTime = _ab._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        self._minSup = self._convert(self._minSup)
-        self._tree = _Tree()
         self._finalPatterns = {}
+        self._tree = _Tree()
+        self._minSup = self._convert(self._minSup)
         self._correlatedOneItem()
         self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._minSup}
         _itemSetBuffer = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in self._Database:
             _transaction = []
             for j in i:
                 if j in _itemSetBuffer:
                     _transaction.append(j)
             _transaction.sort(key=lambda val: self._mapSupport[val], reverse=True)
             self._tree.addTransaction(_transaction)
         self._tree.createHeaderList(self._mapSupport, self._minSup)
         if len(self._tree.headerList) > 0:
             self._itemSetBuffer = []
-            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport)
-        print("Correlated patterns were generated successfully using CoMine algorithm")
+            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport, self._minAllConf)
+        print("Correlated Frequent patterns were generated successfully using CorrelatedPatternGrowth algorithm")
         self._endTime = _ab._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
+        self._memoryRSS = float()
+        self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self) -> float:
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
@@ -634,14 +606,21 @@
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryRSS
 
+    def _getMaxItem(self, prefix: List[_Node], prefixLength: int) -> int:
+        maxItem = prefix[0]
+        for i in range(prefixLength):
+            if self._mapSupport[maxItem] < self._mapSupport[prefix[i]]:
+                maxItem = prefix[i]
+        return maxItem
+
     def getRuntime(self) -> float:
         """
         Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
@@ -662,60 +641,60 @@
             pat = " "
             for i in a:
                 pat += str(i) + " "
             data.append([pat, b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
         return dataframe
 
-    def save(self, outFile) -> None:
+    def save(self, outFile: str) -> None:
         """
-        Complete set of correlated patterns will be saved into an output file
+        Complete set of correlated patterns will be loaded in to an output file
 
-        :param outFile: name of the outputfile
-        :type outFile: file
+        :param outFile: name of the output file
+        :type outFile: csv file
         :return: None
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            pat = ""
+            pattern = str()
             for i in x:
-                pat += str(i) + "\t"
-            patternsAndSupport = pat.strip() + ":" + str(y[0]) + ":" + str(y[1])
-            writer.write("%s \n" % patternsAndSupport)
+                pattern = pattern + i + "\t"
+            s1 = str(pattern.strip()) + ":" + str(y[0]) + ":" + str(y[1])
+            writer.write("%s \n" % s1)
 
-    def getPatterns(self) -> Dict[Tuple[int], List[Union[int, float]]]:
+    def getPatterns(self) -> Dict[Tuple[str], List[Union[int, float]]]:
         """
         Function to send the set of correlated patterns after completion of the mining process
 
         :return: returning correlated patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self) -> None:
         """
         function to print the result after completing the process
-
-        :return: None
         """
         print("Total number of Correlated Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
+
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
-            _ap = CoMine(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
+            _ap = CoMinePlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = CoMine(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
+            _ap = CoMinePlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
         _ap.mine()
+        _correlatedPatterns = _ap.getPatterns()
         print("Total number of Correlated-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.5.1/PAMI/correlatedPattern/basic/CoMinePlus.py` & `pami-2024.5.1.1/PAMI/correlatedPattern/basic/CoMine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-# CPGrowthPlus is one of the efficient algorithm to discover Correlated patterns in a transactional database.
+# CoMine is one of the fundamental algorithm to discover correlated patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
-# -----------------------------------------------
+# --------------------------------------------------------
 #
-#             from PAMI.correlatedPattern.basic import CoMinePlus as alg
+#             from PAMI.correlatedPattern.basic import CoMine as alg
 #
-#             obj = alg.CoMinePlus(iFile, minSup, minAllConf, sep)
+#             iFile = 'sampleTDB.txt'
+#
+#             minSup = 0.25 # can be specified between 0 and 1
+#
+#             minAllConf = 0.2 # can  be specified between 0 and 1
+#
+#             obj = alg.CoMine(iFile, minSup, minAllConf, sep)
 #
 #             obj.mine()
 #
-#             correlatedPattern = obj.getPatterns()
+#             Rules = obj.getPatterns()
 #
-#             print("Total number of correlated Patterns:", len(correlatedPattern))
+#             print("Total number of  Patterns:", len(Patterns))
 #
 #             obj.save(oFile)
 #
 #             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
@@ -27,17 +33,14 @@
 #
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
-
-
-
 __copyright__ = """
 Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -46,84 +49,66 @@
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
+
 """
 
 from PAMI.correlatedPattern.basic import abstract as _ab
 import pandas as _pd
-from typing import List, Dict, Tuple, Set, Union, Any, Optional, Generator
+from typing import List, Dict, Tuple, Union
 from deprecated import deprecated
 
-
 class _Node:
     """
     A class used to represent the node of correlatedPatternTree
 
-    :Attributes:
-
-        itemId: int
-            storing item of a node
-        counter: int
-            To maintain the support of node
-        parent: node
-            To maintain the parent of every node
-        child: list
-            To maintain the children of node
-        nodeLink : node
-            Points to the node with same itemId
-
-    :Methods:
-
-        getChild(itemName)
-            returns the node with same itemName from correlatedPatternTree
+    :**Attributes**:    **itemId** (*int*) -- **storing item of a node**
+                        **counter** (*int*) -- **To maintain the support of node**
+                        **parent** (*node*) -- **To maintain the parent of every node**
+                        **child** (*list*) -- **To maintain the children of node**
+                        **nodeLink** (*node*) -- **Points to the node with same itemId**
+
+    :**Methods**:
+            getChild(itemName)
+                returns the node with same itemName from correlatedPatternTree
     """
 
     def __init__(self) -> None:
-
         self.itemId = -1
         self.counter = 1
         self.parent = None
         self.child = []
         self.nodeLink = None
 
-    def getChild(self, itemName: int) -> Union['_Node', None]:
+    def getChild(self, id1) -> Union[None, '_Node']:
         """
-        Retrieving the child from the tree
-
-        :param itemName: name of the child
-        :type itemName: list
-        :return: returns the node with same itemName from correlatedPatternTree
-        :rtype: list
+        :param id1: give item id as input
+        :type id1: int
+        :return: the node with same itemId
+        :rtype: _Node
         """
         for i in self.child:
-            if i.itemId == itemName:
+            if i.itemId == id1:
                 return i
         return None
 
-
 class _Tree:
     """
     A class used to represent the correlatedPatternGrowth tree structure
 
-    :Attributes:
-
-        headerList : list
-            storing the list of items in tree sorted in ascending of their supports
-        mapItemNodes : dictionary
-            storing the nodes with same item name
-        mapItemLastNodes : dictionary
-            representing the map that indicates the last node for each item
-        root : Node
-            representing the root Node in a tree
+    :**Attributes**:    **headerList** (*list*) -- **storing the list of items in tree sorted in ascending of their supports**
+                        **mapItemNodes** (*dictionary*) -- **storing the nodes with same item name**
+                        **mapItemLastNodes** (*dictionary*) -- **representing the map that indicates the last node for each item**
+                        **root** (*Node*) -- **representing the root Node in a tree**
 
-    :Methods:
+    :**Methods**:
 
         createHeaderList(items,minSup)
             takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
             creating transaction as a branch in correlatedPatternTree
         fixNodeLinks(item,newNode)
             To create the link for nodes with same item
@@ -137,37 +122,36 @@
         self.headerList = []
         self.mapItemNodes = {}
         self.mapItemLastNodes = {}
         self.root = _Node()
 
     def addTransaction(self, transaction: List[int]) -> None:
         """
-        Adding a transaction into a tree
+        Adding transaction into tree
 
-        :param transaction: it represents a transaction in a database
+        :param transaction: it represents a single transaction in a database
         :type transaction: list
         :return: None
         """
 
-        # This method taken a transaction as input and returns the tree
         current = self.root
         for i in transaction:
             child = current.getChild(i)
-            if not child:
+            if child is None:
                 newNode = _Node()
                 newNode.itemId = i
                 newNode.parent = current
                 current.child.append(newNode)
                 self.fixNodeLinks(i, newNode)
                 current = newNode
             else:
                 child.counter += 1
                 current = child
 
-    def fixNodeLinks(self, item: int, newNode: _Node) -> None:
+    def fixNodeLinks(self, item: int, newNode: '_Node') -> None:
         """
         Fixing node link for the newNode that inserted into correlatedPatternTree
 
         :param item: it represents the item of newNode
         :type item: int
         :param newNode: it represents the newNode that inserted in correlatedPatternTree
         :type newNode: Node
@@ -176,169 +160,148 @@
         if item in self.mapItemLastNodes.keys():
             lastNode = self.mapItemLastNodes[item]
             lastNode.nodeLink = newNode
         self.mapItemLastNodes[item] = newNode
         if item not in self.mapItemNodes.keys():
             self.mapItemNodes[item] = newNode
 
-    def printTree(self, root: _Node) -> None:
+    def printTree(self, root: '_Node') -> None:
         """
-        Print the details of Node in correlatedPatternTree
+        This method is to find the details of parent, children, and support of a Node
 
         :param root: it represents the Node in correlatedPatternTree
         :type root: Node
         :return: None
         """
-        # this method is used print the details of tree
-        if not root.child:
+
+        if root.child is None:
             return
         else:
             for i in root.child:
                 print(i.itemId, i.counter, i.parent.itemId)
                 self.printTree(i)
 
     def createHeaderList(self, mapSupport: Dict[int, int], minSup: int) -> None:
         """
         To create the headerList
 
-        :param mapSupport: it represents the items with their supports
-        :type mapSupport: dictionary
-        :param minSup: it represents the minSup
-        :param minSup: float
+        :param mapSupport : it represents the items with their supports
+        :type mapSupport : dictionary
+        :param minSup : it represents the minSup
+        :param minSup : float
         :return: None
         """
-        # the correlatedPatternTree always maintains the header table to start the mining from leaf nodes
+        
         t1 = []
         for x, y in mapSupport.items():
             if y >= minSup:
                 t1.append(x)
-        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda val: val[1], reverse=True)]
+        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
         self.headerList = [i for i in t1 if i in itemSetBuffer]
 
-    def addPrefixPath(self, prefix: List[_Node], mapSupportBeta: Dict[int, int], minSup: int) -> None:
+    def addPrefixPath(self, prefix: List['_Node'], mapSupportBeta, minSup) -> None:
         """
         To construct the conditional tree with prefix paths of a node in correlatedPatternTree
 
-        :param prefix: it represents the prefix items of a Node
-        :type prefix: list
-        :param mapSupportBeta: it represents the items with their supports
-        :param mapSupportBeta: dictionary
-        :param minSup: to check the item meets with minSup
-        :param minSup: float
+        :param prefix : it represents the prefix items of a Node
+        :type prefix : list
+        :param mapSupportBeta : it represents the items with their supports
+        :param mapSupportBeta : dictionary
+        :param minSup : to check the item meets with minSup
+        :param minSup : float
         :return: None
         """
-        # this method is used to add prefix paths in conditional trees of correlatedPatternTree
         pathCount = prefix[0].counter
         current = self.root
         prefix.reverse()
         for i in range(0, len(prefix) - 1):
             pathItem = prefix[i]
             if mapSupportBeta.get(pathItem.itemId) >= minSup:
                 child = current.getChild(pathItem.itemId)
-                if not child:
+                if child is None:
                     newNode = _Node()
                     newNode.itemId = pathItem.itemId
                     newNode.parent = current
                     newNode.counter = pathCount
                     current.child.append(newNode)
                     current = newNode
                     self.fixNodeLinks(pathItem.itemId, newNode)
                 else:
                     child.counter += pathCount
                     current = child
 
 
-class CoMinePlus(_ab._correlatedPatterns):
+class CoMine(_ab._correlatedPatterns):
     """
     About this algorithm
     ====================
 
-    :Description: CoMinePlus is one of the efficient algorithm to discover correlated patterns in a transactional database. Using Item Support Intervals technique which is generating correlated patterns of higher order by combining only with items that have support within specified interval.
+    :**Description**: CoMine is one of the fundamental algorithm to discover correlated  patterns in a transactional database. It is based on the traditional FP-Growth algorithm. This algorithm uses depth-first search technique to find all correlated patterns in a transactional database.
+
+    :**Reference**: Lee, Y.K., Kim, W.Y., Cao, D., Han, J. (2003). CoMine: efficient mining of correlated patterns. In ICDM (pp. 581–584).
 
-    :Reference:
-        Uday Kiran R., Kitsuregawa M. (2012) Efficient Discovery of Correlated Patterns in Transactional Databases Using Items’ Support Intervals.
-        In: Liddle S.W., Schewe KD., Tjoa A.M., Zhou X. (eds) Database and Expert Systems Applications. DEXA 2012. Lecture Notes in Computer Science, vol 7446. Springer, Berlin, Heidelberg.
-        https://doi.org/10.1007/978-3-642-32600-4_18
-
-    :param  iFile: str :
-                   Name of the Input file to mine complete set of correlated patterns
-    :param  oFile: str :
-                   Name of the output file to store complete set of correlated patterns
-    :param  minSup: int or float or str :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
-    :param  minAllConf: str :
-                   Name of Neighbourhood file name
-
-    :param  sep: str :
-                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-
-
-    :Attributes:
-
-        memoryUSS : float
-            To store the total amount of USS memory consumed by the program
-        memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
-        startTime:float
-            To record the start time of the mining process
-        endTime:float
-            To record the completion time of the mining process
-        minSup : float
-            The user given minSup
-        minAllConf: float
-            The user given minimum all confidence Ratio (should be in range of 0 to 1)
-        Database : list
-            To store the transactions of a database in list
-        mapSupport : Dictionary
-            To maintain the information of item and their frequency
-        lno : int
-            it represents the total no of transactions
-        tree : class
-            it represents the Tree class
-        itemSetCount : int
-            it represents the total no of patterns
-        finalPatterns : dict
-            it represents to store the patterns
-        itemSetBuffer : list
-            it represents the store the items in mining
-        maxPatternLength : int
-           it represents the constraint for pattern length
+    :**parameters**:    **iFile** (*str*) -- **Name of the Input file to mine complete set of correlated patterns**
+                        **oFile** (*str*) -- **Name of the output file to store complete set of correlated patterns**
+                        **minSup** (*int or float or str*) -- **The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.**
+                        **minAllConf** (*float*) -- **The user can specify minAllConf values within the range (0, 1).**
+                        **sep** (*str*) -- **This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.**
+
+    :**Attributes**:    **memoryUSS** (*float*) -- **To store the total amount of USS memory consumed by the program**
+                        **memoryRSS** (*float*) -- **To store the total amount of RSS memory consumed by the program**
+                        **startTime** (*float*) -- **To record the start time of the mining process**
+                        **endTime** (*float*) -- **To record the completion time of the mining process**
+                        **minSup** (*int*) -- **The user given minSup**
+                        **minAllConf** (*float*) -- **The user given minimum all confidence Ratio(should be in range of 0 to 1)**
+                        **Database** (*list*) -- **To store the transactions of a database in list**
+                        **mapSupport** (*Dictionary*) -- **To maintain the information of item and their frequency**
+                        **lno** (*int*) -- **it represents the total no of transactions**
+                        **tree** (*class*) -- **it represents the Tree class**
+                        **itemSetCount** (*int*) -- **it represents the total no of patterns**
+                        **finalPatterns** (*dict*) -- **it represents to store the patterns**
+                        **itemSetBuffer** (*list*) -- **it represents the store the items in mining**
+                        **maxPatternLength** (*int*) -- **it represents the constraint for pattern length**
 
     Execution methods
     =================
 
     **Terminal command**
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 CoMinePlus.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
+      (.venv) $ python3 CoMine.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
 
       Example Usage:
 
-      (.venv) $ python3 CoMinePlus.py sampleTDB.txt patterns.txt 0.4 0.5 ','
+      (.venv) $ python3 CoMine.py sampleTDB.txt output.txt 0.25 0.2
 
     .. note:: minSup can be specified in support count or a value between 0 and 1.
 
     **Calling from a python program**
 
     .. code-block:: python
 
-            from PAMI.correlatedPattern.basic import CoMinePlus as alg
+            from PAMI.correlatedPattern.basic import CoMine as alg
+
+            iFile = 'sampleTDB.txt'
+
+            minSup = 0.25 # can be specified between 0 and 1
+
+            minAllConf = 0.2 # can  be specified between 0 and 1
 
-            obj = alg.CoMinePlus(iFile, minSup, minAllConf, sep)
+            obj = alg.CoMine(iFile, minSup, minAllConf,sep)
 
             obj.mine()
 
-            correlatedPatterns = obj.getPatterns()
+            patterns = obj.getPatterns()
 
-            print("Total number of correlated patterns:", len(correlatedPatterns))
+            print("Total number of  Patterns:", len(patterns))
 
-            obj.save(oFile)
+            obj.savePatterns(oFile)
 
             df = obj.getPatternsAsDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
@@ -346,53 +309,50 @@
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
-
     Credits
     =======
 
              The complete program was written by B.Sai Chitra under the supervision of Professor Rage Uday Kiran.
 
-        """
+    """
 
     _startTime = float()
     _endTime = float()
-    _minSup = str()
+    _minSup = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
-    _minAllConf = 0.0
     _memoryUSS = float()
     _memoryRSS = float()
+    _minAllConf = 0.0
     _Database = []
     _mapSupport = {}
     _lno = 0
     _tree = str()
     _itemSetBuffer = None
     _fpNodeTempBuffer = []
     _itemSetCount = 0
     _maxPatternLength = 1000
     _sep = "\t"
 
-    def __init__(self, iFile: Union[str, _pd.DataFrame], minSup: Union[int, float, str], minAllConf: str, sep: str="\t") -> None:
+    def __init__(self, iFile: Union[str, _pd.DataFrame], minSup: Union[int, float, str], minAllConf: float, sep: str="\t") ->None:
         """
-        param iFile: input file name
-
+        param iFile: give the input file
         type iFile: str or DataFrame or url
-        param minSup: user-specified minimum support
-        type minSup: int or float
-        param minAllConf: user-specified minimum all confidence
-        type minAllConf: float
-        param sep: delimiter of input file
-        type sep : str
+        param minSup: minimum support
+        type minSup:   int or float
+        param sep: Delimiter of input file
+        type sep: str
         """
+
         super().__init__(iFile, minSup, minAllConf, sep)
 
     def _creatingItemSets(self) -> None:
         """
         Storing the complete transactions of the database/input file in a database variable
         """
         self._Database = []
@@ -419,47 +379,90 @@
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
+    def _getRatio(self, prefix: List[int], prefixLength: int, s: int) -> float:
+        """
+        A Function to get itemSet Ratio
+
+        :param prefix:the path
+        :type prefix: list
+        :param prefixLength: length
+        :type prefixLength:int
+        :param s:current ratio
+        :type s:float
+        :return: minAllConf of prefix
+        :rtype: float
+        """
+        maximums = 0
+        for ele in range(prefixLength):
+            i = prefix[ele]
+            if maximums < self._mapSupport.get(i):
+                maximums = self._mapSupport.get(i)
+        return s / maximums
+
     def _correlatedOneItem(self) -> None:
         """
-        Generating One correlated items sets
+        Generating One correlated item
         """
         self._mapSupport = {}
         for i in self._Database:
             for j in i:
                 if j not in self._mapSupport:
                     self._mapSupport[j] = 1
                 else:
                     self._mapSupport[j] += 1
 
-    def _saveItemSet(self, prefix: List[_Node], prefixLength: int, support: int, ratio: float) -> None:
+    def _saveItemSet(self, prefix, prefixLength, support) -> None:
         """
         To save the correlated patterns mined form correlatedPatternTree
 
         :param prefix: the correlated pattern
         :type prefix: list
-        :param prefixLength: the length of a correlated pattern
-        :type prefixLength: int
+        :param prefixLength : the length of a correlated pattern
+        :type prefixLength : int
         :param support: the support of a pattern
-        :type support:  int
-        :param ratio: float
+        :type support :  int
         :return: None
-        """
 
-        sample = []
+        The correlated patterns were stored in a global variable finalPatterns
+        """
+        all_conf = self._getRatio(prefix, prefixLength, support)
+        if all_conf < self._minAllConf:
+            return
+        l = []
         for i in range(prefixLength):
-            sample.append(prefix[i])
+            l.append(prefix[i])
         self._itemSetCount += 1
-        self._finalPatterns[tuple(sample)] = [support, ratio]
+        self._finalPatterns[tuple(l)] = [support, all_conf]
+    
+    def _convert(self, value: Union[int, float, str]) -> None:
+        """
+        To convert the type of user specified minSup value
+
+        :param value: user specified minSup value
+        :type value: int or float or str
+        :return: None
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
 
-    def _saveAllCombinations(self, tempBuffer: List[_Node], s: int, position: int, prefix: List[_Node], prefixLength: int) -> None:
+    def _saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength) -> None:
         """
         Generating all the combinations for items in single branch in correlatedPatternTree
 
         :param tempBuffer: items in a single branch
         :type tempBuffer: list
         :param s: support at leaf node of a branch
         :param position: the length of a tempBuffer
@@ -474,34 +477,31 @@
         for i in range(1, max1):
             newPrefixLength = prefixLength
             for j in range(position):
                 isSet = i & (1 << j)
                 if isSet > 0:
                     prefix.insert(newPrefixLength, tempBuffer[j].itemId)
                     newPrefixLength += 1
-            ratio = s/self._mapSupport[self._getMaxItem(prefix, newPrefixLength)]
-            if ratio >= self._minAllConf:
-                self._saveItemSet(prefix, newPrefixLength, s, ratio)
+            self._saveItemSet(prefix, newPrefixLength, s)
 
-    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree: _Tree, prefix: List[_Node], prefixLength: int, mapSupport: Dict[int, int], minConf: float)  -> None:
+    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree, prefix, prefixLength, mapSupport) -> None:
         """
         Mining the fp tree
 
         :param correlatedPatternTree: it represents the correlatedPatternTree
         :type correlatedPatternTree: class Tree
         :param prefix: it represents an empty list and store the patterns that are mined
         :type prefix: list
-        :param param prefixLength: the length of prefix
+        :param prefixLength: the length of prefix
         :type prefixLength: int
-        :param mapSupport : it represents the support of item
-        :type mapSupport : dictionary
-        :param minConf: representing the minimum confidence
-        :type minConf: float
+        :param mapSupport: it represents the support of item
+        :type mapSupport: dictionary
         :return: None
         """
+
         singlePath = True
         position = 0
         s = 0
         if len(correlatedPatternTree.root.child) > 1:
             singlePath = False
         else:
             currentNode = correlatedPatternTree.root.child[0]
@@ -517,112 +517,80 @@
                 currentNode = currentNode.child[0]
         if singlePath is True:
             self._saveAllCombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
         else:
             for i in reversed(correlatedPatternTree.headerList):
                 item = i
                 support = mapSupport[i]
-                low = max(int(_ab._math.floor(mapSupport[i]*self._minAllConf)), self._minSup)
-                high = max(int(_ab._math.floor(mapSupport[i]/minConf)), self._minSup)
                 betaSupport = support
                 prefix.insert(prefixLength, item)
-                max1 = self._getMaxItem(prefix, prefixLength)
-                if self._mapSupport[max1] < self._mapSupport[item]:
-                    max1 = item
-                ratio = support / self._mapSupport[max1]
-                if ratio >= self._minAllConf:
-                    self._saveItemSet(prefix, prefixLength + 1, betaSupport, ratio)
+                self._saveItemSet(prefix, prefixLength + 1, betaSupport)
                 if prefixLength + 1 < self._maxPatternLength:
                     prefixPaths = []
                     path = correlatedPatternTree.mapItemNodes.get(item)
                     mapSupportBeta = {}
                     while path is not None:
                         if path.parent.itemId != -1:
-                            prefixPath = [path]
+                            prefixPath = []
+                            prefixPath.append(path)
                             pathCount = path.counter
                             parent1 = path.parent
-                            if mapSupport.get(parent1.itemId) >= low and mapSupport.get(parent1.itemId) <= high:
-                                while parent1.itemId != -1:
-                                    all_conf = int(support/max(mapSupport.get(parent1.itemId), support))
-                                    if mapSupport.get(parent1.itemId) >= all_conf:
-                                        prefixPath.append(parent1)
-                                        if mapSupportBeta.get(parent1.itemId) is None:
-                                            mapSupportBeta[parent1.itemId] = pathCount
-                                        else:
-                                            mapSupportBeta[parent1.itemId] = mapSupportBeta[parent1.itemId] + pathCount
-                                        parent1 = parent1.parent
-                                    else:
-                                        break
-                                prefixPaths.append(prefixPath)
+                            while parent1.itemId != -1:
+                                prefixPath.append(parent1)
+                                if mapSupportBeta.get(parent1.itemId) is None:
+                                    mapSupportBeta[parent1.itemId] = pathCount
+                                else:
+                                    mapSupportBeta[parent1.itemId] = mapSupportBeta[parent1.itemId] + pathCount
+                                parent1 = parent1.parent
+                            prefixPaths.append(prefixPath)
                         path = path.nodeLink
                     treeBeta = _Tree()
                     for k in prefixPaths:
                         treeBeta.addPrefixPath(k, mapSupportBeta, self._minSup)
                     if len(treeBeta.root.child) > 0:
                         treeBeta.createHeaderList(mapSupportBeta, self._minSup)
-                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta, minConf)
-
-    def _convert(self, value: Union[int, float, str]) -> Union[int, float]:
-        """
-        To convert the type of user specified minSup value
-
-        :param value: user specified minSup value
-        :return: converted type
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
+                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta)
 
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
-        Main program to start the operation
+        main method to start
         """
         self.mine()
 
     def mine(self) -> None:
         """
-        Main program to start the operation
+        main method to start
         """
-
         self._startTime = _ab._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
-            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        self._finalPatterns = {}
-        self._tree = _Tree()
         self._minSup = self._convert(self._minSup)
+        self._tree = _Tree()
+        self._finalPatterns = {}
         self._correlatedOneItem()
         self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._minSup}
         _itemSetBuffer = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in self._Database:
             _transaction = []
             for j in i:
                 if j in _itemSetBuffer:
                     _transaction.append(j)
             _transaction.sort(key=lambda val: self._mapSupport[val], reverse=True)
             self._tree.addTransaction(_transaction)
         self._tree.createHeaderList(self._mapSupport, self._minSup)
         if len(self._tree.headerList) > 0:
             self._itemSetBuffer = []
-            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport, self._minAllConf)
-        print("Correlated Frequent patterns were generated successfully using CorrelatedPatternGrowth algorithm")
+            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport)
+        print("Correlated patterns were generated successfully using CoMine algorithm")
         self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryRSS = float()
         self._memoryUSS = float()
+        self._memoryRSS = float()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self) -> float:
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
@@ -638,21 +606,14 @@
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryRSS
 
-    def _getMaxItem(self, prefix: List[_Node], prefixLength: int) -> int:
-        maxItem = prefix[0]
-        for i in range(prefixLength):
-            if self._mapSupport[maxItem] < self._mapSupport[prefix[i]]:
-                maxItem = prefix[i]
-        return maxItem
-
     def getRuntime(self) -> float:
         """
         Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
@@ -673,60 +634,60 @@
             pat = " "
             for i in a:
                 pat += str(i) + " "
             data.append([pat, b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
         return dataframe
 
-    def save(self, outFile: str) -> None:
+    def save(self, outFile) -> None:
         """
-        Complete set of correlated patterns will be loaded in to an output file
+        Complete set of correlated patterns will be saved into an output file
 
-        :param outFile: name of the output file
-        :type outFile: csv file
+        :param outFile: name of the outputfile
+        :type outFile: file
         :return: None
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            pattern = str()
+            pat = ""
             for i in x:
-                pattern = pattern + i + "\t"
-            s1 = str(pattern.strip()) + ":" + str(y[0]) + ":" + str(y[1])
-            writer.write("%s \n" % s1)
+                pat += str(i) + "\t"
+            patternsAndSupport = pat.strip() + ":" + str(y[0]) + ":" + str(y[1])
+            writer.write("%s \n" % patternsAndSupport)
 
-    def getPatterns(self) -> Dict[Tuple[str], List[Union[int, float]]]:
+    def getPatterns(self) -> Dict[Tuple[int], List[Union[int, float]]]:
         """
         Function to send the set of correlated patterns after completion of the mining process
 
         :return: returning correlated patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self) -> None:
         """
         function to print the result after completing the process
+
+        :return: None
         """
         print("Total number of Correlated Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
-
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
-            _ap = CoMinePlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
+            _ap = CoMine(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = CoMinePlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
+            _ap = CoMine(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
         _ap.mine()
-        _correlatedPatterns = _ap.getPatterns()
         print("Total number of Correlated-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.5.1/PAMI/correlatedPattern/basic/__init__.py` & `pami-2024.5.1.1/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/correlatedPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/coveragePattern/basic/CMine.py` & `pami-2024.5.1.1/PAMI/coveragePattern/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/coveragePattern/basic/CPPG.py` & `pami-2024.5.1.1/PAMI/coveragePattern/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/coveragePattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/coveragePattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/DF2DB/DF2DB.py` & `pami-2024.5.1.1/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2024.5.1.1/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/DF2DB/DenseFormatDF.py` & `pami-2024.5.1.1/PAMI/extras/DF2DB/DenseFormatDF.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/DF2DB/SparseFormatDF.py` & `pami-2024.5.1.1/PAMI/extras/DF2DB/SparseFormatDF.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/DF2DB/createTDB.py` & `pami-2024.5.1.1/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2024.5.1.1/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2024.5.1.1/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2024.5.1.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2024.5.1.1/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2024.5.1.1/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/convertMultiTSIntoFuzzy.py` & `pami-2024.5.1.1/PAMI/extras/convertMultiTSIntoFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/dbStats/FuzzyDatabase.py` & `pami-2024.5.1.1/PAMI/extras/dbStats/FuzzyDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py` & `pami-2024.5.1.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/dbStats/SequentialDatabase.py` & `pami-2024.5.1.1/PAMI/extras/dbStats/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/dbStats/TemporalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/dbStats/TemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/dbStats/TransactionalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/dbStats/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/dbStats/UtilityDatabase.py` & `pami-2024.5.1.1/PAMI/extras/dbStats/UtilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py` & `pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2024.5.1.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/generateLatexGraphFile.py` & `pami-2024.5.1.1/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/graph/DF2Fig.py` & `pami-2024.5.1.1/PAMI/extras/graph/DF2Fig.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/graph/DF2Tex.py` & `pami-2024.5.1.1/PAMI/extras/graph/DF2Tex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2024.5.1.1/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2024.5.1.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/graph/visualizeFuzzyPatterns.py` & `pami-2024.5.1.1/PAMI/extras/graph/visualizeFuzzyPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/graph/visualizePatterns.py` & `pami-2024.5.1.1/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2024.5.1.1/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/messaging/discord.py` & `pami-2024.5.1.1/PAMI/extras/messaging/discord.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/messaging/gmail.py` & `pami-2024.5.1.1/PAMI/extras/messaging/gmail.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py` & `pami-2024.5.1.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2024.5.1.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py` & `pami-2024.5.1.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/plotPointOnMap.py` & `pami-2024.5.1.1/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/plotPointOnMap_dump.py` & `pami-2024.5.1.1/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2024.5.1.1/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/stats/TransactionalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/stats/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/stats/graphDatabase.py` & `pami-2024.5.1.1/PAMI/extras/stats/graphDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/stats/sequentialDatabase.py` & `pami-2024.5.1.1/PAMI/extras/stats/sequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/stats/temporalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/stats/temporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/stats/utilityDatabase.py` & `pami-2024.5.1.1/PAMI/extras/stats/utilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py` & `pami-2024.5.1.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/topKPatterns.py` & `pami-2024.5.1.1/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/uncertaindb_convert.py` & `pami-2024.5.1.1/PAMI/extras/uncertaindb_convert.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/extras/visualize/graphs.py` & `pami-2024.5.1.1/PAMI/extras/visualize/graphs.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/__init__.py` & `pami-2024.5.1.1/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/basic/Apriori.py` & `pami-2024.5.1.1/PAMI/frequentPattern/basic/Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/basic/Aprioribitset.py` & `pami-2024.5.1.1/PAMI/frequentPattern/basic/Aprioribitset.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2024.5.1.1/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+# ECLATbitset is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
 #
-#             import PAMI.frequentPattern.basic.ECLAT as alg
+#             import PAMI.frequentPattern.basic.ECLATbitset as alg
 #
 #             iFile = 'sampleDB.txt'
 #
 #             minSup = 10  # can also be specified between 0 and 1
 #
-#             obj = alg.ECLAT(iFile, minSup)
+#             obj = alg.ECLATbitset(iFile, minSup)
 #
 #             obj.mine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -50,65 +50,61 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 from PAMI.frequentPattern.basic import abstract as _ab
 from deprecated import deprecated
 
-class ECLAT(_ab._frequentPatterns):
-    """
-    About this algorithm
-    ====================
 
-    :**Description**: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+class ECLATbitset(_ab._frequentPatterns):
+    """
+    :*Description*:  ECLATbitset is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 
-    :**Reference**:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
-            372-390 (2000), https://ieeexplore.ieee.org/document/846291
+    :*Reference*:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
+                   372-390 (2000), https://ieeexplore.ieee.org/document/846291
 
     :**Parameters**:    - **iFile** (*str or URL or dataFrame*) -- *Name of the Input file to mine complete set of frequent patterns.*
-                        - **oFile** (*str*) -- *Name of the output file to store complete set of frequent patterns.*
-                        - **minSup** (*int or float or str*) -- *The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.*
-                        - **sep** (*str*) -- *This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.*
+                        - **oFile** (*str*) -- *Name of the output file to store complete set of frequent patterns*
+                        - **minSup** (*int or float or str*) -- *The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.*
+                        - **sep** (*str*) -- **This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.**
 
     :**Attributes**:    - **startTime** (*float*) -- *To record the start time of the mining process.*
-                        - **endTime** (*float*) -- *To record the completion time of the mining process.*
+                        - **endTime** (*float*) -- *To record the end time of the mining process.*
                         - **finalPatterns** (*dict*) -- *Storing the complete set of patterns in a dictionary variable.*
                         - **memoryUSS** (*float*) -- *To store the total amount of USS memory consumed by the program.*
-                        - **memoryRSS** (*float*) -- *To store the total amount of RSS memory consumed by the program.*
+                        - **memoryRSS** *(float*) -- *To store the total amount of RSS memory consumed by the program.*
                         - **Database** (*list*) -- *To store the transactions of a database in list.*
 
     Execution methods
     =================
 
     **Terminal command**
 
-    .. code-block:: console
-
       Format:
 
-      (.venv) $ python3 ECLAT.py <inputFile> <outputFile> <minSup>
+      (.venv) $ python3 ECLATbitset.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 ECLAT.py sampleDB.txt patterns.txt 10.0
+      (.venv) $ python3 ECLATbitset.py sampleDB.txt patterns.txt 10.0
 
     .. note:: minSup can be specified  in support count or a value between 0 and 1.
 
 
     **Calling from a python program**
 
     .. code-block:: python
 
-            import PAMI.frequentPattern.basic.ECLAT as alg
+            import PAMI.frequentPattern.basic.ECLATbitset as alg
 
             iFile = 'sampleDB.txt'
 
             minSup = 10  # can also be specified between 0 and 1
 
-            obj = alg.ECLAT(iFile, minSup)
+            obj = alg.ECLATbitset(iFile, minSup)
 
             obj.mine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
@@ -124,265 +120,268 @@
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
-
     Credits:
     ========
 
-    The complete program was written by Kundai and revised by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
+    The complete program was written by Yudai Masu and revised by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
-    _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
+    _minSup = str()
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
+    _mapSupport = {}
+    _lno = 0
 
-    def _creatingItemSets(self) -> float:
+    def _convert(self, value):
         """
 
-        Storing the complete transactions of the database/input file in a database variable
+        To convert the user specified minSup value
 
-        :return: the complete transactions of the database/input file in a database variable
-        :rtype: float
+        :param value: user specified minSup value
+        :type value: int
+        :return: converted type
+        :rtype: int or float or string
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
+
+    def _creatingItemSets(self):
+        """
+        Storing the complete transactions of the database/input file in a database variable
         """
         self._Database = []
+        self._mapSupport = {}
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
+
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
                     self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
-                            temp = [i.rstrip() for i in line.split(self._sep)]
-                            temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            self._lno += 1
+                            splitter = [i.rstrip() for i in line.split(self._sep)]
+                            splitter = [x for x in splitter if x]
+                            self._Database.append(splitter)
                 except IOError:
                     print("File Not Found")
-                    quit()
-
-    def _convert(self, value) -> float:
-        """
-
-        To convert the user specified minSup value
-
-        :param value: user specified minSup value
-        :return: converted type
-        :rtype: float
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
+        self._minSup = self._convert(self._minSup)
 
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
-    def startMine(self) -> None:
+    def startMine(self):
         """
         Frequent pattern mining process will start from here
-        """
 
+        We start with the scanning the itemSets and store the bitsets respectively.
+        We form the combinations of single items and  check with minSup condition to check the frequency of patterns
+        """
         self.mine()
 
-    def __recursive(self, items, cands):
+    def _bitPacker(self, data, maxIndex):
         """
 
-        This function generates new candidates by taking input as original candidates.
+        It takes the data and maxIndex as input and generates integer as output value.
 
-        :param items: A dictionary containing items and their corresponding support values.
-        :type items: dict
-        :param cands: A list of candidate itemsets.
-        :type cands: list
-        :return: None
+        :param data: it takes data as input.
+        :type data: int or float
+        :param maxIndex: It converts the data into bits By taking the maxIndex value as condition.
+        :type maxIndex: int
         """
+        packed_bits = 0
+        for i in data:
+            packed_bits |= 1 << (maxIndex - i)
 
-        for i in range(len(cands)):
-            newCands = []
-            for j in range(i + 1, len(cands)):
-                intersection = items[cands[i]].intersection(items[cands[j]])
-                if len(intersection) >= self._minSup:
-                    newCand = tuple(cands[i] + tuple([cands[j][-1]]))
-                    newCands.append(newCand)
-                    items[newCand] = intersection
-                    self._finalPatterns[newCand] = len(intersection)
-            if len(newCands) > 1:
-                self.__recursive(items, newCands)
+        return packed_bits
 
     def mine(self) -> None:
         """
         Frequent pattern mining process will start from here
+        # Bitset implementation
         """
-
         self._startTime = _ab._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
-            raise Exception("Please enter the Minimum Support")
-        self._creatingItemSets()
 
-        self._minSup = self._convert(self._minSup)
+        self._Database = []
+
+        self._creatingItemSets()
 
-    
         items = {}
         index = 0
         for line in self._Database:
             for item in line:
-                if item not in items:
-                    items[item] = []
-                items[item].append(index)
+                if tuple([item]) in items:
+                    items[tuple([item])].append(index)
+                else:
+                    items[tuple([item])] = [index]
             index += 1
-        
-        items = {tuple([k]): set(v) for k, v in items.items() if len(v) >= self._minSup}
-        items = {k: v for k, v in sorted(items.items(), key=lambda item: len(item[1]), reverse=False)}
-        for k, v in items.items():
-            self._finalPatterns[k] = len(v)
 
-        cands = list(items.keys())
+        # sort by length in descending order
+        items = dict(sorted(items.items(), key=lambda x: len(x[1]), reverse=True))
+        cands = []
+        for key in items:
+            if len(items[key]) >= self._minSup:
+                self._finalPatterns["\t".join(key)] = len(items[key])
+                cands.append(key)
+                items[key] = self._bitPacker(items[key], index)
+                # print(key, items[key])
+            else:
+                break
 
-        self.__recursive(items, cands)
+        while cands:
+            newCands = []
+            for i in range(len(cands)):
+                for j in range(i + 1, len(cands)):
+                    if cands[i][:-1] == cands[j][:-1]:
+                        newCand = tuple(cands[i] + tuple([cands[j][-1]]))
+                        intersection = items[tuple([newCand[0]])]
+                        for k in range(1, len(newCand)):
+                            intersection &= items[tuple([newCand[k]])]
+                        count = int.bit_count(intersection)
+                        if count >= self._minSup:
+                            newCands.append(newCand)
+                            newCand = "\t".join(newCand)
+                            self._finalPatterns[newCand] = count
+                    else:
+                        break
 
+            cands = newCands
 
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using ECLAT algorithm")
+        print("Frequent patterns were generated successfully using Apriori algorithm ")
 
-    def getMemoryUSS(self) -> float:
+    def getMemoryUSS(self):
         """
 
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
-    def getMemoryRSS(self) -> float:
+    def getMemoryRSS(self):
         """
 
         Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryRSS
 
-    def getRuntime(self) -> float:
+    def getRuntime(self):
         """
+
         Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> _ab._pd.DataFrame:
+    def getPatternsAsDataFrame(self):
         """
 
         Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
-        # time = _ab._time.time()
-        # dataFrame = {}
-        # data = []
-        # for a, b in self._finalPatterns.items():
-        #     # data.append([a.replace('\t', ' '), b])
-        #     data.append([" ".join(a), b])
-        #     dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # print("Time taken to convert the frequent patterns into DataFrame is: ", _ab._time.time() - time)
-
-
-        dataFrame = _ab._pd.DataFrame(list(self._finalPatterns.items()), columns=['Patterns', 'Support'])
-
+        dataFrame = {}
+        data = []
+        for a, b in self._finalPatterns.items():
+            data.append([a.replace('\t', ' '), b])
+            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
-    def save(self, outFile: str) -> None:
+    def save(self, outFile):
         """
 
         Complete set of frequent patterns will be loaded in to an output file
 
-        :param outFile: name of the output file
-        :type outFile: csvfile
-        :return: None
-        """
-        with open(outFile, 'w') as f:
-            for x, y in self._finalPatterns.items():
-                x = self._sep.join(x)
-                f.write(f"{x} : {y}\n")
+        :param outFile: name of the outputfile
+        :type outFile: file
+        """
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
+        for x, y in self._finalPatterns.items():
+            patternsAndSupport = x.strip() + ":" + str(y)
+            writer.write("%s \n" % patternsAndSupport)
 
-    def getPatterns(self) -> dict:
+    def getPatterns(self):
         """
+
         Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self) -> None:
+    def printResults(self):
         """
-        Function used to print the results
+        This function is used to print the result
         """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
+        print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = ECLATbitset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ECLAT(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = ECLATbitset(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        print(_ap.getPatternsAsDataFrame())
-        print("Total Memory in USS:",  _ap.getMemoryUSS())
+        print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
-
-        
-
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.5.1/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2024.5.1.1/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# ECLATDiffest uses diffset to extract the frequent patterns in a transactional database.
-
+# cuApriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+#
+#
 # **Importing this algorithm into a python program**
-# ---------------------------------------------------------
+# ----------------------------------------------------
 #
-#             import PAMI.frequentPattern.basic.ECLATDiffset as alg
+#             import PAMI.frequentPattern.cuda.cuApriori as alg
 #
-#             obj = alg.ECLATDiffset(iFile, minSup)
+#             obj = alg.cuApriori(iFile, minSup)
 #
 #             obj.mine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#             obj.savePatterns(oFile)
+#             obj.save(oFile)
 #
 #             Df = obj.getPatternInDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
@@ -29,16 +30,14 @@
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
 
-
-
 __copyright__ = """
 Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -48,269 +47,266 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-
-# from abstract import *
-
-from PAMI.frequentPattern.basic import abstract as _ab
 from deprecated import deprecated
+from PAMI.frequentPattern.cuda import abstract as _ab
+# import abstract as _ab
 
-
-class ECLATDiffset(_ab._frequentPatterns):
+class cuApriori(_ab._frequentPatterns):
     """
-    :Description:   ECLATDiffset uses diffset to extract the frequent patterns in a transactional database.
+    :Description: cuApriori is one of the fundamental algorithm to discover frequent patterns using Cuda in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+
+    :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
+            In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
 
-    :Reference:  KDD '03: Proceedings of the ninth ACM SIGKDD international conference on Knowledge discovery and data mining
-            August 2003 Pages 326–335 https://doi.org/10.1145/956750.956788
-            
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent pattern's
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
-    :param  minSup: int or float or str :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+    :param  minSup: int :
+                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-    
+
     :Attributes:
-    
+
         startTime : float
           To record the start time of the mining process
 
         endTime : float
           To record the completion time of the mining process
 
         finalPatterns : dict
           Storing the complete set of patterns in a dictionary variable
 
         memoryUSS : float
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
-        
+
         Database : list
           To store the transactions of a database in list
-          
-        
+
+
+
     **Methods to execute code on terminal**
-    ------------------------------------------
+    ----------------------------------------------------
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 ECLATDiffset.py <inputFile> <outputFile> <minSup>
+      (.venv) $ python3 cuApriori.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 ECLATDiffset.py sampleDB.txt patterns.txt 10.0
+      (.venv) $ python3 cuApriori.py sampleDB.txt patterns.txt 10.0
 
     .. note:: minSup will be considered in percentage of database transactions
 
-    
+
     **Importing this algorithm into a python program**
-    ---------------------------------------------------------
+    ----------------------------------------------------
+
     .. code-block:: python
 
-            import PAMI.frequentPattern.basic.ECLATDiffset as alg
+             import PAMI.frequentPattern.cuda.cuApriori as alg
 
-            obj = alg.ECLATDiffset(iFile, minSup)
+             obj = alg.cuApriori(iFile, minSup)
 
-            obj.mine()
+             obj.mine()
 
-            frequentPatterns = obj.getPatterns()
+             frequentPatterns = obj.getPatterns()
 
-            print("Total number of Frequent Patterns:", len(frequentPatterns))
+             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.savePatterns(oFile)
+             obj.save(oFile)
 
-            Df = obj.getPatternInDataFrame()
+             Df = obj.getPatternInDataFrame()
 
-            memUSS = obj.getMemoryUSS()
+             memUSS = obj.getMemoryUSS()
 
-            print("Total Memory in USS:", memUSS)
+             print("Total Memory in USS:", memUSS)
 
-            memRSS = obj.getMemoryRSS()
+             memRSS = obj.getMemoryRSS()
 
-            print("Total Memory in RSS", memRSS)
+             print("Total Memory in RSS", memRSS)
 
-            run = obj.getRuntime()
+             run = obj.getRuntime()
 
-            print("Total ExecutionTime in seconds:", run)
+             print("Total ExecutionTime in seconds:", run)
 
 
     **Credits:**
-    -------------------
+    -------------
 
-               The complete program was written by Kundai under the supervision of Professor Rage Uday Kiran.
+             The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
+    _ab._cp.cuda.Device(0).use()
+
     _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _diffSets = {}
-    _trans_set = set()
+
+    _sumKernel = _ab._cp.RawKernel(r'''
+
+    #define uint32_t unsigned int
+
+    extern "C" __global__
+
+    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
+    {
+        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
+        if (i < numElements)
+        {  
+            atomicAdd(&sum[0], __popc(d_a[i]));
+        }
+        return;    
+    }
+
+    ''', 'sumKernel')
 
     def _creatingItemSets(self):
         """
         Storing the complete transactions of the database/input file in a database variable
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
+            temp = []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
+                temp = self._iFile['Transactions'].tolist()
+
+            for k in temp:
+                self._Database.append(set(k))
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._Database.append(temp)
+                    self._Database.append(set(temp))
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            self._Database.append(set(temp))
                 except IOError:
                     print("File Not Found")
                     quit()
 
     def _convert(self, value):
         """
+
         To convert the user specified minSup value
+
         :param value: user specified minSup value
+
+        :type value: int or float or str
+
         :return: converted type
+
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
-    def _getUniqueItemList(self):
+    def arraysAndItems(self):
+        ArraysAndItems = {}
 
-        # tidSets will store all the initial tids
-        tidSets = {}
-        # uniqueItem will store all frequent 1 items
-        uniqueItem = []
-        for line in self._Database:
-                transNum = 0
-                # Database = [set([i.rstrip() for i in transaction.split('\t')]) for transaction in f]
-                for transaction in self._Database:
-                    transNum += 1
-                    self._trans_set.add(transNum)
-                    for item in transaction:
-                        if item in tidSets:
-                            tidSets[item].add(transNum)
-                        else:
-                            tidSets[item] = {transNum}
-        for key, value in tidSets.items():
-            supp = len(value)
-            if supp >= self._minSup:
-                self._diffSets[key] = [supp, self._trans_set.difference(value)]
-                uniqueItem.append(key)
-        # for x, y in self._diffSets.items():
-        #     print(x, y)
-        uniqueItem.sort()
-        # print()
-        return uniqueItem
-
-    def _runDeclat(self, candidateList):
-        """
-        It will generate the combinations of frequent items
-        :param candidateList :it represents the items with their respective transaction identifiers
-        :type candidateList: list
-        :return: returning transaction dictionary
-        :rtype: dict
-        """
+        for i in range(len(self._Database)):
+            for j in self._Database[i]:
+                j = tuple([j])
+                if j not in ArraysAndItems:
+                    ArraysAndItems[j] = [i]
+                else:
+                    ArraysAndItems[j].append(i)
+
+        newArraysAndItems = {}
+
+        for k, v in ArraysAndItems.items():
+            ArraysAndItems[k] = _ab._cp.array(v, dtype=_ab._np.uint32)
+            if len(v) >= self._minSup:
+                self._finalPatterns[k] = len(v)
+                newArraysAndItems[k] = ArraysAndItems[k]
 
-        newList = []
-        for i in range(0, len(candidateList)):
-            item1 = candidateList[i]
-            iList = item1.split()
-            for j in range(i + 1, len(candidateList)):
-                item2 = candidateList[j]
-                jList = item2.split()
-                if iList[:-1] == jList[:-1]:
-                    unionDiffSet = self._diffSets[item2][1].difference(self._diffSets[item1][1])
-                    unionSup = self._diffSets[item1][0] - len(unionDiffSet)
-                    if unionSup >= self._minSup:
-                        newKey = item1 + "\t" + jList[-1]
-                        self._diffSets[newKey] = [unionSup, unionDiffSet]
-                        newList.append(newKey)
-                    else: 
-                        break
-
-        if len(newList) > 0:
-            self._runDeclat(newList)
+        return newArraysAndItems
 
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self):
         """
         Frequent pattern mining process will start from here
         """
-
         self.mine()
 
     def mine(self):
         """
         Frequent pattern mining process will start from here
         """
-
-        self._startTime = _ab._time.time()
         self._Database = []
-        self._finalPatterns = {}
-        self._diffSets = {}
-        self._trans_set = set()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
-            raise Exception("Please enter the Minimum Support")
+        self._startTime = _ab._time.time()
         self._creatingItemSets()
-        #print(len(self._Database))
         self._minSup = self._convert(self._minSup)
-        uniqueItemList = []
-        uniqueItemList = self._getUniqueItemList()
-        self._runDeclat(uniqueItemList)
-        self._finalPatterns = self._diffSets
-        #print(len(self._finalPatterns), len(uniqueItemList))
+
+        ArraysAndItems = self.arraysAndItems()
+
+        while len(ArraysAndItems) > 0:
+            # print("Total number of ArraysAndItems:", len(ArraysAndItems))
+            newArraysAndItems = {}
+            keys = list(ArraysAndItems.keys())
+            for i in range(len(ArraysAndItems)):
+                # print(i, "/", len(ArraysAndItems), end="\r")
+                iList = list(keys[i])
+                for j in range(i + 1, len(ArraysAndItems)):
+                    jList = list(keys[j])
+                    union = tuple(sorted(set(iList + jList)))
+                    intersect = _ab._cp.intersect1d(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]],
+                                                    assume_unique=True)
+                    if len(intersect) >= self._minSup and union not in self._finalPatterns:
+                        newArraysAndItems[union] = intersect
+                        self._finalPatterns[union] = len(intersect)
+            ArraysAndItems = newArraysAndItems
+            # print()
+
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using ECLAT Diffset algorithm")
+        print("Frequent patterns were generated successfully using cuApriori algorithm ")
 
     def getMemoryUSS(self):
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
@@ -341,59 +337,61 @@
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b[0]])
+            data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
         """
         Complete set of frequent patterns will be loaded in to an output file
         :param outFile: name of the output file
         :type outFile: csvfile
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y[0])
-            writer.write("%s \n" % patternsAndSupport)
+            s1 = x.strip() + ":" + str(y)
+            writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """
         Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
         """
-        This function is used to print the results
+        This function is used to print results
         """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
-
+        print("Total ExecutionTime in s:", self.getRuntime())
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        print(_ap.getPatternsAsDataFrame())
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
+        print("Total ExecutionTime in s:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
+
+
+
```

### Comparing `pami-2024.5.1/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2024.5.1.1/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# ECLATbitset is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+# ECLATDiffest uses diffset to extract the frequent patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
 #
-#             import PAMI.frequentPattern.basic.ECLATbitset as alg
+#             import PAMI.frequentPattern.basic.ECLATDiffset as alg
 #
 #             iFile = 'sampleDB.txt'
 #
 #             minSup = 10  # can also be specified between 0 and 1
 #
-#             obj = alg.ECLATbitset(iFile, minSup)
+#             obj = alg.ECLATDiffset(iFile, minSup)
 #
 #             obj.mine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#             obj.save(oFile)
+#             obj.savePatterns(oFile)
 #
 #             Df = obj.getPatternInDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
@@ -47,77 +47,78 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+
+# from abstract import *
+
 from PAMI.frequentPattern.basic import abstract as _ab
 from deprecated import deprecated
 
 
-class ECLATbitset(_ab._frequentPatterns):
+class ECLATDiffset(_ab._frequentPatterns):
     """
-    About this algorithm
-    ====================
-
-    :*Description*:  ECLATbitset is one of the fundamental algorithm to discover frequent patterns in a transactional database.
-
-    :*Reference*:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
-            372-390 (2000), https://ieeexplore.ieee.org/document/846291
+    :**Description**:   ECLATDiffset uses diffset to extract the frequent patterns in a transactional database.
 
+    :**Reference**:  KDD '03: Proceedings of the ninth ACM SIGKDD international conference on Knowledge discovery and data mining
+                     August 2003 Pages 326–335 https://doi.org/10.1145/956750.956788
+            
     :**Parameters**:    - **iFile** (*str or URL or dataFrame*) -- *Name of the Input file to mine complete set of frequent patterns.*
-                        - **oFile** (*str*) -- *Name of the output file to store complete set of frequent patterns.*
-                        - **minSup** (*int or float or str*) -- *The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.*
-                        - **sep** (*str*) -- *This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.*
+                        - **oFile** (*str*) -- *Name of the output file to store complete set of frequent patterns*
+                        - **minSup** (*int or float or str*) -- *The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.*
+                        - **sep** (*str*) -- **This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.**
 
     :**Attributes**:    - **startTime** (*float*) -- *To record the start time of the mining process.*
-                        - **endTime** (*float*) -- *To record the completion time of the mining process.*
+                        - **endTime** (*float*) -- *To record the end time of the mining process.*
                         - **finalPatterns** (*dict*) -- *Storing the complete set of patterns in a dictionary variable.*
                         - **memoryUSS** (*float*) -- *To store the total amount of USS memory consumed by the program.*
-                        - **memoryRSS** (*float*) -- *To store the total amount of RSS memory consumed by the program.*
+                        - **memoryRSS** *(float*) -- *To store the total amount of RSS memory consumed by the program.*
                         - **Database** (*list*) -- *To store the transactions of a database in list.*
-
+          
+        
     Execution methods
     =================
 
     **Terminal command**
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 ECLATbitset.py <inputFile> <outputFile> <minSup>
+      (.venv) $ python3 ECLATDiffset.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 ECLATbitset.py sampleDB.txt patterns.txt 10.0
+      (.venv) $ python3 ECLATDiffset.py sampleDB.txt patterns.txt 10.0
 
     .. note:: minSup can be specified  in support count or a value between 0 and 1.
 
-
-    **Calling from a python program**
+    
+     **Calling from a python program**
 
     .. code-block:: python
 
-            import PAMI.frequentPattern.basic.ECLATbitset as alg
+            import PAMI.frequentPattern.basic.ECLATDiffset as alg
 
             iFile = 'sampleDB.txt'
 
             minSup = 10  # can also be specified between 0 and 1
 
-            obj = alg.ECLATbitset(iFile, minSup)
+            obj = alg.ECLATDiffset(iFile, minSup)
 
             obj.mine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.save(oFile)
+            obj.savePatterns(oFile)
 
             Df = obj.getPatternInDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
@@ -125,177 +126,182 @@
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
+
     Credits:
     ========
 
-    The complete program was written by Yudai Masu and revised by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
+    The complete program was written by Kundai and revised by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
+    _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    _minSup = str()
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _mapSupport = {}
-    _lno = 0
-
-    def _convert(self, value):
-        """
-        To convert the user specified minSup value
-
-        :param value: user specified minSup value
-        :type value: int
-        :return: converted type
-        :rtype: int or float or string
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
+    _diffSets = {}
+    _trans_set = set()
 
     def _creatingItemSets(self):
         """
         Storing the complete transactions of the database/input file in a database variable
         """
         self._Database = []
-        self._mapSupport = {}
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
-
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
                     self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r') as f:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
-                            self._lno += 1
-                            splitter = [i.rstrip() for i in line.split(self._sep)]
-                            splitter = [x for x in splitter if x]
-                            self._Database.append(splitter)
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
-        self._minSup = self._convert(self._minSup)
+                    quit()
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
-    def startMine(self):
-        """
-        Frequent pattern mining process will start from here
-        We start with the scanning the itemSets and store the bitsets respectively.
-        We form the combinations of single items and  check with minSup condition to check the frequency of patterns
+    def _convert(self, value):
         """
-        self.mine()
 
-    def _bitPacker(self, data, maxIndex):
-        """
-        It takes the data and maxIndex as input and generates integer as output value.
+        To convert the user specified minSup value
 
-        :param data: it takes data as input.
-        :type data: int or float
-        :param maxIndex: It converts the data into bits By taking the maxIndex value as condition.
-        :type maxIndex: int
+        :param value: user specified minSup value
+        :return: converted type
         """
-        packed_bits = 0
-        for i in data:
-            packed_bits |= 1 << (maxIndex - i)
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
 
-        return packed_bits
-    
-    def __recursive(self, items, cands):
+    def _getUniqueItemList(self):
+
+        # tidSets will store all the initial tids
+        tidSets = {}
+        # uniqueItem will store all frequent 1 items
+        uniqueItem = []
+        for line in self._Database:
+                transNum = 0
+                # Database = [set([i.rstrip() for i in transaction.split('\t')]) for transaction in f]
+                for transaction in self._Database:
+                    transNum += 1
+                    self._trans_set.add(transNum)
+                    for item in transaction:
+                        if item in tidSets:
+                            tidSets[item].add(transNum)
+                        else:
+                            tidSets[item] = {transNum}
+        for key, value in tidSets.items():
+            supp = len(value)
+            if supp >= self._minSup:
+                self._diffSets[key] = [supp, self._trans_set.difference(value)]
+                uniqueItem.append(key)
+        # for x, y in self._diffSets.items():
+        #     print(x, y)
+        uniqueItem.sort()
+        # print()
+        return uniqueItem
+
+    def _runDeclat(self, candidateList):
+        """
+
+        It will generate the combinations of frequent items
+
+        :param candidateList :it represents the items with their respective transaction identifiers
+        :type candidateList: list
+        :return: returning transaction dictionary
+        :rtype: dict
         """
 
-        This function generates new candidates by taking input as original candidates.
+        newList = []
+        for i in range(0, len(candidateList)):
+            item1 = candidateList[i]
+            iList = item1.split()
+            for j in range(i + 1, len(candidateList)):
+                item2 = candidateList[j]
+                jList = item2.split()
+                if iList[:-1] == jList[:-1]:
+                    unionDiffSet = self._diffSets[item2][1].difference(self._diffSets[item1][1])
+                    unionSup = self._diffSets[item1][0] - len(unionDiffSet)
+                    if unionSup >= self._minSup:
+                        newKey = item1 + "\t" + jList[-1]
+                        self._diffSets[newKey] = [unionSup, unionDiffSet]
+                        newList.append(newKey)
+                    else: 
+                        break
 
-        :param items: A dictionary containing items and their corresponding support values.
-        :type items: dict
-        :param cands: A list of candidate itemsets.
-        :type cands: list
-        :return: None
-        """
-
-        for i in range(len(cands)):
-            newCands = []
-            for j in range(i + 1, len(cands)):
-                intersection = items[cands[i]] & items[cands[j]]
-                support = int.bit_count(intersection)
-                if support >= self._minSup:
-                    newCand = tuple(cands[i] + tuple([cands[j][-1]]))
-                    newCands.append(newCand)
-                    items[newCand] = intersection
-                    self._finalPatterns[newCand] = support
-            if len(newCands) > 1:
-                self.__recursive(items, newCands)
+        if len(newList) > 0:
+            self._runDeclat(newList)
 
-    def mine(self) -> None:
+    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
+    def startMine(self):
         """
         Frequent pattern mining process will start from here
-        # Bitset implementation
         """
-        self._startTime = _ab._time.time()
+        self.mine()
 
-        self._Database = []
+    def mine(self):
+        """
+        Frequent pattern mining process will start from here
+        """
 
+        self._startTime = _ab._time.time()
+        self._Database = []
+        self._finalPatterns = {}
+        self._diffSets = {}
+        self._trans_set = set()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-
-        items = {}
-        index = 0
-        for line in self._Database:
-            for item in line:
-                if tuple([item]) in items:
-                    items[tuple([item])].append(index)
-                else:
-                    items[tuple([item])] = [index]
-            index += 1
-
-        # sort by length in descending order
-        items = dict(sorted(items.items(), key=lambda x: len(x[1]), reverse=False))
-        cands = []
-        for key in items:
-            if len(items[key]) >= self._minSup:
-                self._finalPatterns[key] = len(items[key])
-                cands.append(key)
-                items[key] = self._bitPacker(items[key], index)
-
-        self.__recursive(items, cands)
-
+        #print(len(self._Database))
+        self._minSup = self._convert(self._minSup)
+        uniqueItemList = []
+        uniqueItemList = self._getUniqueItemList()
+        self._runDeclat(uniqueItemList)
+        self._finalPatterns = self._diffSets
+        #print(len(self._finalPatterns), len(uniqueItemList))
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using Apriori algorithm ")
+        print("Frequent patterns were generated successfully using ECLAT Diffset algorithm")
 
     def getMemoryUSS(self):
         """
 
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
@@ -322,83 +328,75 @@
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> _ab._pd.DataFrame:
+    def getPatternsAsDataFrame(self):
         """
 
         Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
-        # time = _ab._time.time()
-        # dataFrame = {}
-        # data = []
-        # for a, b in self._finalPatterns.items():
-        #     # data.append([a.replace('\t', ' '), b])
-        #     data.append([" ".join(a), b])
-        #     dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # print("Time taken to convert the frequent patterns into DataFrame is: ", _ab._time.time() - time)
-
-
-        dataFrame = _ab._pd.DataFrame(list(self._finalPatterns.items()), columns=['Patterns', 'Support'])
-
+        dataFrame = {}
+        data = []
+        for a, b in self._finalPatterns.items():
+            data.append([a.replace('\t', ' '), b[0]])
+            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
-    def save(self, outFile: str) -> None:
+    def save(self, outFile):
         """
 
         Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csvfile
-        :return: None
         """
-        with open(outFile, 'w') as f:
-            for x, y in self._finalPatterns.items():
-                x = self._sep.join(x)
-                f.write(f"{x} : {y}\n")
-
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
+        for x, y in self._finalPatterns.items():
+            patternsAndSupport = x.strip() + ":" + str(y[0])
+            writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """
 
         Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
         """
-        This function is used to print the result
+        This function is used to print the results
         """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ECLATbitset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ECLATbitset(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
+        print(_ap.getPatternsAsDataFrame())
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2024.5.1/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2024.5.1.1/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/basic/_Apriori.py` & `pami-2024.5.1.1/PAMI/frequentPattern/basic/_Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/basic/_FPGrowth.py` & `pami-2024.5.1.1/PAMI/frequentPattern/basic/_FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/closed/CHARM.py` & `pami-2024.5.1.1/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/closed/abstract.py` & `pami-2024.5.1.1/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/cuda/abstract.py` & `pami-2024.5.1.1/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2024.5.1.1/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# cuApriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+# cuAprioriBit is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
-#             import PAMI.frequentPattern.cuda.cuApriori as alg
+#             import PAMI.frequentPattern.cuda.cuAprioriBit as alg
 #
-#             obj = alg.cuApriori(iFile, minSup)
+#             obj = alg.cuAprioriBit(iFile, minSup)
 #
 #             obj.mine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -29,15 +29,14 @@
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
-
 __copyright__ = """
 Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -47,21 +46,22 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+# from PAMI.frequentPattern.cuda import abstract as _ab
+import abstract as _ab
 from deprecated import deprecated
-from PAMI.frequentPattern.cuda import abstract as _ab
-# import abstract as _ab
 
-class cuApriori(_ab._frequentPatterns):
+
+class cuAprioriBit(_ab._frequentPatterns):
     """
-    :Description: cuApriori is one of the fundamental algorithm to discover frequent patterns using Cuda in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+    :Description: cuAprioriBit is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 
     :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
             In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
@@ -96,64 +96,62 @@
     **Methods to execute code on terminal**
     ----------------------------------------------------
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 cuApriori.py <inputFile> <outputFile> <minSup>
+      (.venv) $ python3 cuAprioriBit.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 cuApriori.py sampleDB.txt patterns.txt 10.0
+      (.venv) $ python3 cuAprioriBit.py sampleDB.txt patterns.txt 10.0
 
     .. note:: minSup will be considered in percentage of database transactions
 
 
     **Importing this algorithm into a python program**
     ----------------------------------------------------
 
     .. code-block:: python
 
-             import PAMI.frequentPattern.cuda.cuApriori as alg
+            import PAMI.frequentPattern.cuda.cuAprioriBit as alg
 
-             obj = alg.cuApriori(iFile, minSup)
+            obj = alg.cuAprioriBit(iFile, minSup)
 
-             obj.mine()
+            obj.mine()
 
-             frequentPatterns = obj.getPatterns()
+            frequentPatterns = obj.getPatterns()
 
-             print("Total number of Frequent Patterns:", len(frequentPatterns))
+            print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-             obj.save(oFile)
+            obj.save(oFile)
 
-             Df = obj.getPatternInDataFrame()
+            Df = obj.getPatternInDataFrame()
 
-             memUSS = obj.getMemoryUSS()
+            memUSS = obj.getMemoryUSS()
 
-             print("Total Memory in USS:", memUSS)
+            print("Total Memory in USS:", memUSS)
 
-             memRSS = obj.getMemoryRSS()
+            memRSS = obj.getMemoryRSS()
 
-             print("Total Memory in RSS", memRSS)
+            print("Total Memory in RSS", memRSS)
 
-             run = obj.getRuntime()
+            run = obj.getRuntime()
 
-             print("Total ExecutionTime in seconds:", run)
+            print("Total ExecutionTime in seconds:", run)
 
 
     **Credits:**
     -------------
 
              The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
-    _ab._cp.cuda.Device(0).use()
-
     _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
@@ -249,21 +247,35 @@
                     ArraysAndItems[j] = [i]
                 else:
                     ArraysAndItems[j].append(i)
 
         newArraysAndItems = {}
 
         for k, v in ArraysAndItems.items():
-            ArraysAndItems[k] = _ab._cp.array(v, dtype=_ab._np.uint32)
+            ArraysAndItems[k] = _ab._np.array(v, dtype=_ab._np.uint32)
             if len(v) >= self._minSup:
                 self._finalPatterns[k] = len(v)
                 newArraysAndItems[k] = ArraysAndItems[k]
 
         return newArraysAndItems
 
+    def createBitRepresentation(self, ArraysAndItems):
+        bitRep = {}
+        arraySize = len(self._Database) // 32 + 1 if len(self._Database) % 32 != 0 else len(self._Database) // 32
+
+        for k, v in ArraysAndItems.items():
+            bitRep[k] = _ab._np.zeros(arraySize, dtype=_ab._np.uint32)
+            for i in v:
+                bitRep[k][i // 32] |= 1 << 31 - (i % 32)
+
+        for k, v in bitRep.items():
+            bitRep[k] = _ab._cp.array(v)
+
+        return bitRep
+
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self):
         """
         Frequent pattern mining process will start from here
         """
         self.mine()
 
@@ -273,40 +285,45 @@
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
 
         ArraysAndItems = self.arraysAndItems()
+        ArraysAndItems = self.createBitRepresentation(ArraysAndItems)
 
         while len(ArraysAndItems) > 0:
             # print("Total number of ArraysAndItems:", len(ArraysAndItems))
             newArraysAndItems = {}
             keys = list(ArraysAndItems.keys())
             for i in range(len(ArraysAndItems)):
                 # print(i, "/", len(ArraysAndItems), end="\r")
                 iList = list(keys[i])
                 for j in range(i + 1, len(ArraysAndItems)):
+                    unionData = _ab._cp.bitwise_and(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]])
+                    sum = _ab._cp.zeros(1, dtype=_ab._np.uint32)
+                    self._sumKernel((len(unionData) // 32 + 1,), (32,),
+                                    (unionData, sum, _ab._cp.uint32(len(unionData))))
+                    sum = sum[0]
                     jList = list(keys[j])
                     union = tuple(sorted(set(iList + jList)))
-                    intersect = _ab._cp.intersect1d(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]],
-                                                    assume_unique=True)
-                    if len(intersect) >= self._minSup and union not in self._finalPatterns:
-                        newArraysAndItems[union] = intersect
-                        self._finalPatterns[union] = len(intersect)
+                    if sum >= self._minSup and union not in self._finalPatterns:
+                        newArraysAndItems[union] = unionData
+                        string = "\t".join(union)
+                        self._finalPatterns[string] = sum
             ArraysAndItems = newArraysAndItems
             # print()
 
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using cuApriori algorithm ")
+        print("Frequent patterns were generated successfully using cuAprioriBit algorithm ")
 
     def getMemoryUSS(self):
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
@@ -364,34 +381,34 @@
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
         """
-        This function is used to print results
+        This function is used to print the result
         """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in s:", self.getRuntime())
+        print("Total ExecutionTime in ms:", self.getRuntime())
+
+
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = cuApriori(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in s:", _ap.getRuntime())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
 
-
-
```

### Comparing `pami-2024.5.1/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2024.5.1.1/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# cuAprioriBit is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+# cuECLATBit is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
-#             import PAMI.frequentPattern.cuda.cuAprioriBit as alg
+#             import PAMI.frequentPattern.cuda.cuEclatBit as alg
 #
-#             obj = alg.cuAprioriBit(iFile, minSup)
+#             obj = alg.cuEclatBit(iFile, minSup)
 #
 #             obj.mine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -29,14 +29,15 @@
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
+
 __copyright__ = """
 Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -46,25 +47,25 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+
 # from PAMI.frequentPattern.cuda import abstract as _ab
 import abstract as _ab
 from deprecated import deprecated
 
-
-class cuAprioriBit(_ab._frequentPatterns):
+class cuEclatBit(_ab._frequentPatterns):
     """
-    :Description: cuAprioriBit is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
+    :Description: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 
-    :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
-            In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
+    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
+            372-390 (2000), https://ieeexplore.ieee.org/document/846291
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minSup: int :
                    The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
@@ -96,62 +97,63 @@
     **Methods to execute code on terminal**
     ----------------------------------------------------
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 cuAprioriBit.py <inputFile> <outputFile> <minSup>
+      (.venv) $ python3 cuEclatBit.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 cuAprioriBit.py sampleDB.txt patterns.txt 10.0
+      (.venv) $ python3 cuEclatBit.py sampleDB.txt patterns.txt 10.0
 
     .. note:: minSup will be considered in percentage of database transactions
 
 
     **Importing this algorithm into a python program**
     ----------------------------------------------------
 
     .. code-block:: python
 
-            import PAMI.frequentPattern.cuda.cuAprioriBit as alg
+             import PAMI.frequentPattern.cuda.cuEclatBit as alg
 
-            obj = alg.cuAprioriBit(iFile, minSup)
+             obj = alg.cuEclatBit(iFile, minSup)
 
-            obj.mine()
+             obj.mine()
 
-            frequentPatterns = obj.getPatterns()
+             frequentPatterns = obj.getPatterns()
 
-            print("Total number of Frequent Patterns:", len(frequentPatterns))
+             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.save(oFile)
+             obj.save(oFile)
 
-            Df = obj.getPatternInDataFrame()
+             Df = obj.getPatternInDataFrame()
 
-            memUSS = obj.getMemoryUSS()
+             memUSS = obj.getMemoryUSS()
 
-            print("Total Memory in USS:", memUSS)
+             print("Total Memory in USS:", memUSS)
 
-            memRSS = obj.getMemoryRSS()
+             memRSS = obj.getMemoryRSS()
 
-            print("Total Memory in RSS", memRSS)
+             print("Total Memory in RSS", memRSS)
 
-            run = obj.getRuntime()
+             run = obj.getRuntime()
 
-            print("Total ExecutionTime in seconds:", run)
+             print("Total ExecutionTime in seconds:", run)
 
 
     **Credits:**
     -------------
 
              The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
 
     """
 
+
     _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
@@ -173,14 +175,18 @@
             atomicAdd(&sum[0], __popc(d_a[i]));
         }
         return;    
     }
 
     ''', 'sumKernel')
 
+
+
+
+
     def _creatingItemSets(self):
         """
         Storing the complete transactions of the database/input file in a database variable
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             temp = []
@@ -232,40 +238,41 @@
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
-
+    
     def arraysAndItems(self):
         ArraysAndItems = {}
 
         for i in range(len(self._Database)):
             for j in self._Database[i]:
                 j = tuple([j])
                 if j not in ArraysAndItems:
                     ArraysAndItems[j] = [i]
                 else:
                     ArraysAndItems[j].append(i)
 
         newArraysAndItems = {}
 
-        for k, v in ArraysAndItems.items():
+        for k,v in ArraysAndItems.items():
             ArraysAndItems[k] = _ab._np.array(v, dtype=_ab._np.uint32)
             if len(v) >= self._minSup:
                 self._finalPatterns[k] = len(v)
                 newArraysAndItems[k] = ArraysAndItems[k]
 
         return newArraysAndItems
-
+    
     def createBitRepresentation(self, ArraysAndItems):
         bitRep = {}
         arraySize = len(self._Database) // 32 + 1 if len(self._Database) % 32 != 0 else len(self._Database) // 32
 
+
         for k, v in ArraysAndItems.items():
             bitRep[k] = _ab._np.zeros(arraySize, dtype=_ab._np.uint32)
             for i in v:
                 bitRep[k][i // 32] |= 1 << 31 - (i % 32)
 
         for k, v in bitRep.items():
             bitRep[k] = _ab._cp.array(v)
@@ -282,48 +289,53 @@
     def mine(self):
         """
         Frequent pattern mining process will start from here
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
+        itemsList = sorted(list(set.union(*self._Database)))  # because Database is list
         self._minSup = self._convert(self._minSup)
 
         ArraysAndItems = self.arraysAndItems()
+
         ArraysAndItems = self.createBitRepresentation(ArraysAndItems)
 
         while len(ArraysAndItems) > 0:
             # print("Total number of ArraysAndItems:", len(ArraysAndItems))
             newArraysAndItems = {}
             keys = list(ArraysAndItems.keys())
             for i in range(len(ArraysAndItems)):
-                # print(i, "/", len(ArraysAndItems), end="\r")
                 iList = list(keys[i])
-                for j in range(i + 1, len(ArraysAndItems)):
-                    unionData = _ab._cp.bitwise_and(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]])
-                    sum = _ab._cp.zeros(1, dtype=_ab._np.uint32)
-                    self._sumKernel((len(unionData) // 32 + 1,), (32,),
-                                    (unionData, sum, _ab._cp.uint32(len(unionData))))
-                    sum = sum[0]
+                # print(i, "/", len(ArraysAndItems), end="\r")
+                for j in range(i+1, len(ArraysAndItems)):
                     jList = list(keys[j])
-                    union = tuple(sorted(set(iList + jList)))
-                    if sum >= self._minSup and union not in self._finalPatterns:
-                        newArraysAndItems[union] = unionData
-                        string = "\t".join(union)
-                        self._finalPatterns[string] = sum
+                    union = []
+                    if iList[:-1] == jList[:-1] and iList[-1] != jList[-1]:
+                        union = iList + [jList[-1]]
+                        union = tuple(union)
+                        unionData = _ab._cp.bitwise_and(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]])
+                        sum = _ab._cp.zeros(1, dtype=_ab._np.uint32)
+                        self._sumKernel((len(unionData) // 32 + 1,), (32,), (unionData, sum, _ab._cp.uint32(len(unionData))))
+                        sum = sum[0]
+                        if sum >= self._minSup and union not in self._finalPatterns:
+                            newArraysAndItems[union] = unionData
+                            string = "\t".join(union)
+                            self._finalPatterns[string] = sum
             ArraysAndItems = newArraysAndItems
             # print()
 
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using cuAprioriBit algorithm ")
+        print("Frequent patterns were generated successfully using cuEclatBit algorithm ")
+            
 
     def getMemoryUSS(self):
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
@@ -389,26 +401,33 @@
         """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
-
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = cuEclatBit(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = cuAprioriBit(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = cuEclatBit(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
+"""_ap = cuEclat("/home/tarun/PAMI/PAMI/frequentPattern/cuda/test.txt", 2, " ")
+    _ap = cuEclat("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
+    _ap.startMine()
+    _ap.mine()
+    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+    print("Total Memory in USS:", _ap.getMemoryUSS())
+    print("Total Memory in RSS", _ap.getMemoryRSS())
+    print("Total ExecutionTime in s:", _ap.getRuntime())"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2024.5.1/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2024.5.1.1/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2024.5.1.1/PAMI/frequentPattern/topk/FAE.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# cuECLATBit is one of the fundamental algorithm to discover frequent patterns in a transactional database.
-#
+# Top - K is and algorithm to discover top frequent patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
-# ----------------------------------------------------
+# ---------------------------------------------------------
 #
-#             import PAMI.frequentPattern.cuda.cuEclatBit as alg
+#             import PAMI.frequentPattern.topK.FAE as alg
 #
-#             obj = alg.cuEclatBit(iFile, minSup)
+#             obj = alg.FAE(iFile, K)
 #
 #             obj.mine()
 #
-#             frequentPatterns = obj.getPatterns()
+#             topKFrequentPatterns = obj.getPatterns()
 #
-#             print("Total number of Frequent Patterns:", len(frequentPatterns))
+#             print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
 #
 #             obj.save(oFile)
 #
 #             Df = obj.getPatternInDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
@@ -30,14 +29,15 @@
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
 
+
 __copyright__ = """
 Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -47,35 +47,40 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-
-# from PAMI.frequentPattern.cuda import abstract as _ab
-import abstract as _ab
+from PAMI.frequentPattern.topk import abstract as _ab
 from deprecated import deprecated
 
-class cuEclatBit(_ab._frequentPatterns):
+
+class FAE(_ab._frequentPatterns):
     """
-    :Description: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
+    :Description: Top - K is and algorithm to discover top frequent patterns in a transactional database.
+
 
-    :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
-            372-390 (2000), https://ieeexplore.ieee.org/document/846291
+    :Reference:   Zhi-Hong Deng, Guo-Dong Fang: Mining Top-Rank-K Frequent Patterns: DOI: 10.1109/ICMLC.2007.4370261 · Source: IEEE Xplore
+                  https://ieeexplore.ieee.org/document/4370261
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
-    :param  minSup: int :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
+    :param  k: int :
+                    User specified count of top frequent patterns
+    :param minimum: int :
+                    Minimum number of frequent patterns to consider in analysis
+
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
+
+
     :Attributes:
 
         startTime : float
           To record the start time of the mining process
 
         endTime : float
           To record the completion time of the mining process
@@ -85,349 +90,371 @@
 
         memoryUSS : float
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
 
-        Database : list
-          To store the transactions of a database in list
-
+        finalPatterns : dict
+            it represents to store the patterns
 
 
     **Methods to execute code on terminal**
-    ----------------------------------------------------
+    -------------------------------------------
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 cuEclatBit.py <inputFile> <outputFile> <minSup>
+      (.venv) $ python3 FAE.py <inputFile> <outputFile> <K>
 
       Example Usage:
 
-      (.venv) $ python3 cuEclatBit.py sampleDB.txt patterns.txt 10.0
+      (.venv) $ python3 FAE.py sampleDB.txt patterns.txt 10
 
-    .. note:: minSup will be considered in percentage of database transactions
+    .. note:: k will be considered as count of top frequent patterns to consider in analysis
 
 
-    **Importing this algorithm into a python program**
-    ----------------------------------------------------
 
+    **Importing this algorithm into a python program**
+    ---------------------------------------------------------
     .. code-block:: python
 
-             import PAMI.frequentPattern.cuda.cuEclatBit as alg
-
-             obj = alg.cuEclatBit(iFile, minSup)
+        import PAMI.frequentPattern.topK.FAE as alg
 
-             obj.mine()
+        obj = alg.FAE(iFile, K)
 
-             frequentPatterns = obj.getPatterns()
+        obj.mine()
 
-             print("Total number of Frequent Patterns:", len(frequentPatterns))
+        topKFrequentPatterns = obj.getPatterns()
 
-             obj.save(oFile)
+        print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
 
-             Df = obj.getPatternInDataFrame()
+        obj.save(oFile)
 
-             memUSS = obj.getMemoryUSS()
+        Df = obj.getPatternInDataFrame()
 
-             print("Total Memory in USS:", memUSS)
+        memUSS = obj.getMemoryUSS()
 
-             memRSS = obj.getMemoryRSS()
+        print("Total Memory in USS:", memUSS)
 
-             print("Total Memory in RSS", memRSS)
+        memRSS = obj.getMemoryRSS()
 
-             run = obj.getRuntime()
+        print("Total Memory in RSS", memRSS)
 
-             print("Total ExecutionTime in seconds:", run)
+        run = obj.getRuntime()
 
+        print("Total ExecutionTime in seconds:", run)
 
-    **Credits:**
-    -------------
-
-             The complete program was written by Tarun Sreepada under the supervision of Professor Rage Uday Kiran.
+    Credits:
+    --------
+        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
     """
 
-
-    _minSup = float()
     _startTime = float()
     _endTime = float()
+    _k = int()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-
-    _sumKernel = _ab._cp.RawKernel(r'''
-
-    #define uint32_t unsigned int
-
-    extern "C" __global__
-
-    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
-    {
-        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
-        if (i < numElements)
-        {  
-            atomicAdd(&sum[0], __popc(d_a[i]));
-        }
-        return;    
-    }
-
-    ''', 'sumKernel')
-
-
-
-
+    _tidList = {}
+    _minimum = int()
 
     def _creatingItemSets(self):
         """
-        Storing the complete transactions of the database/input file in a database variable
+            Storing the complete transactions of the database/input file in a database variable
+
         """
+
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            temp = []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                temp = self._iFile['Transactions'].tolist()
+                self._Database = self._iFile['Transactions'].tolist()
 
-            for k in temp:
-                self._Database.append(set(k))
+            # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._Database.append(set(temp))
+                    self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(set(temp))
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _convert(self, value):
+    def _frequentOneItem(self):
         """
+        Generating one frequent patterns
+        """
+        candidate = {}
+        self._tidList = {}
+        for i in range(len(self._Database)):
+            for j in self._Database[i]:
+                if j not in candidate:
+                    candidate[j] = 1
+                    self._tidList[j] = [i]
+                else:
+                    candidate[j] += 1
+                    self._tidList[j].append(i)
+        self._finalPatterns = {}
+        plist = [key for key, value in sorted(candidate.items(), key=lambda x: x[1], reverse=True)]
+        for i in plist:
+            if len(self._finalPatterns) >= self._k:
+                break
+            else:
+                self._finalPatterns[i] = candidate[i]
+        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+        plist = list(self._finalPatterns.keys())
+        return plist
+
+    def _save(self, prefix, suffix, tidSetI):
+        """Saves the patterns that satisfy the periodic frequent property.
+
+            :param prefix: the prefix of a pattern
+            :type prefix: list
+            :param suffix: the suffix of a patterns
+            :type suffix: list
+            :param tidSetI: the timestamp of a patterns
+            :type tidSetI: list
+        """
+
+        if prefix is None:
+            prefix = suffix
+        else:
+            prefix = prefix + suffix
+        val = len(tidSetI)
+        sample = str()
+        for i in prefix:
+            sample = sample + i + "\t"
+        if len(self._finalPatterns) < self._k:
+            if val > self._minimum:
+                self._finalPatterns[sample] = val
+                self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
+                self._minimum = min([i for i in self._finalPatterns.values()])
+        else:
+            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
+                if val > y:
+                    del self._finalPatterns[x]
+                    self._finalPatterns[sample] = val
+                    self._finalPatterns = {k: v for k, v in
+                                              sorted(self._finalPatterns.items(), key=lambda item: item[1],
+                                                     reverse=True)}
+                    self._minimum = min([i for i in self._finalPatterns.values()])
+                    return
+
+    def _Generation(self, prefix, itemSets, tidSets):
+        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
+
+            :param prefix:  main equivalence prefix
+            :type prefix: periodic-frequent item or pattern
+            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
+                            and frequent with their timestamps
+            :type itemSets: list
+            :param tidSets: timestamps of the items in the argument itemSets
+            :type tidSets: list
+
+
+                    """
+        if len(itemSets) == 1:
+            i = itemSets[0]
+            tidI = tidSets[0]
+            self._save(prefix, [i], tidI)
+            return
+        for i in range(len(itemSets)):
+            itemI = itemSets[i]
+            if itemI is None:
+                continue
+            tidSetI = tidSets[i]
+            classItemSets = []
+            classTidSets = []
+            itemSetX = [itemI]
+            for j in range(i + 1, len(itemSets)):
+                itemJ = itemSets[j]
+                tidSetJ = tidSets[j]
+                y = list(set(tidSetI).intersection(tidSetJ))
+                if len(y) >= self._minimum:
+                    classItemSets.append(itemJ)
+                    classTidSets.append(y)
+            newPrefix = list(set(itemSetX)) + prefix
+            self._Generation(newPrefix, classItemSets, classTidSets)
+            self._save(prefix, list(set(itemSetX)), tidSetI)
 
-        To convert the user specified minSup value
-
+    def _convert(self, value):
+        """
+        to convert the type of user specified minSup value
         :param value: user specified minSup value
-
         :type value: int or float or str
-
         :return: converted type
-
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
-                value = (len(self._Database) * value)
+                value = ((len(self._Database)) * value)
             else:
                 value = int(value)
         return value
-    
-    def arraysAndItems(self):
-        ArraysAndItems = {}
-
-        for i in range(len(self._Database)):
-            for j in self._Database[i]:
-                j = tuple([j])
-                if j not in ArraysAndItems:
-                    ArraysAndItems[j] = [i]
-                else:
-                    ArraysAndItems[j].append(i)
-
-        newArraysAndItems = {}
-
-        for k,v in ArraysAndItems.items():
-            ArraysAndItems[k] = _ab._np.array(v, dtype=_ab._np.uint32)
-            if len(v) >= self._minSup:
-                self._finalPatterns[k] = len(v)
-                newArraysAndItems[k] = ArraysAndItems[k]
-
-        return newArraysAndItems
-    
-    def createBitRepresentation(self, ArraysAndItems):
-        bitRep = {}
-        arraySize = len(self._Database) // 32 + 1 if len(self._Database) % 32 != 0 else len(self._Database) // 32
-
-
-        for k, v in ArraysAndItems.items():
-            bitRep[k] = _ab._np.zeros(arraySize, dtype=_ab._np.uint32)
-            for i in v:
-                bitRep[k][i // 32] |= 1 << 31 - (i % 32)
-
-        for k, v in bitRep.items():
-            bitRep[k] = _ab._cp.array(v)
-
-        return bitRep
 
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self):
         """
-        Frequent pattern mining process will start from here
+            Main function of the program
         """
         self.mine()
 
     def mine(self):
         """
-        Frequent pattern mining process will start from here
+            Main function of the program
         """
-        self._Database = []
         self._startTime = _ab._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._k is None:
+            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        itemsList = sorted(list(set.union(*self._Database)))  # because Database is list
-        self._minSup = self._convert(self._minSup)
-
-        ArraysAndItems = self.arraysAndItems()
-
-        ArraysAndItems = self.createBitRepresentation(ArraysAndItems)
-
-        while len(ArraysAndItems) > 0:
-            # print("Total number of ArraysAndItems:", len(ArraysAndItems))
-            newArraysAndItems = {}
-            keys = list(ArraysAndItems.keys())
-            for i in range(len(ArraysAndItems)):
-                iList = list(keys[i])
-                # print(i, "/", len(ArraysAndItems), end="\r")
-                for j in range(i+1, len(ArraysAndItems)):
-                    jList = list(keys[j])
-                    union = []
-                    if iList[:-1] == jList[:-1] and iList[-1] != jList[-1]:
-                        union = iList + [jList[-1]]
-                        union = tuple(union)
-                        unionData = _ab._cp.bitwise_and(ArraysAndItems[keys[i]], ArraysAndItems[keys[j]])
-                        sum = _ab._cp.zeros(1, dtype=_ab._np.uint32)
-                        self._sumKernel((len(unionData) // 32 + 1,), (32,), (unionData, sum, _ab._cp.uint32(len(unionData))))
-                        sum = sum[0]
-                        if sum >= self._minSup and union not in self._finalPatterns:
-                            newArraysAndItems[union] = unionData
-                            string = "\t".join(union)
-                            self._finalPatterns[string] = sum
-            ArraysAndItems = newArraysAndItems
-            # print()
-
+        self._k = self._convert(self._k)
+        plist = self._frequentOneItem()
+        for i in range(len(plist)):
+            itemI = plist[i]
+            tidSetI = self._tidList[itemI]
+            itemSetX = [itemI]
+            itemSets = []
+            tidSets = []
+            for j in range(i + 1, len(plist)):
+                itemJ = plist[j]
+                tidSetJ = self._tidList[itemJ]
+                y1 = list(set(tidSetI).intersection(tidSetJ))
+                if len(y1) >= self._minimum:
+                    itemSets.append(itemJ)
+                    tidSets.append(y1)
+            self._Generation(itemSetX, itemSets, tidSets)
+        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
         self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using cuEclatBit algorithm ")
-            
 
     def getMemoryUSS(self):
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
+
         :return: returning USS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """
         Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """
         Calculating the total amount of runtime taken by the mining process
+
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """
         Storing final frequent patterns in a dataframe
+
         :return: returning frequent patterns in a dataframe
+
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
         """
         Complete set of frequent patterns will be loaded in to an output file
+
         :param outFile: name of the output file
-        :type outFile: csvfile
+
+        :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
-            writer.write("%s \n" % s1)
+            patternsAndSupport = x.strip() + ":" + str(y)
+            writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """
         Function to send the set of frequent patterns after completion of the mining process
+
         :return: returning frequent patterns
+
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self):
+    def printTOPK(self):
         """
-        This function is used to print the result
+        This function is used to print the results
         """
-        print("Total number of Frequent Patterns:", len(self.getPatterns()))
+        print("Top K Frequent  Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = cuEclatBit(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = cuEclatBit(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
-        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+        print("Top K Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
-"""_ap = cuEclat("/home/tarun/PAMI/PAMI/frequentPattern/cuda/test.txt", 2, " ")
-    _ap = cuEclat("/home/tarun/Transactional_T10I4D100K.csv", 450, "\t")
-    _ap.startMine()
-    _ap.mine()
-    print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-    print("Total Memory in USS:", _ap.getMemoryUSS())
-    print("Total Memory in RSS", _ap.getMemoryRSS())
-    print("Total ExecutionTime in s:", _ap.getRuntime())"""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2024.5.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2024.5.1.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2024.5.1.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2024.5.1.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2024.5.1.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/maximal/__init__.py` & `pami-2024.5.1.1/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/maximal/abstract.py` & `pami-2024.5.1.1/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2024.5.1.1/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2024.5.1.1/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2024.5.1.1/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2024.5.1.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/frequentPattern/topk/FAE.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# Top - K is and algorithm to discover top frequent patterns in a transactional database.
+# PFECLAT is the fundamental approach to mine the periodic-frequent patterns.
+#
 #
 # **Importing this algorithm into a python program**
-# ---------------------------------------------------------
+# --------------------------------------------------------
+#
 #
-#             import PAMI.frequentPattern.topK.FAE as alg
+#             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
 #
-#             obj = alg.FAE(iFile, K)
+#             obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
 #
-#             obj.mine()
+#             obj.startMine()
 #
-#             topKFrequentPatterns = obj.getPatterns()
+#             periodicFrequentPatterns = obj.getPatterns()
 #
-#             print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
+#             print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 #
-#             obj.save(oFile)
+#             obj.save("patterns")
 #
-#             Df = obj.getPatternInDataFrame()
+#             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
 #             memRSS = obj.getMemoryRSS()
 #
@@ -29,160 +31,234 @@
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
 
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+     Copyright (C)  2021 Rage Uday Kiran
+
 """
 
-from PAMI.frequentPattern.topk import abstract as _ab
+from PAMI.periodicFrequentPattern.basic import abstract as _ab
+import pandas as pd
 from deprecated import deprecated
+import numpy as np
 
+from PAMI.periodicFrequentPattern.basic import abstract as _ab
 
-class FAE(_ab._frequentPatterns):
-    """
-    :Description: Top - K is and algorithm to discover top frequent patterns in a transactional database.
 
+class PFECLAT(_ab._periodicFrequentPatterns):
+    """
+    :Description:   PFECLAT is the fundamental approach to mine the periodic-frequent patterns.
 
-    :Reference:   Zhi-Hong Deng, Guo-Dong Fang: Mining Top-Rank-K Frequent Patterns: DOI: 10.1109/ICMLC.2007.4370261 · Source: IEEE Xplore
-                  https://ieeexplore.ieee.org/document/4370261
+    :Reference:   P. Ravikumar, P.Likhitha, R. Uday kiran, Y. Watanobe, and Koji Zettsu, "Towards efficient discovery of
+                  periodic-frequent patterns in columnar temporal databases", 2021 IEA/AIE.
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
+                   Name of the Input file to mine complete set of periodic frequent pattern's
     :param  oFile: str :
-                   Name of the output file to store complete set of frequent patterns
-    :param  k: int :
-                    User specified count of top frequent patterns
-    :param minimum: int :
-                    Minimum number of frequent patterns to consider in analysis
-
+                   Name of the output file to store complete set of periodic frequent pattern's
+    :param  minSup: str:
+                   Controls the minimum number of transactions in which every item must appear in a database.
+    :param  maxPer: str:
+                   Controls the maximum number of transactions in which any two items within a pattern can reappear.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
-
-
     :Attributes:
 
-        startTime : float
-          To record the start time of the mining process
-
-        endTime : float
-          To record the completion time of the mining process
-
-        finalPatterns : dict
-          Storing the complete set of patterns in a dictionary variable
-
+        iFile : file
+            Name of the Input file or path of the input file
+        oFile : file
+            Name of the output file or path of the output file
+        minSup : int or float or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        maxPer : int or float or str
+            The user can specify maxPer either in count or proportion of database size.
+            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
+        sep : str
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            However, the users can override their default separator.
         memoryUSS : float
-          To store the total amount of USS memory consumed by the program
-
+            To store the total amount of USS memory consumed by the program
         memoryRSS : float
-          To store the total amount of RSS memory consumed by the program
-
+            To store the total amount of RSS memory consumed by the program
+        startTime : float
+            To record the start time of the mining process
+        endTime : float
+            To record the completion time of the mining process
+        Database : list
+            To store the transactions of a database in list
+        mapSupport : Dictionary
+            To maintain the information of item and their frequency
+        lno : int
+            it represents the total no of transactions
+        tree : class
+            it represents the Tree class
+        itemSetCount : int
+            it represents the total no of patterns
         finalPatterns : dict
             it represents to store the patterns
-
+        tidList : dict
+            stores the timestamps of an item
+        hashing : dict
+            stores the patterns with their support to check for the closed property
+
+    :Methods:
+
+        startMine()
+            Mining process will start from here
+        getPatterns()
+            Complete set of patterns will be retrieved with this function
+        save(oFile)
+            Complete set of periodic-frequent patterns will be loaded in to a output file
+        getPatternsAsDataFrame()
+            Complete set of periodic-frequent patterns will be loaded in to a dataframe
+        getMemoryUSS()
+            Total amount of USS memory consumed by the mining process will be retrieved from this function
+        getMemoryRSS()
+            Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        getRuntime()
+            Total amount of runtime taken by the mining process will be retrieved from this function
+        creatingOneItemSets()
+            Scan the database and store the items with their timestamps which are periodic frequent 
+        getPeriodAndSupport()
+            Calculates the support and period for a list of timestamps.
+        Generation()
+            Used to implement prefix class equivalence method to generate the periodic patterns recursively
+            
 
     **Methods to execute code on terminal**
-    -------------------------------------------
-
+    ------------------------------------------
     .. code-block:: console
 
-      Format:
 
-      (.venv) $ python3 FAE.py <inputFile> <outputFile> <K>
+       Format:
+
+       (.venv) $ python3 PFECLAT.py <inputFile> <outputFile> <minSup>
 
-      Example Usage:
+       Example usage:
 
-      (.venv) $ python3 FAE.py sampleDB.txt patterns.txt 10
+       (.venv) $ python3 PFECLAT.py sampleDB.txt patterns.txt 10.0
 
-    .. note:: k will be considered as count of top frequent patterns to consider in analysis
 
 
+               .. note:: minSup will be considered in percentage of database transactions
+
 
     **Importing this algorithm into a python program**
-    ---------------------------------------------------------
+    --------------------------------------------------------
     .. code-block:: python
 
-        import PAMI.frequentPattern.topK.FAE as alg
+             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
 
-        obj = alg.FAE(iFile, K)
+                obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
 
-        obj.mine()
+                obj.startMine()
 
-        topKFrequentPatterns = obj.getPatterns()
+                periodicFrequentPatterns = obj.getPatterns()
 
-        print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
+                print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 
-        obj.save(oFile)
+                obj.save("patterns")
 
-        Df = obj.getPatternInDataFrame()
+                Df = obj.getPatternsAsDataFrame()
 
-        memUSS = obj.getMemoryUSS()
+                memUSS = obj.getMemoryUSS()
 
-        print("Total Memory in USS:", memUSS)
+                print("Total Memory in USS:", memUSS)
 
-        memRSS = obj.getMemoryRSS()
+                memRSS = obj.getMemoryRSS()
 
-        print("Total Memory in RSS", memRSS)
+                print("Total Memory in RSS", memRSS)
 
-        run = obj.getRuntime()
+                run = obj.getRuntime()
 
-        print("Total ExecutionTime in seconds:", run)
+                print("Total ExecutionTime in seconds:", run)
 
-    Credits:
-    --------
-        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+    **Credits:**
+    --------------
+             The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
     """
-
-    _startTime = float()
-    _endTime = float()
-    _k = int()
-    _finalPatterns = {}
+    
     _iFile = " "
     _oFile = " "
     _sep = " "
+    _dbSize = None
+    _Database = None
+    _minSup = str()
+    _maxPer = str()
+    _tidSet = set()
+    _finalPatterns = {}
+    _startTime = None
+    _endTime = None
     _memoryUSS = float()
     _memoryRSS = float()
-    _Database = []
-    _tidList = {}
-    _minimum = int()
 
-    def _creatingItemSets(self):
+    def _convert(self, value) -> float:
         """
-            Storing the complete transactions of the database/input file in a database variable
+        To convert the given user specified value
 
+        :param value: user specified value
+        :return: converted value
         """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (self._dbSize * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (self._dbSize * value)
+            else:
+                value = int(value)
+        return value
 
+    def _creatingItemSets(self) -> None:
+        """
+            Storing the complete transactions of the database/input file in a database variable
+        :return: None
+        """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
+            data, ts = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
+            if 'TS' in i:
+                ts = self._iFile['TS'].tolist()
             if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
+                data = self._iFile['Transactions'].tolist()
+            for i in range(len(data)):
+                tr = [ts[i][0]]
+                tr = tr + data[i]
+                self._Database.append(tr)
 
-            # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
@@ -196,265 +272,196 @@
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _frequentOneItem(self):
-        """
-        Generating one frequent patterns
+    @deprecated("It is recommended to use mine() instead of startMine() for mining process")
+    def startMine(self) -> None:
         """
-        candidate = {}
-        self._tidList = {}
-        for i in range(len(self._Database)):
-            for j in self._Database[i]:
-                if j not in candidate:
-                    candidate[j] = 1
-                    self._tidList[j] = [i]
-                else:
-                    candidate[j] += 1
-                    self._tidList[j].append(i)
-        self._finalPatterns = {}
-        plist = [key for key, value in sorted(candidate.items(), key=lambda x: x[1], reverse=True)]
-        for i in plist:
-            if len(self._finalPatterns) >= self._k:
-                break
-            else:
-                self._finalPatterns[i] = candidate[i]
-        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
-        plist = list(self._finalPatterns.keys())
-        return plist
-
-    def _save(self, prefix, suffix, tidSetI):
-        """Saves the patterns that satisfy the periodic frequent property.
-
-            :param prefix: the prefix of a pattern
-            :type prefix: list
-            :param suffix: the suffix of a patterns
-            :type suffix: list
-            :param tidSetI: the timestamp of a patterns
-            :type tidSetI: list
-        """
-
-        if prefix is None:
-            prefix = suffix
-        else:
-            prefix = prefix + suffix
-        val = len(tidSetI)
-        sample = str()
-        for i in prefix:
-            sample = sample + i + "\t"
-        if len(self._finalPatterns) < self._k:
-            if val > self._minimum:
-                self._finalPatterns[sample] = val
-                self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
-                self._minimum = min([i for i in self._finalPatterns.values()])
-        else:
-            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
-                if val > y:
-                    del self._finalPatterns[x]
-                    self._finalPatterns[sample] = val
-                    self._finalPatterns = {k: v for k, v in
-                                              sorted(self._finalPatterns.items(), key=lambda item: item[1],
-                                                     reverse=True)}
-                    self._minimum = min([i for i in self._finalPatterns.values()])
-                    return
-
-    def _Generation(self, prefix, itemSets, tidSets):
-        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
-
-            :param prefix:  main equivalence prefix
-            :type prefix: periodic-frequent item or pattern
-            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
-                            and frequent with their timestamps
-            :type itemSets: list
-            :param tidSets: timestamps of the items in the argument itemSets
-            :type tidSets: list
-
-
-                    """
-        if len(itemSets) == 1:
-            i = itemSets[0]
-            tidI = tidSets[0]
-            self._save(prefix, [i], tidI)
-            return
-        for i in range(len(itemSets)):
-            itemI = itemSets[i]
-            if itemI is None:
-                continue
-            tidSetI = tidSets[i]
-            classItemSets = []
-            classTidSets = []
-            itemSetX = [itemI]
-            for j in range(i + 1, len(itemSets)):
-                itemJ = itemSets[j]
-                tidSetJ = tidSets[j]
-                y = list(set(tidSetI).intersection(tidSetJ))
-                if len(y) >= self._minimum:
-                    classItemSets.append(itemJ)
-                    classTidSets.append(y)
-            newPrefix = list(set(itemSetX)) + prefix
-            self._Generation(newPrefix, classItemSets, classTidSets)
-            self._save(prefix, list(set(itemSetX)), tidSetI)
-
-    def _convert(self, value):
-        """
-        to convert the type of user specified minSup value
-        :param value: user specified minSup value
-        :type value: int or float or str
-        :return: converted type
+        Mining process will start from this function
+        :return: None
         """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = ((len(self._Database)) * value)
-            else:
-                value = int(value)
-        return value
+        self.Mine()
+        # self._startTime = _ab._time.time()
+        # self._finalPatterns = {}
+        # frequentSets = self._creatingOneItemSets()
+        # self._generateEclat(frequentSets)
+        # self._endTime = _ab._time.time()
+        # process = _ab._psutil.Process(_ab._os.getpid())
+        # self._memoryRSS = float()
+        # self._memoryUSS = float()
+        # self._memoryUSS = process.memory_full_info().uss
+        # self._memoryRSS = process.memory_info().rss
+        # print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
+
+    def _getMaxPer(self, arr, maxTS):
+        arr = np.append(list(arr), [0, maxTS])
+        arr = np.sort(arr)
+        arr = np.diff(arr)
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
-    def startMine(self):
-        """
-            Main function of the program
-        """
-        self.mine()
+        return np.max(arr)
 
-    def mine(self):
+    def Mine(self) -> None:
         """
-            Main function of the program
+        Mining process will start from this function
+        :return: None
         """
         self._startTime = _ab._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._k is None:
-            raise Exception("Please enter the Minimum Support")
-        self._creatingItemSets()
-        self._k = self._convert(self._k)
-        plist = self._frequentOneItem()
-        for i in range(len(plist)):
-            itemI = plist[i]
-            tidSetI = self._tidList[itemI]
-            itemSetX = [itemI]
-            itemSets = []
-            tidSets = []
-            for j in range(i + 1, len(plist)):
-                itemJ = plist[j]
-                tidSetJ = self._tidList[itemJ]
-                y1 = list(set(tidSetI).intersection(tidSetJ))
-                if len(y1) >= self._minimum:
-                    itemSets.append(itemJ)
-                    tidSets.append(y1)
-            self._Generation(itemSetX, itemSets, tidSets)
-        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
+        self._finalPatterns = {}
+        frequentSets = self._creatingItemSets()
+
+        items = {}
+        maxTS = 0
+        for line in self._Database:
+            index = int(line[0])
+            maxTS = max(maxTS, index)
+            for item in line[1:]:
+                if tuple([item]) not in items:
+                    items[tuple([item])] = set()
+                items[tuple([item])].add(index)
+
+        self._dbSize = maxTS
+
+        self._minSup = self._convert(self._minSup)
+        self._maxPer = self._convert(self._maxPer)
+        minSup = self._minSup
+        maxPer = self._maxPer
+
+
+        items = {k: v for k, v in items.items() if len(v) >= minSup}
+        items = {k: v for k, v in sorted(items.items(), key = lambda x: len(x[1]), reverse = True)}
+
+        keys = []
+        for item in list(items.keys()):
+            per = self._getMaxPer(items[item], maxTS)
+            if per <= maxPer:
+                keys.append(item)
+                self._finalPatterns[item] = [len(items[item]), per, set(items[item])]
+
+        while keys:
+            newKeys = []
+            for i in range(len(keys)):
+                for j in range(i + 1, len(keys)):
+                    if keys[i][:-1] == keys[j][:-1] and keys[i][-1] != keys[j][-1]:
+                        # print(keys[i], keys[j])
+                        newKey = tuple(keys[i] + (keys[j][-1],))
+                        intersect = items[keys[i]].intersection(items[keys[j]])
+                        per = self._getMaxPer(intersect, maxTS)
+                        sup = len(intersect)
+                        if sup >= minSup and per <= maxPer:
+                            items[newKey] = intersect
+                            newKeys.append(newKey)
+                            self._finalPatterns[newKey] = [sup, per, set(intersect)]
+                    else:
+                        break
+            keys = newKeys
+
+        newPattern = {}
+        for k, v in self._finalPatterns.items():
+            newPattern["\t".join([str(x) for x in k])] = v
+
+        self._finalPatterns = newPattern
+
+        # self._generateEclat(frequentSets)
         self._endTime = _ab._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
+        self._memoryRSS = float()
+        self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
+        print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
 
-    def getMemoryUSS(self):
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+    def getMemoryUSS(self) -> float:
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryUSS
 
-    def getMemoryRSS(self):
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+    def getMemoryRSS(self) -> float:
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryRSS
 
-    def getRuntime(self):
-        """
-        Calculating the total amount of runtime taken by the mining process
+    def getRuntime(self) -> float:
+        """Calculating the total amount of runtime taken by the mining process
 
-        :return: returning total amount of runtime taken by the mining process
 
+        :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self):
+    def getPatternsAsDataFrame(self) -> _ab._pd.DataFrame:
         """
-        Storing final frequent patterns in a dataframe
-
-        :return: returning frequent patterns in a dataframe
+        Storing final periodic-frequent patterns in a dataframe
 
+        :return: returning periodic-frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
-        dataFrame = {}
+        dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
-            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        return dataFrame
+            data.append([a, b[0], b[1]])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
+        return dataframe
 
-    def save(self, outFile):
+    def save(self, outFile: str) -> None:
         """
-        Complete set of frequent patterns will be loaded in to an output file
+        Complete set of periodic-frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
-
-        :type outFile: file
+        :type outFile: csv file
+        :return: None
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y)
-            writer.write("%s \n" % patternsAndSupport)
+            s1 = x + ":" + str(y[0]) + ":" + str(y[1])
+            #s1 = x.replace(' ', '\t') + ":" + str(y[0]) + ":" + str(y[1])
+            writer.write("%s \n" % s1)
 
-    def getPatterns(self):
+    def getPatterns(self) -> dict:
         """
-        Function to send the set of frequent patterns after completion of the mining process
-
-        :return: returning frequent patterns
+        Function to send the set of periodic-frequent patterns after completion of the mining process
 
+        :return: returning periodic-frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printTOPK(self):
+    def printResults(self) -> None:
         """
         This function is used to print the results
+        :return: None
         """
-        print("Top K Frequent  Patterns:", len(self.getPatterns()))
+        print("Total number of Periodic Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
-
+                    
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
+        if len(_ab._sys.argv) == 6:
+            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
-        _ap.mine()
-        print("Top K Frequent Patterns:", len(_ap.getPatterns()))
+        print("Total number of Periodic-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2024.5.1/PAMI/frequentPattern/topk/abstract.py` & `pami-2024.5.1.1/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/fuzzyFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py` & `pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py` & `pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py` & `pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py` & `pami-2024.5.1.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py` & `pami-2024.5.1.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2024.5.1.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/georeferencedFrequentPattern/__init__.py` & `pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py` & `pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py` & `pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/georeferencedFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/georeferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2024.5.1.1/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py` & `pami-2024.5.1.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2024.5.1.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/highUtilityFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py` & `pami-2024.5.1.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py` & `pami-2024.5.1.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2024.5.1.1/PAMI/highUtilityPattern/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2024.5.1.1/PAMI/highUtilityPattern/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2024.5.1.1/PAMI/highUtilityPattern/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/highUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2024.5.1.1/PAMI/highUtilityPattern/basic/efimParallel.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2024.5.1.1/PAMI/highUtilityPattern/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2024.5.1.1/PAMI/highUtilityPattern/parallel/efimparallel.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2024.5.1.1/PAMI/highUtilityPatternsInStreams/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2024.5.1.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2024.5.1.1/PAMI/highUtilityPatternsInStreams/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2024.5.1.1/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/__init__.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/pyspark/__init__.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/pyspark/abstract.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py` & `pami-2024.5.1.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2024.5.1.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/__init__.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# PFECLAT is the fundamental approach to mine the periodic-frequent patterns.
-#
+# PFPMC is the fundamental approach to mine the periodic-frequent patterns.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
+#             from PAMI.periodicFrequentPattern.basic import PFPMC as alg
 #
-#             obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
+#             obj = alg.PFPMC("../basic/sampleTDB.txt", "2", "5")
 #
 #             obj.startMine()
 #
 #             periodicFrequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 #
@@ -30,15 +29,14 @@
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
-
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -53,25 +51,25 @@
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 from PAMI.periodicFrequentPattern.basic import abstract as _ab
 import pandas as pd
 from deprecated import deprecated
-import numpy as np
-
+from itertools import groupby as _groupby
+from operator import itemgetter as _itemgetter
 from PAMI.periodicFrequentPattern.basic import abstract as _ab
+from typing import List, Dict, Tuple, Set, Union, Any, Generator
 
 
-class PFECLAT(_ab._periodicFrequentPatterns):
+class PFPMC(_ab._periodicFrequentPatterns):
     """
-    :Description:   PFECLAT is the fundamental approach to mine the periodic-frequent patterns.
+    :Description:   PFPMC is the fundamental approach to mine the periodic-frequent patterns.
 
-    :Reference:   P. Ravikumar, P.Likhitha, R. Uday kiran, Y. Watanobe, and Koji Zettsu, "Towards efficient discovery of
-                  periodic-frequent patterns in columnar temporal databases", 2021 IEA/AIE.
+    :Reference: (has to be added)
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of periodic frequent pattern's
     :param  oFile: str :
                    Name of the output file to store complete set of periodic frequent pattern's
     :param  minSup: str:
                    Controls the minimum number of transactions in which every item must appear in a database.
@@ -99,17 +97,17 @@
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-        startTime : float
+        startTime:float
             To record the start time of the mining process
-        endTime : float
+        endTime:float
             To record the completion time of the mining process
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
             it represents the total no of transactions
@@ -127,56 +125,54 @@
     :Methods:
 
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of periodic-frequent patterns will be loaded in to a output file
+            Complete set of periodic-frequent patterns will be loaded in to an output file
         getPatternsAsDataFrame()
             Complete set of periodic-frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingOneItemSets()
-            Scan the database and store the items with their timestamps which are periodic frequent 
+            Scan the database and store the items with their timestamps which are periodic frequent
         getPeriodAndSupport()
             Calculates the support and period for a list of timestamps.
         Generation()
             Used to implement prefix class equivalence method to generate the periodic patterns recursively
-            
+
 
     **Methods to execute code on terminal**
     ------------------------------------------
     .. code-block:: console
 
 
        Format:
 
-       (.venv) $ python3 PFECLAT.py <inputFile> <outputFile> <minSup>
+       (.venv) $ python3 PFPMC.py <inputFile> <outputFile> <minSup> <maxPer>
 
        Example usage:
 
-       (.venv) $ python3 PFECLAT.py sampleDB.txt patterns.txt 10.0
-
-
+       (.venv) $ python3 PFPMC.py sampleDB.txt patterns.txt 10.0 4.0
 
-               .. note:: minSup will be considered in percentage of database transactions
 
+               .. note:: minSup and maxPer will be considered in percentage of database transactions
 
     **Importing this algorithm into a python program**
-    --------------------------------------------------------
+    ----------------------------------------------------
     .. code-block:: python
 
-             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
+                from PAMI.periodicFrequentPattern.basic import PFPMC as alg
 
-                obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
+                obj = alg.PFPMC("../basic/sampleTDB.txt", "2", "5")
 
                 obj.startMine()
 
                 periodicFrequentPatterns = obj.getPatterns()
 
                 print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 
@@ -193,33 +189,96 @@
                 print("Total Memory in RSS", memRSS)
 
                 run = obj.getRuntime()
 
                 print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
-    --------------
-             The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
+    ----------------
+
+    The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
     """
-    
+
     _iFile = " "
     _oFile = " "
     _sep = " "
     _dbSize = None
     _Database = None
     _minSup = str()
     _maxPer = str()
     _tidSet = set()
     _finalPatterns = {}
     _startTime = None
     _endTime = None
+    _lastTid = int()
     _memoryUSS = float()
     _memoryRSS = float()
 
+    def _getPeriodic(self, tids: set) -> int:
+        """
+        To get  Periodic frequent patterns
+
+        :param tids: represents the timestamp of a transaction
+        :type tids: set
+        :return: None
+        """
+        tids = list(tids)
+        tids.sort()
+        temp = self._maxPer + 1
+        diffs = []
+        if self._lastTid in tids:
+            tids.remove(self._lastTid)
+        for k, g in _groupby(enumerate(tids), lambda ix: ix[0] - ix[1]):
+            diffs.append(len(list(map(_itemgetter(1), g))))
+        if len(diffs) < 1:
+            return temp
+        return max(diffs) + 1
+
+    def _getPeriodic(self, tids: set):
+
+        tids = list(tids)
+        tids.sort()
+        temp = self._maxPer + 1
+        if self._lastTid in tids:
+            tids.remove(self._lastTid)
+        diffs = []
+        # find the longest consecutive period
+
+        count = 0
+        for i in range(len(tids) - 1):
+            if tids[i + 1] == tids[i] + 1:
+                count += 1
+            else:
+                diffs.append(count)
+                count = 0
+        if len(diffs) < 1:
+            return temp
+        return max(diffs) + 1
+
+    def _getPeriodic(self, tids: set):
+        tids = list(tids)
+        tids.sort()
+        temp = self._maxPer + 1
+        if self._lastTid in tids:
+            tids.remove(self._lastTid)
+        diffs = []
+        tempPer = 0
+        period = 0
+        for i in range(len(tids) - 1):
+            if tids[i+1] - tids[i] == 1:
+                tempPer += 1
+            else:
+                period = max(period, tempPer + 1)
+                if period > self._maxPer:
+                    return temp
+                tempPer = 0
+
+        return period
+
     def _convert(self, value) -> float:
         """
         To convert the given user specified value
 
         :param value: user specified value
         :return: converted value
         """
@@ -231,172 +290,145 @@
             if '.' in value:
                 value = float(value)
                 value = (self._dbSize * value)
             else:
                 value = int(value)
         return value
 
-    def _creatingItemSets(self) -> None:
+    def _creatingOneItemSets(self) -> list:
         """
-            Storing the complete transactions of the database/input file in a database variable
-        :return: None
+        Storing the complete transactions of the database/input file in a database variable
+        :return: list
         """
-        self._Database = []
+        plist = []
+        Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            data, ts = [], []
+            ts, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'TS' in i:
                 ts = self._iFile['TS'].tolist()
             if 'Transactions' in i:
                 data = self._iFile['Transactions'].tolist()
             for i in range(len(data)):
                 tr = [ts[i][0]]
                 tr = tr + data[i]
-                self._Database.append(tr)
-
+                Database.append(tr)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._Database.append(temp)
+                    Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
+        tid = 0
+        itemsets = {}  # {key: item, value: list of tids}
+        periodicHelper = {}  # {key: item, value: [period, last_tid]}
+        for line in Database:
+            tid = int(line[0])
+            self._tidSet.add(tid)
+            for item in line[1:]:
+                if item in itemsets:
+                    itemsets[item].add(tid)
+                else:
+                    itemsets[item] = {tid}
 
-    @deprecated("It is recommended to use mine() instead of startMine() for mining process")
-    def startMine(self) -> None:
-        """
-        Mining process will start from this function
-        :return: None
-        """
-        self.Mine()
-        # self._startTime = _ab._time.time()
-        # self._finalPatterns = {}
-        # frequentSets = self._creatingOneItemSets()
-        # self._generateEclat(frequentSets)
-        # self._endTime = _ab._time.time()
-        # process = _ab._psutil.Process(_ab._os.getpid())
-        # self._memoryRSS = float()
-        # self._memoryUSS = float()
-        # self._memoryUSS = process.memory_full_info().uss
-        # self._memoryRSS = process.memory_info().rss
-        # print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
-
-    def _getMaxPer(self, arr, maxTS):
-        arr = np.append(list(arr), [0, maxTS])
-        arr = np.sort(arr)
-        arr = np.diff(arr)
+        self._dbSize = len(Database)
+        self._lastTid = max(self._tidSet)
+        self._minSup = self._convert(self._minSup)
+        self._maxPer = self._convert(self._maxPer)
+        del Database
+        candidates = []
+        for item, tids in itemsets.items():
+            diff = self._tidSet.difference(tids)
+            per = self._getPeriodic(diff)
+            sup = len(tids)
+            if sup >= self._minSup and per <= self._maxPer:
+                candidates.append(item)
+                self._finalPatterns[item] = [sup, per, diff]
+        return candidates
+
+    def _generateDiffsetEclat(self, candidates: list) -> None:
+        new_freqList = []
+        for i in range(0, len(candidates)):
+            item1 = candidates[i]
+            i1_list = item1.split()
+            for j in range(i + 1, len(candidates)):
+                item2 = candidates[j]
+                i2_list = item2.split()
+                if i1_list[:-1] == i2_list[:-1]:
+                    union_DiffSet = self._finalPatterns[item2][2].union(self._finalPatterns[item1][2])
+                    sorted(union_DiffSet)
+                    union_supp = self._dbSize - len(union_DiffSet)
+                    period = self._getPeriodic(union_DiffSet)
+                    if union_supp >= self._minSup and period <= self._maxPer:
+                        newKey = item1 + "\t" + i2_list[-1]
+                        self._finalPatterns[newKey] = [union_supp, period, union_DiffSet]
+                        new_freqList.append(newKey)
+                else:
+                    break
 
-        return np.max(arr)
+        if len(new_freqList) > 0:
+            self._generateDiffsetEclat(new_freqList)
 
-    def Mine(self) -> None:
+    def startMine(self) -> None:
         """
         Mining process will start from this function
         :return: None
         """
+        # print(f"Optimized {type(self).__name__}")
         self._startTime = _ab._time.time()
         self._finalPatterns = {}
-        frequentSets = self._creatingItemSets()
-
-        items = {}
-        maxTS = 0
-        for line in self._Database:
-            index = int(line[0])
-            maxTS = max(maxTS, index)
-            for item in line[1:]:
-                if tuple([item]) not in items:
-                    items[tuple([item])] = set()
-                items[tuple([item])].add(index)
-
-        self._dbSize = maxTS
-
-        self._minSup = self._convert(self._minSup)
-        self._maxPer = self._convert(self._maxPer)
-        minSup = self._minSup
-        maxPer = self._maxPer
-
-
-        items = {k: v for k, v in items.items() if len(v) >= minSup}
-        items = {k: v for k, v in sorted(items.items(), key = lambda x: len(x[1]), reverse = True)}
-
-        keys = []
-        for item in list(items.keys()):
-            per = self._getMaxPer(items[item], maxTS)
-            if per <= maxPer:
-                keys.append(item)
-                self._finalPatterns[item] = [len(items[item]), per, set(items[item])]
-
-        while keys:
-            newKeys = []
-            for i in range(len(keys)):
-                for j in range(i + 1, len(keys)):
-                    if keys[i][:-1] == keys[j][:-1] and keys[i][-1] != keys[j][-1]:
-                        # print(keys[i], keys[j])
-                        newKey = tuple(keys[i] + (keys[j][-1],))
-                        intersect = items[keys[i]].intersection(items[keys[j]])
-                        per = self._getMaxPer(intersect, maxTS)
-                        sup = len(intersect)
-                        if sup >= minSup and per <= maxPer:
-                            items[newKey] = intersect
-                            newKeys.append(newKey)
-                            self._finalPatterns[newKey] = [sup, per, set(intersect)]
-                    else:
-                        break
-            keys = newKeys
-
-        newPattern = {}
-        for k, v in self._finalPatterns.items():
-            newPattern["\t".join([str(x) for x in k])] = v
-
-        self._finalPatterns = newPattern
-
-        # self._generateEclat(frequentSets)
+        frequentSets = self._creatingOneItemSets()
+        self._generateDiffsetEclat(frequentSets)
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryRSS = float()
         self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
+        print("Periodic-Frequent patterns were generated successfully using PFPDiffset ECLAT algorithm ")
 
     def getMemoryUSS(self) -> float:
-        """Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """
+        Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self) -> float:
-        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """
+        Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self) -> float:
-        """Calculating the total amount of runtime taken by the mining process
-
+        """
+        Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
@@ -413,15 +445,15 @@
         for a, b in self._finalPatterns.items():
             data.append([a, b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
         return dataframe
 
     def save(self, outFile: str) -> None:
         """
-        Complete set of periodic-frequent patterns will be loaded in to a output file
+        Complete set of periodic-frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csv file
         :return: None
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -444,23 +476,23 @@
         This function is used to print the results
         :return: None
         """
         print("Total number of Periodic Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
-                    
+
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
-            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
+            _ap = PFPMC(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = PFPMC(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
         print("Total number of Periodic-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
```

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/_PFECLAT.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# PFPMC is the fundamental approach to mine the periodic-frequent patterns.
+# PFECLAT is the fundamental approach to mine the periodic-frequent patterns.
+#
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.periodicFrequentPattern.basic import PFPMC as alg
+#             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
 #
-#             obj = alg.PFPMC("../basic/sampleTDB.txt", "2", "5")
+#             obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
 #
 #             obj.startMine()
 #
 #             periodicFrequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 #
@@ -29,14 +30,15 @@
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -51,25 +53,24 @@
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 from PAMI.periodicFrequentPattern.basic import abstract as _ab
 import pandas as pd
 from deprecated import deprecated
-from itertools import groupby as _groupby
-from operator import itemgetter as _itemgetter
+
 from PAMI.periodicFrequentPattern.basic import abstract as _ab
-from typing import List, Dict, Tuple, Set, Union, Any, Generator
 
 
-class PFPMC(_ab._periodicFrequentPatterns):
+class PFECLAT(_ab._periodicFrequentPatterns):
     """
-    :Description:   PFPMC is the fundamental approach to mine the periodic-frequent patterns.
+    :Description:   PFECLAT is the fundamental approach to mine the periodic-frequent patterns.
 
-    :Reference: (has to be added)
+    :Reference:   P. Ravikumar, P.Likhitha, R. Uday kiran, Y. Watanobe, and Koji Zettsu, "Towards efficient discovery of
+                  periodic-frequent patterns in columnar temporal databases", 2021 IEA/AIE.
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of periodic frequent pattern's
     :param  oFile: str :
                    Name of the output file to store complete set of periodic frequent pattern's
     :param  minSup: str:
                    Controls the minimum number of transactions in which every item must appear in a database.
@@ -97,17 +98,17 @@
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-        startTime:float
+        startTime : float
             To record the start time of the mining process
-        endTime:float
+        endTime : float
             To record the completion time of the mining process
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
             it represents the total no of transactions
@@ -125,54 +126,56 @@
     :Methods:
 
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of periodic-frequent patterns will be loaded in to an output file
+            Complete set of periodic-frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
             Complete set of periodic-frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingOneItemSets()
-            Scan the database and store the items with their timestamps which are periodic frequent
+            Scan the database and store the items with their timestamps which are periodic frequent 
         getPeriodAndSupport()
             Calculates the support and period for a list of timestamps.
         Generation()
             Used to implement prefix class equivalence method to generate the periodic patterns recursively
-
+            
 
     **Methods to execute code on terminal**
     ------------------------------------------
     .. code-block:: console
 
 
        Format:
 
-       (.venv) $ python3 PFPMC.py <inputFile> <outputFile> <minSup> <maxPer>
+       (.venv) $ python3 PFECLAT.py <inputFile> <outputFile> <minSup>
 
        Example usage:
 
-       (.venv) $ python3 PFPMC.py sampleDB.txt patterns.txt 10.0 4.0
+       (.venv) $ python3 PFECLAT.py sampleDB.txt patterns.txt 10.0
+
 
 
-               .. note:: minSup and maxPer will be considered in percentage of database transactions
+               .. note:: minSup will be considered in percentage of database transactions
+
 
     **Importing this algorithm into a python program**
-    ----------------------------------------------------
+    --------------------------------------------------------
     .. code-block:: python
 
-                from PAMI.periodicFrequentPattern.basic import PFPMC as alg
+             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
 
-                obj = alg.PFPMC("../basic/sampleTDB.txt", "2", "5")
+                obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
 
                 obj.startMine()
 
                 periodicFrequentPatterns = obj.getPatterns()
 
                 print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 
@@ -189,95 +192,45 @@
                 print("Total Memory in RSS", memRSS)
 
                 run = obj.getRuntime()
 
                 print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
-    ----------------
-
-    The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+    --------------
+             The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
     """
-
+    
     _iFile = " "
     _oFile = " "
     _sep = " "
     _dbSize = None
     _Database = None
     _minSup = str()
     _maxPer = str()
     _tidSet = set()
     _finalPatterns = {}
     _startTime = None
     _endTime = None
-    _lastTid = int()
     _memoryUSS = float()
     _memoryRSS = float()
 
     def _getPeriodic(self, tids: set) -> int:
-        """
-        To get  Periodic frequent patterns
-
-        :param tids: represents the timestamp of a transaction
-        :type tids: set
-        :return: None
-        """
-        tids = list(tids)
-        tids.sort()
-        temp = self._maxPer + 1
-        diffs = []
-        if self._lastTid in tids:
-            tids.remove(self._lastTid)
-        for k, g in _groupby(enumerate(tids), lambda ix: ix[0] - ix[1]):
-            diffs.append(len(list(map(_itemgetter(1), g))))
-        if len(diffs) < 1:
-            return temp
-        return max(diffs) + 1
-
-    def _getPeriodic(self, tids: set):
-
-        tids = list(tids)
-        tids.sort()
-        temp = self._maxPer + 1
-        if self._lastTid in tids:
-            tids.remove(self._lastTid)
-        diffs = []
-        # find the longest consecutive period
-
-        count = 0
-        for i in range(len(tids) - 1):
-            if tids[i + 1] == tids[i] + 1:
-                count += 1
-            else:
-                diffs.append(count)
-                count = 0
-        if len(diffs) < 1:
-            return temp
-        return max(diffs) + 1
-
-    def _getPeriodic(self, tids: set):
-        tids = list(tids)
-        tids.sort()
-        temp = self._maxPer + 1
-        if self._lastTid in tids:
-            tids.remove(self._lastTid)
-        diffs = []
-        tempPer = 0
-        period = 0
-        for i in range(len(tids) - 1):
-            if tids[i+1] - tids[i] == 1:
-                tempPer += 1
-            else:
-                period = max(period, tempPer + 1)
-                if period > self._maxPer:
-                    return temp
-                tempPer = 0
-
-        return period
+        tidList = list(tids)
+        tidList.sort()
+        tidList.append(self._dbSize)
+        cur = 0
+        per = 0
+        for tid in tidList:
+            per = max(per, tid - cur)
+            if per > self._maxPer:  # early stopping
+                break
+            cur = tid
+        return per
 
     def _convert(self, value) -> float:
         """
         To convert the given user specified value
 
         :param value: user specified value
         :return: converted value
@@ -339,96 +292,115 @@
         periodicHelper = {}  # {key: item, value: [period, last_tid]}
         for line in Database:
             tid = int(line[0])
             self._tidSet.add(tid)
             for item in line[1:]:
                 if item in itemsets:
                     itemsets[item].add(tid)
+                    periodicHelper[item][0] = max(periodicHelper[item][0],
+                                                  abs(tid - periodicHelper[item][1]))  # update current max period
+                    periodicHelper[item][1] = tid  # update the last tid
                 else:
                     itemsets[item] = {tid}
+                    periodicHelper[item] = [abs(0 - tid), tid]  # initialize helper
 
+        # finish all items' period
         self._dbSize = len(Database)
-        self._lastTid = max(self._tidSet)
         self._minSup = self._convert(self._minSup)
         self._maxPer = self._convert(self._maxPer)
         del Database
+        for item, _ in periodicHelper.items():
+            periodicHelper[item][0] = max(periodicHelper[item][0],
+                                          abs(self._dbSize - periodicHelper[item][1]))  # tid of the last transaction
         candidates = []
         for item, tids in itemsets.items():
-            diff = self._tidSet.difference(tids)
-            per = self._getPeriodic(diff)
+            per = periodicHelper[item][0]
             sup = len(tids)
             if sup >= self._minSup and per <= self._maxPer:
                 candidates.append(item)
-                self._finalPatterns[item] = [sup, per, diff]
+                self._finalPatterns[item] = [sup, per, tids]
         return candidates
+    
+    def _generateEclat(self, candidates: list) -> None:
 
-    def _generateDiffsetEclat(self, candidates: list) -> None:
-        new_freqList = []
+        newCandidates = []
         for i in range(0, len(candidates)):
-            item1 = candidates[i]
-            i1_list = item1.split()
+            prefixItem = candidates[i]
+            prefixItemSet = prefixItem.split()
             for j in range(i + 1, len(candidates)):
-                item2 = candidates[j]
-                i2_list = item2.split()
-                if i1_list[:-1] == i2_list[:-1]:
-                    union_DiffSet = self._finalPatterns[item2][2].union(self._finalPatterns[item1][2])
-                    sorted(union_DiffSet)
-                    union_supp = self._dbSize - len(union_DiffSet)
-                    period = self._getPeriodic(union_DiffSet)
-                    if union_supp >= self._minSup and period <= self._maxPer:
-                        newKey = item1 + "\t" + i2_list[-1]
-                        self._finalPatterns[newKey] = [union_supp, period, union_DiffSet]
-                        new_freqList.append(newKey)
-                else:
-                    break
+                item = candidates[j]
+                itemSet = item.split()
+                if prefixItemSet[:-1] == itemSet[:-1] and prefixItemSet[-1] != itemSet[-1]:
+                    _value = self._finalPatterns[item][2].intersection(self._finalPatterns[prefixItem][2])
+                    sup = len(_value)
+                    per = self._getPeriodic(_value)
+                    if sup >= self._minSup and per <= self._maxPer:
+                        newItem = prefixItem + "\t" + itemSet[-1]
+                        self._finalPatterns[newItem] = [sup, per, _value]
+                        newCandidates.append(newItem)
 
-        if len(new_freqList) > 0:
-            self._generateDiffsetEclat(new_freqList)
+        if len(newCandidates) > 0:
+            self._generateEclat(newCandidates)
 
+    @deprecated("It is recommended to use mine() instead of startMine() for mining process")
     def startMine(self) -> None:
         """
         Mining process will start from this function
         :return: None
         """
-        # print(f"Optimized {type(self).__name__}")
         self._startTime = _ab._time.time()
         self._finalPatterns = {}
         frequentSets = self._creatingOneItemSets()
-        self._generateDiffsetEclat(frequentSets)
+        self._generateEclat(frequentSets)
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryRSS = float()
         self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Periodic-Frequent patterns were generated successfully using PFPDiffset ECLAT algorithm ")
+        print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
 
-    def getMemoryUSS(self) -> float:
+    def Mine(self) -> None:
         """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        Mining process will start from this function
+        :return: None
+        """
+        self._startTime = _ab._time.time()
+        self._finalPatterns = {}
+        frequentSets = self._creatingOneItemSets()
+        self._generateEclat(frequentSets)
+        self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
+        self._memoryRSS = float()
+        self._memoryUSS = float()
+        self._memoryUSS = process.memory_full_info().uss
+        self._memoryRSS = process.memory_info().rss
+        print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
+
+    def getMemoryUSS(self) -> float:
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self) -> float:
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self) -> float:
-        """
-        Calculating the total amount of runtime taken by the mining process
+        """Calculating the total amount of runtime taken by the mining process
+
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
@@ -445,15 +417,15 @@
         for a, b in self._finalPatterns.items():
             data.append([a, b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
         return dataframe
 
     def save(self, outFile: str) -> None:
         """
-        Complete set of periodic-frequent patterns will be loaded in to an output file
+        Complete set of periodic-frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
         :type outFile: csv file
         :return: None
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -476,24 +448,24 @@
         This function is used to print the results
         :return: None
         """
         print("Total number of Periodic Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
-
+                    
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
-            _ap = PFPMC(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
+            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = PFPMC(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
         print("Total number of Periodic-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/_PFECLAT.py` & `pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# PFECLAT is the fundamental approach to mine the periodic-frequent patterns.
-#
+# TUFP is one of the fundamental algorithm to discover top-k frequent patterns in a uncertain transactional database using CUP-Lists.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
+#             from PAMI.uncertainFrequentPattern.basic import TUFP as alg
+#
+#             iFile = 'sampleDB.txt'
 #
-#             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
+#             minSup = 10  # can also be specified between 0 and 1
 #
-#             obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
+#             obj = alg.TUFP(iFile, minSup)
 #
 #             obj.startMine()
 #
-#             periodicFrequentPatterns = obj.getPatterns()
+#             frequentPatterns = obj.getPatterns()
 #
-#             print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+#             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#             obj.save("patterns")
+#             obj.save(oFile)
 #
 #             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
@@ -29,443 +31,544 @@
 #
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
-
-
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
-
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
-
+     
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
-
+     
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-     Copyright (C)  2021 Rage Uday Kiran
-
 """
 
-from PAMI.periodicFrequentPattern.basic import abstract as _ab
+from PAMI.uncertainFrequentPattern.basic import abstract as _ab
+from typing import List, Dict, Union
 import pandas as pd
 from deprecated import deprecated
 
-from PAMI.periodicFrequentPattern.basic import abstract as _ab
+_minSup = float()
+_finalPatterns = {}
+
+
+class _Item:
+    """
+    A class used to represent the item with probability in transaction of dataset
+
+    :Attributes:
 
+        item : int or word
+          Represents the name of the item
 
-class PFECLAT(_ab._periodicFrequentPatterns):
+        probability : float
+          Represent the existential probability(likelihood presence) of an item
     """
-    :Description:   PFECLAT is the fundamental approach to mine the periodic-frequent patterns.
 
-    :Reference:   P. Ravikumar, P.Likhitha, R. Uday kiran, Y. Watanobe, and Koji Zettsu, "Towards efficient discovery of
-                  periodic-frequent patterns in columnar temporal databases", 2021 IEA/AIE.
+    def __init__(self, item, probability) -> None:
+        self.item = item
+        self.probability = probability
 
-    :param  iFile: str :
-                   Name of the Input file to mine complete set of periodic frequent pattern's
-    :param  oFile: str :
-                   Name of the output file to store complete set of periodic frequent pattern's
-    :param  minSup: str:
-                   Controls the minimum number of transactions in which every item must appear in a database.
-    :param  maxPer: str:
-                   Controls the maximum number of transactions in which any two items within a pattern can reappear.
-    :param  sep: str :
-                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
+
+class TUFP(_ab._frequentPatterns):
+    """
+    About this algorithm
+    ====================
+
+    :Description: It is one of the fundamental algorithm to discover top-k frequent patterns in a uncertain transactional database using CUP-Lists.
+
+    :Reference:  Tuong Le, Bay Vo, Van-Nam Huynh, Ngoc Thanh Nguyen, Sung Wook Baik 5, "Mining top-k frequent patterns from uncertain databases",
+                 Springer Science+Business Media, LLC, part of Springer Nature 2020, https://doi.org/10.1007/s10489-019-01622-1
 
     :Attributes:
 
         iFile : file
             Name of the Input file or path of the input file
+
         oFile : file
             Name of the output file or path of the output file
-        minSup : int or float or str
+
+        minSup : float or int or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        maxPer : int or float or str
-            The user can specify maxPer either in count or proportion of database size.
-            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
+
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
+
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
+
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
+
         startTime : float
             To record the start time of the mining process
+
         endTime : float
             To record the completion time of the mining process
+
         Database : list
             To store the transactions of a database in list
+
         mapSupport : Dictionary
             To maintain the information of item and their frequency
+
         lno : int
-            it represents the total no of transactions
+            To represent the total no of transaction
+
         tree : class
-            it represents the Tree class
+            To represents the Tree class
+
         itemSetCount : int
-            it represents the total no of patterns
+            To represents the total no of patterns
+
         finalPatterns : dict
-            it represents to store the patterns
-        tidList : dict
-            stores the timestamps of an item
-        hashing : dict
-            stores the patterns with their support to check for the closed property
+            To store the complete patterns
 
     :Methods:
-
-        startMine()
+        mine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
-        save(oFile)
-            Complete set of periodic-frequent patterns will be loaded in to a output file
-        getPatternsAsDataFrame()
-            Complete set of periodic-frequent patterns will be loaded in to a dataframe
+        storePatternsInFile(oFile)
+            Complete set of frequent patterns will be loaded in to a output file
+        getPatternsInDataFrame()
+            Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingOneItemSets()
-            Scan the database and store the items with their timestamps which are periodic frequent 
-        getPeriodAndSupport()
-            Calculates the support and period for a list of timestamps.
-        Generation()
-            Used to implement prefix class equivalence method to generate the periodic patterns recursively
-            
+        creatingItemSets(fileName)
+            Scans the dataset and stores in a list format
+        frequentOneItem()
+            Extracts the one-length frequent patterns from database
+        updateTransactions()
+            Update the transactions by removing non-frequent items and sort the Database by item decreased support
+        buildTree()
+            After updating the Database, remaining items will be added into the tree by setting root node as null
+        convert()
+            to convert the user specified value
+        startMine()
+            Mining process will start from this function
 
-    **Methods to execute code on terminal**
-    ------------------------------------------
-    .. code-block:: console
+    Execution methods
+    =================
 
 
-       Format:
+    **Terminal command**
+
+
+    .. code-block:: console
 
-       (.venv) $ python3 PFECLAT.py <inputFile> <outputFile> <minSup>
+      Format:
 
-       Example usage:
+      (.venv) $ python3 TUFP.py <inputFile> <outputFile> <minSup>
 
-       (.venv) $ python3 PFECLAT.py sampleDB.txt patterns.txt 10.0
+      Example Usage:
 
+      (.venv) $ python3 TUFP.py sampleDB.txt patterns.txt 0.6
 
+    .. note:: minSup can be specified  in support count or a value between 0 and 1.
 
-               .. note:: minSup will be considered in percentage of database transactions
 
+    **Calling from a python program**
 
-    **Importing this algorithm into a python program**
-    --------------------------------------------------------
     .. code-block:: python
 
-             from PAMI.periodicFrequentPattern.basic import PFECLAT as alg
+            from PAMI.uncertainFrequentPattern.basic import TUFP as alg
 
-                obj = alg.PFECLAT("../basic/sampleTDB.txt", "2", "5")
+            iFile = 'sampleDB.txt'
 
-                obj.startMine()
+            minSup = 10  # can also be specified between 0 and 1
 
-                periodicFrequentPatterns = obj.getPatterns()
+            obj = alg.TUFP(iFile, minSup)
 
-                print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+            obj.startMine()
 
-                obj.save("patterns")
+            frequentPatterns = obj.getPatterns()
 
-                Df = obj.getPatternsAsDataFrame()
+            print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-                memUSS = obj.getMemoryUSS()
+            obj.save(oFile)
 
-                print("Total Memory in USS:", memUSS)
+            Df = obj.getPatternsAsDataFrame()
 
-                memRSS = obj.getMemoryRSS()
+            memUSS = obj.getMemoryUSS()
 
-                print("Total Memory in RSS", memRSS)
+            print("Total Memory in USS:", memUSS)
 
-                run = obj.getRuntime()
+            memRSS = obj.getMemoryRSS()
 
-                print("Total ExecutionTime in seconds:", run)
+            print("Total Memory in RSS", memRSS)
 
-    **Credits:**
-    --------------
-             The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
+            run = obj.getRuntime()
 
+            print("Total ExecutionTime in seconds:", run)
+
+    Credits
+    =======
+
+
+            The complete program was written by   P.Likhitha   under the supervision of Professor Rage Uday Kiran.
     """
-    
+
+    _startTime = float()
+    _endTime = float()
+    _minSup = str()
+    _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    _dbSize = None
-    _Database = None
-    _minSup = str()
-    _maxPer = str()
-    _tidSet = set()
-    _finalPatterns = {}
-    _startTime = None
-    _endTime = None
     _memoryUSS = float()
     _memoryRSS = float()
+    _Database = []
+    _cupList = {}
+    _topk = {}
+    _minimum = 9999
 
-    def _getPeriodic(self, tids: set) -> int:
-        tidList = list(tids)
-        tidList.sort()
-        tidList.append(self._dbSize)
-        cur = 0
-        per = 0
-        for tid in tidList:
-            per = max(per, tid - cur)
-            if per > self._maxPer:  # early stopping
-                break
-            cur = tid
-        return per
-
-    def _convert(self, value) -> float:
-        """
-        To convert the given user specified value
 
-        :param value: user specified value
-        :return: converted value
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (self._dbSize * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (self._dbSize * value)
-            else:
-                value = int(value)
-        return value
 
-    def _creatingOneItemSets(self) -> list:
+    def _creatingItemSets(self) -> None:
         """
-        Storing the complete transactions of the database/input file in a database variable
-        :return: list
+        Scans the dataset
         """
-        plist = []
-        Database = []
+        self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            ts, data = [], []
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
-            if 'TS' in i:
-                ts = self._iFile['TS'].tolist()
             if 'Transactions' in i:
-                data = self._iFile['Transactions'].tolist()
-            for i in range(len(data)):
-                tr = [ts[i][0]]
-                tr = tr + data[i]
-                Database.append(tr)
+                self._Database = self._iFile['Transactions'].tolist()
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
+
+            # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    Database.append(temp)
+                    tr = []
+                    for i in temp:
+                        i1 = i.index('(')
+                        i2 = i.index(')')
+                        item = i[0:i1]
+                        probability = float(i[i1 + 1:i2])
+                        product = _Item(item, probability)
+                        tr.append(product)
+                    self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            Database.append(temp)
+                            tr = []
+                            for i in temp:
+                                i1 = i.index('(')
+                                i2 = i.index(')')
+                                item = i[0:i1]
+                                probability = float(i[i1 + 1:i2])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
-        tid = 0
-        itemsets = {}  # {key: item, value: list of tids}
-        periodicHelper = {}  # {key: item, value: [period, last_tid]}
-        for line in Database:
-            tid = int(line[0])
-            self._tidSet.add(tid)
-            for item in line[1:]:
-                if item in itemsets:
-                    itemsets[item].add(tid)
-                    periodicHelper[item][0] = max(periodicHelper[item][0],
-                                                  abs(tid - periodicHelper[item][1]))  # update current max period
-                    periodicHelper[item][1] = tid  # update the last tid
+
+    def _frequentOneItem(self) -> List[str]:
+        """
+        Takes the self.Database and calculates the support of each item in the dataset and assign the ranks to the items by decreasing support and returns the frequent items list
+
+        :param self.Database : it represents the one self.Database in database
+        :type self.Database : list
+        """
+
+        mapSupport = {}
+        k = 0
+        for i in self._Database:
+            k += 1
+            for j in i:
+                if j.item not in mapSupport:
+                    mapSupport[j.item] = j.probability
+                    self._cupList[j.item] = {k:j.probability}
                 else:
-                    itemsets[item] = {tid}
-                    periodicHelper[item] = [abs(0 - tid), tid]  # initialize helper
+                    mapSupport[j.item] += j.probability
+                    self._cupList[j.item].update({k: j.probability})
+        plist = [k for k,v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        k = 0
+        for x, in plist:
+            k +=1
+            if k >= self._minSup:
+                break
+            self._finalPatterns[x] = mapSupport[x]
+        self._minimum = min(list(self._finalPatterns.values()))
+        return plist
 
-        # finish all items' period
-        self._dbSize = len(Database)
-        self._minSup = self._convert(self._minSup)
-        self._maxPer = self._convert(self._maxPer)
-        del Database
-        for item, _ in periodicHelper.items():
-            periodicHelper[item][0] = max(periodicHelper[item][0],
-                                          abs(self._dbSize - periodicHelper[item][1]))  # tid of the last transaction
-        candidates = []
-        for item, tids in itemsets.items():
-            per = periodicHelper[item][0]
-            sup = len(tids)
-            if sup >= self._minSup and per <= self._maxPer:
-                candidates.append(item)
-                self._finalPatterns[item] = [sup, per, tids]
-        return candidates
-    
-    def _generateEclat(self, candidates: list) -> None:
-
-        newCandidates = []
-        for i in range(0, len(candidates)):
-            prefixItem = candidates[i]
-            prefixItemSet = prefixItem.split()
-            for j in range(i + 1, len(candidates)):
-                item = candidates[j]
-                itemSet = item.split()
-                if prefixItemSet[:-1] == itemSet[:-1] and prefixItemSet[-1] != itemSet[-1]:
-                    _value = self._finalPatterns[item][2].intersection(self._finalPatterns[prefixItem][2])
-                    sup = len(_value)
-                    per = self._getPeriodic(_value)
-                    if sup >= self._minSup and per <= self._maxPer:
-                        newItem = prefixItem + "\t" + itemSet[-1]
-                        self._finalPatterns[newItem] = [sup, per, _value]
-                        newCandidates.append(newItem)
+    @staticmethod
+    def _convert(value: Union[int, float, str]) -> Union[int, float]:
+        """
+        To convert the type of user specified minSup value
+
+        :param value: user specified minSup value
+        :return: converted type minSup value
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = float(value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+            else:
+                value = int(value)
+        return value
 
-        if len(newCandidates) > 0:
-            self._generateEclat(newCandidates)
+    def _save(self, prefix: List[str], suffix: List[str], tidSetI: Dict[int, float]) -> None:
+        """
+        Saves the patterns that satisfy the periodic frequent property.
+
+        :param prefix: the prefix of a pattern
+        :type prefix: list
+        :param suffix: the suffix of a patterns
+        :type suffix: list
+        :param tidSetI: the timestamp of a patterns
+        :type tidSetI: dict
+        """
+
+        if prefix is None:
+            prefix = suffix
+        else:
+            prefix = prefix + suffix
+        val = sum(tidSetI.values())
+        # print(prefix, val)
+        if len(self._finalPatterns) <= self._minSup:
+            sample = str()
+            for i in prefix:
+                sample = sample + i + " "
+            self._finalPatterns[sample] = val
+        if len(self._finalPatterns) == self._minSup:
+            if val > self._minimum:
+                sample = str()
+                for i in prefix:
+                    sample = sample + i + " "
+                index = list(self._finalPatterns.keys())[list(self._finalPatterns.values()).index(self._minimum)]
+                del self._finalPatterns[index]
+                self._finalPatterns[sample] = val
+                self._minimum = min(list(self._finalPatterns.values()))
+        # print(self.finalPatterns, self.minimum, self.minSup)
+
+    def _Generation(self, prefix: List[str], itemSets: List[str], tidSets: List[Dict[int, float]]) -> None:
+        """
+        Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
+
+        :param prefix:  main equivalence prefix
+        :type prefix: periodic-frequent item or pattern
+        :param itemSets: patterns which are items combined with prefix and satisfying the periodicity and frequent with their timestamps
+        :type itemSets: list
+        :param tidSets: timestamps of the items in the argument itemSets
+        :type tidSets: list
+        """
+        if len(itemSets) == 1:
+            i = itemSets[0]
+            tidI = tidSets[0]
+            self._save(prefix, [i], tidI)
+            return
+        for i in range(0, len(itemSets)):
+            itemI = itemSets[i]
+            if itemI is None:
+                continue
+            tidSetI = tidSets[i]
+            classItemSets = []
+            classTidSets = []
+            itemSetX = [itemI]
+            for j in range(i + 1, len(itemSets)):
+                itemJ = itemSets[j]
+                tidSetJ = tidSets[j]
+                y = {key: tidSetJ[key] * tidSetI.get(key, 0) for key in tidSetJ.keys()}
+                sum2 = sum(list(y.values()))
+                # print(prefix, itemJ, y, sum2)
+                # if sum2 >= self.minimum:
+                self._save(prefix, [itemJ], y)
+                classItemSets.append(itemJ)
+                classTidSets.append(y)
+            # print(itemI, tidSetI, classItemSets)
+            newPrefix = list(set(itemSetX)) + prefix
+            self._Generation(newPrefix, classItemSets, classTidSets)
+            # self.save(prefix, list(set(itemSetX)), tidSetI)
 
-    @deprecated("It is recommended to use mine() instead of startMine() for mining process")
+    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
-        Mining process will start from this function
-        :return: None
+        Main method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns
         """
-        self._startTime = _ab._time.time()
-        self._finalPatterns = {}
-        frequentSets = self._creatingOneItemSets()
-        self._generateEclat(frequentSets)
-        self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryRSS = float()
-        self._memoryUSS = float()
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
-        print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
+        self.mine()
 
-    def Mine(self) -> None:
+    def mine(self) -> None:
         """
-        Mining process will start from this function
-        :return: None
+        Main method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns
         """
+        global _minSup
         self._startTime = _ab._time.time()
-        self._finalPatterns = {}
-        frequentSets = self._creatingOneItemSets()
-        self._generateEclat(frequentSets)
+        self._creatingItemSets()
+        self._minSup = self._convert(self._minSup)
+        _minSup = self._minSup
+        plist = self._frequentOneItem()
+        for i in range(len(plist)):
+            itemI = plist[i]
+            tidSetI = self._cupList[itemI]
+            itemSetX = [itemI]
+            itemSets = []
+            tidSets = []
+            for j in range(i + 1, len(plist)):
+                itemJ = plist[j]
+                tidSetJ = self._cupList[itemJ]
+                y1 = {key: tidSetJ[key] * tidSetI.get(key, 0) for key in tidSetJ.keys()}
+                self._save(itemSetX, [itemJ], y1)
+                itemSets.append(itemJ)
+                tidSets.append(y1)
+            self._Generation(itemSetX, itemSets, tidSets)
+        print("Top-K Frequent patterns were generated from uncertain databases successfully using TUFP algorithm")
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryRSS = float()
         self._memoryUSS = float()
+        self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Periodic-Frequent patterns were generated successfully using PFECLAT algorithm ")
 
     def getMemoryUSS(self) -> float:
-        """Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """
+
+        Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self) -> float:
-        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """
+
+        Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self) -> float:
-        """Calculating the total amount of runtime taken by the mining process
+        """
 
+        Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> _ab._pd.DataFrame:
+    def getPatternsAsDataFrame(self) -> pd.DataFrame:
         """
-        Storing final periodic-frequent patterns in a dataframe
 
-        :return: returning periodic-frequent patterns in a dataframe
+        Storing final frequent patterns in a dataframe
+
+        :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a, b[0], b[1]])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
+            data.append([a, b])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile: str) -> None:
         """
-        Complete set of periodic-frequent patterns will be loaded in to a output file
+
+        Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
-        :type outFile: csv file
-        :return: None
+        :type outFile: file
         """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
+        self.oFile = outFile
+        writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x + ":" + str(y[0]) + ":" + str(y[1])
-            #s1 = x.replace(' ', '\t') + ":" + str(y[0]) + ":" + str(y[1])
+            s1 = x + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self) -> dict:
+    def getPatterns(self) -> Dict[str, float]:
         """
-        Function to send the set of periodic-frequent patterns after completion of the mining process
 
-        :return: returning periodic-frequent patterns
+        Function to send the set of frequent patterns after completion of the mining process
+
+        :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self) -> None:
         """
         This function is used to print the results
-        :return: None
         """
-        print("Total number of Periodic Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
-                    
+        print("Total ExecutionTime in ms:", self.getRuntime())
+
+    if __name__ == "__main__":
+        _ap = str()
+        if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+            if len(_ab._sys.argv) == 5:
+                _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            if len(_ab._sys.argv) == 4:
+                _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap.startMine()
+            _ap.mine()
+            _Patterns = _ap.getPatterns()
+            print("Total number of Patterns:", len(_Patterns))
+            _ap.save(_ab._sys.argv[2])
+            _memUSS = _ap.getMemoryUSS()
+            print("Total Memory in USS:", _memUSS)
+            _memRSS = _ap.getMemoryRSS()
+            print("Total Memory in RSS", _memRSS)
+            _run = _ap.getRuntime()
+            print("Total ExecutionTime in ms:", _run)
+        else:
+            '''ap = TUFP("/home/apiiit-rkv/Desktop/uncertain/tubeSample", 10, ' ')
+            ap.startMine()
+            Patterns = ap.getPatterns()
+            print("Total number of Patterns:", len(Patterns))
+            ap.save("patterns.txt")
+            memUSS = ap.getMemoryUSS()
+            print("Total Memory in USS:", memUSS)
+            memRSS = ap.getMemoryRSS()
+            print("Total Memory in RSS", memRSS)
+            run = ap.getRuntime()
+            print("Total ExecutionTime in ms:", run)'''
+            print("Error! The number of input parameters do not match the total number of parameters provided")
 
-if __name__ == "__main__":
-    _ap = str()
-    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
-        if len(_ab._sys.argv) == 6:
-            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
-        if len(_ab._sys.argv) == 5:
-            _ap = PFECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        _ap.startMine()
-        print("Total number of Periodic-Frequent Patterns:", len(_ap.getPatterns()))
-        _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
-        print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
-    else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/_PFPGrowth.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/_PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/pyspark/abstract.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2024.5.1.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2024.5.1.1/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/recurringPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2024.5.1.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/relativeFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2024.5.1.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/relativeHighUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/sequentialPatternMining/basic/SPAM.py` & `pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/SPAM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2024.5.1.1/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2024.5.1.1/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2024.5.1.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/basic/abstract.py` & `pami-2024.5.1.1/PAMI/subgraphMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/basic/dfsCode.py` & `pami-2024.5.1.1/PAMI/subgraphMining/basic/dfsCode.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/basic/edge.py` & `pami-2024.5.1.1/PAMI/subgraphMining/basic/edge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/basic/extendedEdge.py` & `pami-2024.5.1.1/PAMI/subgraphMining/basic/extendedEdge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/basic/frequentSubgraph.py` & `pami-2024.5.1.1/PAMI/subgraphMining/basic/frequentSubgraph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/basic/graph.py` & `pami-2024.5.1.1/PAMI/subgraphMining/basic/graph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/basic/gspan.py` & `pami-2024.5.1.1/PAMI/subgraphMining/basic/gspan.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py` & `pami-2024.5.1.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/basic/vertex.py` & `pami-2024.5.1.1/PAMI/subgraphMining/basic/vertex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/DFSCode.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/DFSCode.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/DFSThread.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/DFSThread.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/abstract.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/edge.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/edge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/extendedEdge.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/extendedEdge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/frequentSubgraph.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/frequentSubgraph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/graph.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/graph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/tkg.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/tkg.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/subgraphMining/topK/vertex.py` & `pami-2024.5.1.1/PAMI/subgraphMining/topK/vertex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py` & `pami-2024.5.1.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py` & `pami-2024.5.1.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2024.5.1.1/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # TUFP is one of the fundamental algorithm to discover top-k frequent patterns in a uncertain transactional database using CUP-Lists.
 #
 # **Importing this algorithm into a python program**
-# --------------------------------------------------------
 #
 #             from PAMI.uncertainFrequentPattern.basic import TUFP as alg
 #
 #             iFile = 'sampleDB.txt'
 #
 #             minSup = 10  # can also be specified between 0 and 1
 #
 #             obj = alg.TUFP(iFile, minSup)
 #
-#             obj.startMine()
+#             obj.mine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
 #             obj.save(oFile)
 #
@@ -47,14 +46,15 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
      
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+
 from PAMI.uncertainFrequentPattern.basic import abstract as _ab
 from typing import List, Dict, Union
 import pandas as pd
 from deprecated import deprecated
 
 _minSup = float()
 _finalPatterns = {}
@@ -175,57 +175,57 @@
 
       Format:
 
       (.venv) $ python3 TUFP.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 TUFP.py sampleDB.txt patterns.txt 0.6
+      (.venv) $ python3 TUFP.py sampleDB.txt patterns.txt 10.0
 
     .. note:: minSup can be specified  in support count or a value between 0 and 1.
 
 
     **Calling from a python program**
 
     .. code-block:: python
 
             from PAMI.uncertainFrequentPattern.basic import TUFP as alg
 
+
             iFile = 'sampleDB.txt'
 
             minSup = 10  # can also be specified between 0 and 1
 
             obj = alg.TUFP(iFile, minSup)
 
-            obj.startMine()
+            obj.mine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
             obj.save(oFile)
 
             Df = obj.getPatternsAsDataFrame()
 
-            memUSS = obj.getMemoryUSS()
+            memUSS = obj.getmemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     Credits
     =======
 
-
             The complete program was written by   P.Likhitha   under the supervision of Professor Rage Uday Kiran.
     """
 
     _startTime = float()
     _endTime = float()
     _minSup = str()
     _finalPatterns = {}
@@ -235,16 +235,14 @@
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
     _cupList = {}
     _topk = {}
     _minimum = 9999
 
-
-
     def _creatingItemSets(self) -> None:
         """
         Scans the dataset
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             uncertain, data = [], []
@@ -359,30 +357,31 @@
         """
 
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
         val = sum(tidSetI.values())
-        # print(prefix, val)
+        #print(prefix, val)
         if len(self._finalPatterns) <= self._minSup:
             sample = str()
             for i in prefix:
                 sample = sample + i + " "
             self._finalPatterns[sample] = val
         if len(self._finalPatterns) == self._minSup:
             if val > self._minimum:
                 sample = str()
                 for i in prefix:
                     sample = sample + i + " "
                 index = list(self._finalPatterns.keys())[list(self._finalPatterns.values()).index(self._minimum)]
                 del self._finalPatterns[index]
                 self._finalPatterns[sample] = val
                 self._minimum = min(list(self._finalPatterns.values()))
-        # print(self.finalPatterns, self.minimum, self.minSup)
+        #print(self.finalPatterns, self.minimum, self.minSup)
+
 
     def _Generation(self, prefix: List[str], itemSets: List[str], tidSets: List[Dict[int, float]]) -> None:
         """
         Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
 
         :param prefix:  main equivalence prefix
         :type prefix: periodic-frequent item or pattern
@@ -400,36 +399,37 @@
             itemI = itemSets[i]
             if itemI is None:
                 continue
             tidSetI = tidSets[i]
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
-            for j in range(i + 1, len(itemSets)):
+            for j in range(i+1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
                 y = {key: tidSetJ[key] * tidSetI.get(key, 0) for key in tidSetJ.keys()}
                 sum2 = sum(list(y.values()))
-                # print(prefix, itemJ, y, sum2)
-                # if sum2 >= self.minimum:
+                #print(prefix, itemJ, y, sum2)
+                #if sum2 >= self.minimum:
                 self._save(prefix, [itemJ], y)
                 classItemSets.append(itemJ)
                 classTidSets.append(y)
-            # print(itemI, tidSetI, classItemSets)
+            #print(itemI, tidSetI, classItemSets)
             newPrefix = list(set(itemSetX)) + prefix
             self._Generation(newPrefix, classItemSets, classTidSets)
-            # self.save(prefix, list(set(itemSetX)), tidSetI)
+            #self.save(prefix, list(set(itemSetX)), tidSetI)
 
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
         Main method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns
         """
         self.mine()
 
+
     def mine(self) -> None:
         """
         Main method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns
         """
         global _minSup
         self._startTime = _ab._time.time()
         self._creatingItemSets()
@@ -438,18 +438,18 @@
         plist = self._frequentOneItem()
         for i in range(len(plist)):
             itemI = plist[i]
             tidSetI = self._cupList[itemI]
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
-            for j in range(i + 1, len(plist)):
+            for j in range(i+1, len(plist)):
                 itemJ = plist[j]
                 tidSetJ = self._cupList[itemJ]
-                y1 = {key: tidSetJ[key] * tidSetI.get(key, 0) for key in tidSetJ.keys()}
+                y1 = {key: tidSetJ[key] * tidSetI.get(key, 0)  for key in tidSetJ.keys()}
                 self._save(itemSetX, [itemJ], y1)
                 itemSets.append(itemJ)
                 tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
         print("Top-K Frequent patterns were generated from uncertain databases successfully using TUFP algorithm")
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
@@ -534,41 +534,41 @@
     def printResults(self) -> None:
         """
         This function is used to print the results
         """
         print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
-    if __name__ == "__main__":
-        _ap = str()
-        if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
-            if len(_ab._sys.argv) == 5:
-                _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-            if len(_ab._sys.argv) == 4:
-                _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3])
-            _ap.startMine()
-            _ap.mine()
-            _Patterns = _ap.getPatterns()
-            print("Total number of Patterns:", len(_Patterns))
-            _ap.save(_ab._sys.argv[2])
-            _memUSS = _ap.getMemoryUSS()
-            print("Total Memory in USS:", _memUSS)
-            _memRSS = _ap.getMemoryRSS()
-            print("Total Memory in RSS", _memRSS)
-            _run = _ap.getRuntime()
-            print("Total ExecutionTime in ms:", _run)
-        else:
-            '''ap = TUFP("/home/apiiit-rkv/Desktop/uncertain/tubeSample", 10, ' ')
-            ap.startMine()
-            Patterns = ap.getPatterns()
-            print("Total number of Patterns:", len(Patterns))
-            ap.save("patterns.txt")
-            memUSS = ap.getMemoryUSS()
-            print("Total Memory in USS:", memUSS)
-            memRSS = ap.getMemoryRSS()
-            print("Total Memory in RSS", memRSS)
-            run = ap.getRuntime()
-            print("Total ExecutionTime in ms:", run)'''
-            print("Error! The number of input parameters do not match the total number of parameters provided")
+if __name__ == "__main__":
+    _ap = str()
+    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+        if len(_ab._sys.argv) == 5:
+            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+        if len(_ab._sys.argv) == 4:
+            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3])
+        _ap.startMine()
+        _ap.mine()
+        _Patterns = _ap.getPatterns()
+        print("Total number of Patterns:", len(_Patterns))
+        _ap.save(_ab._sys.argv[2])
+        _memUSS = _ap.getMemoryUSS()
+        print("Total Memory in USS:", _memUSS)
+        _memRSS = _ap.getMemoryRSS()
+        print("Total Memory in RSS", _memRSS)
+        _run = _ap.getRuntime()
+        print("Total ExecutionTime in ms:", _run)
+    else:
+        '''ap = TUFP("/home/apiiit-rkv/Desktop/uncertain/tubeSample", 10, ' ')
+        ap.startMine()
+        Patterns = ap.getPatterns()
+        print("Total number of Patterns:", len(Patterns))
+        ap.save("patterns.txt")
+        memUSS = ap.getMemoryUSS()
+        print("Total Memory in USS:", memUSS)
+        memRSS = ap.getMemoryRSS()
+        print("Total Memory in RSS", memRSS)
+        run = ap.getRuntime()
+        print("Total ExecutionTime in ms:", run)'''
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# TUFP is one of the fundamental algorithm to discover top-k frequent patterns in a uncertain transactional database using CUP-Lists.
+# UVEclat is one of the fundamental algorithm to discover frequent patterns in an uncertain transactional database using PUF-Tree.
 #
 # **Importing this algorithm into a python program**
 #
-#             from PAMI.uncertainFrequentPattern.basic import TUFP as alg
+#             from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
 #
 #             iFile = 'sampleDB.txt'
 #
 #             minSup = 10  # can also be specified between 0 and 1
 #
-#             obj = alg.TUFP(iFile, minSup)
+#             obj = alg.UVEclat(iFile, minSup)
 #
 #             obj.mine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -29,15 +29,14 @@
 #             print("Total Memory in RSS", memRSS)
 #
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
-
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
      
@@ -46,19 +45,17 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
      
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-
+import operator as _operator
 from PAMI.uncertainFrequentPattern.basic import abstract as _ab
-from typing import List, Dict, Union
-import pandas as pd
-from deprecated import deprecated
+import deprecated
 
 _minSup = float()
 _finalPatterns = {}
 
 
 class _Item:
     """
@@ -69,28 +66,29 @@
         item : int or word
           Represents the name of the item
 
         probability : float
           Represent the existential probability(likelihood presence) of an item
     """
 
-    def __init__(self, item, probability) -> None:
+    def __init__(self, item, probability):
         self.item = item
         self.probability = probability
 
 
-class TUFP(_ab._frequentPatterns):
+class UVEclat(_ab._frequentPatterns):
     """
     About this algorithm
     ====================
 
-    :Description: It is one of the fundamental algorithm to discover top-k frequent patterns in a uncertain transactional database using CUP-Lists.
+    :Description: It is one of the fundamental algorithm to discover frequent patterns in an uncertain transactional database using PUF-Tree.
 
-    :Reference:  Tuong Le, Bay Vo, Van-Nam Huynh, Ngoc Thanh Nguyen, Sung Wook Baik 5, "Mining top-k frequent patterns from uncertain databases",
-                 Springer Science+Business Media, LLC, part of Springer Nature 2020, https://doi.org/10.1007/s10489-019-01622-1
+    :Reference:  Carson Kai-Sang Leung, Lijing Sun: "Equivalence class transformation based mining of frequent itemsets from uncertain data",
+                 SAC '11: Proceedings of the 2011 ACM Symposium on Applied ComputingMarch, 2011, Pages 983–984,
+                 https://doi.org/10.1145/1982185.1982399
 
     :Attributes:
 
         iFile : file
             Name of the Input file or path of the input file
 
         oFile : file
@@ -108,31 +106,31 @@
 
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-        startTime : float
+        startTime:float
             To record the start time of the mining process
 
-        endTime : float
+        endTime:float
             To record the completion time of the mining process
 
         Database : list
             To store the transactions of a database in list
 
         mapSupport : Dictionary
             To maintain the information of item and their frequency
 
         lno : int
             To represent the total no of transaction
 
         tree : class
-            To represents the Tree class
+            To represent the Tree class
 
         itemSetCount : int
             To represents the total no of patterns
 
         finalPatterns : dict
             To store the complete patterns
 
@@ -151,55 +149,46 @@
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingItemSets(fileName)
             Scans the dataset and stores in a list format
         frequentOneItem()
             Extracts the one-length frequent patterns from database
-        updateTransactions()
-            Update the transactions by removing non-frequent items and sort the Database by item decreased support
-        buildTree()
-            After updating the Database, remaining items will be added into the tree by setting root node as null
-        convert()
-            to convert the user specified value
-        startMine()
-            Mining process will start from this function
 
     Execution methods
     =================
 
 
     **Terminal command**
 
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 TUFP.py <inputFile> <outputFile> <minSup>
+      (.venv) $ python3 uveclat.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 TUFP.py sampleDB.txt patterns.txt 10.0
+      (.venv) $ python3 uveclat.py sampleDB.txt patterns.txt 3
 
     .. note:: minSup can be specified  in support count or a value between 0 and 1.
 
 
     **Calling from a python program**
-
+    ---------------------------------------------------
     .. code-block:: python
 
-            from PAMI.uncertainFrequentPattern.basic import TUFP as alg
-
+            from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
 
             iFile = 'sampleDB.txt'
 
             minSup = 10  # can also be specified between 0 and 1
 
-            obj = alg.TUFP(iFile, minSup)
+            obj = alg.UVEclat(iFile, minSup)
 
             obj.mine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
@@ -218,32 +207,30 @@
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     Credits
     =======
 
-            The complete program was written by   P.Likhitha   under the supervision of Professor Rage Uday Kiran.
+             The complete program was written by   P.Likhitha   under the supervision of Professor Rage Uday Kiran.
     """
-
     _startTime = float()
     _endTime = float()
     _minSup = str()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _cupList = {}
-    _topk = {}
-    _minimum = 9999
+    _tidList = {}
+    _rank = {}
 
-    def _creatingItemSets(self) -> None:
+    def _creatingItemSets(self):
         """
         Scans the dataset
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             uncertain, data = [], []
             if self._iFile.empty:
@@ -292,45 +279,56 @@
                                 probability = float(i[i1 + 1:i2])
                                 product = _Item(item, probability)
                                 tr.append(product)
                             self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
 
-    def _frequentOneItem(self) -> List[str]:
+    def _frequentOneItem(self):
         """
         Takes the self.Database and calculates the support of each item in the dataset and assign the ranks to the items by decreasing support and returns the frequent items list
-
-        :param self.Database : it represents the one self.Database in database
-        :type self.Database : list
         """
-
         mapSupport = {}
         k = 0
         for i in self._Database:
             k += 1
             for j in i:
                 if j.item not in mapSupport:
-                    mapSupport[j.item] = j.probability
-                    self._cupList[j.item] = {k:j.probability}
+                    mapSupport[str(j.item)] = j.probability
+                    self._tidList[str(j.item)] = {k: j.probability}
                 else:
-                    mapSupport[j.item] += j.probability
-                    self._cupList[j.item].update({k: j.probability})
-        plist = [k for k,v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        k = 0
-        for x, in plist:
-            k +=1
-            if k >= self._minSup:
-                break
-            self._finalPatterns[x] = mapSupport[x]
-        self._minimum = min(list(self._finalPatterns.values()))
-        return plist
+                    mapSupport[str(j.item)] += j.probability
+                    self._tidList[str(j.item)].update({k: j.probability})
+        mapSupport = {k: v for k, v in mapSupport.items() if v >= self._minSup}
+        plist = dict( sorted(mapSupport.items(), key=_operator.itemgetter(1),reverse=True))
+        return list(plist.keys())
+
+    @staticmethod
+    def _check(i, x):
+        """
+        To check the presence of item or pattern in transaction
+
+        :param x: it represents the pattern
+        :type x : list
+        :param i : represents the uncertain self.Database
+        :type i : list
+        """
+
+        # This method taken a transaction as input and returns the tree
+        for m in x:
+            k = 0
+            for n in i:
+                if m == n.item:
+                    k += 1
+            if k == 0:
+                return 0
+        return 1
 
     @staticmethod
-    def _convert(value: Union[int, float, str]) -> Union[int, float]:
+    def _convert(value):
         """
         To convert the type of user specified minSup value
 
         :param value: user specified minSup value
         :return: converted type minSup value
         """
         if type(value) is int:
@@ -340,50 +338,95 @@
         if type(value) is str:
             if '.' in value:
                 value = float(value)
             else:
                 value = int(value)
         return value
 
-    def _save(self, prefix: List[str], suffix: List[str], tidSetI: Dict[int, float]) -> None:
+    def _removeFalsePositives(self):
+        """
+        To remove the false positive patterns generated in frequent patterns
+
+        :return: patterns with accurate probability
+        """
+        global _finalPatterns
+        periods = {}
+        for i in self._Database:
+            for x, y in _finalPatterns.items():
+                if len(x) == 1:
+                    periods[x] = y
+                else:
+                    s = 1
+                    check = self._check(i, x)
+                    if check == 1:
+                        for j in i:
+                            if j.item in x:
+                                s *= j.probability
+                        if x in periods:
+                            periods[x] += s
+                        else:
+                            periods[x] = s
+        for x, y in periods.items():
+            if y >= self._minSup:
+                sample = str()
+                for i in x:
+                    sample = sample + i + "\t"
+                self._finalPatterns[sample] = y
+
+    @staticmethod
+    def _Intersection(tidSetx, tidSetY):
+        """
+        This function is used to find the intersection
+
+        :param tidSetx: the timestamp of a patterns
+        :type tidSetx: dict
+        :param tidSetY: the timestamp of a patterns
+        :type tidSetY: dict
+        """
+        tids = []
+        support = []
+        tidDict = {}
+        for x, y in tidSetx.items():
+            for x1, y1 in tidSetY.items():
+                if x == x1:
+                    tids.append(x)
+                    support.append(y * y1)
+                    tidDict.update({x: y * y1})
+        return tidDict
+
+    def _calculateExpSup(self, tidList):
+        """
+        This function is used to calculate support of tidList
+
+        :param tidList: timestamp of a list.
+        :type tidList: List
+        """
+        return sum(tidList.values())
+
+    def _save(self, prefix, suffix, tidSetI):
         """
         Saves the patterns that satisfy the periodic frequent property.
 
         :param prefix: the prefix of a pattern
         :type prefix: list
         :param suffix: the suffix of a patterns
         :type suffix: list
         :param tidSetI: the timestamp of a patterns
         :type tidSetI: dict
         """
 
+        global _finalPatterns
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
-        val = sum(tidSetI.values())
-        #print(prefix, val)
-        if len(self._finalPatterns) <= self._minSup:
-            sample = str()
-            for i in prefix:
-                sample = sample + i + " "
-            self._finalPatterns[sample] = val
-        if len(self._finalPatterns) == self._minSup:
-            if val > self._minimum:
-                sample = str()
-                for i in prefix:
-                    sample = sample + i + " "
-                index = list(self._finalPatterns.keys())[list(self._finalPatterns.values()).index(self._minimum)]
-                del self._finalPatterns[index]
-                self._finalPatterns[sample] = val
-                self._minimum = min(list(self._finalPatterns.values()))
-        #print(self.finalPatterns, self.minimum, self.minSup)
-
+        val = self._calculateExpSup(tidSetI)
+        _finalPatterns[tuple(prefix)] = val
 
-    def _Generation(self, prefix: List[str], itemSets: List[str], tidSets: List[Dict[int, float]]) -> None:
+    def _Generation(self, prefix, itemSets, tidSets):
         """
         Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
 
         :param prefix:  main equivalence prefix
         :type prefix: periodic-frequent item or pattern
         :param itemSets: patterns which are items combined with prefix and satisfying the periodicity and frequent with their timestamps
         :type itemSets: list
@@ -391,184 +434,158 @@
         :type tidSets: list
         """
         if len(itemSets) == 1:
             i = itemSets[0]
             tidI = tidSets[0]
             self._save(prefix, [i], tidI)
             return
-        for i in range(0, len(itemSets)):
+        for i in range(len(itemSets)):
             itemI = itemSets[i]
             if itemI is None:
                 continue
             tidSetI = tidSets[i]
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
-            for j in range(i+1, len(itemSets)):
+            for j in range(i + 1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
-                y = {key: tidSetJ[key] * tidSetI.get(key, 0) for key in tidSetJ.keys()}
-                sum2 = sum(list(y.values()))
-                #print(prefix, itemJ, y, sum2)
-                #if sum2 >= self.minimum:
-                self._save(prefix, [itemJ], y)
-                classItemSets.append(itemJ)
-                classTidSets.append(y)
-            #print(itemI, tidSetI, classItemSets)
+                y = self._Intersection(tidSetI, tidSetJ)
+                if self._calculateExpSup(y) >= self._minSup:
+                    classItemSets.append(itemJ)
+                    classTidSets.append(y)
             newPrefix = list(set(itemSetX)) + prefix
             self._Generation(newPrefix, classItemSets, classTidSets)
-            #self.save(prefix, list(set(itemSetX)), tidSetI)
+            self._save(prefix, list(set(itemSetX)), tidSetI)
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
-    def startMine(self) -> None:
-        """
-        Main method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns
-        """
-        self.mine()
-
-
-    def mine(self) -> None:
+    def mine(self):
         """
         Main method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns
         """
         global _minSup
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
         _minSup = self._minSup
         plist = self._frequentOneItem()
         for i in range(len(plist)):
             itemI = plist[i]
-            tidSetI = self._cupList[itemI]
+            tidSetI = self._tidList[itemI]
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
             for j in range(i+1, len(plist)):
                 itemJ = plist[j]
-                tidSetJ = self._cupList[itemJ]
-                y1 = {key: tidSetJ[key] * tidSetI.get(key, 0)  for key in tidSetJ.keys()}
-                self._save(itemSetX, [itemJ], y1)
-                itemSets.append(itemJ)
-                tidSets.append(y1)
+                tidSetJ = self._tidList[itemJ]
+                y1 = self._Intersection(tidSetI, tidSetJ)
+                if self._calculateExpSup(y1) >= self._minSup:
+                    itemSets.append(itemJ)
+                    tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
-        print("Top-K Frequent patterns were generated from uncertain databases successfully using TUFP algorithm")
+            self._save(None, itemSetX, tidSetI)
+        self._removeFalsePositives()
+        print("Frequent patterns were generated from uncertain databases successfully using PUF algorithm")
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = float()
         self._memoryRSS = float()
+        self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
-    def getMemoryUSS(self) -> float:
+    def getMemoryUSS(self):
         """
 
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
-    def getMemoryRSS(self) -> float:
+    def getMemoryRSS(self):
         """
 
         Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryRSS
 
-    def getRuntime(self) -> float:
+    def getRuntime(self):
         """
 
         Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> pd.DataFrame:
+    def getPatternsAsDataFrame(self):
         """
 
         Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a, b])
+            data.append([a.replace('\t', ' '), b])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
-    def save(self, outFile: str) -> None:
+    def save(self, oFile):
         """
 
         Complete set of frequent patterns will be loaded in to an output file
 
-        :param outFile: name of the output file
-        :type outFile: file
+        :param oFile: name of the output file
+        :type oFile: csv file
         """
-        self.oFile = outFile
+        self.oFile = oFile
         writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x + ":" + str(y)
+            s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self) -> Dict[str, float]:
+    def getPatterns(self):
         """
 
         Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self) -> None:
+    def printResults(self):
         """
         This function is used to print the results
         """
         print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
+
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3])
-        _ap.startMine()
+            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.mine()
-        _Patterns = _ap.getPatterns()
-        print("Total number of Patterns:", len(_Patterns))
+        print("Total number of Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        _memUSS = _ap.getMemoryUSS()
-        print("Total Memory in USS:", _memUSS)
-        _memRSS = _ap.getMemoryRSS()
-        print("Total Memory in RSS", _memRSS)
-        _run = _ap.getRuntime()
-        print("Total ExecutionTime in ms:", _run)
+        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        '''ap = TUFP("/home/apiiit-rkv/Desktop/uncertain/tubeSample", 10, ' ')
-        ap.startMine()
-        Patterns = ap.getPatterns()
-        print("Total number of Patterns:", len(Patterns))
-        ap.save("patterns.txt")
-        memUSS = ap.getMemoryUSS()
-        print("Total Memory in USS:", memUSS)
-        memRSS = ap.getMemoryRSS()
-        print("Total Memory in RSS", memRSS)
-        run = ap.getRuntime()
-        print("Total ExecutionTime in ms:", run)'''
         print("Error! The number of input parameters do not match the total number of parameters provided")
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2024.5.1.1/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-# UVEclat is one of the fundamental algorithm to discover frequent patterns in an uncertain transactional database using PUF-Tree.
+# WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
+# It stores the database in compressed fp-tree decreasing the memory usage and extracts the
+# patterns from tree.It employs downward closure property to  reduce the search space effectively.
 #
 # **Importing this algorithm into a python program**
 #
-#             from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
+#             from PAMI.weightFrequentPattern.basic import basic as alg
 #
 #             iFile = 'sampleDB.txt'
 #
 #             minSup = 10  # can also be specified between 0 and 1
 #
-#             obj = alg.UVEclat(iFile, minSup)
+#             obj = alg.basic(iFile, wFile, minSup, minWeight)
 #
 #             obj.mine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#             obj.save(oFile)
+#             obj.savePatterns(oFile)
 #
 #             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
@@ -31,172 +33,350 @@
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
+
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
-     
+
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
-     
+
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-import operator as _operator
-from PAMI.uncertainFrequentPattern.basic import abstract as _ab
-import deprecated
+from PAMI.weightedFrequentPattern.basic import abstract as _fp
+from typing import List, Dict, Tuple, Union, Generator
+import pandas as pd
+from deprecated import deprecated
+
 
-_minSup = float()
-_finalPatterns = {}
+_minSup = str()
+_minWeight = int()
+_miniWeight = int()
+_maxWeight = int()
+_weights = {}
+_fp._sys.setrecursionlimit(20000)
 
 
-class _Item:
+class _Node:
     """
-    A class used to represent the item with probability in transaction of dataset
+    A class used to represent the node of frequentPatternTree
 
     :Attributes:
 
-        item : int or word
-          Represents the name of the item
+        itemId: int
+            storing item of a node
+
+        counter: int
+            To maintain the support of node
+
+        parent: node
+            To maintain the parent of node
+
+        children: list
+            To maintain the children of node
 
-        probability : float
-          Represent the existential probability(likelihood presence) of an item
+    :Methods:
+
+        addChild(node)
+            Updates the nodes children list and parent for the given node
     """
 
-    def __init__(self, item, probability):
-        self.item = item
-        self.probability = probability
+    def __init__(self, item: str, children: list) -> None:
+        self.itemId = item
+        self.counter = 1
+        self.parent = None
+        self.children = children
+
+    def addChild(self, node: '_Node') -> None:
+        """
+        Retrieving the child from the tree
+
+        :param node: Children node
+        :type node: _Node
+        :return: Updates the children nodes and parent nodes
+        """
+        self.children[node.itemId] = node
+        node.parent = self
 
 
-class UVEclat(_ab._frequentPatterns):
+class _Tree:
+    """
+    A class used to represent the frequentPatternGrowth tree structure
+
+    :Attributes:
+
+        root : Node
+            The first node of the tree set to Null.
+
+        summaries : dictionary
+            Stores the nodes itemId which shares same itemId
+
+        info : dictionary
+            frequency of items in the transactions
+
+    :Methods:
+
+        addTransaction(transaction, freq)
+            adding items of  transactions into the tree as nodes and freq is the count of nodes
+        getFinalConditionalPatterns(node)
+            getting the conditional patterns from fp-tree for a node
+        getConditionalPatterns(patterns, frequencies)
+            sort the patterns by removing the items with lower minSup
+        generatePatterns(prefix)
+            generating the patterns from fp-tree
+    """
+
+    def __init__(self) -> None:
+        self.root = _Node(None, {})
+        self.summaries = {}
+        self.info = {}
+
+    def addTransaction(self, transaction: List[str], count: int) -> None:
+        """
+        Adding transaction into tree
+
+        :param transaction: it represents the one transaction in database
+        :type transaction: list
+        :param count: frequency of item
+        :type count: int
+        :return: None
+        """
+        # This method takes transaction as input and returns the tree
+        currentNode = self.root
+        for i in range(len(transaction)):
+            if transaction[i] not in currentNode.children:
+                newNode = _Node(transaction[i], {})
+                newNode.freq = count
+                currentNode.addChild(newNode)
+                if transaction[i] in self.summaries:
+                    self.summaries[transaction[i]].append(newNode)
+                else:
+                    self.summaries[transaction[i]] = [newNode]
+                currentNode = newNode
+            else:
+                currentNode = currentNode.children[transaction[i]]
+                currentNode.freq += count
+
+    def getFinalConditionalPatterns(self, alpha: str) -> Tuple[List[List[str]], List[int], Dict[str, int]]:
+        """
+        Generates the conditional patterns for a node
+
+        :param alpha: node to generate conditional patterns
+        :return: returns conditional patterns, frequency of each item in conditional patterns
+        """
+        finalPatterns = []
+        finalFreq = []
+        for i in self.summaries[alpha]:
+            set1 = i.freq
+            set2 = []
+            while i.parent.itemId is not None:
+                set2.append(i.parent.itemId)
+                i = i.parent
+            if len(set2) > 0:
+                set2.reverse()
+                finalPatterns.append(set2)
+                finalFreq.append(set1)
+        finalPatterns, finalFreq, info = self.getConditionalTransactions(finalPatterns, finalFreq)
+        return finalPatterns, finalFreq, info
+
+    @staticmethod
+    def getConditionalTransactions(ConditionalPatterns: List[List[str]], conditionalFreq: List[int]) -> Tuple[List[List[str]], List[int], Dict[str, int]]:
+        """
+        To calculate the frequency of items in conditional patterns and sorting the patterns
+
+        :param ConditionalPatterns: paths of a node
+        :param conditionalFreq: frequency of each item in the path
+        :return: conditional patterns and frequency of each item in transactions
+        """
+        global _minSup, _miniWeight
+        pat = []
+        freq = []
+        data1 = {}
+        for i in range(len(ConditionalPatterns)):
+            for j in ConditionalPatterns[i]:
+                if j in data1:
+                    data1[j] += conditionalFreq[i]
+                else:
+                    data1[j] = conditionalFreq[i]
+        up_dict = {k: v for k, v in data1.items() if v >= _minSup and v * _miniWeight > _minSup}
+        count = 0
+        for p in ConditionalPatterns:
+            p1 = [v for v in p if v in up_dict]
+            trans = sorted(p1, key=lambda x: (up_dict.get(x), -x), reverse=True)
+            if len(trans) > 0:
+                pat.append(trans)
+                freq.append(conditionalFreq[count])
+            count += 1
+        return pat, freq, up_dict
+
+    def generatePatterns(self, prefix: List[str]) -> Generator[Tuple[List[str], int], None, None]:
+        """
+        To generate the frequent patterns
+
+        :param prefix: an empty list
+        :return: Frequent patterns that are extracted from fp-tree
+        """
+        global _miniWeight, _maxWeight, _minWeight, _minSup
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
+            pattern = prefix[:]
+            pattern.append(i)
+            yield pattern, self.info[i]
+            patterns, freq, info = self.getFinalConditionalPatterns(i)
+            conditionalTree = _Tree()
+            conditionalTree.info = info.copy()
+            for pat in range(len(patterns)):
+                conditionalTree.addTransaction(patterns[pat], freq[pat])
+            if len(patterns) > 0:
+                for q in conditionalTree.generatePatterns(pattern):
+                    yield q
+
+
+class WFIM(_fp._weightedFrequentPatterns):
     """
     About this algorithm
     ====================
 
-    :Description: It is one of the fundamental algorithm to discover frequent patterns in an uncertain transactional database using PUF-Tree.
+    :Description: * WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
+                  * It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
 
-    :Reference:  Carson Kai-Sang Leung, Lijing Sun: "Equivalence class transformation based mining of frequent itemsets from uncertain data",
-                 SAC '11: Proceedings of the 2011 ACM Symposium on Applied ComputingMarch, 2011, Pages 983–984,
-                 https://doi.org/10.1145/1982185.1982399
+    :Reference:  U. Yun and J. J. Leggett, “Wfim: weighted frequent itemset mining with a weight range and a minimum weight,”
+           In:   Proceedings of the 2005 SIAM International Conference on Data Mining. SIAM, 2005, pp. 636–640.
+                 https://epubs.siam.org/doi/pdf/10.1137/1.9781611972757.76
+
+    :param  iFile: str :
+                   Name of the Input file to mine complete set of weighted Frequent Patterns.
+    :param  oFile: str :
+                   Name of the output file to store complete set of weighted Frequent Patterns.
+    :param  minSup: str or int or float:
+                   minimum support thresholds were tuned to find the appropriate ranges in the limited memory
+    :param  sep: str :
+                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
-    :Attributes:
 
-        iFile : file
-            Name of the Input file or path of the input file
+    :Attributes :
 
-        oFile : file
-            Name of the output file or path of the output file
+        iFile : file
+            Input file name or path of the input file
 
-        minSup : float or int or str
+        minSup: float or int or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
 
+        minWeight: float or int or str
+            The user can specify minWeight either in count or proportion of database size.
+            If the program detects the data type of minWeight is integer, then it treats minWeight is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minWeight=10 will be treated as integer, while minWeight=10.0 will be treated as float
+
         sep : str
-            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
             However, the users can override their default separator.
 
-        memoryUSS : float
-            To store the total amount of USS memory consumed by the program
-
-        memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
+        oFile : file
+            Name of the output file or the path of the output file
 
         startTime:float
             To record the start time of the mining process
 
         endTime:float
             To record the completion time of the mining process
 
+        memoryUSS : float
+            To store the total amount of USS memory consumed by the program
+
+        memoryRSS : float
+            To store the total amount of RSS memory consumed by the program
+
         Database : list
             To store the transactions of a database in list
 
         mapSupport : Dictionary
             To maintain the information of item and their frequency
 
         lno : int
-            To represent the total no of transaction
+            it represents the total no of transactions
 
         tree : class
-            To represent the Tree class
-
-        itemSetCount : int
-            To represents the total no of patterns
+            it represents the Tree class
 
         finalPatterns : dict
-            To store the complete patterns
+            it represents to store the patterns
+
+    :Methods :
 
-    :Methods:
         mine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
-        storePatternsInFile(oFile)
+        save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
-        getPatternsInDataFrame()
+        getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets(fileName)
-            Scans the dataset and stores in a list format
+        creatingItemSets()
+            Scans the dataset or dataframes and stores in list format
         frequentOneItem()
-            Extracts the one-length frequent patterns from database
+            Extracts the one-frequent patterns from transactions
 
     Execution methods
     =================
 
 
     **Terminal command**
 
 
     .. code-block:: console
 
-      Format:
+       Format:
 
-      (.venv) $ python3 uveclat.py <inputFile> <outputFile> <minSup>
+       (.venv) $ python3 basic.py <inputFile> <weightFile> <outputFile> <minSup> <minWeight>
 
-      Example Usage:
+       Example Usage:
 
-      (.venv) $ python3 uveclat.py sampleDB.txt patterns.txt 3
+       (.venv) $ python3 basic.py sampleDB.txt weightSample.txt patterns.txt 10.0 3.4
 
-    .. note:: minSup can be specified  in support count or a value between 0 and 1.
+    .. note:: minSup and maxPer will be considered in support count or frequency
 
 
     **Calling from a python program**
-    ---------------------------------------------------
+
     .. code-block:: python
 
-            from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
+            from PAMI.weightFrequentPattern.basic import basic as alg
 
             iFile = 'sampleDB.txt'
 
             minSup = 10  # can also be specified between 0 and 1
 
-            obj = alg.UVEclat(iFile, minSup)
+            obj = alg.basic(iFile, wFile, minSup, minWeight)
 
             obj.mine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.save(oFile)
+            obj.savePatterns(oFile)
 
             Df = obj.getPatternsAsDataFrame()
 
             memUSS = obj.getmemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
@@ -207,385 +387,347 @@
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     Credits
     =======
 
-             The complete program was written by   P.Likhitha   under the supervision of Professor Rage Uday Kiran.
+
+             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
     """
-    _startTime = float()
-    _endTime = float()
+
+    __startTime = float()
+    __endTime = float()
     _minSup = str()
-    _finalPatterns = {}
+    __finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    _memoryUSS = float()
-    _memoryRSS = float()
-    _Database = []
-    _tidList = {}
-    _rank = {}
-
-    def _creatingItemSets(self):
-        """
-        Scans the dataset
-        """
-        self._Database = []
-        if isinstance(self._iFile, _ab._pd.DataFrame):
-            uncertain, data = [], []
+    __memoryUSS = float()
+    __memoryRSS = float()
+    __Database = []
+    __mapSupport = {}
+    __lno = 0
+    __tree = _Tree()
+    __rank = {}
+    __rankDup = {}
+
+    def __init__(self, iFile: str, wFile: str, minSup: str, minWeight: int, sep: str='\t') -> None:
+        super().__init__(iFile, wFile, minSup, minWeight, sep)
+
+    def __creatingItemSets(self) -> None:
+        """
+        Storing the complete transactions of the database/input file in a database variable
+
+        :return: None
+        """
+        self.__Database = []
+        if isinstance(self._iFile, _fp._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
-            if 'uncertain' in i:
-                uncertain = self._iFile['uncertain'].tolist()
-            for k in range(len(data)):
-                tr = []
-                for j in range(len(data[k])):
-                    product = _Item(data[k][j], uncertain[k][j])
-                    tr.append(product)
-                self._Database.append(tr)
+                self.__Database = self._iFile['Transactions'].tolist()
 
             # print(self.Database)
         if isinstance(self._iFile, str):
-            if _ab._validators.url(self._iFile):
-                data = _ab._urlopen(self._iFile)
+            if _fp._validators.url(self._iFile):
+                data = _fp._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    tr = []
-                    for i in temp:
-                        i1 = i.index('(')
-                        i2 = i.index(')')
-                        item = i[0:i1]
-                        probability = float(i[i1 + 1:i2])
-                        product = _Item(item, probability)
-                        tr.append(product)
-                    self._Database.append(temp)
+                    self.__Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r') as f:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
+                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            tr = []
-                            for i in temp:
-                                i1 = i.index('(')
-                                i2 = i.index(')')
-                                item = i[0:i1]
-                                probability = float(i[i1 + 1:i2])
-                                product = _Item(item, probability)
-                                tr.append(product)
-                            self._Database.append(tr)
+                            # print(len(temp))
+                            self.__Database.append(temp)
                 except IOError:
                     print("File Not Found")
+                    quit()
 
-    def _frequentOneItem(self):
+    def _scanningWeights(self) -> None:
         """
-        Takes the self.Database and calculates the support of each item in the dataset and assign the ranks to the items by decreasing support and returns the frequent items list
-        """
-        mapSupport = {}
-        k = 0
-        for i in self._Database:
-            k += 1
-            for j in i:
-                if j.item not in mapSupport:
-                    mapSupport[str(j.item)] = j.probability
-                    self._tidList[str(j.item)] = {k: j.probability}
-                else:
-                    mapSupport[str(j.item)] += j.probability
-                    self._tidList[str(j.item)].update({k: j.probability})
-        mapSupport = {k: v for k, v in mapSupport.items() if v >= self._minSup}
-        plist = dict( sorted(mapSupport.items(), key=_operator.itemgetter(1),reverse=True))
-        return list(plist.keys())
+        Storing the weights of the variables in input file in a weights variable
 
-    @staticmethod
-    def _check(i, x):
+        :return: None
         """
-        To check the presence of item or pattern in transaction
+        global _weights
+        _weights = {}
+        if isinstance(self._wFile, _fp._pd.DataFrame):
+            items, weights = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                items = self._wFile['items'].tolist()
+            if 'weights' in i:
+                weights = self._wFile['weights'].tolist()
+            for i in range(len(weights)):
+                _weights[items[i]] = weights[i]
 
-        :param x: it represents the pattern
-        :type x : list
-        :param i : represents the uncertain self.Database
-        :type i : list
-        """
-
-        # This method taken a transaction as input and returns the tree
-        for m in x:
-            k = 0
-            for n in i:
-                if m == n.item:
-                    k += 1
-            if k == 0:
-                return 0
-        return 1
+            # print(self.Database)
+        if isinstance(self._wFile, str):
+            if _fp._validators.url(self._wFile):
+                data = _fp._urlopen(self._wFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    _weights[temp[0]] = temp[1]
+            else:
+                try:
+                    with open(self._wFile, 'r', encoding='utf-8') as f:
+                        for line in f:
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            s = int(float(temp[1]))
+                            _weights[temp[0]] = s
+                except IOError:
+                    print("File Not Found")
+                    quit()
 
-    @staticmethod
-    def _convert(value):
+    def __convert(self, value: Union[int, float, str]) -> Union[int, float]:
         """
-        To convert the type of user specified minSup value
+        To convert the type of user specified minSup value.
 
         :param value: user specified minSup value
-        :return: converted type minSup value
+        :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = float(value)
+            value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
+                value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    def _removeFalsePositives(self):
+    def __frequentOneItem(self) -> List[str]:
         """
-        To remove the false positive patterns generated in frequent patterns
+        Generating One frequent items sets
 
-        :return: patterns with accurate probability
+        :return: list
         """
-        global _finalPatterns
-        periods = {}
-        for i in self._Database:
-            for x, y in _finalPatterns.items():
-                if len(x) == 1:
-                    periods[x] = y
+        global _maxWeight
+        self.__mapSupport = {}
+        for tr in self.__Database:
+            for i in range(0, len(tr)):
+                if tr[i] not in self.__mapSupport:
+                    self.__mapSupport[tr[i]] = 1
                 else:
-                    s = 1
-                    check = self._check(i, x)
-                    if check == 1:
-                        for j in i:
-                            if j.item in x:
-                                s *= j.probability
-                        if x in periods:
-                            periods[x] += s
-                        else:
-                            periods[x] = s
-        for x, y in periods.items():
-            if y >= self._minSup:
-                sample = str()
-                for i in x:
-                    sample = sample + i + "\t"
-                self._finalPatterns[sample] = y
+                    self.__mapSupport[tr[i]] += 1
+        self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= self._minSup and v * _maxWeight > self._minSup}
+        genList = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.__rank = dict([(index, item) for (item, index) in enumerate(genList)])
+        return genList
+
+    def __updateTransactions(self, itemSet: List[str]) -> List[List[int]]:
+        """
+        Updates the items in transactions with rank of items according to their support
+
+        :Example: oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
+                    rank = {'a':0, 'b':1, 'c':2, 'd':3}
+
+        :param itemSet: list of one-frequent items
+        :return: list
+        """
+        list1 = []
+        for tr in self.__Database:
+            list2 = []
+            for i in range(len(tr)):
+                if tr[i] in itemSet:
+                    list2.append(self.__rank[tr[i]])
+            if len(list2) >= 1:
+                list2.sort()
+                list1.append(list2)
+        return list1
 
     @staticmethod
-    def _Intersection(tidSetx, tidSetY):
+    def __buildTree(transactions: List[List[int]], info: Dict[int, int]) -> '_Tree':
+        """
+        Builds the tree with updated transactions
+
+        :param transactions: updated transactions
+        :param info: support details of each item in transactions.
+        :return: Transactions compressed in fp-tree
+        """
+        rootNode = _Tree()
+        rootNode.info = info.copy()
+        for i in range(len(transactions)):
+            rootNode.addTransaction(transactions[i], 1)
+        return rootNode
+
+    def __savePeriodic(self, itemSet: List[int]) -> str:
+        """
+        The duplication items and their ranks
+
+        :param itemSet: frequent itemSet that generated
+        :return: patterns with original item names.
+        """
+        temp = str()
+        for i in itemSet:
+            temp = temp + self.__rankDup[i] + "\t"
+        return temp
+
+    @deprecated(
+        "It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
+    def startMine(self) -> None:
+        """
+        main program to start the operation
+
+        :return: None
+        """
+        self.mine()
+
+    def mine(self) -> None:
         """
-        This function is used to find the intersection
+        main program to start the operation
 
-        :param tidSetx: the timestamp of a patterns
-        :type tidSetx: dict
-        :param tidSetY: the timestamp of a patterns
-        :type tidSetY: dict
-        """
-        tids = []
-        support = []
-        tidDict = {}
-        for x, y in tidSetx.items():
-            for x1, y1 in tidSetY.items():
-                if x == x1:
-                    tids.append(x)
-                    support.append(y * y1)
-                    tidDict.update({x: y * y1})
-        return tidDict
-
-    def _calculateExpSup(self, tidList):
-        """
-        This function is used to calculate support of tidList
-
-        :param tidList: timestamp of a list.
-        :type tidList: List
-        """
-        return sum(tidList.values())
-
-    def _save(self, prefix, suffix, tidSetI):
-        """
-        Saves the patterns that satisfy the periodic frequent property.
-
-        :param prefix: the prefix of a pattern
-        :type prefix: list
-        :param suffix: the suffix of a patterns
-        :type suffix: list
-        :param tidSetI: the timestamp of a patterns
-        :type tidSetI: dict
-        """
-
-        global _finalPatterns
-        if prefix is None:
-            prefix = suffix
-        else:
-            prefix = prefix + suffix
-        val = self._calculateExpSup(tidSetI)
-        _finalPatterns[tuple(prefix)] = val
-
-    def _Generation(self, prefix, itemSets, tidSets):
-        """
-        Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
-
-        :param prefix:  main equivalence prefix
-        :type prefix: periodic-frequent item or pattern
-        :param itemSets: patterns which are items combined with prefix and satisfying the periodicity and frequent with their timestamps
-        :type itemSets: list
-        :param tidSets: timestamps of the items in the argument itemSets
-        :type tidSets: list
-        """
-        if len(itemSets) == 1:
-            i = itemSets[0]
-            tidI = tidSets[0]
-            self._save(prefix, [i], tidI)
-            return
-        for i in range(len(itemSets)):
-            itemI = itemSets[i]
-            if itemI is None:
-                continue
-            tidSetI = tidSets[i]
-            classItemSets = []
-            classTidSets = []
-            itemSetX = [itemI]
-            for j in range(i + 1, len(itemSets)):
-                itemJ = itemSets[j]
-                tidSetJ = tidSets[j]
-                y = self._Intersection(tidSetI, tidSetJ)
-                if self._calculateExpSup(y) >= self._minSup:
-                    classItemSets.append(itemJ)
-                    classTidSets.append(y)
-            newPrefix = list(set(itemSetX)) + prefix
-            self._Generation(newPrefix, classItemSets, classTidSets)
-            self._save(prefix, list(set(itemSetX)), tidSetI)
-
-    def mine(self):
-        """
-        Main method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns
-        """
-        global _minSup
-        self._startTime = _ab._time.time()
-        self._creatingItemSets()
-        self._minSup = self._convert(self._minSup)
+        :return: None
+        """
+        global _minSup, _minWeight, _miniWeight, _maxWeight, _weights
+        self.__startTime = _fp._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
+        self.__creatingItemSets()
+        self._scanningWeights()
+        _weights = {k: v for k, v in _weights.items() if v >= _minWeight}
+        _maxWeight = max([s for s in _weights.values()])
+        _miniWeight = min([s for s in _weights.values()])
+        self._minSup = self.__convert(self._minSup)
         _minSup = self._minSup
-        plist = self._frequentOneItem()
-        for i in range(len(plist)):
-            itemI = plist[i]
-            tidSetI = self._tidList[itemI]
-            itemSetX = [itemI]
-            itemSets = []
-            tidSets = []
-            for j in range(i+1, len(plist)):
-                itemJ = plist[j]
-                tidSetJ = self._tidList[itemJ]
-                y1 = self._Intersection(tidSetI, tidSetJ)
-                if self._calculateExpSup(y1) >= self._minSup:
-                    itemSets.append(itemJ)
-                    tidSets.append(y1)
-            self._Generation(itemSetX, itemSets, tidSets)
-            self._save(None, itemSetX, tidSetI)
-        self._removeFalsePositives()
-        print("Frequent patterns were generated from uncertain databases successfully using PUF algorithm")
-        self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryRSS = float()
-        self._memoryUSS = float()
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        itemSet = self.__frequentOneItem()
+        updatedTransactions = self.__updateTransactions(itemSet)
+        for x, y in self.__rank.items():
+            self.__rankDup[y] = x
+        info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
+        __Tree = self.__buildTree(updatedTransactions, info)
+        patterns = __Tree.generatePatterns([])
+        self.__finalPatterns = {}
+        for k in patterns:
+            s = self.__savePeriodic(k[0])
+            self.__finalPatterns[str(s)] = k[1]
+        print("Weighted Frequent patterns were generated successfully using basic algorithm")
+        self.__endTime = _fp._time.time()
+        self.__memoryUSS = float()
+        self.__memoryRSS = float()
+        process = _fp._psutil.Process(_fp._os.getpid())
+        self.__memoryUSS = process.memory_full_info().uss
+        self.__memoryRSS = process.memory_info().rss
+
 
-    def getMemoryUSS(self):
+    def getMemoryUSS(self) -> float:
         """
 
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
-        return self._memoryUSS
+        return self.__memoryUSS
 
-    def getMemoryRSS(self):
+    def getMemoryRSS(self) -> float:
         """
 
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        Total amount of RSS memory consumed by the mining process will be retrieved from this function.
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
-        return self._memoryRSS
+        return self.__memoryRSS
 
-    def getRuntime(self):
+    def getRuntime(self) -> float:
         """
 
-        Calculating the total amount of runtime taken by the mining process
+        Calculating the total amount of runtime taken by the mining process.
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
-        return self._endTime - self._startTime
+        return self.__endTime - self.__startTime
 
-    def getPatternsAsDataFrame(self):
+    def getPatternsAsDataFrame(self) -> pd.DataFrame:
         """
 
-        Storing final frequent patterns in a dataframe
+        Storing final frequent patterns in a dataframe.
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self._finalPatterns.items():
+        for a, b in self.__finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+            dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
-    def save(self, oFile):
+    def save(self, outFile: str) -> None:
         """
 
-        Complete set of frequent patterns will be loaded in to an output file
+        Complete set of frequent patterns will be loaded in to an output file.
 
-        :param oFile: name of the output file
-        :type oFile: csv file
+        :param outFile: name of the output file
+        :type outFile: csv file
+        :return: None
         """
-        self.oFile = oFile
-        writer = open(self.oFile, 'w+')
-        for x, y in self._finalPatterns.items():
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
+        for x, y in self.__finalPatterns.items():
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self):
+    def getPatterns(self) -> Dict[str, int]:
         """
 
-        Function to send the set of frequent patterns after completion of the mining process
+        Function to send the set of frequent patterns after completion of the mining process.
 
         :return: returning frequent patterns
         :rtype: dict
         """
-        return self._finalPatterns
+        return self.__finalPatterns
 
-    def printResults(self):
+    def printResults(self) -> None:
         """
         This function is used to print the results
         """
-        print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of  Weighted Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
+        
+
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
-        if len(_ab._sys.argv) == 5:
-            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3])
+    if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
+        if len(_fp._sys.argv) == 7:
+            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
+        if len(_fp._sys.argv) == 6:
+            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
+        _ap.startMine()
         _ap.mine()
-        print("Total number of Patterns:", len(_ap.getPatterns()))
-        _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total number of Weighted Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_fp._sys.argv[2])
+        print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.5.1/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py` & `pami-2024.5.1.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2024.5.1.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2024.5.1.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-# WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
-# It stores the database in compressed fp-tree decreasing the memory usage and extracts the
-# patterns from tree.It employs downward closure property to  reduce the search space effectively.
+# WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database. It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
 #
 # **Importing this algorithm into a python program**
 #
-#             from PAMI.weightFrequentPattern.basic import basic as alg
+#             from PAMI.weightedFrequentRegularPattern.basic import WFRIMiner as alg
 #
 #             iFile = 'sampleDB.txt'
 #
 #             minSup = 10  # can also be specified between 0 and 1
 #
-#             obj = alg.basic(iFile, wFile, minSup, minWeight)
+#             obj = alg.WFRIMiner(iFile, WS, regularity)
 #
 #             obj.mine()
 #
-#             frequentPatterns = obj.getPatterns()
+#             weightedFrequentRegularPatterns = obj.getPatterns()
 #
-#             print("Total number of Frequent Patterns:", len(frequentPatterns))
+#             print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
 #
-#             obj.savePatterns(oFile)
+#             obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#             Df = obj.getPatternInDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
 #             memRSS = obj.getMemoryRSS()
 #
 #             print("Total Memory in RSS", memRSS)
 #
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -48,25 +47,25 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from PAMI.weightedFrequentPattern.basic import abstract as _fp
-from typing import List, Dict, Tuple, Union, Generator
+from PAMI.weightedFrequentRegularPattern.basic import abstract as _fp
 import pandas as pd
 from deprecated import deprecated
+from typing import List, Dict
 
 
-_minSup = str()
-_minWeight = int()
-_miniWeight = int()
-_maxWeight = int()
+_WS = str()
+_regularity = str()
+_lno = int()
 _weights = {}
+_wf = {}
 _fp._sys.setrecursionlimit(20000)
 
 
 class _Node:
     """
     A class used to represent the node of frequentPatternTree
 
@@ -84,31 +83,42 @@
         children: list
             To maintain the children of node
 
     :Methods:
 
         addChild(node)
             Updates the nodes children list and parent for the given node
+
     """
 
-    def __init__(self, item: str, children: list) -> None:
-        self.itemId = item
-        self.counter = 1
-        self.parent = None
+    def __init__(self, item: int, children: dict) -> None:
+        """
+        Initializing the Node class
+
+        :param item: Storing the item of a node
+        :type item: int or None
+        :param children: To maintain the children of a node
+        :type children: dict
+        :return: None
+        """
+
+        self.item = item
         self.children = children
+        self.parent = None
+        self.timeStamps = []
 
-    def addChild(self, node: '_Node') -> None:
+    def addChild(self, node) -> None:
         """
-        Retrieving the child from the tree
+        To add the children to a node
 
-        :param node: Children node
-        :type node: _Node
-        :return: Updates the children nodes and parent nodes
+        :param node: parent node in the tree
+        :return: None
         """
-        self.children[node.itemId] = node
+
+        self.children[node.item] = node
         node.parent = self
 
 
 class _Tree:
     """
     A class used to represent the frequentPatternGrowth tree structure
 
@@ -120,15 +130,14 @@
         summaries : dictionary
             Stores the nodes itemId which shares same itemId
 
         info : dictionary
             frequency of items in the transactions
 
     :Methods:
-
         addTransaction(transaction, freq)
             adding items of  transactions into the tree as nodes and freq is the count of nodes
         getFinalConditionalPatterns(node)
             getting the conditional patterns from fp-tree for a node
         getConditionalPatterns(patterns, frequencies)
             sort the patterns by removing the items with lower minSup
         generatePatterns(prefix)
@@ -136,152 +145,229 @@
     """
 
     def __init__(self) -> None:
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
-    def addTransaction(self, transaction: List[str], count: int) -> None:
+    def addTransaction(self, transaction: list, tid: list) -> None:
         """
-        Adding transaction into tree
+        Adding a transaction into tree
 
-        :param transaction: it represents the one transaction in database
+        :param transaction: To represent the complete database
         :type transaction: list
-        :param count: frequency of item
-        :type count: int
-        :return: None
+        :param tid: To represent the timestamp of a database
+        :type tid: list
+        :return: pfp-growth tree
         """
-        # This method takes transaction as input and returns the tree
         currentNode = self.root
         for i in range(len(transaction)):
             if transaction[i] not in currentNode.children:
                 newNode = _Node(transaction[i], {})
-                newNode.freq = count
                 currentNode.addChild(newNode)
                 if transaction[i] in self.summaries:
                     self.summaries[transaction[i]].append(newNode)
                 else:
                     self.summaries[transaction[i]] = [newNode]
                 currentNode = newNode
             else:
                 currentNode = currentNode.children[transaction[i]]
-                currentNode.freq += count
+        currentNode.timeStamps = currentNode.timeStamps + tid
 
-    def getFinalConditionalPatterns(self, alpha: str) -> Tuple[List[List[str]], List[int], Dict[str, int]]:
+    def getConditionalPatterns(self, alpha, pattern) -> tuple:
         """
-        Generates the conditional patterns for a node
+        Generates all the conditional patterns of a respective node
 
-        :param alpha: node to generate conditional patterns
-        :return: returns conditional patterns, frequency of each item in conditional patterns
+        :param alpha: To represent a Node in the tree
+        :type alpha: Node
+        :param pattern: prefix of the pattern
+        :type alpha: list
+        :return: A tuple consisting of finalPatterns, conditional pattern base and information
         """
         finalPatterns = []
-        finalFreq = []
+        finalSets = []
         for i in self.summaries[alpha]:
-            set1 = i.freq
+            set1 = i.timeStamps
             set2 = []
-            while i.parent.itemId is not None:
-                set2.append(i.parent.itemId)
+            while i.parent.item is not None:
+                set2.append(i.parent.item)
                 i = i.parent
             if len(set2) > 0:
                 set2.reverse()
                 finalPatterns.append(set2)
-                finalFreq.append(set1)
-        finalPatterns, finalFreq, info = self.getConditionalTransactions(finalPatterns, finalFreq)
-        return finalPatterns, finalFreq, info
+                finalSets.append(set1)
+        finalPatterns, finalSets, info = self.conditionalDatabases(finalPatterns, finalSets, pattern)
+        return finalPatterns, finalSets, info
+
+    @staticmethod
+    def generateTimeStamps(node) -> list:
+        """
+        To get the timestamps of a node
+
+        :param node: A node in the tree
+        :return: Timestamps of a node
+        """
+
+        finalTimeStamps = node.timeStamps
+        return finalTimeStamps
+
+    def removeNode(self, nodeValue) -> None:
+        """
+        Removing the node from tree
+
+        :param nodeValue: To represent a node in the tree
+        :type nodeValue: node
+        :return: Tree with their nodes updated with timestamps
+        """
+
+        for i in self.summaries[nodeValue]:
+            i.parent.timeStamps = i.parent.timeStamps + i.timeStamps
+            del i.parent.children[nodeValue]
+
+    def getTimeStamps(self, alpha) -> list:
+        """
+        To get all the timestamps of the nodes which share same item name
+
+        :param alpha: Node in a tree
+        :return: Timestamps of a  node
+        """
+        temporary = []
+        for i in self.summaries[alpha]:
+            temporary += i.timeStamps
+        return temporary
 
     @staticmethod
-    def getConditionalTransactions(ConditionalPatterns: List[List[str]], conditionalFreq: List[int]) -> Tuple[List[List[str]], List[int], Dict[str, int]]:
+    def getSupportAndPeriod(timeStamps: list, pattern: list) -> list:
         """
-        To calculate the frequency of items in conditional patterns and sorting the patterns
+        To calculate the periodicity and support
 
-        :param ConditionalPatterns: paths of a node
-        :param conditionalFreq: frequency of each item in the path
-        :return: conditional patterns and frequency of each item in transactions
+        :param timeStamps: Timestamps of an item set
+        :type timeStamps: list
+        :param pattern: pattern to evaluate the weighted frequent regular or not
+        :type pattern: list
+        :return: support, periodicity
+        """
+        global _WS, _regularity, _lno, _weights
+        timeStamps.sort()
+        cur = 0
+        per = list()
+        sup = 0
+        for j in range(len(timeStamps)):
+            per.append(timeStamps[j] - cur)
+            cur = timeStamps[j]
+            sup += 1
+        per.append(_lno - cur)
+        l = int()
+        for i in pattern:
+            l = l + _weights[i]
+        wf = (l / (len(pattern))) * sup
+        if len(per) == 0:
+            return [0, 0]
+        return [sup, max(per), wf]
+
+    def conditionalDatabases(self, conditionalPatterns: list, conditionalTimeStamps: list, pattern: list) -> tuple:
+        """
+        It generates the conditional patterns with periodic-frequent items
+
+        :param conditionalPatterns: conditionalPatterns generated from conditionPattern method of a respective node
+        :type conditionalPatterns: list
+        :param conditionalTimeStamps: Represents the timestamps of a conditional patterns of a node
+        :type conditionalTimeStamps: list
+        :param pattern: prefix of the pattern
+        :type pattern: list
+        :returns: Returns conditional transactions by removing non-periodic and non-frequent items
         """
-        global _minSup, _miniWeight
+        global _WS, _regularity
         pat = []
-        freq = []
+        timeStamps = []
         data1 = {}
-        for i in range(len(ConditionalPatterns)):
-            for j in ConditionalPatterns[i]:
+        for i in range(len(conditionalPatterns)):
+            for j in conditionalPatterns[i]:
                 if j in data1:
-                    data1[j] += conditionalFreq[i]
+                    data1[j] = data1[j] + conditionalTimeStamps[i]
                 else:
-                    data1[j] = conditionalFreq[i]
-        up_dict = {k: v for k, v in data1.items() if v >= _minSup and v * _miniWeight > _minSup}
+                    data1[j] = conditionalTimeStamps[i]
+        updatedDictionary = {}
+        for m in data1:
+            updatedDictionary[m] = self.getSupportAndPeriod(data1[m], pattern + [m])
+        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _WS and v[1] <= _regularity}
         count = 0
-        for p in ConditionalPatterns:
-            p1 = [v for v in p if v in up_dict]
-            trans = sorted(p1, key=lambda x: (up_dict.get(x), -x), reverse=True)
+        for p in conditionalPatterns:
+            p1 = [v for v in p if v in updatedDictionary]
+            trans = sorted(p1, key=lambda x: (updatedDictionary.get(x)[0], -x), reverse=True)
             if len(trans) > 0:
                 pat.append(trans)
-                freq.append(conditionalFreq[count])
+                timeStamps.append(conditionalTimeStamps[count])
             count += 1
-        return pat, freq, up_dict
+        return pat, timeStamps, updatedDictionary
 
-    def generatePatterns(self, prefix: List[str]) -> Generator[Tuple[List[str], int], None, None]:
+    def generatePatterns(self, prefix: list) -> None:
         """
-        To generate the frequent patterns
+        Generates the patterns
 
-        :param prefix: an empty list
-        :return: Frequent patterns that are extracted from fp-tree
+        :param prefix: Forms the combination of items
+        :type prefix: list
+        :returns: yields patterns with their support and periodicity
         """
-        global _miniWeight, _maxWeight, _minWeight, _minSup
-        for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
+        global _WS
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x)[0], -x)):
             pattern = prefix[:]
             pattern.append(i)
-            yield pattern, self.info[i]
-            patterns, freq, info = self.getFinalConditionalPatterns(i)
-            conditionalTree = _Tree()
-            conditionalTree.info = info.copy()
-            for pat in range(len(patterns)):
-                conditionalTree.addTransaction(patterns[pat], freq[pat])
-            if len(patterns) > 0:
-                for q in conditionalTree.generatePatterns(pattern):
-                    yield q
+            if self.info[i][2] >= _WS:
+                yield pattern, self.info[i]
+                patterns, timeStamps, info = self.getConditionalPatterns(i, pattern)
+                conditionalTree = _Tree()
+                conditionalTree.info = info.copy()
+                for pat in range(len(patterns)):
+                    conditionalTree.addTransaction(patterns[pat], timeStamps[pat])
+                if len(patterns) > 0:
+                    for q in conditionalTree.generatePatterns(pattern):
+                        yield q
+            self.removeNode(i)
 
 
-class WFIM(_fp._weightedFrequentPatterns):
+class WFRIMiner(_fp._weightedFrequentRegularPatterns):
     """
     About this algorithm
     ====================
 
-    :Description: * WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
-                  * It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+    :Description: WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database.
+       * It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
 
-    :Reference:  U. Yun and J. J. Leggett, “Wfim: weighted frequent itemset mining with a weight range and a minimum weight,”
-           In:   Proceedings of the 2005 SIAM International Conference on Data Mining. SIAM, 2005, pp. 636–640.
-                 https://epubs.siam.org/doi/pdf/10.1137/1.9781611972757.76
+    :Reference:  K. Klangwisan and K. Amphawan, "Mining weighted-frequent-regular itemsets from transactional database,"
+                 2017 9th International Conference on Knowledge and Smart Technology (KST), 2017, pp. 66-71,
+                 doi: 10.1109/KST.2017.7886090.
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of weighted Frequent Patterns.
+                   Name of the Input file to mine complete set of Weighted Frequent Regular Patterns.
     :param  oFile: str :
-                   Name of the output file to store complete set of weighted Frequent Patterns.
-    :param  minSup: str or int or float:
-                   minimum support thresholds were tuned to find the appropriate ranges in the limited memory
+                   Name of the output file to store complete set of Weighted Frequent Regular Patterns.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
+    :param  wFile: str :
+                   This is a weighted file.
+
 
 
-    :Attributes :
+    :Attributes:
 
         iFile : file
             Input file name or path of the input file
 
-        minSup: float or int or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+        WS: float or int or str
+            The user can specify WS either in count or proportion of database size.
+            If the program detects the data type of WS is integer, then it treats WS is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+            Example: WS=10 will be treated as integer, while WS=10.0 will be treated as float
 
-        minWeight: float or int or str
-            The user can specify minWeight either in count or proportion of database size.
-            If the program detects the data type of minWeight is integer, then it treats minWeight is expressed in count.
+        regularity: float or int or str
+            The user can specify regularity either in count or proportion of database size.
+            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minWeight=10 will be treated as integer, while minWeight=10.0 will be treated as float
+            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
 
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
             However, the users can override their default separator.
 
         oFile : file
             Name of the output file or the path of the output file
@@ -309,425 +395,434 @@
 
         tree : class
             it represents the Tree class
 
         finalPatterns : dict
             it represents to store the patterns
 
-    :Methods :
+    :Methods:
 
-        mine()
+        startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of frequent patterns will be loaded in to a output file
+            Complete set of frequent patterns will be loaded in to an output file
         getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingItemSets()
             Scans the dataset or dataframes and stores in list format
         frequentOneItem()
             Extracts the one-frequent patterns from transactions
 
+
     Execution methods
     =================
 
 
     **Terminal command**
 
-
     .. code-block:: console
 
-       Format:
+      Format:
 
-       (.venv) $ python3 basic.py <inputFile> <weightFile> <outputFile> <minSup> <minWeight>
+      (.venv) $ python3 WFRIMiner.py <inputFile> <outputFile> <weightSupport> <regularity>
 
-       Example Usage:
+      Example Usage:
 
-       (.venv) $ python3 basic.py sampleDB.txt weightSample.txt patterns.txt 10.0 3.4
+      (.venv) $ python3 WFRIMiner.py sampleDB.txt patterns.txt 10 5
 
-    .. note:: minSup and maxPer will be considered in support count or frequency
+    .. note:: WS & regularity will be considered in support count or frequency
 
 
     **Calling from a python program**
 
     .. code-block:: python
 
-            from PAMI.weightFrequentPattern.basic import basic as alg
+            from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
 
             iFile = 'sampleDB.txt'
 
             minSup = 10  # can also be specified between 0 and 1
 
-            obj = alg.basic(iFile, wFile, minSup, minWeight)
+            obj = alg.WFRIMiner(iFile, WS, regularity)
 
             obj.mine()
 
-            frequentPatterns = obj.getPatterns()
+            weightedFrequentRegularPatterns = obj.getPatterns()
 
-            print("Total number of Frequent Patterns:", len(frequentPatterns))
+            print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
 
-            obj.savePatterns(oFile)
+            obj.save(oFile)
 
-            Df = obj.getPatternsAsDataFrame()
+            Df = obj.getPatternInDataFrame()
 
-            memUSS = obj.getmemoryUSS()
+            memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     Credits
     =======
 
-
              The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+
     """
 
-    __startTime = float()
-    __endTime = float()
-    _minSup = str()
-    __finalPatterns = {}
+    _startTime = float()
+    _endTime = float()
+    _WS = str()
+    _regularity = str()
+    _weight = {}
+    _finalPatterns = {}
+    _wFile = " "
     _iFile = " "
     _oFile = " "
     _sep = " "
-    __memoryUSS = float()
-    __memoryRSS = float()
-    __Database = []
-    __mapSupport = {}
-    __lno = 0
-    __tree = _Tree()
-    __rank = {}
-    __rankDup = {}
+    _memoryUSS = float()
+    _memoryRSS = float()
+    _Database = []
+    _mapSupport = {}
+    _lno = 0
+    _tree = _Tree()
+    _rank = {}
+    _rankDup = {}
 
-    def __init__(self, iFile: str, wFile: str, minSup: str, minWeight: int, sep: str='\t') -> None:
-        super().__init__(iFile, wFile, minSup, minWeight, sep)
+    def __init__(self, iFile, _wFile, WS, regularity, sep='\t') -> None:
+        super().__init__(iFile, _wFile, WS, regularity, sep)
 
-    def __creatingItemSets(self) -> None:
+    def _creatingItemSets(self) -> None:
         """
         Storing the complete transactions of the database/input file in a database variable
 
         :return: None
         """
-        self.__Database = []
+        self._Database = []
+        self._weight = {}
         if isinstance(self._iFile, _fp._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self.__Database = self._iFile['Transactions'].tolist()
+                self._Database = self._iFile['Transactions'].tolist()
+
+        if isinstance(self._wFile, _fp._pd.DataFrame):
+            _items, _weights = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                _items = self._wFile['items'].tolist()
+            if 'weight' in i:
+                _weights = self._wFile['weight'].tolist()
+            for i in range(len(_items)):
+                self._weight[_items[i]] = _weights[i]
 
             # print(self.Database)
         if isinstance(self._iFile, str):
             if _fp._validators.url(self._iFile):
                 data = _fp._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self.__Database.append(temp)
+                    self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            # print(len(temp))
-                            self.__Database.append(temp)
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _scanningWeights(self) -> None:
-        """
-        Storing the weights of the variables in input file in a weights variable
-
-        :return: None
-        """
-        global _weights
-        _weights = {}
-        if isinstance(self._wFile, _fp._pd.DataFrame):
-            items, weights = [], []
-            if self._wFile.empty:
-                print("its empty..")
-            i = self._wFile.columns.values.tolist()
-            if 'items' in i:
-                items = self._wFile['items'].tolist()
-            if 'weights' in i:
-                weights = self._wFile['weights'].tolist()
-            for i in range(len(weights)):
-                _weights[items[i]] = weights[i]
-
-            # print(self.Database)
         if isinstance(self._wFile, str):
             if _fp._validators.url(self._wFile):
                 data = _fp._urlopen(self._wFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    _weights[temp[0]] = temp[1]
+                    self._weight[temp[0]] = float(temp[1])
             else:
                 try:
                     with open(self._wFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            s = int(float(temp[1]))
-                            _weights[temp[0]] = s
+                            self._weight[temp[0]] = float(temp[1])
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def __convert(self, value: Union[int, float, str]) -> Union[int, float]:
+    def _convert(self, value) -> float:
         """
-        To convert the type of user specified minSup value.
+        To convert the type of user specified minSup value
 
         :param value: user specified minSup value
         :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = (len(self.__Database) * value)
+            value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
-                value = (len(self.__Database) * value)
+                value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
-    def __frequentOneItem(self) -> List[str]:
+    def _frequentOneItem(self) -> List[str]:
         """
         Generating One frequent items sets
 
         :return: list
         """
-        global _maxWeight
-        self.__mapSupport = {}
-        for tr in self.__Database:
-            for i in range(0, len(tr)):
-                if tr[i] not in self.__mapSupport:
-                    self.__mapSupport[tr[i]] = 1
+        global _lno, _wf, _weights
+        self._mapSupport = {}
+        _owf = {}
+        for tr in self._Database:
+            for i in range(1, len(tr)):
+                if tr[i] not in self._mapSupport:
+                    self._mapSupport[tr[i]] = [int(tr[0]), int(tr[0]), 1]
                 else:
-                    self.__mapSupport[tr[i]] += 1
-        self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= self._minSup and v * _maxWeight > self._minSup}
-        genList = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        self.__rank = dict([(index, item) for (item, index) in enumerate(genList)])
+                    self._mapSupport[tr[i]][0] = max(self._mapSupport[tr[i]][0], (int(tr[0]) - self._mapSupport[tr[i]][1]))
+                    self._mapSupport[tr[i]][1] = int(tr[0])
+                    self._mapSupport[tr[i]][2] += 1
+        for key in self._mapSupport:
+            self._mapSupport[key][0] = max(self._mapSupport[key][0], abs(len(self._Database) - self._mapSupport[key][1]))
+        _lno = len(self._Database)
+        self._mapSupport = {k: [v[2], v[0]] for k, v in self._mapSupport.items() if v[0] <= self._regularity}
+        for x, y in self._mapSupport.items():
+            if self._weight.get(x) is None:
+                self._weight[x] = 0
+        gmax = max([self._weight[values] for values in self._mapSupport.keys()])
+        for x, y in self._mapSupport.items():
+            _owf[x] = y[0] * gmax
+        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v[0] * _owf[k] >= self._WS}
+        for x, y in self._mapSupport.items():
+            temp = self._weight[x] * y[0]
+            _wf[x] = temp
+            self._mapSupport[x].append(temp)
+        genList = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse= True)]
+        self._rank = dict([(index, item) for (item, index) in enumerate(genList)])
+        for x, y in self._rank.items():
+            _weights[y] = self._weight[x]
         return genList
 
-    def __updateTransactions(self, itemSet: List[str]) -> List[List[int]]:
+    def _updateTransactions(self, itemSet) -> List[List[int]]:
         """
         Updates the items in transactions with rank of items according to their support
 
         :Example: oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
-                    rank = {'a':0, 'b':1, 'c':2, 'd':3}
+                  rank = {'a':0, 'b':1, 'c':2, 'd':3}
 
         :param itemSet: list of one-frequent items
-        :return: list
+        :return: None
         """
         list1 = []
-        for tr in self.__Database:
-            list2 = []
-            for i in range(len(tr)):
+        for tr in self._Database:
+            list2 = [int(tr[0])]
+            for i in range(1, len(tr)):
                 if tr[i] in itemSet:
-                    list2.append(self.__rank[tr[i]])
-            if len(list2) >= 1:
-                list2.sort()
+                    list2.append(self._rank[tr[i]])
+            if len(list2) >= 2:
+                basket = list2[1:]
+                basket.sort()
+                list2[1:] = basket[0:]
                 list1.append(list2)
         return list1
 
     @staticmethod
-    def __buildTree(transactions: List[List[int]], info: Dict[int, int]) -> '_Tree':
+    def _buildTree(transactions, info) -> _Tree:
         """
         Builds the tree with updated transactions
 
         :param transactions: updated transactions
-        :param info: support details of each item in transactions.
-        :return: Transactions compressed in fp-tree
+        :param info: support details of each item in transactions
+        :return: transactions compressed in fp-tree
+
         """
         rootNode = _Tree()
         rootNode.info = info.copy()
         for i in range(len(transactions)):
-            rootNode.addTransaction(transactions[i], 1)
+            set1 = [transactions[i][0]]
+            rootNode.addTransaction(transactions[i][1:], set1)
         return rootNode
 
-    def __savePeriodic(self, itemSet: List[int]) -> str:
+    def _savePeriodic(self, itemSet) -> str:
         """
         The duplication items and their ranks
 
         :param itemSet: frequent itemSet that generated
         :return: patterns with original item names.
+
         """
         temp = str()
         for i in itemSet:
-            temp = temp + self.__rankDup[i] + "\t"
+            temp = temp + self._rankDup[i] + "\t"
         return temp
 
     @deprecated(
         "It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
-        main program to start the operation
-
-        :return: None
+        Frequent pattern mining process will start from here
         """
         self.mine()
 
     def mine(self) -> None:
         """
-        main program to start the operation
-
-        :return: None
+        Frequent pattern mining process will start from here
         """
-        global _minSup, _minWeight, _miniWeight, _maxWeight, _weights
-        self.__startTime = _fp._time.time()
+        global _WS, _regularity, _weights
+        self._startTime = _fp._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
+        if self._WS is None:
             raise Exception("Please enter the Minimum Support")
-        self.__creatingItemSets()
-        self._scanningWeights()
-        _weights = {k: v for k, v in _weights.items() if v >= _minWeight}
-        _maxWeight = max([s for s in _weights.values()])
-        _miniWeight = min([s for s in _weights.values()])
-        self._minSup = self.__convert(self._minSup)
-        _minSup = self._minSup
-        itemSet = self.__frequentOneItem()
-        updatedTransactions = self.__updateTransactions(itemSet)
-        for x, y in self.__rank.items():
-            self.__rankDup[y] = x
-        info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
-        __Tree = self.__buildTree(updatedTransactions, info)
-        patterns = __Tree.generatePatterns([])
-        self.__finalPatterns = {}
+        self._creatingItemSets()
+        self._WS = self._convert(self._WS)
+        self._regularity = self._convert(self._regularity)
+        _WS, _regularity, _weights = self._WS, self._regularity, self._weight
+        itemSet = self._frequentOneItem()
+        updatedTransactions = self._updateTransactions(itemSet)
+        for x, y in self._rank.items():
+            self._rankDup[y] = x
+        info = {self._rank[k]: v for k, v in self._mapSupport.items()}
+        _Tree = self._buildTree(updatedTransactions, info)
+        patterns = _Tree.generatePatterns([])
+        self._finalPatterns = {}
         for k in patterns:
-            s = self.__savePeriodic(k[0])
-            self.__finalPatterns[str(s)] = k[1]
-        print("Weighted Frequent patterns were generated successfully using basic algorithm")
-        self.__endTime = _fp._time.time()
-        self.__memoryUSS = float()
-        self.__memoryRSS = float()
+            s = self._savePeriodic(k[0])
+            self._finalPatterns[str(s)] = k[1]
+        print("Weighted Frequent Regular patterns were generated successfully using WFRIM algorithm")
+        self._endTime = _fp._time.time()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
         process = _fp._psutil.Process(_fp._os.getpid())
-        self.__memoryUSS = process.memory_full_info().uss
-        self.__memoryRSS = process.memory_info().rss
-
+        self._memoryRSS = float()
+        self._memoryUSS = float()
+        self._memoryUSS = process.memory_full_info().uss
+        self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self) -> float:
         """
 
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
-        return self.__memoryUSS
+        return self._memoryUSS
 
     def getMemoryRSS(self) -> float:
         """
 
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function.
+        Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
-        return self.__memoryRSS
+        return self._memoryRSS
 
     def getRuntime(self) -> float:
         """
 
-        Calculating the total amount of runtime taken by the mining process.
+        Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
-        return self.__endTime - self.__startTime
+        return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> pd.DataFrame:
+    def getPatternsAsDataFrame(self) -> _fp._pd.DataFrame:
         """
 
-        Storing final frequent patterns in a dataframe.
+        Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self.__finalPatterns.items():
+        for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile: str) -> None:
         """
 
-        Complete set of frequent patterns will be loaded in to an output file.
+        Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csv file
         :return: None
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
-        for x, y in self.__finalPatterns.items():
+        for x, y in self._finalPatterns.items():
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self) -> Dict[str, int]:
+    def getPatterns(self) -> Dict[str, float]:
         """
 
-        Function to send the set of frequent patterns after completion of the mining process.
+        Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
-        return self.__finalPatterns
+        return self._finalPatterns
 
     def printResults(self) -> None:
         """
         This function is used to print the results
         """
-        print("Total number of  Weighted Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of  Weighted Frequent Regular Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
-        
-
 
 if __name__ == "__main__":
     _ap = str()
     if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
         if len(_fp._sys.argv) == 7:
-            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
-        if len(_fp._sys.argv) == 6:
-            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
+            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
+        if len(_fp._sys.argv) == 5:
+            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
         _ap.startMine()
         _ap.mine()
-        print("Total number of Weighted Frequent Patterns:", len(_ap.getPatterns()))
+        print("Total number of Weighted Frequent Regular Patterns:", len(_ap.getPatterns()))
         _ap.save(_fp._sys.argv[2])
         print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2024.5.1/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2024.5.1.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database. It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
+# WUFIM is one of the algorithm to discover weighted frequent patterns in an uncertain transactional database using PUF-Tree.
 #
 # **Importing this algorithm into a python program**
 #
-#             from PAMI.weightedFrequentRegularPattern.basic import WFRIMiner as alg
+#             from PAMI.weightedUncertainFrequentPattern.basic import basic as alg
 #
 #             iFile = 'sampleDB.txt'
 #
-#             minSup = 10  # can also be specified between 0 and 1
+#             minSup = 10
 #
-#             obj = alg.WFRIMiner(iFile, WS, regularity)
+#             obj = alg.basic(iFile, wFile, minSup, sep)
 #
 #             obj.mine()
 #
-#             weightedFrequentRegularPatterns = obj.getPatterns()
+#             Patterns = obj.getPatterns()
 #
-#             print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
+#             print("Total number of  Patterns:", len(Patterns))
 #
 #             obj.save(oFile)
 #
-#             Df = obj.getPatternInDataFrame()
+#             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
 #             memRSS = obj.getMemoryRSS()
 #
@@ -44,691 +44,730 @@
 
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
-     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+     along with this program.  If not, see `<https://www.gnu.org/licenses/>`_.    
 """
 
-from PAMI.weightedFrequentRegularPattern.basic import abstract as _fp
+from PAMI.weightedUncertainFrequentPattern.basic import abstract as _ab
 import pandas as pd
 from deprecated import deprecated
-from typing import List, Dict
 
-
-_WS = str()
-_regularity = str()
-_lno = int()
+_expSup = str()
+_expWSup = str()
 _weights = {}
-_wf = {}
-_fp._sys.setrecursionlimit(20000)
+_finalPatterns = {}
+_ab._sys.setrecursionlimit(20000)
+class _Item:
+    """
+    A class used to represent the item with probability in transaction of dataset
+
+    :Attributes:
+
+        item : int or word
+          Represents the name of the item
+
+        probability : float
+          Represent the existential probability(likelihood presence) of an item
+    """
+
+    def __init__(self, item: int, probability: float) -> None:
+        self.item = item
+        self.probability = probability
 
 
-class _Node:
+class _Node(object):
     """
     A class used to represent the node of frequentPatternTree
 
     :Attributes:
 
-        itemId: int
-            storing item of a node
+        item : int
+          storing item of a node
 
-        counter: int
-            To maintain the support of node
+        probability : int
+          To maintain the expected support of node
 
-        parent: node
-            To maintain the parent of node
+        parent : node
+          To maintain the parent of every node
 
-        children: list
-            To maintain the children of node
+        children : list
+          To maintain the children of node
 
     :Methods:
 
-        addChild(node)
-            Updates the nodes children list and parent for the given node
-
+        addChild(itemName)
+            storing the children to their respective parent nodes
     """
 
-    def __init__(self, item: int, children: dict) -> None:
-        """
-        Initializing the Node class
-
-        :param item: Storing the item of a node
-        :type item: int or None
-        :param children: To maintain the children of a node
-        :type children: dict
-        :return: None
-        """
-
+    def __init__(self, item, children: list) -> None:
         self.item = item
+        self.probability = 1
         self.children = children
         self.parent = None
-        self.timeStamps = []
 
     def addChild(self, node) -> None:
         """
-        To add the children to a node
+        This method is used to add a child node to the current node in the frequent pattern tree.
 
-        :param node: parent node in the tree
+        :param node:The node to be added as a child
+        :type node:_Node
         :return: None
         """
-
         self.children[node.item] = node
         node.parent = self
 
 
-class _Tree:
+class _Tree(object):
     """
     A class used to represent the frequentPatternGrowth tree structure
 
     :Attributes:
 
         root : Node
-            The first node of the tree set to Null.
+            Represents the root node of the tree
 
         summaries : dictionary
-            Stores the nodes itemId which shares same itemId
+            storing the nodes with same item name
 
         info : dictionary
-            frequency of items in the transactions
+            stores the support of items
 
     :Methods:
-        addTransaction(transaction, freq)
-            adding items of  transactions into the tree as nodes and freq is the count of nodes
-        getFinalConditionalPatterns(node)
-            getting the conditional patterns from fp-tree for a node
-        getConditionalPatterns(patterns, frequencies)
-            sort the patterns by removing the items with lower minSup
-        generatePatterns(prefix)
-            generating the patterns from fp-tree
+
+        addTransaction(transaction)
+            creating transaction as a branch in frequentPatternTree
+        addConditionalPattern(prefixPaths, supportOfItems)
+            construct the conditional tree for prefix paths
+        conditionalPatterns(Node)
+            generates the conditional patterns from tree for specific node
+        conditionalTransactions(prefixPaths,Support)
+            takes the prefixPath of a node and support at child of the path and extract the frequent items from prefixPaths and generates prefixPaths with items which are frequent
+        remove(Node)
+            removes the node from tree once after generating all the patterns respective to the node
+        generatePatterns(Node)
+            starts from the root node of the tree and mines the frequent patterns
+
     """
 
     def __init__(self) -> None:
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
-    def addTransaction(self, transaction: list, tid: list) -> None:
+    def addTransaction(self, transaction) -> None:
         """
-        Adding a transaction into tree
+        Adding transaction into tree
 
-        :param transaction: To represent the complete database
+        :param transaction: it represents the one self.Database in database
         :type transaction: list
-        :param tid: To represent the timestamp of a database
-        :type tid: list
-        :return: pfp-growth tree
+        :return: None
         """
         currentNode = self.root
         for i in range(len(transaction)):
+            if transaction[i].item not in currentNode.children:
+                newNode = _Node(transaction[i].item, {})
+                l1 = i - 1
+                lp = []
+                while l1 >= 0:
+                    lp.append(transaction[l1].probability)
+                    l1 -= 1
+                if len(lp) == 0:
+                    newNode.probability = transaction[i].probability
+                else:
+                    newNode.probability = max(lp) * transaction[i].probability
+                currentNode.addChild(newNode)
+                if transaction[i].item in self.summaries:
+                    self.summaries[transaction[i].item].append(newNode)
+                else:
+                    self.summaries[transaction[i].item] = [newNode]
+                currentNode = newNode
+            else:
+                currentNode = currentNode.children[transaction[i].item]
+                l1 = i - 1
+                lp = []
+                while l1 >= 0:
+                    lp.append(transaction[l1].probability)
+                    l1 -= 1
+                if len(lp) == 0:
+                    currentNode.probability += transaction[i].probability
+                else:
+                    currentNode.probability += max(lp) * transaction[i].probability
+
+    def addConditionalPattern(self, transaction, sup) -> None:
+        """
+        constructing conditional tree from prefixPaths
+
+        :param transaction : it represents the one self.Database in database
+        :type transaction : list
+        :param sup : support of prefixPath taken at last child of the path
+        :type sup : int
+        :return: None
+        """
+        # This method takes transaction, support and constructs the conditional tree
+        currentNode = self.root
+        for i in range(len(transaction)):
             if transaction[i] not in currentNode.children:
                 newNode = _Node(transaction[i], {})
+                newNode.probability = sup
                 currentNode.addChild(newNode)
                 if transaction[i] in self.summaries:
                     self.summaries[transaction[i]].append(newNode)
                 else:
                     self.summaries[transaction[i]] = [newNode]
                 currentNode = newNode
             else:
                 currentNode = currentNode.children[transaction[i]]
-        currentNode.timeStamps = currentNode.timeStamps + tid
+                currentNode.probability += sup
 
-    def getConditionalPatterns(self, alpha, pattern) -> tuple:
+    def conditionalPatterns(self, alpha) -> tuple:
         """
-        Generates all the conditional patterns of a respective node
+        generates all the conditional patterns of respective node
 
-        :param alpha: To represent a Node in the tree
-        :type alpha: Node
-        :param pattern: prefix of the pattern
-        :type alpha: list
-        :return: A tuple consisting of finalPatterns, conditional pattern base and information
+        :param alpha : it represents the Node in tree
+        :type alpha : _Node
+        :return: tuple
         """
+        # This method generates conditional patterns of node by traversing the tree
         finalPatterns = []
-        finalSets = []
+        sup = []
         for i in self.summaries[alpha]:
-            set1 = i.timeStamps
+            s = i.probability
             set2 = []
             while i.parent.item is not None:
                 set2.append(i.parent.item)
                 i = i.parent
             if len(set2) > 0:
                 set2.reverse()
                 finalPatterns.append(set2)
-                finalSets.append(set1)
-        finalPatterns, finalSets, info = self.conditionalDatabases(finalPatterns, finalSets, pattern)
-        return finalPatterns, finalSets, info
-
-    @staticmethod
-    def generateTimeStamps(node) -> list:
-        """
-        To get the timestamps of a node
-
-        :param node: A node in the tree
-        :return: Timestamps of a node
-        """
-
-        finalTimeStamps = node.timeStamps
-        return finalTimeStamps
+                sup.append(s)
+        finalPatterns, support, info = self.conditionalTransactions(finalPatterns, sup)
+        return finalPatterns, support, info
 
     def removeNode(self, nodeValue) -> None:
         """
         Removing the node from tree
 
-        :param nodeValue: To represent a node in the tree
-        :type nodeValue: node
-        :return: Tree with their nodes updated with timestamps
+        :param nodeValue : it represents the node in tree
+        :type nodeValue : node
+        :return: None
         """
 
         for i in self.summaries[nodeValue]:
-            i.parent.timeStamps = i.parent.timeStamps + i.timeStamps
             del i.parent.children[nodeValue]
 
-    def getTimeStamps(self, alpha) -> list:
+    def conditionalTransactions(self, condPatterns, support) -> tuple:
         """
-        To get all the timestamps of the nodes which share same item name
+        It generates the conditional patterns with frequent items
 
-        :param alpha: Node in a tree
-        :return: Timestamps of a  node
+        :param condPatterns : conditionalPatterns generated from conditionalPattern method for respective node
+        :type condPatterns : list
+        :support : the support of conditional pattern in tree
+        :support : int
+        :return: tuple
         """
-        temporary = []
-        for i in self.summaries[alpha]:
-            temporary += i.timeStamps
-        return temporary
-
-    @staticmethod
-    def getSupportAndPeriod(timeStamps: list, pattern: list) -> list:
-        """
-        To calculate the periodicity and support
-
-        :param timeStamps: Timestamps of an item set
-        :type timeStamps: list
-        :param pattern: pattern to evaluate the weighted frequent regular or not
-        :type pattern: list
-        :return: support, periodicity
-        """
-        global _WS, _regularity, _lno, _weights
-        timeStamps.sort()
-        cur = 0
-        per = list()
-        sup = 0
-        for j in range(len(timeStamps)):
-            per.append(timeStamps[j] - cur)
-            cur = timeStamps[j]
-            sup += 1
-        per.append(_lno - cur)
-        l = int()
-        for i in pattern:
-            l = l + _weights[i]
-        wf = (l / (len(pattern))) * sup
-        if len(per) == 0:
-            return [0, 0]
-        return [sup, max(per), wf]
-
-    def conditionalDatabases(self, conditionalPatterns: list, conditionalTimeStamps: list, pattern: list) -> tuple:
-        """
-        It generates the conditional patterns with periodic-frequent items
-
-        :param conditionalPatterns: conditionalPatterns generated from conditionPattern method of a respective node
-        :type conditionalPatterns: list
-        :param conditionalTimeStamps: Represents the timestamps of a conditional patterns of a node
-        :type conditionalTimeStamps: list
-        :param pattern: prefix of the pattern
-        :type pattern: list
-        :returns: Returns conditional transactions by removing non-periodic and non-frequent items
-        """
-        global _WS, _regularity
+        global _expSup, _expWSup
         pat = []
-        timeStamps = []
-        data1 = {}
-        for i in range(len(conditionalPatterns)):
-            for j in conditionalPatterns[i]:
-                if j in data1:
-                    data1[j] = data1[j] + conditionalTimeStamps[i]
+        sup = []
+        count = {}
+        for i in range(len(condPatterns)):
+            for j in condPatterns[i]:
+                if j in count:
+                    count[j] += support[i]
                 else:
-                    data1[j] = conditionalTimeStamps[i]
-        updatedDictionary = {}
-        for m in data1:
-            updatedDictionary[m] = self.getSupportAndPeriod(data1[m], pattern + [m])
-        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _WS and v[1] <= _regularity}
+                    count[j] = support[i]
+        updatedDict = {}
+        updatedDict = {k: v for k, v in count.items() if v >= _expSup}
         count = 0
-        for p in conditionalPatterns:
-            p1 = [v for v in p if v in updatedDictionary]
-            trans = sorted(p1, key=lambda x: (updatedDictionary.get(x)[0], -x), reverse=True)
+        for p in condPatterns:
+            p1 = [v for v in p if v in updatedDict]
+            trans = sorted(p1, key=lambda x: updatedDict[x], reverse=True)
             if len(trans) > 0:
                 pat.append(trans)
-                timeStamps.append(conditionalTimeStamps[count])
-            count += 1
-        return pat, timeStamps, updatedDictionary
+                sup.append(support[count])
+                count += 1
+        return pat, sup, updatedDict
 
-    def generatePatterns(self, prefix: list) -> None:
+    def generatePatterns(self, prefix) -> None:
         """
         Generates the patterns
 
-        :param prefix: Forms the combination of items
-        :type prefix: list
-        :returns: yields patterns with their support and periodicity
+        :param prefix : forms the combination of items
+        :type prefix : list
+        :return: None
         """
-        global _WS
-        for i in sorted(self.summaries, key=lambda x: (self.info.get(x)[0], -x)):
+
+        global _finalPatterns, _expSup, _expWSup, _weights
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x))):
             pattern = prefix[:]
             pattern.append(i)
-            if self.info[i][2] >= _WS:
-                yield pattern, self.info[i]
-                patterns, timeStamps, info = self.getConditionalPatterns(i, pattern)
+            weight = 0
+            for k in pattern:
+                weight = weight + _weights[k]
+            weight = weight/len(pattern)
+            if self.info.get(i) >= _expSup and self.info.get(i) * weight >= _expWSup:
+                _finalPatterns[tuple(pattern)] = self.info.get(i)
+                patterns, support, info = self.conditionalPatterns(i)
                 conditionalTree = _Tree()
                 conditionalTree.info = info.copy()
                 for pat in range(len(patterns)):
-                    conditionalTree.addTransaction(patterns[pat], timeStamps[pat])
+                    conditionalTree.addConditionalPattern(patterns[pat], support[pat])
                 if len(patterns) > 0:
-                    for q in conditionalTree.generatePatterns(pattern):
-                        yield q
+                    conditionalTree.generatePatterns(pattern)
             self.removeNode(i)
 
-
-class WFRIMiner(_fp._weightedFrequentRegularPatterns):
+class WUFIM(_ab._weightedFrequentPatterns):
     """
     About this algorithm
     ====================
 
-    :Description: WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database.
-       * It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
+    :Description: It is one of the algorithm to discover weighted frequent patterns in a uncertain transactional database using PUF-Tree.
 
-    :Reference:  K. Klangwisan and K. Amphawan, "Mining weighted-frequent-regular itemsets from transactional database,"
-                 2017 9th International Conference on Knowledge and Smart Technology (KST), 2017, pp. 66-71,
-                 doi: 10.1109/KST.2017.7886090.
+    :Reference: Efficient Mining of Weighted Frequent Itemsets in Uncertain Databases.
+           In : Machine Learning and Data Mining in Pattern Recognition book Chun-Wei Jerry Lin, Wensheng Gan, Philippe Fournier Viger, Tzung-Pei Hong
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of Weighted Frequent Regular Patterns.
+                   Name of the Input file to mine complete set of Weighted Uncertain Periodic Frequent Patterns
     :param  oFile: str :
-                   Name of the output file to store complete set of Weighted Frequent Regular Patterns.
+                   Name of the output file to store complete set of Weighted  Uncertain Periodic Frequent Patterns
+    :param  minSup: str:
+                   minimum support thresholds were tuned to find the appropriate ranges in the limited memory
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
     :param  wFile: str :
-                   This is a weighted file.
-
+                    This is a weighted file.
 
 
     :Attributes:
 
         iFile : file
-            Input file name or path of the input file
-
-        WS: float or int or str
-            The user can specify WS either in count or proportion of database size.
-            If the program detects the data type of WS is integer, then it treats WS is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: WS=10 will be treated as integer, while WS=10.0 will be treated as float
-
-        regularity: float or int or str
-            The user can specify regularity either in count or proportion of database size.
-            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
+          Name of the Input file or path of the input file
 
-        sep : str
-            This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
-            However, the users can override their default separator.
+        wFile : file
+          Name of the Input file or path of the input file
 
         oFile : file
-            Name of the output file or the path of the output file
+          Name of the output file or path of the output file
 
-        startTime:float
-            To record the start time of the mining process
+        minSup : float or int or str
+          The user can specify minSup either in count or proportion of database size.
+          If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+          Otherwise, it will be treated as float.
+          Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
 
-        endTime:float
-            To record the completion time of the mining process
+        sep : str
+          This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+          However, the users can override their default separator.
 
         memoryUSS : float
-            To store the total amount of USS memory consumed by the program
+          To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
+          To store the total amount of RSS memory consumed by the program
+
+        startTime:float
+          To record the start time of the mining process
+
+        endTime:float
+          To record the completion time of the mining process
 
         Database : list
-            To store the transactions of a database in list
+          To store the transactions of a database in list
 
         mapSupport : Dictionary
-            To maintain the information of item and their frequency
+          To maintain the information of item and their frequency
 
         lno : int
-            it represents the total no of transactions
+          To represent the total no of transaction
 
         tree : class
-            it represents the Tree class
+          To represents the Tree class
+
+        itemSetCount : int
+          To represents the total no of patterns
 
         finalPatterns : dict
-            it represents to store the patterns
+          To store the complete patterns
 
     :Methods:
 
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of frequent patterns will be loaded in to an output file
+            Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets()
-            Scans the dataset or dataframes and stores in list format
+        creatingItemSets(fileName)
+            Scans the dataset and stores in a list format
         frequentOneItem()
-            Extracts the one-frequent patterns from transactions
-
+            Extracts the one-length frequent patterns from database
+        updateTransactions()
+            Update the transactions by removing non-frequent items and sort the Database by item decreased support
+        buildTree()
+            After updating the Database, remaining items will be added into the tree by setting root node as null
+        convert()
+            to convert the user specified value
+        startMine()
+            Mining process will start from this function
 
     Execution methods
     =================
 
 
     **Terminal command**
 
+
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 WFRIMiner.py <inputFile> <outputFile> <weightSupport> <regularity>
+      (.venv) $ python3 basic.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 WFRIMiner.py sampleDB.txt patterns.txt 10 5
-
-    .. note:: WS & regularity will be considered in support count or frequency
+      (.venv) $ python3 basic.py sampleTDB.txt patterns.txt 3
 
+    .. note:: minSup  will be considered in support count or frequency
 
     **Calling from a python program**
 
     .. code-block:: python
 
-            from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
+            from PAMI.weightedUncertainFrequentPattern.basic import basic as alg
 
             iFile = 'sampleDB.txt'
 
             minSup = 10  # can also be specified between 0 and 1
 
-            obj = alg.WFRIMiner(iFile, WS, regularity)
+            obj = alg.basic(iFile, wFile, expSup, expWSup)
 
             obj.mine()
 
-            weightedFrequentRegularPatterns = obj.getPatterns()
+            Patterns = obj.getPatterns()
 
-            print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
+            print("Total number of  Patterns:", len(Patterns))
 
             obj.save(oFile)
 
-            Df = obj.getPatternInDataFrame()
+            Df = obj.getPatternsAsDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
-    Credits
-    =======
-
-             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
-
-    """
-
+   """
     _startTime = float()
     _endTime = float()
-    _WS = str()
-    _regularity = str()
-    _weight = {}
+    _minSup = str()
     _finalPatterns = {}
-    _wFile = " "
     _iFile = " "
+    _wFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _mapSupport = {}
-    _lno = 0
-    _tree = _Tree()
     _rank = {}
-    _rankDup = {}
+    _expSup = float()
+    _expWSup = float()
 
-    def __init__(self, iFile, _wFile, WS, regularity, sep='\t') -> None:
-        super().__init__(iFile, _wFile, WS, regularity, sep)
+    def __init__(self, iFile, wFile, expSup, expWSup, sep='\t') -> None:
+        super().__init__(iFile, wFile, expSup, expWSup, sep)
 
     def _creatingItemSets(self) -> None:
         """
-        Storing the complete transactions of the database/input file in a database variable
+        Scans the uncertain transactional dataset
 
         :return: None
         """
         self._Database = []
-        self._weight = {}
-        if isinstance(self._iFile, _fp._pd.DataFrame):
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
-
-        if isinstance(self._wFile, _fp._pd.DataFrame):
-            _items, _weights = [], []
-            if self._wFile.empty:
-                print("its empty..")
-            i = self._wFile.columns.values.tolist()
-            if 'items' in i:
-                _items = self._wFile['items'].tolist()
-            if 'weight' in i:
-                _weights = self._wFile['weight'].tolist()
-            for i in range(len(_items)):
-                self._weight[_items[i]] = _weights[i]
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
 
             # print(self.Database)
         if isinstance(self._iFile, str):
-            if _fp._validators.url(self._iFile):
-                data = _fp._urlopen(self._iFile)
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
                 for line in data:
-                    line.strip()
                     line = line.decode("utf-8")
-                    temp = [i.rstrip() for i in line.split(self._sep)]
-                    temp = [x for x in temp if x]
-                    self._Database.append(temp)
+                    line = line.strip()
+                    line = [i for i in line.split(':')]
+                    temp1 = [i.rstrip() for i in line[0].split(self._sep)]
+                    temp2 = [i.rstrip() for i in line[1].split(self._sep)]
+                    temp1 = [x for x in temp1 if x]
+                    temp2 = [x for x in temp2 if x]
+                    tr = []
+                    for i in range(len(temp1)):
+                        item = temp1[i]
+                        probability = float(temp2[i])
+                        product = _Item(item, probability)
+                        tr.append(product)
+                    self._Database.append(tr)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
-                            temp = [i.rstrip() for i in line.split(self._sep)]
-                            temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            line = line.strip()
+                            line = [i for i in line.split(':')]
+                            temp1 = [i.rstrip() for i in line[0].split(self._sep)]
+                            temp2 = [i.rstrip() for i in line[1].split(self._sep)]
+                            temp1 = [x for x in temp1 if x]
+                            temp2 = [x for x in temp2 if x]
+                            tr = []
+                            for i in range(len(temp1)):
+                                item = temp1[i]
+                                probability = float(temp2[i])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
 
+    def _scanningWeights(self) -> None:
+        """
+        Scans the uncertain transactional dataset
+
+        :return: None
+        """
+        self._weights = {}
+        if isinstance(self._wFile, _ab._pd.DataFrame):
+            weights, data = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                data = self._wFile['items'].tolist()
+            if 'weights' in i:
+                weights = self._wFile['weights'].tolist()
+            for k in range(len(data)):
+                self._weights[data[k]] = int(float(weights[k]))
+
+            # print(self.Database)
         if isinstance(self._wFile, str):
-            if _fp._validators.url(self._wFile):
-                data = _fp._urlopen(self._wFile)
+            if _ab._validators.url(self._wFile):
+                data = _ab._urlopen(self._wFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._weight[temp[0]] = float(temp[1])
+                    self._weights[temp[0]] = int(float(temp[1]))
             else:
                 try:
-                    with open(self._wFile, 'r', encoding='utf-8') as f:
+                    with open(self._wFile, 'r') as f:
                         for line in f:
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._weight[temp[0]] = float(temp[1])
+                            self._weights[temp[0]] = float(temp[1])
                 except IOError:
                     print("File Not Found")
-                    quit()
 
-    def _convert(self, value) -> float:
+    def _frequentOneItem(self) -> tuple:
         """
-        To convert the type of user specified minSup value
+        Takes the self.Database and calculates the support of each item in the dataset and assign the ranks to the items by decreasing support and returns the frequent items list
 
-        :param value: user specified minSup value
-        :return: converted type
+        :param self.Database : it represents the one self.Database in database
+        :type self.Database : list
+        :return: tuple
         """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
 
-    def _frequentOneItem(self) -> List[str]:
-        """
-        Generating One frequent items sets
+        mapSupport = {}
+        for i in self._Database:
+            for j in i:
+                if j.item not in mapSupport:
+                    if self._weights.get(j.item) is not None:
+                        mapSupport[j.item] = [j.probability, self._weights[j.item]]
+                else:
+                    mapSupport[j.item][0] += j.probability
+        mapSupport = {k: v[0] for k, v in mapSupport.items() if v[0] >= self._expSup and v[0] * v[1] >= self._expWSup}
+        plist = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.rank = dict([(index, item) for (item, index) in enumerate(plist)])
+        return mapSupport, plist
 
-        :return: list
+    @staticmethod
+    def _buildTree(data, info) -> _Tree:
         """
-        global _lno, _wf, _weights
-        self._mapSupport = {}
-        _owf = {}
-        for tr in self._Database:
-            for i in range(1, len(tr)):
-                if tr[i] not in self._mapSupport:
-                    self._mapSupport[tr[i]] = [int(tr[0]), int(tr[0]), 1]
-                else:
-                    self._mapSupport[tr[i]][0] = max(self._mapSupport[tr[i]][0], (int(tr[0]) - self._mapSupport[tr[i]][1]))
-                    self._mapSupport[tr[i]][1] = int(tr[0])
-                    self._mapSupport[tr[i]][2] += 1
-        for key in self._mapSupport:
-            self._mapSupport[key][0] = max(self._mapSupport[key][0], abs(len(self._Database) - self._mapSupport[key][1]))
-        _lno = len(self._Database)
-        self._mapSupport = {k: [v[2], v[0]] for k, v in self._mapSupport.items() if v[0] <= self._regularity}
-        for x, y in self._mapSupport.items():
-            if self._weight.get(x) is None:
-                self._weight[x] = 0
-        gmax = max([self._weight[values] for values in self._mapSupport.keys()])
-        for x, y in self._mapSupport.items():
-            _owf[x] = y[0] * gmax
-        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v[0] * _owf[k] >= self._WS}
-        for x, y in self._mapSupport.items():
-            temp = self._weight[x] * y[0]
-            _wf[x] = temp
-            self._mapSupport[x].append(temp)
-        genList = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse= True)]
-        self._rank = dict([(index, item) for (item, index) in enumerate(genList)])
-        for x, y in self._rank.items():
-            _weights[y] = self._weight[x]
-        return genList
+        It takes the self.Database and support of each item and construct the main tree with setting root node as null
 
-    def _updateTransactions(self, itemSet) -> List[List[int]]:
+        :param data : it represents the one self.Database in database
+        :type data : list
+        :param info : it represents the support of each item
+        :type info : dictionary
+        :return: tree
         """
-        Updates the items in transactions with rank of items according to their support
 
-        :Example: oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
-                  rank = {'a':0, 'b':1, 'c':2, 'd':3}
+        rootNode = _Tree()
+        rootNode.info = info.copy()
+        for i in range(len(data)):
+            rootNode.addTransaction(data[i])
+        return rootNode
 
-        :param itemSet: list of one-frequent items
-        :return: None
+    def _updateTransactions(self, dict1) -> list:
+        """
+        Remove the items which are not frequent from self.Database and updates the self.Database with rank of items
+
+        :param dict1 : frequent items with support
+        :type dict1 : dictionary
+        :return: list
         """
         list1 = []
         for tr in self._Database:
-            list2 = [int(tr[0])]
-            for i in range(1, len(tr)):
-                if tr[i] in itemSet:
-                    list2.append(self._rank[tr[i]])
+            list2 = []
+            for i in range(0, len(tr)):
+                if tr[i].item in dict1:
+                    list2.append(tr[i])
             if len(list2) >= 2:
-                basket = list2[1:]
-                basket.sort()
-                list2[1:] = basket[0:]
+                basket = list2
+                basket.sort(key=lambda val: self.rank[val.item])
+                list2 = basket
                 list1.append(list2)
         return list1
 
     @staticmethod
-    def _buildTree(transactions, info) -> _Tree:
+    def _check(i, x) -> int:
         """
-        Builds the tree with updated transactions
+        To check the presence of item or pattern in transaction
 
-        :param transactions: updated transactions
-        :param info: support details of each item in transactions
-        :return: transactions compressed in fp-tree
+        :param x: it represents the pattern
+        :type x : list
+        :param i : represents the uncertain self.Database
+        :type i : list
+        :return: integer number
+        """
+
+        # This method taken a transaction as input and returns the tree
+        for m in x:
+            k = 0
+            for n in i:
+                if m == n.item:
+                    k += 1
+            if k == 0:
+                return 0
+        return 1
 
+    def _convert(self, value) -> float:
         """
-        rootNode = _Tree()
-        rootNode.info = info.copy()
-        for i in range(len(transactions)):
-            set1 = [transactions[i][0]]
-            rootNode.addTransaction(transactions[i][1:], set1)
-        return rootNode
+        To convert the type of user specified minSup value
 
-    def _savePeriodic(self, itemSet) -> str:
+        :param value: user specified minSup value
+        :return: converted type minSup value
         """
-        The duplication items and their ranks
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
 
-        :param itemSet: frequent itemSet that generated
-        :return: patterns with original item names.
+    def _removeFalsePositives(self) -> None:
+        """
+        To remove the false positive patterns generated in frequent patterns.
 
+        :return: patterns with accurate probability
         """
-        temp = str()
-        for i in itemSet:
-            temp = temp + self._rankDup[i] + "\t"
-        return temp
+        global _finalPatterns
+        periods = {}
+        for i in self._Database:
+            for x, y in _finalPatterns.items():
+                if len(x) == 1:
+                    periods[x] = y
+                else:
+                    s = 1
+                    check = self._check(i, x)
+                    if check == 1:
+                        for j in i:
+                            if j.item in x:
+                                s *= j.probability
+                        if x in periods:
+                            periods[x] += s
+                        else:
+                            periods[x] = s
+        for x, y in periods.items():
+            weight = 0
+            for i in x:
+                weight += self._weights[i]
+            weight = weight / len(x)
+            if weight * y >= self._expWSup:
+                sample = str()
+                for i in x:
+                    sample = sample + i + "\t"
+                self._finalPatterns[sample] = y
 
     @deprecated(
         "It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
-        Frequent pattern mining process will start from here
+        startMine() method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns.
         """
         self.mine()
 
     def mine(self) -> None:
         """
-        Frequent pattern mining process will start from here
+        mine() method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patternS
         """
-        global _WS, _regularity, _weights
-        self._startTime = _fp._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._WS is None:
-            raise Exception("Please enter the Minimum Support")
+        global _expSup, _expWSup, _weights, _finalPatterns
+        self._startTime = _ab._time.time()
+        self._Database, self._weights = [], {}
         self._creatingItemSets()
-        self._WS = self._convert(self._WS)
-        self._regularity = self._convert(self._regularity)
-        _WS, _regularity, _weights = self._WS, self._regularity, self._weight
-        itemSet = self._frequentOneItem()
-        updatedTransactions = self._updateTransactions(itemSet)
-        for x, y in self._rank.items():
-            self._rankDup[y] = x
-        info = {self._rank[k]: v for k, v in self._mapSupport.items()}
-        _Tree = self._buildTree(updatedTransactions, info)
-        patterns = _Tree.generatePatterns([])
+        self._scanningWeights()
+        _weights = self._weights
+        self._expSup = float(self._expSup)
+        self._expWSup = float(self._expWSup)
+        _expSup = self._expSup
+        _expWSup = self._expWSup
         self._finalPatterns = {}
-        for k in patterns:
-            s = self._savePeriodic(k[0])
-            self._finalPatterns[str(s)] = k[1]
-        print("Weighted Frequent Regular patterns were generated successfully using WFRIM algorithm")
-        self._endTime = _fp._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
-        process = _fp._psutil.Process(_fp._os.getpid())
-        self._memoryRSS = float()
+        mapSupport, plist = self._frequentOneItem()
+        self.Database1 = self._updateTransactions(mapSupport)
+        info = {k: v for k, v in mapSupport.items()}
+        Tree1 = self._buildTree(self.Database1, info)
+        Tree1.generatePatterns([])
+        self._removeFalsePositives()
+        print("Weighted Frequent patterns were generated  successfully using basic algorithm")
+        self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
+        self.memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        self.memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self) -> float:
         """
 
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
@@ -741,88 +780,100 @@
         """
 
         Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
-
-        return self._memoryRSS
+        return self.memoryRSS
 
     def getRuntime(self) -> float:
         """
 
         Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> _fp._pd.DataFrame:
+    def getPatternsAsDataFrame(self) -> pd.DataFrame:
         """
 
         Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
-
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
-            dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
+            s = str()
+            for i in a:
+                s = s + i + " "
+            data.append([s, b])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile: str) -> None:
         """
-
         Complete set of frequent patterns will be loaded in to an output file
 
-        :param outFile: name of the output file
+        :param outFile: Specify name of the output file
         :type outFile: csv file
         :return: None
         """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
+        self.oFile = outFile
+        writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
+            s = str()
+            for i in x:
+                s = s + i + "\t"
+            s1 = s.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self) -> Dict[str, float]:
+    def getPatterns(self) -> dict:
         """
 
         Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self) -> None:
         """
         This function is used to print the results
         """
-        print("Total number of  Weighted Frequent Regular Patterns:", len(self.getPatterns()))
+        print("Total number of  Weighted Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
-        if len(_fp._sys.argv) == 7:
-            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
-        if len(_fp._sys.argv) == 5:
-            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
+    if len(_ab._sys.argv) == 6 or len(_ab._sys.argv) == 7:
+        if len(_ab._sys.argv) == 7:
+            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
+        if len(_ab._sys.argv) == 6:
+            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         _ap.startMine()
         _ap.mine()
-        print("Total number of Weighted Frequent Regular Patterns:", len(_ap.getPatterns()))
-        _ap.save(_fp._sys.argv[2])
-        print("Total Memory in USS:",  _ap.getMemoryUSS())
+        print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_ab._sys.argv[2])
+        print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        for k in [120, 140, 160, 180, 200]:
+            _ap = WUFIM('/Users/likhitha/Downloads/uncertainTransaction_T10I4D200K.csv', '/Users/likhitha/Downloads/T10_weights.txt',
+                        k, 500, '\t')
+            _ap.startMine()
+            print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
+            _ap.save('/Users/likhitha/Downloads/WUFIM_output.txt')
+            print("Total Memory in USS:", _ap.getMemoryUSS())
+            print("Total Memory in RSS", _ap.getMemoryRSS())
+            print("Total ExecutionTime in ms:", _ap.getRuntime())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.5.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2024.5.1.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/PKG-INFO` & `pami-2024.5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2024.5.1
+Version: 2024.5.1.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pami-2024.5.1/README.md` & `pami-2024.5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1/pami.egg-info/PKG-INFO` & `pami-2024.5.1.1/pami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2024.5.1
+Version: 2024.5.1.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pami-2024.5.1/pami.egg-info/SOURCES.txt` & `pami-2024.5.1.1/pami.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 README.md
 setup.py
 PAMI/__init__.py
 PAMI/AssociationRules/__init__.py
-PAMI/AssociationRules/basic/ARWithConfidence.py
-PAMI/AssociationRules/basic/ARWithLeverage.py
-PAMI/AssociationRules/basic/ARWithLift.py
-PAMI/AssociationRules/basic/RuleMiner.py
+PAMI/AssociationRules/basic/_ARWithLeverage.py
+PAMI/AssociationRules/basic/_ARWithLift.py
+PAMI/AssociationRules/basic/_RuleMiner.py
 PAMI/AssociationRules/basic/__init__.py
 PAMI/AssociationRules/basic/abstract.py
+PAMI/AssociationRules/basic/confidence.py
+PAMI/AssociationRules/basic/leverage.py
+PAMI/AssociationRules/basic/lift.py
 PAMI/correlatedPattern/__init__.py
 PAMI/correlatedPattern/basic/CoMine.py
 PAMI/correlatedPattern/basic/CoMinePlus.py
 PAMI/correlatedPattern/basic/__init__.py
 PAMI/correlatedPattern/basic/abstract.py
 PAMI/coveragePattern/__init__.py
 PAMI/coveragePattern/basic/CMine.py
@@ -109,15 +111,14 @@
 PAMI/faultTolerantFrequentPattern/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
 PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
 PAMI/faultTolerantFrequentPattern/basic/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/abstract.py
 PAMI/frequentPattern/__init__.py
 PAMI/frequentPattern/basic/Apriori.py
-PAMI/frequentPattern/basic/Apriori2.py
 PAMI/frequentPattern/basic/Aprioribitset.py
 PAMI/frequentPattern/basic/ECLAT.py
 PAMI/frequentPattern/basic/ECLATDiffset.py
 PAMI/frequentPattern/basic/ECLATbitset.py
 PAMI/frequentPattern/basic/FPGrowth.py
 PAMI/frequentPattern/basic/_Apriori.py
 PAMI/frequentPattern/basic/_FPGrowth.py
```

### Comparing `pami-2024.5.1/setup.py` & `pami-2024.5.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pami',
-    version='2024.5.1',
+    version='2024.5.1.1',
     author='Rage Uday Kiran',
     author_email='uday.rage@gmail.com',
     description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     url='https://github.com/udayLab/PAMI',
```

