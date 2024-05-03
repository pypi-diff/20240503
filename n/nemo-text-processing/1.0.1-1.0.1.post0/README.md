# Comparing `tmp/nemo_text_processing-1.0.1.tar.gz` & `tmp/nemo_text_processing-1.0.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo_text_processing-1.0.1.tar", last modified: Fri May  3 21:44:26 2024, max compression
+gzip compressed data, was "nemo_text_processing-1.0.1.post0.tar", last modified: Fri May  3 21:42:14 2024, max compression
```

## Comparing `nemo_text_processing-1.0.1.tar` & `nemo_text_processing-1.0.1.post0.tar`

### file list

```diff
@@ -1,1771 +1,1771 @@
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.997373 nemo_text_processing-1.0.1/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11356 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/LICENSE
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       52 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/MANIFEST.in
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7202 2024-05-03 21:44:25.997373 nemo_text_processing-1.0.1/PKG-INFO
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4204 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/README.md
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.765369 nemo_text_processing-1.0.1/nemo_text_processing/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.769369 nemo_text_processing-1.0.1/nemo_text_processing/fst_alignment/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      622 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/fst_alignment/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9240 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/fst_alignment/alignment.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.769369 nemo_text_processing-1.0.1/nemo_text_processing/g2p/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/g2p/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.769369 nemo_text_processing-1.0.1/nemo_text_processing/g2p/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/g2p/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.769369 nemo_text_processing-1.0.1/nemo_text_processing/hybrid/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      622 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/hybrid/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3439 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/hybrid/mlm_scorer.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/hybrid/model_utils.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    26837 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/hybrid/utils.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12855 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/hybrid/wfst_lm_rescoring.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.769369 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      707 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.769369 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1036 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.773369 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1036 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1580 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2506 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4813 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2986 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3326 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1189 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5084 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1211 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1240 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.773369 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1668 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2360 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2056 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2224 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2899 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2060 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1750 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1296 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.773369 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      923 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.777370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3299 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3579 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2644 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1595 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2659 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3902 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3572 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1629 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2078 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1982 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8415 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1701 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/whitelist.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.777370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1476 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1978 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2441 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1524 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2471 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2446 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1816 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize_final.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.777370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      923 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/clean_eval_data.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.781370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3146 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/currency.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      137 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/date_period.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.781370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       32 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      121 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      263 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/electronic/symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       42 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/electronic/url_symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       41 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/magnitudes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2183 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/measurements.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/months.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/months_cased.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.781370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       62 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/numbers/hundred.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      109 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/numbers/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      261 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/numbers/thousands.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       78 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/numbers/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.781370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/ordinals/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/ordinals/teen.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.781370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/time/minute_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/time/time_suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/time/time_suffix_cased.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/time/time_zone.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/time/time_zone_cased.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       89 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/time/to_hour.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5481 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6080 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/whitelist_tech.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/year_suffix.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.785370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9966 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7649 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5153 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5520 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1098 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4359 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5175 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2068 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8703 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6894 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2188 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1241 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1620 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.789370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1656 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3032 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2347 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1884 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      916 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2193 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1484 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2043 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1551 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2697 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2867 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1780 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1326 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.789370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.789370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.789370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/dates/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/dates/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       88 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/dates/months.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      253 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/dates/year_suffix.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.789370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      117 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      311 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/electronic/symbols.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.789370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/fractions/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/fractions/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       85 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/fractions/numbers_read_as_ordinals.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       28 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/fractions/ordinal_exceptions.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.793370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/measures/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/measures/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       29 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/measures/math_symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      439 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/measures/measurements_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      432 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/measures/measurements_singular.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.793370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      739 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4273 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural_ext.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      660 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3933 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular_ext.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      743 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural_ext.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       58 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      807 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular_ext.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       88 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/months.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.793370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       77 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      239 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/numbers/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      108 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/numbers/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       82 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/numbers/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      158 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/numbers/twenties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.793370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      280 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      473 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1324 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      312 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1403 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/twenties.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.797370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/roman/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/roman/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/roman/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/roman/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       15 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/roman/thousands.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/roman/ties.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.797370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       95 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/minutes_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      157 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/time_suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      448 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/time_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1056 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3192 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone_ext.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1989 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.797370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8080 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4965 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4012 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4981 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5580 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5540 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4370 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1190 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5703 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8063 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1809 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1212 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      864 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.801370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1669 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2387 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2902 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1974 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1894 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2559 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1485 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1645 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1247 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2721 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3057 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1751 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1354 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1297 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.801370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.805370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/data/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5474 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/data/en_whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/data/es_whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1989 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.805370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9374 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      864 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.805370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5241 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1754 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/verbalize_final.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.805370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.805370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.805370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       77 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      120 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      126 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/electronic/symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      737 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/fractions.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.805370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/measurements/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/measurements/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      122 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/measurements/magnitudes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      391 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/measurements/measurements.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.805370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      674 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_major.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       60 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_minor.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       87 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/months.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.809370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       68 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       10 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/thousands.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      146 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      470 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/ties_unique.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        8 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.809370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      318 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/digits_root_change.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       51 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/firsts.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/key_nouns.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       43 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/second.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.809370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/roman/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/roman/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/roman/digits_large.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/roman/hundreds_large.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/roman/ties_large.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/suppletive.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.809370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/hour_to_night.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      255 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/hours.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/hours_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      881 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        8 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/time_suffix_am.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/time_suffix_pm.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      300 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6090 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.813370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11884 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2601 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5182 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3343 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3388 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5785 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3459 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1293 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4481 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5585 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5781 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1796 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1220 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      864 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.813370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1677 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2544 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3588 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1661 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1944 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2567 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1515 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3203 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1259 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3060 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1759 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1326 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.813370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.817370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1375 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/currency.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       69 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/measurement_dates.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1121 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/measurements.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.817370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      114 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/numbers/digits_no_one.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      157 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/numbers/ties.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.817370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      239 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/ordinals/digit.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.817370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      448 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/time/hours.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/time/minute_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/time/minutes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      354 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/time/minutes_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/time/to_hour.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      305 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/whitelist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.817370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4144 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4632 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1866 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4357 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2424 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2087 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1204 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4984 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1541 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1263 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1654 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.821370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1366 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2261 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1568 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2363 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1541 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1604 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1917 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1817 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1390 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1348 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10328 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/inverse_normalize.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.821370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      923 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.821370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.821370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/date/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/date/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      616 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/date/dates.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      233 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/date/months.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       80 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/date/prefixes.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.821370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      116 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/numbers/digits.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       22 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/numbers/hundred.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2661 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/numbers/tens.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       48 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/numbers/thousands.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       19 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.821370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      173 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/time/hours.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      173 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/time/hours_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1475 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/time/minutes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1455 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/time/minutes_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6744 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.825370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4753 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2777 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3861 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1227 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4512 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4186 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1270 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1654 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.825370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1904 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3407 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2601 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2039 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1709 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1903 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1375 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.825370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.825370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       74 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/currency_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       65 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/currency_singular.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.825370 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       80 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       80 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/electronic/symbols.tsv
--rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)      890 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/measurements_plural.tsv
--rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)      814 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/measurements_singular.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       90 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/months.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.829371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       77 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      213 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/onehundred.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      113 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       80 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      128 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/twenties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.829371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      167 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      471 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/ties.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.829371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        3 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/time/hour_to_am.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        4 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/time/hour_to_pm.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      119 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/time/hours_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/time/minutes_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       45 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/time/time_suffix_am.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       35 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/time/time_suffix_pm.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/whitelist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.829371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    16258 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3501 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5043 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4011 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5063 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3609 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1190 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/punctuation.py
--rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)     5000 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/telephone.py
--rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)     9385 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5457 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1809 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1212 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      856 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.833371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1669 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2776 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2902 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1974 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2164 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1514 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1569 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1246 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/telephone.py
--rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)     2626 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2839 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1750 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1370 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1297 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.833371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.833371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1874 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2576 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/decimals.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1576 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1601 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1514 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1696 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1706 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2985 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5963 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1878 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/whitelist.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.837371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1195 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1930 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1217 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1347 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1212 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1453 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1233 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1779 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2817 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1751 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5309 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/run_evaluate.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.837371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.837371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.837371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       33 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/data/time/suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       50 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/data/whitelist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.837371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2820 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3426 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2803 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2241 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1567 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2190 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7008 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7354 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2082 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      851 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.841371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1476 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2362 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2299 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3047 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2016 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1816 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/verbalize_final.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.841371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      923 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.841371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/currency.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.841371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       35 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      113 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      213 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/electronic/symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       40 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/magnitudes.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.841371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/math/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/math/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       82 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/math/symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2692 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/measurements.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      120 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/months.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.841371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       71 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        5 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/numbers/hundred.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      172 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/numbers/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/numbers/thousands.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       63 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/numbers/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        8 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.841371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       85 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/digit.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.845371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      356 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/hours.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/hours_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/hours_to_night.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1789 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      335 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/time_suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/time_zone.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5106 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.845371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6394 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6160 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5056 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3719 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2387 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3655 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2820 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1513 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1224 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1775 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4464 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5808 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1846 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1247 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      843 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.849371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1660 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2341 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1886 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1762 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2690 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1490 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1398 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3038 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3071 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1787 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1410 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.849371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.849371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.849371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/date/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/date/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      708 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/date/day.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/date/months.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.849371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1255 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_major.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      136 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_minor.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        9 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_rmb_minor_cent.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       18 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_rmb_minor_tencent.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.849371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      132 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/numbers/digit-nano.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      162 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/numbers/ties-nano.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.853371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      506 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/time_hours.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      675 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/time_mandarin.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1832 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/time_minutes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/time_quarters.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1626 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/time_seconds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      465 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6385 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.853371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    16629 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4022 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3254 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2022 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6030 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1257 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1254 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4984 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4873 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1715 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1218 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1922 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.853371 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2734 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3202 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3000 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2264 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4131 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1315 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4709 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2502 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1759 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1422 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1324 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1442 2024-05-03 21:43:57.000000 nemo_text_processing-1.0.1/nemo_text_processing/package_info.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.857371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      777 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.857371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1265 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.857371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.857371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/measure/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/measure/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      317 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/measure/measurements.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.857371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      577 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/money/currency_major.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/money/currency_minor_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       30 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/money/currency_minor_singular.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      552 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/money/local_currency.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.861371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      107 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/digit_100.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       83 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/digit_1000.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      432 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/flops.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/fraction.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      118 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/fraction_dual.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/fraction_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       82 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/fraction_singular.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       73 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/quantities.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      175 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/teens.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/tens.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       10 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/zero.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8591 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.861371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6624 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3641 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3368 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6004 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8425 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5429 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1325 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1667 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.861371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1785 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2250 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4503 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2124 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2384 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2831 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1526 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12188 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/data_loader_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.861371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.861371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.861371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      118 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       84 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      258 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/electronic/symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      542 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/fractions.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.865371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/measure/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/measure/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1198 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/measure/measurements.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      139 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/measure/suppletive.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.865371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      396 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/money/currency.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/money/currency_minor_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/money/currency_minor_singular.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.865371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/months/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/months/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      147 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/months/abbr_to_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      230 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/months/numbers.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.865371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       59 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/numbers/ones.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      119 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/numbers/quantities.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      109 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/numbers/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       81 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/numbers/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.865371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       93 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/ordinals/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       70 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/ordinals/thousands.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      139 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/ordinals/ties.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.865371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       53 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/time/hour_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/time/hour_to_night.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/time/minute_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/time/time_zone.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       89 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/whitelist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.869371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7656 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5770 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3692 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3197 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2226 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7046 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7226 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2002 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3701 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3981 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7199 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2811 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1313 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1350 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.869371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1734 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2759 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2435 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3561 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3030 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3378 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2303 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1850 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5518 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3770 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2831 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/verbalize_final.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.873371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      899 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12763 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/clean_eval_data.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.873371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.873371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/address/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/address/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      161 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/address/address_word.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      617 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/address/state.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.873371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/date/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/date/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      257 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/date/day.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      141 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/date/month_abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/date/month_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      234 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/date/month_number.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      128 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/date/year_suffix.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.873371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      222 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/electronic/symbol.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/electronic/words.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.873371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/measure/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/measure/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       71 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/measure/math_operation.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1554 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/measure/unit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      544 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/measure/unit_alternatives.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.873371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      656 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/money/currency_major.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       36 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/money/currency_minor_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/money/currency_minor_singular.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       15 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/money/per_unit.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.877371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/__init__.py
--rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)   325078 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name.far
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    54511 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name_au.far
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       62 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/fraction.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/hundred.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      107 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/quantity_abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      109 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      261 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/thousand.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       69 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/ty.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.877371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/ordinal/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/ordinal/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/ordinal/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/ordinal/teen.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.877371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    35561 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/female.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       45 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/key_word.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    20334 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/male.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    72815 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/roman_to_spoken.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1843 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/suppletive.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.877371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/telephone/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/telephone/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       19 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/telephone/ip_prompt.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       38 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/telephone/ssn_prompt.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       56 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/telephone/telephone_prompt.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.877371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       84 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/time/suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      116 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/time/zone.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.881371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      520 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/alternatives.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      155 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/alternatives_all_format.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)   175146 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/asr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      865 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/asr_with_pc.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2532 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/ipa_symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      263 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/lj_speech.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      240 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/symbol.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    36553 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/tts.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9160 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.885372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2070 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/abbreviation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7174 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    15334 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5490 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5057 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2401 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11525 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9522 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2549 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2566 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4937 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/range.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4552 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/roman.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6175 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/serial.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6035 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5200 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10941 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12298 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_lm.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12748 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_with_audio.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6290 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4000 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1654 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.885372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1447 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/abbreviation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1954 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3924 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3295 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4728 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3720 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4474 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2743 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2113 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6845 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/post_processing.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2509 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/roman.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2373 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3638 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3986 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3117 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1582 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1512 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.885372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      682 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.889371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.889371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/dates/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/dates/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      348 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/dates/days_abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      115 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/dates/months.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      551 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/dates/months_abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1184 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/dates/year_suffix.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.889371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       73 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      311 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/electronic/symbols.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.889371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/fractions/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/fractions/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      117 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/fractions/fraction_symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       28 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/fractions/ordinal_exceptions.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      224 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/fractions/powers_of_ten.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      137 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/fractions/powers_of_ten_fem.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.889371 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/measures/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/measures/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       52 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/measures/math_symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      260 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/measures/measurements.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       95 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/measures/measurements_complex.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       55 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_fem.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_masc.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.893372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1030 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_major.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_major_ext.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      773 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_minor.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2155 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_minor_ext.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      177 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1800 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem_ext.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5659 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc_ext.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.893372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      111 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       52 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/quantities.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      108 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       72 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      141 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/twenties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.893372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      137 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      286 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/gender_suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      471 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/roman_exceptions.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      200 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      165 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      295 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/twenties.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.893372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/roman/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/roman/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/roman/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/roman/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       15 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/roman/thousands.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/roman/ties.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.893372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/telephone/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/telephone/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       66 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/telephone/ip_prompt.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      143 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/telephone/telephone_prompt.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.897372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       31 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/afternoon_times.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/alt_minutes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/evening_times.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       53 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/hour_to_12.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      128 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/hour_to_24.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/hour_to_night.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/minute_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       60 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/morning_times.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      150 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/time_suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1056 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/time_zone.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3192 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/time_zone_ext.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      869 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8365 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.897372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5598 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6128 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/decimals.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3464 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5931 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7950 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8830 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7466 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8013 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9440 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7301 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2811 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1169 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.901372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2399 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3469 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3707 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/decimals.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3587 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8535 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5238 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7014 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2962 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2518 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8940 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3589 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2827 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/verbalize_final.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.901372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.901372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.901372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/fractions/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/fractions/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      116 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/fractions/irregular_denominators.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.901372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/measures/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/measures/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      232 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/measures/measurements.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.905372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       62 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/eighty.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/ninety.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       90 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/quantities.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       10 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/seventy.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       93 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/teens.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/ten.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       50 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/tens_simple.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.905372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      855 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/ordinals/irregular_numbers.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       55 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/ordinals/suffixes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      260 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/whitelist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.905372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6737 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5168 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/decimals.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2947 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2068 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5720 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2812 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1329 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1170 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.905372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1589 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2741 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/decimals.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2686 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3033 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2321 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2910 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/verbalize_final.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.905372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.905372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.909372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/dates/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/dates/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      499 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/dates/days.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      694 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/dates/days_to_numbers.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      162 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/dates/month_abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      132 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/dates/months.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      143 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/dates/months_roman.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.909372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      198 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      100 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/electronic/symbols.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.909372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/fractions/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/fractions/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      150 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/fractions/fraction_symbols.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.909372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/inflection/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/inflection/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3803 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/inflection/endings.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/inflection/plural_endings.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/inflection/word_endings.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       81 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/math_operations.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.909372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/measures/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/measures/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      215 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/measures/greek_lower.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      215 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/measures/greek_upper.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      757 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/measures/measurements.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.909372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      278 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/money/alphabet.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      166 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/money/currency.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      106 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/money/currency_minor.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.913372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       68 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       66 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/digit_inline.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      111 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/digit_nom.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      250 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/quantities.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       94 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/tens.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       87 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/tens_inline.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        8 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.913372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      382 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/ordinals/endings.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       55 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/ordinals/exceptional.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       63 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/ordinals/superessive_endings.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/ordinals/superscript_digits.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.913372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      212 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/area_codes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      804 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/country_codes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       19 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/ip_prompt.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       44 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/special_numbers.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       29 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/telephone_abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       10 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/telephone_prompt.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.913372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       87 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/time/time_zone.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      354 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      548 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/whitelist_inflect.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      291 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/whitelist_inflect_sg.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1546 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.917372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12472 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10479 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5767 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3649 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2466 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5749 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7804 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3363 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6670 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11365 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7376 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3686 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5516 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.917372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1767 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2022 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2989 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3782 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2368 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3493 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1583 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2331 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3983 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3588 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2911 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/verbalize_final.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.917372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.917372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1343 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/currency.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      147 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/measurement_dates.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      967 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/measurements.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.917372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       90 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       42 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/numbers/quantities.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      135 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/numbers/ties.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.917372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/ordinal/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/ordinal/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      123 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/ordinal/digit.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.921372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      427 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/time/hours.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1235 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/time/minutes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      624 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/whitelist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.921372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4305 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3504 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1661 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3579 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3276 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3214 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1156 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1644 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5031 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1957 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1164 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1170 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.921372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1321 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2245 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1714 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2744 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1486 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1473 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1566 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2676 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2333 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1290 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1520 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.921372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      912 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.925372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.925372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      187 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       73 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/electronic/symbols.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.925372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/measure/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/measure/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      822 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/measure/measurements.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      189 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/measure/suppletive.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.925372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      157 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/money/currency_major.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      132 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/money/currency_minor.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       30 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/money/currency_plural_fem.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/money/currency_plural_masc.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.925372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       98 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       16 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/quantities.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      117 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       81 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/tens.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      113 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/tens_eight.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/tens_one.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.925372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/whitelist/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/whitelist/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1051 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/whitelist/whitelist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.929372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7840 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5060 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/decimals.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3751 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8249 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3305 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6135 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2877 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1332 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1164 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.929372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1731 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2951 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3223 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1902 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6211 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3707 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3015 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2827 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    33677 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/normalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    22719 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/normalize_with_audio.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2891 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/preprocessing_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.929372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2078 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/alphabet.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.929372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.929372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/currency/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/currency/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1420 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/currency/currency_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1085 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/currency/currency_singular.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.929372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       47 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      290 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      668 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/electronic/symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      275 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/latin_to_cyrillic.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/measurements.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.933372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/months/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/months/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      239 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/months/abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1541 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/months/abbr_to_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      214 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/months/numbers.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.933372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      969 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/1_cardinals_nominative.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      911 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/2_cardinals_genitive.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      933 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/3_cardinals_dative.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      913 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/4_cardinals_accusative.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1048 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/5_cardinals_instrumental.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      951 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/6_cardinals_prepositional.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      549 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_alternatives.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      710 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_nominative_case.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      565 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/decimal_delimiter.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1026 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/decimal_endings.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      119 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/digits_nominative_case.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      430 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/ordinal_endings.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    21537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/ordinals.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/quantity.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.933372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      469 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/time/increment_hour_cardinal.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      611 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/time/increment_hour_ordinal.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      828 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/time/minutes_to_hour.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       62 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/time/time_convert.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.945372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3206 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/g.fst
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    69495 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/universal_thousands_punct.far
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)  7085564 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/util_arithmetic.far
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    14099 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/util_byte.far
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/whitelist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.945372 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6819 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6015 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4466 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/decimals.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4797 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6943 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3998 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6606 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/number_names.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2951 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3266 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5254 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7098 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3045 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1313 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1337 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.949373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1892 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1498 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2190 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1571 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1760 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1495 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1463 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1783 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2116 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2993 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2879 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5161 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/run_evaluate.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.949373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.949373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      334 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/abbreviations_nondet.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.949373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/dates/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/dates/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      208 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/dates/era_suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       94 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/dates/era_words.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      176 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/dates/month_abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      112 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/dates/months.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.949373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/electronic/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/electronic/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/electronic/domain.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/electronic/server_name.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      263 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/electronic/symbols.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      162 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/fillers.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       71 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/math_operations.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.953373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      196 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/greek_lower.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      196 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/greek_upper.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2121 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/unit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      157 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/unit_neuter.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1461 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/unit_plural.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.953373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1344 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/currency_major.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/currency_major_nt.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      745 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/currency_minor_plural.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/currency_minor_singular.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1197 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/currency_plurals.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.953373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/fraction.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1586 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/millions.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/millions_abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/quantities.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       94 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       72 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.953373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/ordinals/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/ordinals/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       83 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/ordinals/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      115 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/ordinals/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       96 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/ordinals/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        9 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/ordinals/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.953373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/roman/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/roman/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/roman/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/roman/hundreds.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/roman/ties.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.957373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      804 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/country_codes.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       22 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/ip_prompt.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       96 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/special_numbers.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       28 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/ssn_prompt.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      381 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/telephone_abbr.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       58 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/telephone_prompt.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.957373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       53 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/time/hour_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/time/hour_to_night.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/time/minute_to.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      261 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/time/suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/time/time_zone.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1046 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2521 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.957373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2168 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/abbreviation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    18416 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8095 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7106 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3481 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4238 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10130 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12313 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9471 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8363 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8753 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9197 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11054 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify_with_audio.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3024 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1323 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1173 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.961373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1733 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2618 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2838 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/decimals.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3679 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3156 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3750 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2807 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1585 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2380 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4271 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3589 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2910 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5164 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/token_parser.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/utils_audio_based.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.961373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.961373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.961373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/charset_extension.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    32616 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/charset_national_standard_2013_8105.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      553 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/fullwidth_to_halfwidth.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       13 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/oov_tags.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      291 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/punctuations_zh.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       72 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/upper_to_lower.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.965373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/date/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/date/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      363 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/date/day.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      144 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/date/months.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      222 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/date/suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      206 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/date/suffixes.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.965373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/denylist/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/denylist/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/denylist/denylist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.965373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/erhua/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/erhua/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      350 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/erhua/whitelist.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.965373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/math/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/math/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/math/score.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/math/symbol.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.965373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/measure/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/measure/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      839 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/measure/units_en.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.965373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/money/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/money/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4047 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/money/currency_major.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      565 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/money/currency_mandarin.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.965373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/digit.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/digit_alt.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       47 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/digit_tens.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       12 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/sign.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      143 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/suffix.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       97 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/teen.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      127 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/teen_alt.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       72 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/ties.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/zero.tsv
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.965373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       35 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/AM.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       36 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/PM.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      288 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/hour.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      744 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/minute.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      744 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/second.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        2 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/zero.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1362 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/whitelist.tsv
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5130 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/graph_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.969373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10133 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6028 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3924 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6208 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3126 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5065 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2808 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1856 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/preprocessor.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2655 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6613 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4990 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/tokenize_and_classify.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2358 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1909 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.973373 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2022 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3669 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2510 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2692 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2784 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2127 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3695 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/post_processing.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3049 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/postprocessor.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3893 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3202 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/verbalize.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2149 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/verbalize_final.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1292 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1106 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.973373 nemo_text_processing-1.0.1/nemo_text_processing/utils/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      677 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/utils/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1021 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/nemo_text_processing/utils/logging.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.997373 nemo_text_processing-1.0.1/nemo_text_processing.egg-info/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7202 2024-05-03 21:44:25.000000 nemo_text_processing-1.0.1/nemo_text_processing.egg-info/PKG-INFO
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)   101841 2024-05-03 21:44:25.000000 nemo_text_processing-1.0.1/nemo_text_processing.egg-info/SOURCES.txt
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        1 2024-05-03 21:44:25.000000 nemo_text_processing-1.0.1/nemo_text_processing.egg-info/dependency_links.txt
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)        1 2024-05-03 21:44:25.000000 nemo_text_processing-1.0.1/nemo_text_processing.egg-info/not-zip-safe
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      488 2024-05-03 21:44:25.000000 nemo_text_processing-1.0.1/nemo_text_processing.egg-info/requires.txt
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:44:25.000000 nemo_text_processing-1.0.1/nemo_text_processing.egg-info/top_level.txt
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.973373 nemo_text_processing-1.0.1/requirements/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      139 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/requirements/requirements.txt
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      167 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/requirements/requirements_test.txt
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1153 2024-05-03 21:44:26.001374 nemo_text_processing-1.0.1/setup.cfg
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8341 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/setup.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.973373 nemo_text_processing-1.0.1/tests/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8115 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/conftest.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.973373 nemo_text_processing-1.0.1/tests/nemo_text_processing/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.973373 nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1874 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2649 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2303 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2918 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2375 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1955 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_whitelist.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.973373 nemo_text_processing-1.0.1/tests/nemo_text_processing/audio_based_utils/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/audio_based_utils/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1325 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/audio_based_utils/test_audio_based_utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.977373 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2314 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2323 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2332 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2324 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2318 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1547 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_normalization_with_audio.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2047 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2314 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2315 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.977373 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1886 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_address.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3054 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3753 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2951 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2944 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1786 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1843 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_math.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2932 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3065 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1531 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_normalization_with_audio.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2943 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1840 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_punctuation.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1848 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_range.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1853 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_roman.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1866 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_serial.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1957 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_special_text.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2963 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1749 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_text_split.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2929 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3636 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3025 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.981373 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2339 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2259 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2335 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1810 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2345 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1508 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_normalization_with_audio.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2350 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2335 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2348 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2397 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.981373 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1292 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1283 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1301 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1279 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1296 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1283 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1287 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1300 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1299 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.985373 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1768 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1764 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1286 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1768 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1765 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1285 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1756 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.985373 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.985373 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/data_text_normalization/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/data_text_normalization/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1244 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1242 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1248 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1245 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1243 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1239 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1243 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1247 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1246 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.985373 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1772 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1765 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1769 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1762 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1772 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1762 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.989373 nemo_text_processing-1.0.1/tests/nemo_text_processing/it/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/it/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1257 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1256 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1284 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1254 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1278 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1258 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_whitelist.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.989373 nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1275 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1267 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1273 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1267 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1268 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.989373 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1283 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1280 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1286 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1285 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1285 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1275 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.989373 nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.993373 nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/data_text_normalization/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/data_text_normalization/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6340 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/test_ru_inverse_normalization.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6527 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/test_ru_normalization.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.993373 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.993373 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/data_inverse_text_normalization/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/data_inverse_text_normalization/__init__.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.993373 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/data_text_normalization/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/data_text_normalization/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2611 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2600 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2608 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2617 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2612 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1808 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1804 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1603 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_normalization_with_audio.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2615 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2600 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2614 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2648 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_word.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2812 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/utils.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.993373 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1600 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1591 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1597 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1603 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_electronic.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1600 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1598 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1594 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1598 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1602 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_telephone.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1591 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1602 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1592 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_word.py
-drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:44:25.997373 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/__init__.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1748 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_cardinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1794 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_date.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1743 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_decimal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1810 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_fraction.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1268 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_measure.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1757 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_money.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1746 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_ordinal.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1794 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_time.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1758 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_whitelist.py
--rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1783 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.959042 nemo_text_processing-1.0.1.post0/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11356 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/LICENSE
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       52 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/MANIFEST.in
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7208 2024-05-03 21:42:14.959042 nemo_text_processing-1.0.1.post0/PKG-INFO
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4204 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/README.md
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.727038 nemo_text_processing-1.0.1.post0/nemo_text_processing/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.727038 nemo_text_processing-1.0.1.post0/nemo_text_processing/fst_alignment/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      622 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/fst_alignment/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9240 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/fst_alignment/alignment.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.727038 nemo_text_processing-1.0.1.post0/nemo_text_processing/g2p/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/g2p/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.727038 nemo_text_processing-1.0.1.post0/nemo_text_processing/g2p/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/g2p/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.731038 nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      622 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3439 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/mlm_scorer.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/model_utils.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    26837 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/utils.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12855 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/wfst_lm_rescoring.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.731038 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      707 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.731038 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1036 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.731038 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1036 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1580 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2506 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4813 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2986 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3326 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1189 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5084 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1211 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1240 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.731038 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1668 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2360 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2056 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2224 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2899 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2060 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1750 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1296 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.731038 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      923 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.735038 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3299 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3579 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2644 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1595 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2659 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3902 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3572 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1629 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2078 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1982 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8415 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1701 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/whitelist.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.735038 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1476 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1978 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2441 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1524 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2471 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2446 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1816 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize_final.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.735038 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      923 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/clean_eval_data.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.739039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3146 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/currency.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      137 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/date_period.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.739039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       32 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      121 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      263 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/electronic/symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       42 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/electronic/url_symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       41 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/magnitudes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2183 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/measurements.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/months.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/months_cased.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.739039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       62 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/numbers/hundred.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      109 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/numbers/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      261 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/numbers/thousands.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       78 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/numbers/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.739039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/teen.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.739039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/time/minute_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/time/time_suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/time/time_suffix_cased.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/time/time_zone.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/time/time_zone_cased.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       89 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/time/to_hour.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5481 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6080 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/whitelist_tech.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/year_suffix.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.743039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9966 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7649 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5153 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5520 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1098 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4359 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5175 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2068 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8703 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6894 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2188 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1241 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1620 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.743039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1656 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3032 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2347 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1884 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      916 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2193 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1484 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2043 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1551 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2697 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2867 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1780 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1326 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.747039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.747039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.747039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/dates/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/dates/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       88 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/dates/months.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      253 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/dates/year_suffix.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.747039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      117 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      311 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/electronic/symbols.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.747039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/fractions/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/fractions/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       85 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/fractions/numbers_read_as_ordinals.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       28 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/fractions/ordinal_exceptions.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.747039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/measures/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/measures/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       29 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/measures/math_symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      439 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/measures/measurements_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      432 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/measures/measurements_singular.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.747039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      739 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4273 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural_ext.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      660 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3933 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular_ext.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      743 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural_ext.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       58 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      807 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular_ext.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       88 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/months.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.751039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       77 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      239 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/numbers/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      108 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/numbers/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       82 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/numbers/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      158 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/numbers/twenties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.751039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      280 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      473 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1324 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      312 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1403 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/twenties.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.751039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/roman/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/roman/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/roman/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/roman/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       15 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/roman/thousands.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/roman/ties.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.751039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       95 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/minutes_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      157 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/time_suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      448 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/time_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1056 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3192 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone_ext.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1989 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.755039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8080 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4965 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4012 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4981 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5580 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5540 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4370 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1190 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5703 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8063 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1809 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1212 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      864 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.755039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1669 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2387 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2902 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1974 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1894 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2559 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1485 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1645 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1247 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2721 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3057 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1751 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1354 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1297 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.759039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.759039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/data/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5474 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/data/en_whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/data/es_whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1989 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.759039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9374 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      864 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.759039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5241 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1754 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/verbalize_final.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.759039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.759039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.759039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       77 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      120 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      126 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      737 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/fractions.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.759039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      122 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/magnitudes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      391 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/measurements.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.759039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      674 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_major.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       60 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_minor.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       87 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/months.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.763039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       68 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       10 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/thousands.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      146 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      470 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/ties_unique.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        8 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.763039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      318 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/digits_root_change.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       51 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/firsts.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/key_nouns.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       43 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/second.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.763039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/roman/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/roman/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/roman/digits_large.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/roman/hundreds_large.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/roman/ties_large.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/suppletive.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.763039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/hour_to_night.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      255 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/hours.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/hours_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      881 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        8 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/time_suffix_am.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/time_suffix_pm.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      300 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6090 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.767039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11884 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2601 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5182 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3343 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3388 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5785 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3459 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1293 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4481 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5585 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5781 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1796 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1220 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      864 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.767039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1677 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2544 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3588 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1661 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1944 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2567 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1515 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3203 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1259 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3060 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1759 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1326 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.767039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.771039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1375 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/currency.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       69 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/measurement_dates.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1121 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/measurements.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.771039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      114 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/numbers/digits_no_one.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      157 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/numbers/ties.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.771039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      239 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/ordinals/digit.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.771039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      448 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/time/hours.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/time/minute_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/time/minutes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      354 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/time/minutes_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/time/to_hour.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      305 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/whitelist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.771039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4144 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4632 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1866 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4357 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2424 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2087 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1204 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4984 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1541 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1263 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1654 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.775039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1366 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2261 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1568 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2363 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1541 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1604 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1917 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1817 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1390 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1348 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10328 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/inverse_normalize.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.775039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      923 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.775039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.775039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/date/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/date/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      616 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/date/dates.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      233 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/date/months.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       80 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/date/prefixes.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.775039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      116 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/numbers/digits.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       22 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/numbers/hundred.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2661 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/numbers/tens.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       48 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/numbers/thousands.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       19 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.779039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      173 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/time/hours.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      173 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/time/hours_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1475 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/time/minutes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1455 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/time/minutes_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6744 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.779039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4753 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2777 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3861 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1227 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4512 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4186 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1270 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1654 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.779039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1904 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3407 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2601 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2039 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1709 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1903 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1375 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.779039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.783039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       74 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/currency_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       65 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/currency_singular.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.783039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       80 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       80 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/symbols.tsv
+-rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)      890 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_plural.tsv
+-rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)      814 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_singular.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       90 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/months.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.783039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       77 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      213 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/onehundred.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      113 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       80 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      128 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/twenties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.783039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      167 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      471 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/ties.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.783039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        3 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/time/hour_to_am.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        4 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/time/hour_to_pm.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      119 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/time/hours_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/time/minutes_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       45 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/time/time_suffix_am.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       35 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/time/time_suffix_pm.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/whitelist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.787039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    16258 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3501 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5043 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4011 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5063 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3609 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1190 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/punctuation.py
+-rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)     5000 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/telephone.py
+-rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)     9385 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5457 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1809 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1212 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      856 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.787039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1669 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2776 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2902 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1974 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2164 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1514 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1569 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1246 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/telephone.py
+-rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)     2626 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2839 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1750 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1370 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1297 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.787039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.791039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1874 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2576 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/decimals.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1576 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1601 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1514 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1696 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1706 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2985 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5963 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1878 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/whitelist.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.791039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1195 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1930 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1217 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1347 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1212 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1453 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1233 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1779 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2817 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1751 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5309 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/run_evaluate.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.791039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.791039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.791039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       33 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/data/time/suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       50 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/data/whitelist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.795040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2820 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3426 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2803 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2241 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1567 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2190 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7008 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7354 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2082 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      851 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.795040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1476 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2362 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2299 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3047 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2016 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1816 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/verbalize_final.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.795040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      923 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.795040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/currency.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.799039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       35 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      113 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      213 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       40 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/magnitudes.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.799039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/math/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/math/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       82 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/math/symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2692 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/measurements.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      120 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/months.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.799039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       71 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        5 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/hundred.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      172 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/thousands.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       63 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        8 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.799039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       85 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/digit.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.799039 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      356 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/hours.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/hours_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/hours_to_night.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1789 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      335 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       61 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/time_suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/time_zone.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5106 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.803040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6394 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6160 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5056 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3719 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2387 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3655 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2820 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1513 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1224 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1775 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4464 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5808 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1846 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1247 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      843 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.803040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1660 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2341 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1886 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1762 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2690 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1490 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1398 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3038 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3071 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1787 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1410 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.803040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      936 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.807040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.807040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/date/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/date/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      708 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/date/day.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      383 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/date/months.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.807040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1255 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_major.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      136 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_minor.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        9 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_rmb_minor_cent.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       18 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_rmb_minor_tencent.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.807040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      132 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/numbers/digit-nano.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      162 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/numbers/ties-nano.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.807040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      506 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/time_hours.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      675 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/time_mandarin.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1832 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/time_minutes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/time_quarters.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1626 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/time_seconds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      465 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6385 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.811040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    16629 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4022 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3254 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2022 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6030 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1257 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1254 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4984 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4873 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1715 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1218 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1922 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.811040 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2734 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3202 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3000 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2264 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4131 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1315 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4709 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2502 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1759 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1422 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1324 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1443 2024-05-03 21:40:28.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/package_info.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.811040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      777 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.811040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1265 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.815040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.815040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/measure/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/measure/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      317 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/measure/measurements.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.815040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      577 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/money/currency_major.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/money/currency_minor_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       30 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/money/currency_minor_singular.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      552 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/money/local_currency.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.815040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      107 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/digit_100.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       83 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/digit_1000.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      432 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/flops.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/fraction.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      118 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/fraction_dual.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/fraction_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       82 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/fraction_singular.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       73 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/quantities.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      175 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/teens.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/tens.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       10 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/zero.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8591 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.815040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6624 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3641 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3368 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6004 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8425 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5429 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1325 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1667 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.819040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1785 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2250 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4503 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2124 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2384 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2831 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1526 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12188 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/data_loader_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.819040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.819040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.819040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      118 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       84 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      258 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/electronic/symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      542 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/fractions.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.819040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/measure/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/measure/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1198 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/measure/measurements.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      139 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/measure/suppletive.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.819040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      396 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/money/currency.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/money/currency_minor_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/money/currency_minor_singular.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.819040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/months/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/months/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      147 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/months/abbr_to_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      230 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/months/numbers.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.823040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       59 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/numbers/ones.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      119 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/numbers/quantities.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      109 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/numbers/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       81 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/numbers/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.823040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       93 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/ordinals/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       70 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/ordinals/thousands.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      139 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/ordinals/ties.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.823040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       53 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/time/hour_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/time/hour_to_night.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/time/minute_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/time/time_zone.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       89 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/whitelist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.827040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7656 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5770 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3692 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3197 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2226 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7046 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7226 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2002 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3701 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3981 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7199 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2811 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1313 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1350 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.827040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1734 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2759 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2435 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3561 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3030 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3378 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2303 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1850 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5518 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3770 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2831 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/verbalize_final.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.827040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      899 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12763 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/clean_eval_data.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.827040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.827040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/address/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/address/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      161 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/address/address_word.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      617 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/address/state.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.831040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/date/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/date/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      257 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/date/day.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      141 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/date/month_abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/date/month_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      234 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/date/month_number.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      128 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/date/year_suffix.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.831040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      222 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/electronic/symbol.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/electronic/words.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.831040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/measure/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/measure/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       71 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/measure/math_operation.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1554 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/measure/unit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      544 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/measure/unit_alternatives.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.831040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      656 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/money/currency_major.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       36 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/money/currency_minor_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/money/currency_minor_singular.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       15 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/money/per_unit.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.835040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/__init__.py
+-rwxr-xr-x   0 tbartley (361899520) domain-users (748400513)   325078 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name.far
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    54511 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name_au.far
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       62 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/fraction.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/hundred.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      107 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/quantity_abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      109 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      261 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/thousand.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       69 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/ty.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.835040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/ordinal/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/ordinal/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/ordinal/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/ordinal/teen.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.835040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    35561 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/female.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       45 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/key_word.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    20334 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/male.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    72815 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/roman_to_spoken.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1843 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/suppletive.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.835040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/telephone/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/telephone/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       19 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/telephone/ip_prompt.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       38 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/telephone/ssn_prompt.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       56 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/telephone/telephone_prompt.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.835040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       84 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/time/suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      116 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/time/zone.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.839040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      520 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/alternatives.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      155 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/alternatives_all_format.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)   175146 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/asr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      865 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/asr_with_pc.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2532 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/ipa_symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      263 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/lj_speech.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      240 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/symbol.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    36553 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/tts.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9160 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.839040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2070 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/abbreviation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7174 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    15334 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5490 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5057 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2401 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11525 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9522 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2549 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2566 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4937 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/range.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4552 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/roman.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6175 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/serial.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6035 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5200 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10941 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12298 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_lm.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12748 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_with_audio.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6290 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4000 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1654 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.843040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1447 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/abbreviation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1954 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3924 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3295 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4728 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3720 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4474 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2743 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2113 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6845 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/post_processing.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2509 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/roman.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2373 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3638 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3986 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3117 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1582 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1512 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.843040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      682 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.843040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.843040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/dates/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/dates/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      348 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/dates/days_abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      115 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/dates/months.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      551 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/dates/months_abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1184 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/dates/year_suffix.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.843040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       86 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       73 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      311 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/electronic/symbols.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.847041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/fractions/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/fractions/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      117 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/fractions/fraction_symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       28 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/fractions/ordinal_exceptions.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      224 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/fractions/powers_of_ten.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      137 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/fractions/powers_of_ten_fem.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.847041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/measures/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/measures/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       52 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/measures/math_symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      260 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/measures/measurements.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       95 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/measures/measurements_complex.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       55 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_fem.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_masc.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.847041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1030 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_major.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_major_ext.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      773 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_minor.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2155 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_minor_ext.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      177 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1800 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem_ext.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5659 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc_ext.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.847041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      111 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       52 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/quantities.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      108 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       72 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      141 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/twenties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.851040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      137 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      286 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/gender_suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      471 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/roman_exceptions.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      200 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      165 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      295 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/twenties.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.851040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/roman/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/roman/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/roman/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/roman/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       15 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/roman/thousands.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/roman/ties.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.851040 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/telephone/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/telephone/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       66 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/telephone/ip_prompt.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      143 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/telephone/telephone_prompt.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.855041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       31 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/afternoon_times.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/alt_minutes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/evening_times.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       53 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/hour_to_12.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      128 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/hour_to_24.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/hour_to_night.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/minute_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       60 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/morning_times.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      150 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/time_suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1056 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/time_zone.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3192 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/time_zone_ext.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      869 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8365 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.855041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5598 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6128 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/decimals.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3464 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5931 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7950 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8830 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7466 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8013 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9440 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7301 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2811 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1169 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.859041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2399 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3469 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3707 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/decimals.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3587 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8535 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5238 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7014 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2962 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2518 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8940 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3589 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2827 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/verbalize_final.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.859041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.859041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.859041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/fractions/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/fractions/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      116 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/fractions/irregular_denominators.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.859041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/measures/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/measures/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      232 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/measures/measurements.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.859041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       62 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/eighty.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/ninety.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       90 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/quantities.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       10 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/seventy.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       93 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/teens.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/ten.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       50 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/tens_simple.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.859041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      855 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/ordinals/irregular_numbers.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       55 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/ordinals/suffixes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      260 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/whitelist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.863041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6737 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5168 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/decimals.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2947 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2068 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5720 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2812 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1329 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1170 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.863041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1589 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2741 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/decimals.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2686 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3033 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2321 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2910 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/verbalize_final.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.863041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.863041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.863041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/dates/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/dates/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      499 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/dates/days.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      694 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/dates/days_to_numbers.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      162 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/dates/month_abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      132 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/dates/months.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      143 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/dates/months_roman.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.867041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      198 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      100 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/electronic/symbols.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.867041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/fractions/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/fractions/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      150 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/fractions/fraction_symbols.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.867041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/inflection/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/inflection/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3803 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/inflection/endings.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/inflection/plural_endings.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/inflection/word_endings.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       81 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/math_operations.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.867041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/measures/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/measures/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      215 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/measures/greek_lower.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      215 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/measures/greek_upper.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      757 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/measures/measurements.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.867041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      278 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/money/alphabet.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      166 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/money/currency.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      106 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/money/currency_minor.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.867041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       68 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       66 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/digit_inline.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      111 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/digit_nom.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      250 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/quantities.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       94 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/tens.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       87 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/tens_inline.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        8 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.867041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      382 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/ordinals/endings.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       55 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/ordinals/exceptional.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       63 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/ordinals/superessive_endings.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/ordinals/superscript_digits.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.871041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      212 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/area_codes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      804 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/country_codes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       19 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/ip_prompt.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       44 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/special_numbers.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       29 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/telephone_abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       10 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/telephone_prompt.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.871041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       87 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/time/time_zone.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      354 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      548 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/whitelist_inflect.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      291 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/whitelist_inflect_sg.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1546 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.871041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12472 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10479 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5767 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3649 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2466 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5749 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7804 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3363 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6670 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11365 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7376 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3686 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5516 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.875041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1767 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2022 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2989 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3782 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2368 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2129 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3493 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1583 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2331 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3983 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3588 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2911 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/verbalize_final.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.875041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.875041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1343 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/currency.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      147 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/measurement_dates.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      967 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/measurements.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.875041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       90 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       42 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/numbers/quantities.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      135 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/numbers/ties.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.875041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/ordinal/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/ordinal/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      123 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/ordinal/digit.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.875041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      427 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/time/hours.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1235 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/time/minutes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      624 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/whitelist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.879041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4305 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3504 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1661 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3579 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3276 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3214 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1156 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1644 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5031 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1957 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1164 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1170 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.879041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1321 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2245 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1714 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2744 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1486 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1473 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1566 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2676 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2333 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1290 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1520 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.879041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      912 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.879041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.883041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      187 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       73 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/electronic/symbols.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.883041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/measure/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/measure/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      822 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/measure/measurements.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      189 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/measure/suppletive.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.883041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      157 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/money/currency_major.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      132 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/money/currency_minor.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       30 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/money/currency_plural_fem.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/money/currency_plural_masc.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.883041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       98 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       16 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/quantities.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      117 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       81 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/tens.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      113 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/tens_eight.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      105 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/tens_one.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.883041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/whitelist/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/whitelist/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1051 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/whitelist/whitelist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.887041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7840 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5060 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/decimals.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3751 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8249 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3305 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6135 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2877 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1332 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1164 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.887041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1731 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2951 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3223 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1902 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6211 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3707 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3015 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2827 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    33677 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/normalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    22719 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/normalize_with_audio.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2891 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/preprocessing_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.887041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2078 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/alphabet.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.887041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.887041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/currency/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/currency/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1420 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/currency/currency_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1085 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/currency/currency_singular.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.887041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       47 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      290 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      668 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/electronic/symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      275 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/latin_to_cyrillic.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/measurements.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.891041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/months/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/months/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      239 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/months/abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1541 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/months/abbr_to_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      214 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/months/numbers.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.891041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      969 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/1_cardinals_nominative.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      911 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/2_cardinals_genitive.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      933 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/3_cardinals_dative.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      913 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/4_cardinals_accusative.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1048 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/5_cardinals_instrumental.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      951 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/6_cardinals_prepositional.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      549 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_alternatives.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      710 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_nominative_case.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      565 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_delimiter.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1026 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_endings.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      119 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/digits_nominative_case.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      430 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/ordinal_endings.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    21537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/ordinals.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      537 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/quantity.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.891041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      469 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/time/increment_hour_cardinal.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      611 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/time/increment_hour_ordinal.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      828 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/time/minutes_to_hour.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       62 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/time/time_convert.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.903041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3206 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/g.fst
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    69495 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/universal_thousands_punct.far
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)  7085564 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/util_arithmetic.far
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    14099 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/util_byte.far
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1005 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/whitelist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.903041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6819 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6015 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4466 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/decimals.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4797 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6943 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3998 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6606 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/number_names.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2951 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3266 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5254 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7098 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3045 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1313 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1337 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.907041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1892 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1498 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2190 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1571 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1760 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1495 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1463 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1783 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2116 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2993 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2879 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5161 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/run_evaluate.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.907041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.907041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      334 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/abbreviations_nondet.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.907041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/dates/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/dates/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      208 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/dates/era_suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       94 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/dates/era_words.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      176 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/dates/month_abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      112 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/dates/months.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.907041 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/electronic/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/electronic/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/electronic/domain.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/electronic/server_name.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      263 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/electronic/symbols.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      162 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/fillers.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       71 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/math_operations.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.911042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      196 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/greek_lower.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      196 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/greek_upper.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2121 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/unit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      157 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/unit_neuter.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1461 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/unit_plural.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.911042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1344 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/currency_major.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/currency_major_nt.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      745 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_plural.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      735 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_singular.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1197 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/currency_plurals.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.911042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      142 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/fraction.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1586 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/millions.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/millions_abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/quantities.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       94 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       72 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.911042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/ordinals/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/ordinals/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       83 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/ordinals/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      115 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/ordinals/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       96 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/ordinals/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        9 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/ordinals/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.915042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/roman/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/roman/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/roman/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/roman/hundreds.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       46 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/roman/ties.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.915042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      804 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/country_codes.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       22 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/ip_prompt.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       96 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/special_numbers.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       28 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/ssn_prompt.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      381 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/telephone_abbr.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       58 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/telephone_prompt.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.915042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       53 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/time/hour_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       67 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/time/hour_to_night.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/time/minute_to.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      261 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/time/suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       64 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/time/time_zone.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1046 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2521 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.919042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2168 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/abbreviation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    18416 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8095 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7106 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3481 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4238 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10130 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12313 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9471 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8363 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8753 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     9197 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    11054 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify_with_audio.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3024 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1323 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1173 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.919042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1733 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2618 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2838 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/decimals.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3679 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3156 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3750 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2807 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1585 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2380 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4271 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3589 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2910 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5164 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/token_parser.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    12219 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/utils_audio_based.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.919042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.919042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.919042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       24 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/charset_extension.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    32616 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/charset_national_standard_2013_8105.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      553 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/fullwidth_to_halfwidth.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       13 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/oov_tags.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      291 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/punctuations_zh.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       72 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/upper_to_lower.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.923042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/date/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/date/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      363 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/date/day.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      144 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/date/months.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      222 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/date/suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      206 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/date/suffixes.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.923042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/denylist/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/denylist/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        7 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/denylist/denylist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.923042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/erhua/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/erhua/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      350 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/erhua/whitelist.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.923042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/math/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/math/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       14 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/math/score.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       57 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/math/symbol.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.923042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/measure/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/measure/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      839 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/measure/units_en.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.923042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/money/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/money/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4047 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/money/currency_major.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      565 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/money/currency_mandarin.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.923042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/digit.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       54 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/digit_alt.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       47 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/digit_tens.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       12 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/sign.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      143 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/suffix.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       97 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/teen.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      127 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/teen_alt.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       72 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/ties.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        6 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/zero.tsv
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.927042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       35 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/AM.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       36 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/PM.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      288 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/hour.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      744 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/minute.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      744 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/second.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        2 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/zero.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1362 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/whitelist.tsv
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5130 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/graph_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.927042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)    10133 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6028 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3924 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6208 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3126 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     5065 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2808 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1856 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/preprocessor.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2655 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6613 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     4990 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/tokenize_and_classify.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2358 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1909 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.931042 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2022 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3669 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2510 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2692 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2784 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2127 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3695 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/post_processing.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3049 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/postprocessor.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3893 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3202 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2149 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize_final.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1292 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1106 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.931042 nemo_text_processing-1.0.1.post0/nemo_text_processing/utils/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      677 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/utils/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1021 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing/utils/logging.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.955042 nemo_text_processing-1.0.1.post0/nemo_text_processing.egg-info/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     7208 2024-05-03 21:42:14.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing.egg-info/PKG-INFO
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)   101841 2024-05-03 21:42:14.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        1 2024-05-03 21:42:14.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)        1 2024-05-03 21:42:14.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing.egg-info/not-zip-safe
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      488 2024-05-03 21:42:14.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing.egg-info/requires.txt
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)       27 2024-05-03 21:42:14.000000 nemo_text_processing-1.0.1.post0/nemo_text_processing.egg-info/top_level.txt
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.931042 nemo_text_processing-1.0.1.post0/requirements/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      139 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/requirements/requirements.txt
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      167 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/requirements/requirements_test.txt
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1153 2024-05-03 21:42:14.959042 nemo_text_processing-1.0.1.post0/setup.cfg
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8341 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/setup.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.931042 nemo_text_processing-1.0.1.post0/tests/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     8115 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/conftest.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.931042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.931042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1874 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2649 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2303 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2918 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2375 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1955 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_whitelist.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.931042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/audio_based_utils/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/audio_based_utils/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1325 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/audio_based_utils/test_audio_based_utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.935042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2314 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2323 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2332 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2327 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2324 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2318 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1547 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_normalization_with_audio.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2047 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2314 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2315 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.935042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1886 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_address.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3054 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3753 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2951 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2944 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1786 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1843 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_math.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2932 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3065 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1531 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_normalization_with_audio.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2943 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1840 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_punctuation.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1848 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_range.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1853 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_roman.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1866 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_serial.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1957 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_special_text.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2963 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1749 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_text_split.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2929 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3636 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     3025 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.939042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2339 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2259 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2335 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2353 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1810 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2345 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2330 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1508 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_normalization_with_audio.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2336 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2350 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2335 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2348 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2397 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.939042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1292 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1283 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1301 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1279 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1296 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1283 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1287 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1300 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1299 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1289 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.943042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1768 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1764 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1286 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1768 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1765 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1285 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1756 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.943042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.943042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/data_text_normalization/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/data_text_normalization/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1244 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1242 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1248 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1245 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1243 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1239 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1243 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1247 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1246 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1236 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.947042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1772 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1771 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1765 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1769 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1762 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1772 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1762 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.947042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1257 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1256 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1284 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1254 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1278 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1258 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_whitelist.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.947042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1275 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1267 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1273 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1267 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1268 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.947042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1283 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1280 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1286 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1277 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1281 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1285 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1274 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1285 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1275 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.951042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.951042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/data_text_normalization/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/data_text_normalization/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6340 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/test_ru_inverse_normalization.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     6527 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/test_ru_normalization.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.951042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.951042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/data_inverse_text_normalization/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/data_inverse_text_normalization/__init__.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.951042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/data_text_normalization/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/data_text_normalization/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2611 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2600 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2608 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2617 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2612 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1808 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1804 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1603 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_normalization_with_audio.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2615 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2600 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2614 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2648 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_word.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     2812 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/utils.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.955042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      610 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1600 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1591 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1597 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1603 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_electronic.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1600 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1598 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1594 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1598 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1602 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_telephone.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1591 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1602 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1592 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_word.py
+drwxr-xr-x   0 tbartley (361899520) domain-users (748400513)        0 2024-05-03 21:42:14.955042 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)      623 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/__init__.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1748 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_cardinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1794 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_date.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1743 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_decimal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1810 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_fraction.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1268 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_measure.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1757 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_money.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1746 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_ordinal.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1794 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_time.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1758 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_whitelist.py
+-rw-r--r--   0 tbartley (361899520) domain-users (748400513)     1783 2024-05-03 21:39:10.000000 nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_word.py
```

### Comparing `nemo_text_processing-1.0.1/LICENSE` & `nemo_text_processing-1.0.1.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/PKG-INFO` & `nemo_text_processing-1.0.1.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo_text_processing
-Version: 1.0.1
+Version: 1.0.1.post0
 Summary: NeMo text processing for ASR and TTS
 Home-page: https://github.com/nvidia/nemo-text-processing
 Download-URL: https://github.com/NVIDIA/NeMo-text-processing/releases
 Author: NVIDIA
 Author-email: nemo-toolkit@nvidia.com
 Maintainer: NVIDIA
 Maintainer-email: nemo-toolkit@nvidia.com
```

### Comparing `nemo_text_processing-1.0.1/README.md` & `nemo_text_processing-1.0.1.post0/README.md`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/fst_alignment/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/fst_alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/fst_alignment/alignment.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/fst_alignment/alignment.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/g2p/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/g2p/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/g2p/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/g2p/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/hybrid/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/hybrid/mlm_scorer.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/mlm_scorer.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/hybrid/model_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/model_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/hybrid/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/hybrid/wfst_lm_rescoring.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/hybrid/wfst_lm_rescoring.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ar/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/clean_eval_data.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/clean_eval_data.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/currency.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/currency.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/measurements.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/whitelist.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/data/whitelist_tech.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/data/whitelist_tech.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/en/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/en/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/dates/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/fractions/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/fractions/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/measures/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/teen.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/teen.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/ordinals/twenties.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/twenties.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/roman/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/data/en_whitelist.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/data/en_whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/es_en/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/fractions.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/fractions.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/measurements/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_major.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/roman/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/fr/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/currency.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/currency.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/measurements.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/data/time/minutes.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/data/time/minutes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/hy/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/hy/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/inverse_normalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/inverse_normalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/date/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/date/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/date/dates.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/date/dates.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/numbers/tens.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/numbers/tens.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/time/minutes.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/time/minutes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/data/time/minutes_to.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/data/time/minutes_to.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/mr/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/mr/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/measurements_plural.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/measurements_singular.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_singular.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/pt/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/decimals.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/run_evaluate.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/run_evaluate.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/sv/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/sv/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/math/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/math/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/measurements.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/vi/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/date/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/date/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/date/day.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/date/day.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_major.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/time_mandarin.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/time_mandarin.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/time_minutes.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/time_minutes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/data/time/time_seconds.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/data/time/time_seconds.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/inverse_text_normalization/zh/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/inverse_text_normalization/zh/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/package_info.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/package_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 MAJOR = 1
 MINOR = 0
 PATCH = 1
-PRE_RELEASE = ''
+PRE_RELEASE = 'r'
 
 # Use the following formatting: (major, minor, patch, pre-release)
 VERSION = (MAJOR, MINOR, PATCH, PRE_RELEASE)
 
 __shortversion__ = '.'.join(map(str, VERSION[:3]))
 __version__ = '.'.join(map(str, VERSION[:3])) + ''.join(VERSION[3:])
```

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/measure/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/money/currency_major.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/money/local_currency.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/money/local_currency.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/data/number/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/data/number/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ar/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ar/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/data_loader_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/data_loader_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/fractions.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/fractions.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/measure/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/measure/measurements.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/measure/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/months/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/months/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/de/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/de/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/clean_eval_data.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/clean_eval_data.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/address/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/address/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/address/state.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/address/state.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/date/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/date/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/measure/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/measure/unit.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/measure/unit.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/measure/unit_alternatives.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/measure/unit_alternatives.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/money/currency_major.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name.far` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name_au.far` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name_au.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/ordinal/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/ordinal/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/female.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/female.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/male.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/male.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/roman/roman_to_spoken.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/roman/roman_to_spoken.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/suppletive.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/suppletive.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/telephone/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/telephone/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/alternatives.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/alternatives.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/asr.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/asr.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/asr_with_pc.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/asr_with_pc.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/ipa_symbols.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/ipa_symbols.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/data/whitelist/tts.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/data/whitelist/tts.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/abbreviation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/abbreviation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/range.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/range.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/roman.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/roman.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/serial.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/serial.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_lm.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_lm.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_with_audio.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/abbreviation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/abbreviation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/post_processing.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/post_processing.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/roman.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/roman.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/en/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/en/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/dates/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/dates/months_abbr.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/dates/months_abbr.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/dates/year_suffix.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/dates/year_suffix.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/fractions/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/fractions/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/measures/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_masc.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_masc.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_major.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_major_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_major_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_minor.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_minor.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_minor_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_minor_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/roman/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/telephone/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/telephone/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/time_zone.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/time_zone.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/time/time_zone_ext.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/time/time_zone_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/data/whitelist.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/decimals.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/decimals.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/es/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/es/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/fractions/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/fractions/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/measures/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/data/ordinals/irregular_numbers.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/data/ordinals/irregular_numbers.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/decimals.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/decimals.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/fr/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/fr/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/dates/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/dates/days_to_numbers.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/dates/days_to_numbers.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/fractions/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/fractions/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/inflection/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/inflection/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/inflection/endings.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/inflection/endings.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/measures/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/measures/measurements.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/measures/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/number/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/number/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/telephone/country_codes.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/telephone/country_codes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/data/whitelist_inflect.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/data/whitelist_inflect.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hu/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hu/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/currency.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/currency.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/measurements.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/ordinal/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/ordinal/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/time/minutes.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/time/minutes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/data/whitelist.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/hy/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/hy/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/measure/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/measure/measurements.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/measure/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/whitelist/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/whitelist/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/data/whitelist/whitelist.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/data/whitelist/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/decimals.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/it/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/it/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/normalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/normalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/normalize_with_audio.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/normalize_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/preprocessing_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/alphabet.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/alphabet.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/currency/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/currency/currency_plural.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/currency/currency_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/currency/currency_singular.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/currency/currency_singular.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/electronic/symbols.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/electronic/symbols.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/measurements.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/months/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/months/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/months/abbr_to_name.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/months/abbr_to_name.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/1_cardinals_nominative.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/1_cardinals_nominative.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/2_cardinals_genitive.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/2_cardinals_genitive.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/3_cardinals_dative.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/3_cardinals_dative.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/4_cardinals_accusative.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/4_cardinals_accusative.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/5_cardinals_instrumental.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/5_cardinals_instrumental.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/6_cardinals_prepositional.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/6_cardinals_prepositional.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_alternatives.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_alternatives.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_nominative_case.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_nominative_case.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/decimal_delimiter.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_delimiter.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/decimal_endings.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_endings.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/ordinals.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/ordinals.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/numbers/quantity.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/numbers/quantity.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/time/increment_hour_ordinal.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/time/increment_hour_ordinal.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/time/minutes_to_hour.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/time/minutes_to_hour.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/g.fst` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/g.fst`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/universal_thousands_punct.far` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/universal_thousands_punct.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/util_arithmetic.far` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/util_arithmetic.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/utils/util_byte.far` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/utils/util_byte.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/data/whitelist.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/decimals.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/number_names.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/number_names.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/ru/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/run_evaluate.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/run_evaluate.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/dates/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/electronic/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/unit.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/unit.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/measure/unit_plural.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/measure/unit_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/currency_major.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/currency_minor_plural.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/currency_minor_singular.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_singular.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/money/currency_plurals.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/money/currency_plurals.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/numbers/millions.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/numbers/millions.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/ordinals/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/roman/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/telephone/country_codes.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/telephone/country_codes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/data/whitelist.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/abbreviation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/abbreviation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify_with_audio.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/decimals.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/electronic.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/telephone.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/sv/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/token_parser.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/token_parser.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/utils_audio_based.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/utils_audio_based.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/charset_national_standard_2013_8105.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/charset_national_standard_2013_8105.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/char/fullwidth_to_halfwidth.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/char/fullwidth_to_halfwidth.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/date/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/date/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/denylist/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/denylist/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/erhua/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/erhua/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/math/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/math/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/measure/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/measure/units_en.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/measure/units_en.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/money/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/money/currency_major.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/money/currency_mandarin.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/money/currency_mandarin.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/number/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/number/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/minute.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/minute.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/time/second.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/time/second.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/data/whitelist.tsv` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/graph_utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/preprocessor.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/preprocessor.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/punctuation.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/tokenize_and_classify.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/taggers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/utils.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/cardinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/date.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/decimal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/fraction.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/measure.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/money.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/ordinal.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/post_processing.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/post_processing.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/postprocessor.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/postprocessor.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/time.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/verbalize.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/verbalize_final.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/whitelist.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/text_normalization/zh/verbalizers/word.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/text_normalization/zh/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/utils/__init__.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing/utils/logging.py` & `nemo_text_processing-1.0.1.post0/nemo_text_processing/utils/logging.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing.egg-info/PKG-INFO` & `nemo_text_processing-1.0.1.post0/nemo_text_processing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo_text_processing
-Version: 1.0.1
+Version: 1.0.1.post0
 Summary: NeMo text processing for ASR and TTS
 Home-page: https://github.com/nvidia/nemo-text-processing
 Download-URL: https://github.com/NVIDIA/NeMo-text-processing/releases
 Author: NVIDIA
 Author-email: nemo-toolkit@nvidia.com
 Maintainer: NVIDIA
 Maintainer-email: nemo-toolkit@nvidia.com
```

### Comparing `nemo_text_processing-1.0.1/nemo_text_processing.egg-info/SOURCES.txt` & `nemo_text_processing-1.0.1.post0/nemo_text_processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/setup.cfg` & `nemo_text_processing-1.0.1.post0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/setup.py` & `nemo_text_processing-1.0.1.post0/setup.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/conftest.py` & `nemo_text_processing-1.0.1.post0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ar/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ar/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/audio_based_utils/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/audio_based_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/audio_based_utils/test_audio_based_utils.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/audio_based_utils/test_audio_based_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_normalization_with_audio.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_normalization_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_telephone.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/de/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/de/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_address.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_address.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_math.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_math.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_normalization_with_audio.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_normalization_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_punctuation.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_range.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_range.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_roman.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_roman.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_serial.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_serial.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_special_text.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_special_text.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_telephone.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_text_split.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_text_split.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/en/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/en/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_normalization_with_audio.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_normalization_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_telephone.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_telephone.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/es_en/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/es_en/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_telephone.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/fr/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/fr/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/data_text_normalization/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/data_text_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_telephone.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hu/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hu/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/hy/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/hy/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/it/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/it/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/it/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/mr/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/mr/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_telephone.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/pt/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/pt/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/data_text_normalization/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/data_text_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/test_ru_inverse_normalization.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/test_ru_inverse_normalization.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/ru/test_ru_normalization.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/ru/test_ru_normalization.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/data_inverse_text_normalization/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/data_inverse_text_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/data_text_normalization/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/data_text_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_normalization_with_audio.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_normalization_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_telephone.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/sv/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/sv/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/utils.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_electronic.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_telephone.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/vi/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/vi/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/__init__.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_cardinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_date.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_decimal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_fraction.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_measure.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_money.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_ordinal.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_time.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_whitelist.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-1.0.1/tests/nemo_text_processing/zh/test_word.py` & `nemo_text_processing-1.0.1.post0/tests/nemo_text_processing/zh/test_word.py`

 * *Files identical despite different names*

