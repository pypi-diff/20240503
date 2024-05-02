# Comparing `tmp/rapidfuzz-3.8.0.tar.gz` & `tmp/rapidfuzz-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidfuzz-3.8.0.tar", last modified: Sat Apr  6 13:50:32 2024, max compression
+gzip compressed data, was "rapidfuzz-3.8.1.tar", last modified: Sun Apr  7 20:36:58 2024, max compression
```

## Comparing `rapidfuzz-3.8.0.tar` & `rapidfuzz-3.8.1.tar`

### file list

```diff
@@ -1,288 +1,288 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.448758 rapidfuzz-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    31203 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-06 13:50:32.448758 rapidfuzz-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.392758 rapidfuzz-3.8.0/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/_custom_build/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.392758 rapidfuzz-3.8.0/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/cmake/CheckCPUArch.c.in
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/cmake/CheckCPUArch.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.392758 rapidfuzz-3.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.392758 rapidfuzz-3.8.0/docs/Contributing/
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/License.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/References.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.392758 rapidfuzz-3.8.0/docs/Usage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.396758 rapidfuzz-3.8.0/docs/Usage/distance/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/DamerauLevenshtein.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/Hamming.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/Indel.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/Jaro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/JaroWinkler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/LCSseq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/Levenshtein.rst
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/OSA.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/Postfix.rst
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/Prefix.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.396758 rapidfuzz-3.8.0/docs/Usage/distance/img/
--rw-r--r--   0 runner    (1001) docker     (127)    37487 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/img/damerau_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/img/indel_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34090 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/img/jaro.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34913 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/img/jaro_winkler.svg
--rw-r--r--   0 runner    (1001) docker     (127)    37821 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/img/osa.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/img/uniform_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/distance/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/fuzz.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.400758 rapidfuzz-3.8.0/docs/Usage/img/
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/WRatio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/indel_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41626 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/partial_ratio_long_needle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/partial_ratio_short_needle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28491 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/partial_token_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24769 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/partial_token_set_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25404 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/partial_token_sort_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24367 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    27273 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/token_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/token_set_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/token_sort_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/img/uniform_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/process.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/Usage/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/changelog_link.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.400758 rapidfuzz-3.8.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/img/RapidFuzz.svg
--rw-r--r--   0 runner    (1001) docker     (127)    56024 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/img/cdist.svg
--rw-r--r--   0 runner    (1001) docker     (127)    54183 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/img/scorer.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.388758 rapidfuzz-3.8.0/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.400758 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.400758 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.404758 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17962 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.408758 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30315 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    45010 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    37942 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-06 13:50:05.000000 rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/rapidfuzz_all.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.408758 rapidfuzz-3.8.0/extern/taskflow/
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-06 13:50:06.000000 rapidfuzz-3.8.0/extern/taskflow/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-06 13:50:06.000000 rapidfuzz-3.8.0/extern/taskflow/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-06 13:50:06.000000 rapidfuzz-3.8.0/extern/taskflow/TaskflowConfig.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.408758 rapidfuzz-3.8.0/extern/taskflow/taskflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.408758 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/critical.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/data_pipeline.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14972 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/find.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/for_each.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/launch.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/partitioner.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    44892 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/pipeline.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/reduce.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/scan.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20947 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/sort.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/transform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.412758 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/
--rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/async.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/async_task.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/declarations.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/environment.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/error.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    54781 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/executor-module-opt.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    66789 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/executor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    41751 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/flow_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24153 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/notifier.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/observer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/semaphore.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/task.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/taskflow.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/topology.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/tsq.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/core/worker.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/taskflow.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.412758 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/math.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19899 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/object_pool.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/os.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    29321 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/serializer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/singleton.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    31329 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/small_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/stream.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-06 13:50:07.000000 rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/uuid.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-06 13:50:29.000000 rapidfuzz-3.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 13:50:32.448758 rapidfuzz-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.388758 rapidfuzz-3.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.428758 rapidfuzz-3.8.0/src/rapidfuzz/
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.428758 rapidfuzz-3.8.0/src/rapidfuzz/FeatureDetector/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/FeatureDetector/CpuInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/FeatureDetector/CpuInfo.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.428758 rapidfuzz-3.8.0/src/rapidfuzz/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/__pyinstaller/hook-rapidfuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/_common_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/_feature_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)   265576 2024-04-06 13:50:25.000000 rapidfuzz-3.8.0/src/rapidfuzz/_feature_detector_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/_feature_detector_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/cpp_common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17428 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/cpp_common.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.444758 rapidfuzz-3.8.0/src/rapidfuzz/distance/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/DamerauLevenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/DamerauLevenshtein.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/DamerauLevenshtein_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Hamming.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Hamming_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Indel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Indel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Indel_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Jaro.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Jaro.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/JaroWinkler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/JaroWinkler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/JaroWinkler_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Jaro_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/LCSseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/LCSseq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/LCSseq_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Levenshtein.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Levenshtein_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/OSA.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/OSA.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/OSA_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Postfix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Postfix_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/Prefix_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize.pyi
--rw-r--r--   0 runner    (1001) docker     (127)  1692690 2024-04-06 13:50:26.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize_cpp.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    29674 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    28459 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize_py.py
--rw-r--r--   0 runner    (1001) docker     (127)    49089 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)  1506523 2024-04-06 13:50:27.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    62859 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1514554 2024-04-06 13:50:28.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp_avx2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1514554 2024-04-06 13:50:29.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp_sse2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp_sse2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   677932 2024-04-06 13:50:21.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   679913 2024-04-06 13:50:21.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp_avx2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   679913 2024-04-06 13:50:22.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp_sse2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp_sse2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    26867 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/fuzz_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/process.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/process_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/process_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)  2150891 2024-04-06 13:50:24.000000 rapidfuzz-3.8.0/src/rapidfuzz/process_cpp_impl.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/process_cpp_impl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    79018 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/process_cpp_impl.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    31494 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/process_py.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/rapidfuzz.h
--rw-r--r--   0 runner    (1001) docker     (127)   293266 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/unicodetype_db.h
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   501828 2024-04-06 13:50:24.000000 rapidfuzz-3.8.0/src/rapidfuzz/utils_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/utils_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/utils_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/src/rapidfuzz/utils_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.448758 rapidfuzz-3.8.0/src/rapidfuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-06 13:50:32.000000 rapidfuzz-3.8.0/src/rapidfuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-04-06 13:50:32.000000 rapidfuzz-3.8.0/src/rapidfuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:50:32.000000 rapidfuzz-3.8.0/src/rapidfuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 13:50:32.000000 rapidfuzz-3.8.0/src/rapidfuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 13:50:32.000000 rapidfuzz-3.8.0/src/rapidfuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 13:50:32.000000 rapidfuzz-3.8.0/src/rapidfuzz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.444758 rapidfuzz-3.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:32.448758 rapidfuzz-3.8.0/tests/distance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_DamerauLevenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_Hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_Indel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_Jaro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_JaroWinkler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_LCSseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_Levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_OSA.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_Postfix.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_Prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/distance/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/test_cpp_fallback.py
--rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/test_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (127)    26380 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/test_pure_python_fallback.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-06 13:50:03.000000 rapidfuzz-3.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.646793 rapidfuzz-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    31353 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-07 20:36:58.646793 rapidfuzz-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.590792 rapidfuzz-3.8.1/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/_custom_build/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.590792 rapidfuzz-3.8.1/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/cmake/CheckCPUArch.c.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/cmake/CheckCPUArch.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.594792 rapidfuzz-3.8.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.594792 rapidfuzz-3.8.1/docs/Contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/License.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/References.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.594792 rapidfuzz-3.8.1/docs/Usage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.594792 rapidfuzz-3.8.1/docs/Usage/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/DamerauLevenshtein.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/Hamming.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/Indel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/Jaro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/JaroWinkler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/LCSseq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/Levenshtein.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/OSA.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/Postfix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/Prefix.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.598792 rapidfuzz-3.8.1/docs/Usage/distance/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    37487 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/img/damerau_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/img/indel_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34090 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/img/jaro.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34913 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/img/jaro_winkler.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    37821 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/img/osa.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/img/uniform_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/distance/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/fuzz.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.598792 rapidfuzz-3.8.1/docs/Usage/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/WRatio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/indel_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41626 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/partial_ratio_long_needle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/partial_ratio_short_needle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28491 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/partial_token_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24769 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/partial_token_set_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25404 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/partial_token_sort_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24367 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    27273 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/token_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/token_set_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/token_sort_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/img/uniform_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/process.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/Usage/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/changelog_link.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.598792 rapidfuzz-3.8.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/img/RapidFuzz.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    56024 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/img/cdist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    54183 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/img/scorer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.586792 rapidfuzz-3.8.1/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.602792 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.602792 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.602792 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17962 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.606792 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30315 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45010 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    37942 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-07 20:36:27.000000 rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/rapidfuzz_all.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.606792 rapidfuzz-3.8.1/extern/taskflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/TaskflowConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.606792 rapidfuzz-3.8.1/extern/taskflow/taskflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.610792 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/critical.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/data_pipeline.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14972 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/find.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/for_each.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/launch.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/partitioner.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    44892 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/pipeline.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/reduce.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/scan.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20947 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/sort.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/transform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.610792 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/async.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/async_task.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/declarations.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/error.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54781 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/executor-module-opt.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    66789 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/executor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    41751 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/flow_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24153 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/notifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/observer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/semaphore.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/task.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/taskflow.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/topology.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/tsq.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/core/worker.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/taskflow.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.614792 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/math.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19899 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/object_pool.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/os.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29321 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/serializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/singleton.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31329 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/small_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/stream.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-07 20:36:29.000000 rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/uuid.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-07 20:36:54.000000 rapidfuzz-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 20:36:58.646793 rapidfuzz-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.590792 rapidfuzz-3.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.626792 rapidfuzz-3.8.1/src/rapidfuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.626792 rapidfuzz-3.8.1/src/rapidfuzz/FeatureDetector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/FeatureDetector/CpuInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/FeatureDetector/CpuInfo.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.626792 rapidfuzz-3.8.1/src/rapidfuzz/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/__pyinstaller/hook-rapidfuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/_common_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/_feature_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   266395 2024-04-07 20:36:50.000000 rapidfuzz-3.8.1/src/rapidfuzz/_feature_detector_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/_feature_detector_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/cpp_common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17428 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/cpp_common.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.642792 rapidfuzz-3.8.1/src/rapidfuzz/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/DamerauLevenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/DamerauLevenshtein.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/DamerauLevenshtein_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Hamming.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Hamming_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Indel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Indel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Indel_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Jaro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Jaro.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/JaroWinkler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/JaroWinkler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/JaroWinkler_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Jaro_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/LCSseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/LCSseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/LCSseq_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Levenshtein.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Levenshtein_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/OSA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/OSA.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/OSA_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Postfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Postfix_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/Prefix_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)  1693674 2024-04-07 20:36:51.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize_cpp.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    29674 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    28459 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49089 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)  1507372 2024-04-07 20:36:52.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    62859 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1515403 2024-04-07 20:36:53.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp_avx2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1515403 2024-04-07 20:36:54.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp_sse2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp_sse2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   678772 2024-04-07 20:36:46.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   680753 2024-04-07 20:36:47.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp_avx2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   680753 2024-04-07 20:36:47.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp_sse2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp_sse2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    26867 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/fuzz_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/process.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/process_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/process_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2151344 2024-04-07 20:36:49.000000 rapidfuzz-3.8.1/src/rapidfuzz/process_cpp_impl.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/process_cpp_impl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    79018 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/process_cpp_impl.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    31494 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/process_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/rapidfuzz.h
+-rw-r--r--   0 runner    (1001) docker     (127)   293266 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/unicodetype_db.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   502668 2024-04-07 20:36:50.000000 rapidfuzz-3.8.1/src/rapidfuzz/utils_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/utils_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/utils_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/src/rapidfuzz/utils_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.646793 rapidfuzz-3.8.1/src/rapidfuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-07 20:36:58.000000 rapidfuzz-3.8.1/src/rapidfuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-04-07 20:36:58.000000 rapidfuzz-3.8.1/src/rapidfuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:36:58.000000 rapidfuzz-3.8.1/src/rapidfuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-07 20:36:58.000000 rapidfuzz-3.8.1/src/rapidfuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 20:36:58.000000 rapidfuzz-3.8.1/src/rapidfuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 20:36:58.000000 rapidfuzz-3.8.1/src/rapidfuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.642792 rapidfuzz-3.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:58.646793 rapidfuzz-3.8.1/tests/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_DamerauLevenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_Hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_Indel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_Jaro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_JaroWinkler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_LCSseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_Levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_OSA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_Postfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_Prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/distance/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/test_cpp_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/test_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26380 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/test_pure_python_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-07 20:36:24.000000 rapidfuzz-3.8.1/tests/test_utils.py
```

### Comparing `rapidfuzz-3.8.0/CHANGELOG.rst` & `rapidfuzz-3.8.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 ---------
 
+[3.8.1] - 2024-04-07
+^^^^^^^^^^^^^^^^^^^^
+Fixed
+~~~~~
+* use the correct version of `rapidfuzz-cpp` when building against a system installed version
+
+
 [3.8.0] - 2024-04-06
 ^^^^^^^^^^^^^^^^^^^^
 Added
 ~~~~~
 * added ``process.cpdist`` which allows pairwise comparision of two collection of inputs
 
 Fixed
```

### Comparing `rapidfuzz-3.8.0/CMakeLists.txt` & `rapidfuzz-3.8.1/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
   set(TF_BUILD_EXAMPLES
       OFF
       CACHE BOOL "Enables build of examples")
   add_subdirectory(extern/taskflow EXCLUDE_FROM_ALL)
   add_library(Taskflow::Taskflow ALIAS Taskflow)
 endif()
 
-find_package(rapidfuzz 3.0.2 QUIET)
+find_package(rapidfuzz 3.0.4 QUIET)
 if(rapidfuzz_FOUND)
   message(STATUS "Using system supplied version of rapidfuzz-cpp")
 else()
   message(STATUS "Using packaged version of rapidfuzz-cpp")
   add_subdirectory(extern/rapidfuzz-cpp)
 endif()
```

### Comparing `rapidfuzz-3.8.0/LICENSE` & `rapidfuzz-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/MANIFEST.in` & `rapidfuzz-3.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/PKG-INFO` & `rapidfuzz-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidfuzz
-Version: 3.8.0
+Version: 3.8.1
 Summary: rapid fuzzy string matching
 Home-page: https://github.com/rapidfuzz/RapidFuzz
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidfuzz Version: 3.8.0 Summary: rapid fuzzy
+Metadata-Version: 2.1 Name: rapidfuzz Version: 3.8.1 Summary: rapid fuzzy
 string matching Home-page: https://github.com/rapidfuzz/RapidFuzz Author: Max
 Bachmann Author-email: pypi@maxbachmann.de License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
```

### Comparing `rapidfuzz-3.8.0/README.md` & `rapidfuzz-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/_custom_build/backend.py` & `rapidfuzz-3.8.1/_custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/cmake/CheckCPUArch.cmake` & `rapidfuzz-3.8.1/cmake/CheckCPUArch.cmake`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Contributing/index.rst` & `rapidfuzz-3.8.1/docs/Contributing/index.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Installation.rst` & `rapidfuzz-3.8.1/docs/Installation.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/DamerauLevenshtein.rst` & `rapidfuzz-3.8.1/docs/Usage/distance/DamerauLevenshtein.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/Indel.rst` & `rapidfuzz-3.8.1/docs/Usage/distance/Indel.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/Jaro.rst` & `rapidfuzz-3.8.1/docs/Usage/distance/Jaro.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/JaroWinkler.rst` & `rapidfuzz-3.8.1/docs/Usage/distance/JaroWinkler.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/LCSseq.rst` & `rapidfuzz-3.8.1/docs/Usage/distance/LCSseq.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/Levenshtein.rst` & `rapidfuzz-3.8.1/docs/Usage/distance/Levenshtein.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/OSA.rst` & `rapidfuzz-3.8.1/docs/Usage/distance/OSA.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/img/damerau_levenshtein.svg` & `rapidfuzz-3.8.1/docs/Usage/distance/img/damerau_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/img/indel_levenshtein.svg` & `rapidfuzz-3.8.1/docs/Usage/distance/img/indel_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/img/jaro.svg` & `rapidfuzz-3.8.1/docs/Usage/distance/img/jaro.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/img/jaro_winkler.svg` & `rapidfuzz-3.8.1/docs/Usage/distance/img/jaro_winkler.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/img/osa.svg` & `rapidfuzz-3.8.1/docs/Usage/distance/img/osa.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/distance/img/uniform_levenshtein.svg` & `rapidfuzz-3.8.1/docs/Usage/distance/img/uniform_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/fuzz.rst` & `rapidfuzz-3.8.1/docs/Usage/fuzz.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/WRatio.svg` & `rapidfuzz-3.8.1/docs/Usage/img/WRatio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/indel_levenshtein.svg` & `rapidfuzz-3.8.1/docs/Usage/img/indel_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/partial_ratio_long_needle.svg` & `rapidfuzz-3.8.1/docs/Usage/img/partial_ratio_long_needle.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/partial_ratio_short_needle.svg` & `rapidfuzz-3.8.1/docs/Usage/img/partial_ratio_short_needle.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/partial_token_ratio.svg` & `rapidfuzz-3.8.1/docs/Usage/img/partial_token_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/partial_token_set_ratio.svg` & `rapidfuzz-3.8.1/docs/Usage/img/partial_token_set_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/partial_token_sort_ratio.svg` & `rapidfuzz-3.8.1/docs/Usage/img/partial_token_sort_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/ratio.svg` & `rapidfuzz-3.8.1/docs/Usage/img/ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/token_ratio.svg` & `rapidfuzz-3.8.1/docs/Usage/img/token_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/token_set_ratio.svg` & `rapidfuzz-3.8.1/docs/Usage/img/token_set_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/token_sort_ratio.svg` & `rapidfuzz-3.8.1/docs/Usage/img/token_sort_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/Usage/img/uniform_levenshtein.svg` & `rapidfuzz-3.8.1/docs/Usage/img/uniform_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/conf.py` & `rapidfuzz-3.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/img/RapidFuzz.svg` & `rapidfuzz-3.8.1/docs/img/RapidFuzz.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/img/cdist.svg` & `rapidfuzz-3.8.1/docs/img/cdist.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/img/scorer.svg` & `rapidfuzz-3.8.1/docs/img/scorer.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/index.rst` & `rapidfuzz-3.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/docs/refs.bib` & `rapidfuzz-3.8.1/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/CMakeLists.txt` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # RapidFuzz's build breaks if done in-tree. You probably should not build
 # things in tree anyway, but we can allow projects that include RapidFuzz
 # as a subproject to build in-tree as long as it is not in our tree.
 if (CMAKE_BINARY_DIR STREQUAL CMAKE_CURRENT_SOURCE_DIR)
     message(FATAL_ERROR "Building in-source is not supported! Create a build dir and remove ${CMAKE_SOURCE_DIR}/CMakeCache.txt")
 endif()
 
-project(rapidfuzz LANGUAGES CXX VERSION 3.0.2)
+project(rapidfuzz LANGUAGES CXX VERSION 3.0.4)
 
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/cmake")
 include(GNUInstallDirs)
 include(CMakePackageConfigHelpers)
 
 # Basic paths
 set(BASE_DIR ${CMAKE_CURRENT_SOURCE_DIR})
```

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/LICENSE` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp` & `rapidfuzz-3.8.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/CMakeLists.txt` & `rapidfuzz-3.8.1/extern/taskflow/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/LICENSE` & `rapidfuzz-3.8.1/extern/taskflow/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/critical.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/critical.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/data_pipeline.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/data_pipeline.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/find.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/find.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/for_each.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/for_each.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/launch.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/launch.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/partitioner.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/partitioner.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/pipeline.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/pipeline.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/reduce.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/reduce.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/scan.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/scan.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/sort.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/sort.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/algorithm/transform.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/algorithm/transform.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/async.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/async.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/async_task.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/async_task.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/declarations.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/declarations.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/error.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/error.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/executor-module-opt.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/executor-module-opt.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/executor.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/executor.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/flow_builder.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/flow_builder.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/graph.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/graph.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/notifier.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/notifier.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/observer.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/observer.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/semaphore.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/semaphore.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/task.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/task.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/taskflow.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/taskflow.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/topology.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/topology.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/tsq.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/tsq.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/core/worker.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/core/worker.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/taskflow.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/taskflow.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/iterator.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/iterator.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/math.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/math.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/object_pool.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/object_pool.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/os.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/os.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/serializer.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/serializer.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/singleton.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/singleton.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/small_vector.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/small_vector.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/stream.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/stream.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/traits.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/traits.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/extern/taskflow/taskflow/utility/uuid.hpp` & `rapidfuzz-3.8.1/extern/taskflow/taskflow/utility/uuid.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/pyproject.toml` & `rapidfuzz-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/setup.py` & `rapidfuzz-3.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 with open("README.md", encoding="utf8") as f:
     readme = f.read()
 
 setup_args = {
     "name": "rapidfuzz",
-    "version": "3.8.0",
+    "version": "3.8.1",
     "extras_require": {"full": ["numpy"]},
     "url": "https://github.com/rapidfuzz/RapidFuzz",
     "author": "Max Bachmann",
     "author_email": "pypi@maxbachmann.de",
     "description": "rapid fuzzy string matching",
     "long_description": readme,
     "long_description_content_type": "text/markdown",
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/CMakeLists.txt` & `rapidfuzz-3.8.1/src/rapidfuzz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/FeatureDetector/CpuInfo.cpp` & `rapidfuzz-3.8.1/src/rapidfuzz/FeatureDetector/CpuInfo.cpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/FeatureDetector/CpuInfo.hpp` & `rapidfuzz-3.8.1/src/rapidfuzz/FeatureDetector/CpuInfo.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/__init__.pxd` & `rapidfuzz-3.8.1/src/rapidfuzz/__init__.pxd`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/__init__.py` & `rapidfuzz-3.8.1/src/rapidfuzz/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 rapid string matching library
 """
 
 from __future__ import annotations
 
 __author__: str = "Max Bachmann"
 __license__: str = "MIT"
-__version__: str = "3.8.0"
+__version__: str = "3.8.1"
 
 from rapidfuzz import distance, fuzz, process, utils
 
 __all__ = ["distance", "fuzz", "process", "utils", "get_include"]
 
 
 def get_include():
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py` & `rapidfuzz-3.8.1/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/_common_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/_common_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/_feature_detector_cpp.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/_feature_detector_cpp.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/_utils.py` & `rapidfuzz-3.8.1/src/rapidfuzz/_utils.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/cpp_common.hpp` & `rapidfuzz-3.8.1/src/rapidfuzz/cpp_common.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/cpp_common.pxd` & `rapidfuzz-3.8.1/src/rapidfuzz/cpp_common.pxd`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/CMakeLists.txt` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/DamerauLevenshtein.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/DamerauLevenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/DamerauLevenshtein.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/DamerauLevenshtein.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/DamerauLevenshtein_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/DamerauLevenshtein_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Hamming.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Hamming.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Hamming.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Hamming.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Hamming_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Hamming_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Indel.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Indel.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Indel.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Indel.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Indel_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Indel_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Jaro.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Jaro.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/JaroWinkler.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/JaroWinkler.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/JaroWinkler_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/JaroWinkler_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Jaro_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Jaro_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/LCSseq.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/LCSseq.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/LCSseq.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/LCSseq.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/LCSseq_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/LCSseq_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Levenshtein.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Levenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Levenshtein.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Levenshtein.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Levenshtein_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Levenshtein_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/OSA.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/OSA.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/OSA_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/OSA_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Postfix_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Postfix_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/Prefix_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/Prefix_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/__init__.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/__init__.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize_cpp.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize_cpp.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2598,30 +2628,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -28218,24 +28248,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__ *__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__[8];
 static int __pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__[--__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -28254,15 +28286,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__)))) {
     __pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__[__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__++] = ((struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -28377,24 +28409,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__ *__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__[8];
 static int __pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__[--__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -28413,15 +28447,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__)))) {
     __pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__[__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__++] = ((struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -28536,24 +28570,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__ *__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__[8];
 static int __pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__[--__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -28572,15 +28608,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__)))) {
     __pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__[__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__++] = ((struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -28695,24 +28731,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr *__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr[8];
 static int __pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr[--__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -28732,15 +28770,15 @@
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_op);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr)))) {
     __pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr[__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr++] = ((struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -28858,24 +28896,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__ *__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__[8];
 static int __pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__[--__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -28894,15 +28934,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__)))) {
     __pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__[__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__++] = ((struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -29017,24 +29057,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__ *__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__[8];
 static int __pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__[--__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -29053,15 +29095,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__)))) {
     __pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__[__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__++] = ((struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -29176,24 +29218,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr *__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr[8];
 static int __pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr[--__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -29213,15 +29257,15 @@
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_op);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr)))) {
     __pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr[__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr++] = ((struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -29339,24 +29383,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__ *__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__[8];
 static int __pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__[--__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -29375,15 +29421,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__)))) {
     __pyx_freelist_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__[__pyx_freecount_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__++] = ((struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -30571,23 +30617,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -34641,18 +34687,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -34698,23 +34744,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize_cpp.pyx` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/_initialize_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/_initialize_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics.hpp` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2326,30 +2356,30 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
 static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
 #else
 #define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -24674,29 +24704,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rapidfuzz.distance._initialize_cpp"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_9(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(3, 9, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_9(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_9(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_10(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(3, 9, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_10(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_10(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -30204,18 +30234,18 @@
         else
             value = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyDict_Type_get, d, key, default_value);
     }
     return value;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -30261,23 +30291,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp.pyx` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp_avx2.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp_avx2.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2327,30 +2357,30 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
 static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
 #else
 #define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -24675,29 +24705,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rapidfuzz.distance._initialize_cpp"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_9(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(4, 9, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_9(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(4, 12, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_9(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_10(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(4, 9, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_10(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(4, 12, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_10(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -30205,18 +30235,18 @@
         else
             value = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyDict_Type_get, d, key, default_value);
     }
     return value;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -30262,23 +30292,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_cpp_sse2.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_cpp_sse2.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2327,30 +2357,30 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
 static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
 #else
 #define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -24675,29 +24705,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rapidfuzz.distance._initialize_cpp"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_9(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(4, 9, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_9(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(4, 12, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_9(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_10(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(4, 9, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_10(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(4, 12, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_10(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -30205,18 +30235,18 @@
         else
             value = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyDict_Type_get, d, key, default_value);
     }
     return value;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -30262,23 +30292,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/distance/metrics_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/distance/metrics_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/fuzz.py` & `rapidfuzz-3.8.1/src/rapidfuzz/fuzz.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/fuzz.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/fuzz.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2239,30 +2269,30 @@
   #include <utility>
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
 #else
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -10100,23 +10130,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -13317,18 +13347,18 @@
 bad:
     Py_XDECREF(key);
     Py_XDECREF(value);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -13374,23 +13404,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp.hpp` & `rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp.pyx` & `rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp_avx2.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp_sse2.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1194,16 +1224,16 @@
     #else
     #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
     #endif
 #else
     #define __PYX_EXTERN_C extern "C++"
 #endif
 
-#define __PYX_HAVE__rapidfuzz__fuzz_cpp_avx2
-#define __PYX_HAVE_API__rapidfuzz__fuzz_cpp_avx2
+#define __PYX_HAVE__rapidfuzz__fuzz_cpp_sse2
+#define __PYX_HAVE_API__rapidfuzz__fuzz_cpp_sse2
 /* Early includes */
 #include <stdint.h>
 #include "rapidfuzz.h"
 #include <string.h>
 #include <stdio.h>
 #include <stddef.h>
 #include <stdlib.h>
@@ -1476,15 +1506,15 @@
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "./src/rapidfuzz/cpp_common.pxd",
   "src/rapidfuzz/fuzz_cpp.pyx",
-  "src/rapidfuzz/fuzz_cpp_avx2.pyx",
+  "src/rapidfuzz/fuzz_cpp_sse2.pyx",
   "type.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
@@ -2240,30 +2270,30 @@
   #include <utility>
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
 #else
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -2596,35 +2626,35 @@
 static CYTHON_INLINE RF_String __pyx_f_10cpp_common_conv_sequence(PyObject *); /*proto*/
 static CYTHON_INLINE bool __pyx_f_10cpp_common_preprocess_strings(PyObject *, PyObject *, PyObject *, RF_StringWrapper *, RF_StringWrapper *); /*proto*/
 static CYTHON_INLINE bool __pyx_f_10cpp_common_NoKwargsInit(RF_Kwargs *, PyObject *); /*proto*/
 static CYTHON_INLINE RF_Scorer __pyx_f_10cpp_common_CreateScorerContext(RF_KwargsInit, RF_GetScorerFlags, RF_ScorerFuncInit, RF_UncachedScorerFunc); /*proto*/
 static CYTHON_INLINE void __pyx_f_10cpp_common_SetFuncAttrs(PyObject *, PyObject *); /*proto*/
 static CYTHON_INLINE void __pyx_f_10cpp_common_SetScorerAttrs(PyObject *, PyObject *, RF_Scorer *); /*proto*/
 
-/* Module declarations from "rapidfuzz.fuzz_cpp_avx2" */
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_RatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSortRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSetRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSortRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSetRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_WRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_QRatioContext;
-static CYTHON_INLINE void __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas(void); /*proto*/
-static bool __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz(RF_Kwargs const *, RF_ScorerFlags *); /*proto*/
-static bool __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio(RF_Kwargs const *, RF_ScorerFlags *); /*proto*/
+/* Module declarations from "rapidfuzz.fuzz_cpp_sse2" */
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_RatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSortRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSetRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSortRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSetRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_WRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_QRatioContext;
+static CYTHON_INLINE void __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas(void); /*proto*/
+static bool __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz(RF_Kwargs const *, RF_ScorerFlags *); /*proto*/
+static bool __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio(RF_Kwargs const *, RF_ScorerFlags *); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
-#define __Pyx_MODULE_NAME "rapidfuzz.fuzz_cpp_avx2"
-extern int __pyx_module_is_main_rapidfuzz__fuzz_cpp_avx2;
-int __pyx_module_is_main_rapidfuzz__fuzz_cpp_avx2 = 0;
+#define __Pyx_MODULE_NAME "rapidfuzz.fuzz_cpp_sse2"
+extern int __pyx_module_is_main_rapidfuzz__fuzz_cpp_sse2;
+int __pyx_module_is_main_rapidfuzz__fuzz_cpp_sse2 = 0;
 
-/* Implementation of "rapidfuzz.fuzz_cpp_avx2" */
+/* Implementation of "rapidfuzz.fuzz_cpp_sse2" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_TypeError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = " - ";
 static const char __pyx_k_NA[] = "NA";
@@ -2675,32 +2705,32 @@
 static const char __pyx_k_token_sort_ratio[] = "token_sort_ratio";
 static const char __pyx_k_RF_OriginalScorer[] = "_RF_OriginalScorer";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_partial_token_ratio[] = "partial_token_ratio";
 static const char __pyx_k_partial_ratio_alignment[] = "partial_ratio_alignment";
 static const char __pyx_k_partial_token_set_ratio[] = "partial_token_set_ratio";
-static const char __pyx_k_rapidfuzz_fuzz_cpp_avx2[] = "rapidfuzz.fuzz_cpp_avx2";
+static const char __pyx_k_rapidfuzz_fuzz_cpp_sse2[] = "rapidfuzz.fuzz_cpp_sse2";
 static const char __pyx_k_distance__initialize_cpp[] = "distance._initialize_cpp";
 static const char __pyx_k_partial_token_sort_ratio[] = "partial_token_sort_ratio";
 static const char __pyx_k_src_rapidfuzz_fuzz_cpp_pyx[] = "src/rapidfuzz/fuzz_cpp.pyx";
 static const char __pyx_k_Got_unexpected_keyword_arguments[] = "Got unexpected keyword arguments: ";
 static const char __pyx_k_score_cutoff_has_to_be_in_the_ra[] = "score_cutoff has to be in the range of ";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_2partial_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_4partial_ratio_alignment(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_6token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_8token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_10token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_12partial_token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_14partial_token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_16partial_token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_18WRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_20QRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_2partial_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_4partial_ratio_alignment(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_6token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_8token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_10token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_12partial_token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_14partial_token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_16partial_token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_18WRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_20QRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_keys = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -2802,15 +2832,15 @@
   PyObject *__pyx_n_s_partial_ratio_alignment;
   PyObject *__pyx_n_s_partial_token_ratio;
   PyObject *__pyx_n_s_partial_token_set_ratio;
   PyObject *__pyx_n_s_partial_token_sort_ratio;
   PyObject *__pyx_n_s_processor;
   PyObject *__pyx_n_s_qualname;
   PyObject *__pyx_n_s_range;
-  PyObject *__pyx_n_s_rapidfuzz_fuzz_cpp_avx2;
+  PyObject *__pyx_n_s_rapidfuzz_fuzz_cpp_sse2;
   PyObject *__pyx_n_s_ratio;
   PyObject *__pyx_n_s_res;
   PyObject *__pyx_n_s_s1;
   PyObject *__pyx_n_s_s1_proc;
   PyObject *__pyx_n_s_s2;
   PyObject *__pyx_n_s_s2_proc;
   PyObject *__pyx_n_s_score_cutoff;
@@ -2921,15 +2951,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_partial_ratio_alignment);
   Py_CLEAR(clear_module_state->__pyx_n_s_partial_token_ratio);
   Py_CLEAR(clear_module_state->__pyx_n_s_partial_token_set_ratio);
   Py_CLEAR(clear_module_state->__pyx_n_s_partial_token_sort_ratio);
   Py_CLEAR(clear_module_state->__pyx_n_s_processor);
   Py_CLEAR(clear_module_state->__pyx_n_s_qualname);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
-  Py_CLEAR(clear_module_state->__pyx_n_s_rapidfuzz_fuzz_cpp_avx2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_rapidfuzz_fuzz_cpp_sse2);
   Py_CLEAR(clear_module_state->__pyx_n_s_ratio);
   Py_CLEAR(clear_module_state->__pyx_n_s_res);
   Py_CLEAR(clear_module_state->__pyx_n_s_s1);
   Py_CLEAR(clear_module_state->__pyx_n_s_s1_proc);
   Py_CLEAR(clear_module_state->__pyx_n_s_s2);
   Py_CLEAR(clear_module_state->__pyx_n_s_s2_proc);
   Py_CLEAR(clear_module_state->__pyx_n_s_score_cutoff);
@@ -3018,15 +3048,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_partial_ratio_alignment);
   Py_VISIT(traverse_module_state->__pyx_n_s_partial_token_ratio);
   Py_VISIT(traverse_module_state->__pyx_n_s_partial_token_set_ratio);
   Py_VISIT(traverse_module_state->__pyx_n_s_partial_token_sort_ratio);
   Py_VISIT(traverse_module_state->__pyx_n_s_processor);
   Py_VISIT(traverse_module_state->__pyx_n_s_qualname);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
-  Py_VISIT(traverse_module_state->__pyx_n_s_rapidfuzz_fuzz_cpp_avx2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_rapidfuzz_fuzz_cpp_sse2);
   Py_VISIT(traverse_module_state->__pyx_n_s_ratio);
   Py_VISIT(traverse_module_state->__pyx_n_s_res);
   Py_VISIT(traverse_module_state->__pyx_n_s_s1);
   Py_VISIT(traverse_module_state->__pyx_n_s_s1_proc);
   Py_VISIT(traverse_module_state->__pyx_n_s_s2);
   Py_VISIT(traverse_module_state->__pyx_n_s_s2_proc);
   Py_VISIT(traverse_module_state->__pyx_n_s_score_cutoff);
@@ -3159,15 +3189,15 @@
 #define __pyx_n_s_partial_ratio_alignment __pyx_mstate_global->__pyx_n_s_partial_ratio_alignment
 #define __pyx_n_s_partial_token_ratio __pyx_mstate_global->__pyx_n_s_partial_token_ratio
 #define __pyx_n_s_partial_token_set_ratio __pyx_mstate_global->__pyx_n_s_partial_token_set_ratio
 #define __pyx_n_s_partial_token_sort_ratio __pyx_mstate_global->__pyx_n_s_partial_token_sort_ratio
 #define __pyx_n_s_processor __pyx_mstate_global->__pyx_n_s_processor
 #define __pyx_n_s_qualname __pyx_mstate_global->__pyx_n_s_qualname
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
-#define __pyx_n_s_rapidfuzz_fuzz_cpp_avx2 __pyx_mstate_global->__pyx_n_s_rapidfuzz_fuzz_cpp_avx2
+#define __pyx_n_s_rapidfuzz_fuzz_cpp_sse2 __pyx_mstate_global->__pyx_n_s_rapidfuzz_fuzz_cpp_sse2
 #define __pyx_n_s_ratio __pyx_mstate_global->__pyx_n_s_ratio
 #define __pyx_n_s_res __pyx_mstate_global->__pyx_n_s_res
 #define __pyx_n_s_s1 __pyx_mstate_global->__pyx_n_s_s1
 #define __pyx_n_s_s1_proc __pyx_mstate_global->__pyx_n_s_s1_proc
 #define __pyx_n_s_s2 __pyx_mstate_global->__pyx_n_s_s2
 #define __pyx_n_s_s2_proc __pyx_mstate_global->__pyx_n_s_s2_proc
 #define __pyx_n_s_score_cutoff __pyx_mstate_global->__pyx_n_s_score_cutoff
@@ -6407,15 +6437,15 @@
  * pandas_NA = None
  * 
  * cdef inline void setupPandas() noexcept:             # <<<<<<<<<<<<<<
  *     global pandas_NA
  *     if pandas_NA is None:
  */
 
-static CYTHON_INLINE void __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas(void) {
+static CYTHON_INLINE void __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas(void) {
   PyObject *__pyx_v_pandas = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -6533,15 +6563,15 @@
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_WriteUnraisable("rapidfuzz.fuzz_cpp_avx2.setupPandas", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("rapidfuzz.fuzz_cpp_sse2.setupPandas", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pandas);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
 /* "src/rapidfuzz/fuzz_cpp.pyx":86
@@ -6549,23 +6579,23 @@
  * 
  * def ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_1ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_1ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_1ratio = {"ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_1ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_1ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_1ratio = {"ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_1ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_1ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -6656,32 +6686,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -6718,15 +6748,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(90,0,__PYX_ERR(1, 90, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":91
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -6803,15 +6833,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -6821,23 +6851,23 @@
  * 
  * def partial_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio = {"partial_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio = {"partial_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -6928,32 +6958,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_2partial_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_2partial_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_2partial_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_2partial_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -6990,15 +7020,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(102,0,__PYX_ERR(1, 102, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":103
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -7075,15 +7105,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -7093,23 +7123,23 @@
  * 
  * def partial_ratio_alignment(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment = {"partial_ratio_alignment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment = {"partial_ratio_alignment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -7200,32 +7230,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_ratio_alignment", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_ratio_alignment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_4partial_ratio_alignment(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_4partial_ratio_alignment(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_4partial_ratio_alignment(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_4partial_ratio_alignment(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   rapidfuzz::ScoreAlignment<double>  __pyx_v_res;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
@@ -7272,15 +7302,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return None
  */
   __Pyx_TraceLine(114,0,__PYX_ERR(1, 114, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":115
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return None
  * 
@@ -7444,15 +7474,15 @@
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_ratio_alignment", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_ratio_alignment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -7462,23 +7492,23 @@
  * 
  * def token_sort_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio = {"token_sort_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio = {"token_sort_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -7569,32 +7599,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_6token_sort_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_6token_sort_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_6token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_6token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -7631,15 +7661,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(131,0,__PYX_ERR(1, 131, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":132
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -7716,15 +7746,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -7734,23 +7764,23 @@
  * 
  * def token_set_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio = {"token_set_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio = {"token_set_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -7841,32 +7871,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_8token_set_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_8token_set_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_8token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_8token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -7903,15 +7933,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(143,0,__PYX_ERR(1, 143, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":144
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -7988,15 +8018,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -8006,23 +8036,23 @@
  * 
  * def token_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio = {"token_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio = {"token_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -8113,32 +8143,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_10token_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_10token_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_10token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_10token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -8175,15 +8205,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(155,0,__PYX_ERR(1, 155, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":156
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -8260,15 +8290,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -8278,23 +8308,23 @@
  * 
  * def partial_token_sort_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio = {"partial_token_sort_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio = {"partial_token_sort_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -8385,32 +8415,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_12partial_token_sort_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_12partial_token_sort_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_12partial_token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_12partial_token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -8447,15 +8477,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(167,0,__PYX_ERR(1, 167, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":168
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -8532,15 +8562,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -8550,23 +8580,23 @@
  * 
  * def partial_token_set_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio = {"partial_token_set_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio = {"partial_token_set_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -8657,32 +8687,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_14partial_token_set_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_14partial_token_set_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_14partial_token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_14partial_token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -8719,15 +8749,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(179,0,__PYX_ERR(1, 179, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":180
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -8804,15 +8834,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -8822,23 +8852,23 @@
  * 
  * def partial_token_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio = {"partial_token_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio = {"partial_token_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -8929,32 +8959,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_16partial_token_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_16partial_token_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_16partial_token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_16partial_token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -8991,15 +9021,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(191,0,__PYX_ERR(1, 191, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":192
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -9076,15 +9106,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9094,23 +9124,23 @@
  * 
  * def WRatio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_19WRatio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_19WRatio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_19WRatio = {"WRatio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_19WRatio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_19WRatio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_19WRatio = {"WRatio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_19WRatio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_19WRatio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -9201,32 +9231,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.WRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.WRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_18WRatio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_18WRatio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_18WRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_18WRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -9263,15 +9293,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(203,0,__PYX_ERR(1, 203, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":204
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -9348,15 +9378,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.WRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.WRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9366,23 +9396,23 @@
  * 
  * def QRatio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_21QRatio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_21QRatio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_21QRatio = {"QRatio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_21QRatio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_21QRatio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_21QRatio = {"QRatio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_21QRatio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_21QRatio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -9473,32 +9503,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.QRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.QRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_20QRatio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_20QRatio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_20QRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_20QRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -9535,15 +9565,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(214,0,__PYX_ERR(1, 214, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":215
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -9620,15 +9650,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.QRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.QRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9637,15 +9667,15 @@
  * 
  * 
  * cdef bool GetScorerFlagsFuzz(const RF_Kwargs* self, RF_ScorerFlags* scorer_flags) except False nogil:             # <<<<<<<<<<<<<<
  *     scorer_flags.flags = RF_SCORER_FLAG_RESULT_F64 | RF_SCORER_FLAG_SYMMETRIC | RF_SCORER_NONE_IS_WORST_SCORE
  *     scorer_flags.optimal_score.f64 = 100
  */
 
-static bool __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz(CYTHON_UNUSED RF_Kwargs const *__pyx_v_self, RF_ScorerFlags *__pyx_v_scorer_flags) {
+static bool __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz(CYTHON_UNUSED RF_Kwargs const *__pyx_v_self, RF_ScorerFlags *__pyx_v_scorer_flags) {
   bool __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
@@ -9702,15 +9732,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   #ifdef WITH_THREAD
   __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.GetScorerFlagsFuzz", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.GetScorerFlagsFuzz", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
@@ -9720,15 +9750,15 @@
  *     return True
  * 
  * cdef bool GetScorerFlagsFuzzRatio(const RF_Kwargs* self, RF_ScorerFlags* scorer_flags) except False nogil:             # <<<<<<<<<<<<<<
  *     scorer_flags.flags = RF_SCORER_FLAG_RESULT_F64 | RF_SCORER_FLAG_SYMMETRIC | RF_SCORER_NONE_IS_WORST_SCORE
  *     if RatioMultiStringSupport(self):
  */
 
-static bool __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio(RF_Kwargs const *__pyx_v_self, RF_ScorerFlags *__pyx_v_scorer_flags) {
+static bool __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio(RF_Kwargs const *__pyx_v_self, RF_ScorerFlags *__pyx_v_scorer_flags) {
   bool __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
@@ -9816,15 +9846,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   #ifdef WITH_THREAD
   __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.GetScorerFlagsFuzzRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.GetScorerFlagsFuzzRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
@@ -9886,15 +9916,15 @@
     {&__pyx_n_s_partial_ratio_alignment, __pyx_k_partial_ratio_alignment, sizeof(__pyx_k_partial_ratio_alignment), 0, 0, 1, 1},
     {&__pyx_n_s_partial_token_ratio, __pyx_k_partial_token_ratio, sizeof(__pyx_k_partial_token_ratio), 0, 0, 1, 1},
     {&__pyx_n_s_partial_token_set_ratio, __pyx_k_partial_token_set_ratio, sizeof(__pyx_k_partial_token_set_ratio), 0, 0, 1, 1},
     {&__pyx_n_s_partial_token_sort_ratio, __pyx_k_partial_token_sort_ratio, sizeof(__pyx_k_partial_token_sort_ratio), 0, 0, 1, 1},
     {&__pyx_n_s_processor, __pyx_k_processor, sizeof(__pyx_k_processor), 0, 0, 1, 1},
     {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-    {&__pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_k_rapidfuzz_fuzz_cpp_avx2, sizeof(__pyx_k_rapidfuzz_fuzz_cpp_avx2), 0, 0, 1, 1},
+    {&__pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_k_rapidfuzz_fuzz_cpp_sse2, sizeof(__pyx_k_rapidfuzz_fuzz_cpp_sse2), 0, 0, 1, 1},
     {&__pyx_n_s_ratio, __pyx_k_ratio, sizeof(__pyx_k_ratio), 0, 0, 1, 1},
     {&__pyx_n_s_res, __pyx_k_res, sizeof(__pyx_k_res), 0, 0, 1, 1},
     {&__pyx_n_s_s1, __pyx_k_s1, sizeof(__pyx_k_s1), 0, 0, 1, 1},
     {&__pyx_n_s_s1_proc, __pyx_k_s1_proc, sizeof(__pyx_k_s1_proc), 0, 0, 1, 1},
     {&__pyx_n_s_s2, __pyx_k_s2, sizeof(__pyx_k_s2), 0, 0, 1, 1},
     {&__pyx_n_s_s2_proc, __pyx_k_s2_proc, sizeof(__pyx_k_s2_proc), 0, 0, 1, 1},
     {&__pyx_n_s_score_cutoff, __pyx_k_score_cutoff, sizeof(__pyx_k_score_cutoff), 0, 0, 1, 1},
@@ -10101,23 +10131,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -10139,31 +10169,31 @@
   return 0;
 }
 
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_fuzz_cpp_avx2(PyObject* module); /*proto*/
+static int __pyx_pymod_exec_fuzz_cpp_sse2(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_fuzz_cpp_avx2},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_fuzz_cpp_sse2},
   {0, NULL}
 };
 #endif
 
 #ifdef __cplusplus
 namespace {
   struct PyModuleDef __pyx_moduledef =
   #else
   static struct PyModuleDef __pyx_moduledef =
   #endif
   {
       PyModuleDef_HEAD_INIT,
-      "fuzz_cpp_avx2",
+      "fuzz_cpp_sse2",
       0, /* m_doc */
     #if CYTHON_PEP489_MULTI_PHASE_INIT
       0, /* m_size */
     #elif CYTHON_USE_MODULE_STATE
       sizeof(__pyx_mstate), /* m_size */
     #else
       -1, /* m_size */
@@ -10203,19 +10233,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initfuzz_cpp_avx2(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initfuzz_cpp_avx2(void)
+__Pyx_PyMODINIT_FUNC initfuzz_cpp_sse2(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initfuzz_cpp_sse2(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_avx2(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_avx2(void)
+__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_sse2(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_sse2(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -10288,15 +10318,15 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_fuzz_cpp_avx2(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_fuzz_cpp_sse2(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   int stringtab_initialized = 0;
   #if CYTHON_USE_MODULE_STATE
   int pystate_addmodule_run = 0;
   #endif
@@ -10309,33 +10339,33 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'fuzz_cpp_avx2' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'fuzz_cpp_sse2' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("fuzz_cpp_avx2", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("fuzz_cpp_sse2", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(2, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "fuzz_cpp_avx2" pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "fuzz_cpp_sse2" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
@@ -10351,15 +10381,15 @@
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_avx2(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_sse2(void)", 0);
   if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(2, 1, __pyx_L1_error)
@@ -10389,22 +10419,22 @@
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitConstants() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_rapidfuzz__fuzz_cpp_avx2) {
+  if (__pyx_module_is_main_rapidfuzz__fuzz_cpp_sse2) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(2, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "rapidfuzz.fuzz_cpp_avx2")) {
-      if (unlikely((PyDict_SetItemString(modules, "rapidfuzz.fuzz_cpp_avx2", __pyx_m) < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "rapidfuzz.fuzz_cpp_sse2")) {
+      if (unlikely((PyDict_SetItemString(modules, "rapidfuzz.fuzz_cpp_sse2", __pyx_m) < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
@@ -10416,15 +10446,15 @@
   if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
-  __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_avx2(void)", __pyx_f[2], 1, 0, __PYX_ERR(2, 1, __pyx_L1_error));
+  __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_sse2(void)", __pyx_f[2], 1, 0, __PYX_ERR(2, 1, __pyx_L1_error));
 
   /* "cpp_common.pxd":255
  *     void validate_string(object py_str, const char* err) except +
  * 
  * cdef inline bool hash_array(arr, RF_String* s_proc) except False:             # <<<<<<<<<<<<<<
  *     # TODO on Cpython this does not require any copies
  *     cdef Py_UCS4 typecode = <Py_UCS4>arr.typecode
@@ -10675,29 +10705,29 @@
  *             pandas_NA = pandas.NA
  * 
  * setupPandas()             # <<<<<<<<<<<<<<
  * 
  * cdef extern from "fuzz_cpp.hpp":
  */
   __Pyx_TraceLine(46,0,__PYX_ERR(1, 46, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":86
  *     bool RatioMultiStringSupport(const RF_Kwargs*) nogil
  * 
  * def ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(86,0,__PYX_ERR(1, 86, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 86, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 86, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_1ratio, 0, __pyx_n_s_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 86, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_1ratio, 0, __pyx_n_s_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ratio, __pyx_t_2) < 0) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":98
@@ -10708,15 +10738,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(98,0,__PYX_ERR(1, 98, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 98, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 98, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio, 0, __pyx_n_s_partial_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 98, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio, 0, __pyx_n_s_partial_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_ratio, __pyx_t_3) < 0) __PYX_ERR(1, 98, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":110
@@ -10727,15 +10757,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(110,0,__PYX_ERR(1, 110, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 110, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 110, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment, 0, __pyx_n_s_partial_ratio_alignment, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment, 0, __pyx_n_s_partial_ratio_alignment, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_ratio_alignment, __pyx_t_2) < 0) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":127
@@ -10746,15 +10776,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(127,0,__PYX_ERR(1, 127, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 127, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 127, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio, 0, __pyx_n_s_token_sort_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 127, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio, 0, __pyx_n_s_token_sort_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_token_sort_ratio, __pyx_t_3) < 0) __PYX_ERR(1, 127, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":139
@@ -10765,15 +10795,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(139,0,__PYX_ERR(1, 139, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 139, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 139, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio, 0, __pyx_n_s_token_set_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 139, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio, 0, __pyx_n_s_token_set_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_token_set_ratio, __pyx_t_2) < 0) __PYX_ERR(1, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":151
@@ -10784,15 +10814,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(151,0,__PYX_ERR(1, 151, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio, 0, __pyx_n_s_token_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 151, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio, 0, __pyx_n_s_token_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_token_ratio, __pyx_t_3) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":163
@@ -10803,15 +10833,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(163,0,__PYX_ERR(1, 163, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 163, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 163, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio, 0, __pyx_n_s_partial_token_sort_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio, 0, __pyx_n_s_partial_token_sort_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_token_sort_ratio, __pyx_t_2) < 0) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":175
@@ -10822,15 +10852,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(175,0,__PYX_ERR(1, 175, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 175, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 175, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio, 0, __pyx_n_s_partial_token_set_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 175, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio, 0, __pyx_n_s_partial_token_set_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_token_set_ratio, __pyx_t_3) < 0) __PYX_ERR(1, 175, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":187
@@ -10841,15 +10871,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(187,0,__PYX_ERR(1, 187, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 187, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 187, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio, 0, __pyx_n_s_partial_token_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 187, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio, 0, __pyx_n_s_partial_token_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_token_ratio, __pyx_t_2) < 0) __PYX_ERR(1, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":199
@@ -10860,15 +10890,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(199,0,__PYX_ERR(1, 199, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 199, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_19WRatio, 0, __pyx_n_s_WRatio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_19WRatio, 0, __pyx_n_s_WRatio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_WRatio, __pyx_t_3) < 0) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":210
@@ -10879,15 +10909,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(210,0,__PYX_ERR(1, 210, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_21QRatio, 0, __pyx_n_s_QRatio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 210, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_21QRatio, 0, __pyx_n_s_QRatio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_QRatio, __pyx_t_2) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":222
@@ -10914,16 +10944,16 @@
  *     return True
  * 
  * cdef RF_Scorer RatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, RatioInit, UncachedRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(ratio, fuzz_py.ratio, &RatioContext)
  * 
  */
   __Pyx_TraceLine(237,0,__PYX_ERR(1, 237, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio, RatioInit, UncachedRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 237, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_RatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio, RatioInit, UncachedRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 237, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_RatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":238
  * 
  * cdef RF_Scorer RatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, RatioInit, UncachedRatioFuncInit())
  * SetScorerAttrs(ratio, fuzz_py.ratio, &RatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer PartialRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit())
@@ -10932,28 +10962,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_RatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_RatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":240
  * SetScorerAttrs(ratio, fuzz_py.ratio, &RatioContext)
  * 
  * cdef RF_Scorer PartialRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(partial_ratio, fuzz_py.partial_ratio, &PartialRatioContext)
  * 
  */
   __Pyx_TraceLine(240,0,__PYX_ERR(1, 240, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 240, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 240, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":241
  * 
  * cdef RF_Scorer PartialRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit())
  * SetScorerAttrs(partial_ratio, fuzz_py.partial_ratio, &PartialRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer TokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit())
@@ -10962,28 +10992,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_partial_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_partial_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 241, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":243
  * SetScorerAttrs(partial_ratio, fuzz_py.partial_ratio, &PartialRatioContext)
  * 
  * cdef RF_Scorer TokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(token_sort_ratio, fuzz_py.token_sort_ratio, &TokenSortRatioContext)
  * 
  */
   __Pyx_TraceLine(243,0,__PYX_ERR(1, 243, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 243, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSortRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 243, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSortRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":244
  * 
  * cdef RF_Scorer TokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit())
  * SetScorerAttrs(token_sort_ratio, fuzz_py.token_sort_ratio, &TokenSortRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer TokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit())
@@ -10992,28 +11022,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_token_sort_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_sort_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSortRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 244, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSortRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":246
  * SetScorerAttrs(token_sort_ratio, fuzz_py.token_sort_ratio, &TokenSortRatioContext)
  * 
  * cdef RF_Scorer TokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(token_set_ratio, fuzz_py.token_set_ratio, &TokenSetRatioContext)
  * 
  */
   __Pyx_TraceLine(246,0,__PYX_ERR(1, 246, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 246, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSetRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 246, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSetRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":247
  * 
  * cdef RF_Scorer TokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit())
  * SetScorerAttrs(token_set_ratio, fuzz_py.token_set_ratio, &TokenSetRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer TokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit())
@@ -11022,28 +11052,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_token_set_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_set_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSetRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 247, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSetRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":249
  * SetScorerAttrs(token_set_ratio, fuzz_py.token_set_ratio, &TokenSetRatioContext)
  * 
  * cdef RF_Scorer TokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(token_ratio, fuzz_py.token_ratio, &TokenRatioContext)
  * 
  */
   __Pyx_TraceLine(249,0,__PYX_ERR(1, 249, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 249, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 249, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":250
  * 
  * cdef RF_Scorer TokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit())
  * SetScorerAttrs(token_ratio, fuzz_py.token_ratio, &TokenRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer PartialTokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit())
@@ -11052,28 +11082,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_token_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_token_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 250, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":252
  * SetScorerAttrs(token_ratio, fuzz_py.token_ratio, &TokenRatioContext)
  * 
  * cdef RF_Scorer PartialTokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(partial_token_sort_ratio, fuzz_py.partial_token_sort_ratio, &PartialTokenSortRatioContext)
  * 
  */
   __Pyx_TraceLine(252,0,__PYX_ERR(1, 252, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 252, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSortRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 252, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSortRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":253
  * 
  * cdef RF_Scorer PartialTokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit())
  * SetScorerAttrs(partial_token_sort_ratio, fuzz_py.partial_token_sort_ratio, &PartialTokenSortRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer PartialTokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit())
@@ -11082,28 +11112,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_partial_token_sort_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_partial_token_sort_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSortRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 253, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSortRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":255
  * SetScorerAttrs(partial_token_sort_ratio, fuzz_py.partial_token_sort_ratio, &PartialTokenSortRatioContext)
  * 
  * cdef RF_Scorer PartialTokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(partial_token_set_ratio, fuzz_py.partial_token_set_ratio, &PartialTokenSetRatioContext)
  * 
  */
   __Pyx_TraceLine(255,0,__PYX_ERR(1, 255, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSetRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSetRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":256
  * 
  * cdef RF_Scorer PartialTokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit())
  * SetScorerAttrs(partial_token_set_ratio, fuzz_py.partial_token_set_ratio, &PartialTokenSetRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer PartialTokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit())
@@ -11112,28 +11142,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_partial_token_set_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_partial_token_set_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSetRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 256, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSetRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 256, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":258
  * SetScorerAttrs(partial_token_set_ratio, fuzz_py.partial_token_set_ratio, &PartialTokenSetRatioContext)
  * 
  * cdef RF_Scorer PartialTokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(partial_token_ratio, fuzz_py.partial_token_ratio, &PartialTokenRatioContext)
  * 
  */
   __Pyx_TraceLine(258,0,__PYX_ERR(1, 258, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 258, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 258, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":259
  * 
  * cdef RF_Scorer PartialTokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit())
  * SetScorerAttrs(partial_token_ratio, fuzz_py.partial_token_ratio, &PartialTokenRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer WRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit())
@@ -11142,28 +11172,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_partial_token_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_partial_token_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 259, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":261
  * SetScorerAttrs(partial_token_ratio, fuzz_py.partial_token_ratio, &PartialTokenRatioContext)
  * 
  * cdef RF_Scorer WRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(WRatio, fuzz_py.WRatio, &WRatioContext)
  * 
  */
   __Pyx_TraceLine(261,0,__PYX_ERR(1, 261, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 261, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_WRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 261, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_WRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":262
  * 
  * cdef RF_Scorer WRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit())
  * SetScorerAttrs(WRatio, fuzz_py.WRatio, &WRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer QRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit())
@@ -11172,46 +11202,46 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_WRatio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_WRatio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_WRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 262, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_WRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 262, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":264
  * SetScorerAttrs(WRatio, fuzz_py.WRatio, &WRatioContext)
  * 
  * cdef RF_Scorer QRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(QRatio, fuzz_py.QRatio, &QRatioContext)
  */
   __Pyx_TraceLine(264,0,__PYX_ERR(1, 264, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 264, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_QRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 264, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_QRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":265
  * 
  * cdef RF_Scorer QRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit())
  * SetScorerAttrs(QRatio, fuzz_py.QRatio, &QRatioContext)             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(265,0,__PYX_ERR(1, 265, __pyx_L1_error))
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_QRatio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_QRatio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_QRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 265, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_QRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "rapidfuzz/fuzz_cpp_avx2.pyx":1
+  /* "rapidfuzz/fuzz_cpp_sse2.pyx":1
  * # distutils: language=c++             # <<<<<<<<<<<<<<
  * # cython: language_level=3, binding=True, linetrace=True
  * 
  */
   __Pyx_TraceLine(1,0,__PYX_ERR(2, 1, __pyx_L1_error))
   __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -11224,29 +11254,29 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
-      __Pyx_AddTraceback("init rapidfuzz.fuzz_cpp_avx2", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init rapidfuzz.fuzz_cpp_sse2", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
     Py_DECREF(__pyx_m);
     if (pystate_addmodule_run) {
       PyObject *tp, *value, *tb;
       PyErr_Fetch(&tp, &value, &tb);
       PyState_RemoveModule(&__pyx_moduledef);
       PyErr_Restore(tp, value, tb);
     }
     #endif
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init rapidfuzz.fuzz_cpp_avx2");
+    PyErr_SetString(PyExc_ImportError, "init rapidfuzz.fuzz_cpp_sse2");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -13318,18 +13348,18 @@
 bad:
     Py_XDECREF(key);
     Py_XDECREF(value);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -13375,23 +13405,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/fuzz_cpp_sse2.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/fuzz_cpp_avx2.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1194,16 +1224,16 @@
     #else
     #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
     #endif
 #else
     #define __PYX_EXTERN_C extern "C++"
 #endif
 
-#define __PYX_HAVE__rapidfuzz__fuzz_cpp_sse2
-#define __PYX_HAVE_API__rapidfuzz__fuzz_cpp_sse2
+#define __PYX_HAVE__rapidfuzz__fuzz_cpp_avx2
+#define __PYX_HAVE_API__rapidfuzz__fuzz_cpp_avx2
 /* Early includes */
 #include <stdint.h>
 #include "rapidfuzz.h"
 #include <string.h>
 #include <stdio.h>
 #include <stddef.h>
 #include <stdlib.h>
@@ -1476,15 +1506,15 @@
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "./src/rapidfuzz/cpp_common.pxd",
   "src/rapidfuzz/fuzz_cpp.pyx",
-  "src/rapidfuzz/fuzz_cpp_sse2.pyx",
+  "src/rapidfuzz/fuzz_cpp_avx2.pyx",
   "type.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
@@ -2240,30 +2270,30 @@
   #include <utility>
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
 #else
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -2596,35 +2626,35 @@
 static CYTHON_INLINE RF_String __pyx_f_10cpp_common_conv_sequence(PyObject *); /*proto*/
 static CYTHON_INLINE bool __pyx_f_10cpp_common_preprocess_strings(PyObject *, PyObject *, PyObject *, RF_StringWrapper *, RF_StringWrapper *); /*proto*/
 static CYTHON_INLINE bool __pyx_f_10cpp_common_NoKwargsInit(RF_Kwargs *, PyObject *); /*proto*/
 static CYTHON_INLINE RF_Scorer __pyx_f_10cpp_common_CreateScorerContext(RF_KwargsInit, RF_GetScorerFlags, RF_ScorerFuncInit, RF_UncachedScorerFunc); /*proto*/
 static CYTHON_INLINE void __pyx_f_10cpp_common_SetFuncAttrs(PyObject *, PyObject *); /*proto*/
 static CYTHON_INLINE void __pyx_f_10cpp_common_SetScorerAttrs(PyObject *, PyObject *, RF_Scorer *); /*proto*/
 
-/* Module declarations from "rapidfuzz.fuzz_cpp_sse2" */
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_RatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSortRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSetRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSortRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSetRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_WRatioContext;
-static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_QRatioContext;
-static CYTHON_INLINE void __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas(void); /*proto*/
-static bool __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz(RF_Kwargs const *, RF_ScorerFlags *); /*proto*/
-static bool __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio(RF_Kwargs const *, RF_ScorerFlags *); /*proto*/
+/* Module declarations from "rapidfuzz.fuzz_cpp_avx2" */
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_RatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSortRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSetRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSortRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSetRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_WRatioContext;
+static RF_Scorer __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_QRatioContext;
+static CYTHON_INLINE void __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas(void); /*proto*/
+static bool __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz(RF_Kwargs const *, RF_ScorerFlags *); /*proto*/
+static bool __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio(RF_Kwargs const *, RF_ScorerFlags *); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
-#define __Pyx_MODULE_NAME "rapidfuzz.fuzz_cpp_sse2"
-extern int __pyx_module_is_main_rapidfuzz__fuzz_cpp_sse2;
-int __pyx_module_is_main_rapidfuzz__fuzz_cpp_sse2 = 0;
+#define __Pyx_MODULE_NAME "rapidfuzz.fuzz_cpp_avx2"
+extern int __pyx_module_is_main_rapidfuzz__fuzz_cpp_avx2;
+int __pyx_module_is_main_rapidfuzz__fuzz_cpp_avx2 = 0;
 
-/* Implementation of "rapidfuzz.fuzz_cpp_sse2" */
+/* Implementation of "rapidfuzz.fuzz_cpp_avx2" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_TypeError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = " - ";
 static const char __pyx_k_NA[] = "NA";
@@ -2675,32 +2705,32 @@
 static const char __pyx_k_token_sort_ratio[] = "token_sort_ratio";
 static const char __pyx_k_RF_OriginalScorer[] = "_RF_OriginalScorer";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_partial_token_ratio[] = "partial_token_ratio";
 static const char __pyx_k_partial_ratio_alignment[] = "partial_ratio_alignment";
 static const char __pyx_k_partial_token_set_ratio[] = "partial_token_set_ratio";
-static const char __pyx_k_rapidfuzz_fuzz_cpp_sse2[] = "rapidfuzz.fuzz_cpp_sse2";
+static const char __pyx_k_rapidfuzz_fuzz_cpp_avx2[] = "rapidfuzz.fuzz_cpp_avx2";
 static const char __pyx_k_distance__initialize_cpp[] = "distance._initialize_cpp";
 static const char __pyx_k_partial_token_sort_ratio[] = "partial_token_sort_ratio";
 static const char __pyx_k_src_rapidfuzz_fuzz_cpp_pyx[] = "src/rapidfuzz/fuzz_cpp.pyx";
 static const char __pyx_k_Got_unexpected_keyword_arguments[] = "Got unexpected keyword arguments: ";
 static const char __pyx_k_score_cutoff_has_to_be_in_the_ra[] = "score_cutoff has to be in the range of ";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_2partial_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_4partial_ratio_alignment(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_6token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_8token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_10token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_12partial_token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_14partial_token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_16partial_token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_18WRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_20QRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_2partial_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_4partial_ratio_alignment(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_6token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_8token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_10token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_12partial_token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_14partial_token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_16partial_token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_18WRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_20QRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff); /* proto */
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_keys = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -2802,15 +2832,15 @@
   PyObject *__pyx_n_s_partial_ratio_alignment;
   PyObject *__pyx_n_s_partial_token_ratio;
   PyObject *__pyx_n_s_partial_token_set_ratio;
   PyObject *__pyx_n_s_partial_token_sort_ratio;
   PyObject *__pyx_n_s_processor;
   PyObject *__pyx_n_s_qualname;
   PyObject *__pyx_n_s_range;
-  PyObject *__pyx_n_s_rapidfuzz_fuzz_cpp_sse2;
+  PyObject *__pyx_n_s_rapidfuzz_fuzz_cpp_avx2;
   PyObject *__pyx_n_s_ratio;
   PyObject *__pyx_n_s_res;
   PyObject *__pyx_n_s_s1;
   PyObject *__pyx_n_s_s1_proc;
   PyObject *__pyx_n_s_s2;
   PyObject *__pyx_n_s_s2_proc;
   PyObject *__pyx_n_s_score_cutoff;
@@ -2921,15 +2951,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_partial_ratio_alignment);
   Py_CLEAR(clear_module_state->__pyx_n_s_partial_token_ratio);
   Py_CLEAR(clear_module_state->__pyx_n_s_partial_token_set_ratio);
   Py_CLEAR(clear_module_state->__pyx_n_s_partial_token_sort_ratio);
   Py_CLEAR(clear_module_state->__pyx_n_s_processor);
   Py_CLEAR(clear_module_state->__pyx_n_s_qualname);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
-  Py_CLEAR(clear_module_state->__pyx_n_s_rapidfuzz_fuzz_cpp_sse2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_rapidfuzz_fuzz_cpp_avx2);
   Py_CLEAR(clear_module_state->__pyx_n_s_ratio);
   Py_CLEAR(clear_module_state->__pyx_n_s_res);
   Py_CLEAR(clear_module_state->__pyx_n_s_s1);
   Py_CLEAR(clear_module_state->__pyx_n_s_s1_proc);
   Py_CLEAR(clear_module_state->__pyx_n_s_s2);
   Py_CLEAR(clear_module_state->__pyx_n_s_s2_proc);
   Py_CLEAR(clear_module_state->__pyx_n_s_score_cutoff);
@@ -3018,15 +3048,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_partial_ratio_alignment);
   Py_VISIT(traverse_module_state->__pyx_n_s_partial_token_ratio);
   Py_VISIT(traverse_module_state->__pyx_n_s_partial_token_set_ratio);
   Py_VISIT(traverse_module_state->__pyx_n_s_partial_token_sort_ratio);
   Py_VISIT(traverse_module_state->__pyx_n_s_processor);
   Py_VISIT(traverse_module_state->__pyx_n_s_qualname);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
-  Py_VISIT(traverse_module_state->__pyx_n_s_rapidfuzz_fuzz_cpp_sse2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_rapidfuzz_fuzz_cpp_avx2);
   Py_VISIT(traverse_module_state->__pyx_n_s_ratio);
   Py_VISIT(traverse_module_state->__pyx_n_s_res);
   Py_VISIT(traverse_module_state->__pyx_n_s_s1);
   Py_VISIT(traverse_module_state->__pyx_n_s_s1_proc);
   Py_VISIT(traverse_module_state->__pyx_n_s_s2);
   Py_VISIT(traverse_module_state->__pyx_n_s_s2_proc);
   Py_VISIT(traverse_module_state->__pyx_n_s_score_cutoff);
@@ -3159,15 +3189,15 @@
 #define __pyx_n_s_partial_ratio_alignment __pyx_mstate_global->__pyx_n_s_partial_ratio_alignment
 #define __pyx_n_s_partial_token_ratio __pyx_mstate_global->__pyx_n_s_partial_token_ratio
 #define __pyx_n_s_partial_token_set_ratio __pyx_mstate_global->__pyx_n_s_partial_token_set_ratio
 #define __pyx_n_s_partial_token_sort_ratio __pyx_mstate_global->__pyx_n_s_partial_token_sort_ratio
 #define __pyx_n_s_processor __pyx_mstate_global->__pyx_n_s_processor
 #define __pyx_n_s_qualname __pyx_mstate_global->__pyx_n_s_qualname
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
-#define __pyx_n_s_rapidfuzz_fuzz_cpp_sse2 __pyx_mstate_global->__pyx_n_s_rapidfuzz_fuzz_cpp_sse2
+#define __pyx_n_s_rapidfuzz_fuzz_cpp_avx2 __pyx_mstate_global->__pyx_n_s_rapidfuzz_fuzz_cpp_avx2
 #define __pyx_n_s_ratio __pyx_mstate_global->__pyx_n_s_ratio
 #define __pyx_n_s_res __pyx_mstate_global->__pyx_n_s_res
 #define __pyx_n_s_s1 __pyx_mstate_global->__pyx_n_s_s1
 #define __pyx_n_s_s1_proc __pyx_mstate_global->__pyx_n_s_s1_proc
 #define __pyx_n_s_s2 __pyx_mstate_global->__pyx_n_s_s2
 #define __pyx_n_s_s2_proc __pyx_mstate_global->__pyx_n_s_s2_proc
 #define __pyx_n_s_score_cutoff __pyx_mstate_global->__pyx_n_s_score_cutoff
@@ -6407,15 +6437,15 @@
  * pandas_NA = None
  * 
  * cdef inline void setupPandas() noexcept:             # <<<<<<<<<<<<<<
  *     global pandas_NA
  *     if pandas_NA is None:
  */
 
-static CYTHON_INLINE void __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas(void) {
+static CYTHON_INLINE void __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas(void) {
   PyObject *__pyx_v_pandas = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -6533,15 +6563,15 @@
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_WriteUnraisable("rapidfuzz.fuzz_cpp_sse2.setupPandas", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("rapidfuzz.fuzz_cpp_avx2.setupPandas", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pandas);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
 /* "src/rapidfuzz/fuzz_cpp.pyx":86
@@ -6549,23 +6579,23 @@
  * 
  * def ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_1ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_1ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_1ratio = {"ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_1ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_1ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_1ratio = {"ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_1ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_1ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -6656,32 +6686,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -6718,15 +6748,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(90,0,__PYX_ERR(1, 90, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":91
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -6803,15 +6833,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -6821,23 +6851,23 @@
  * 
  * def partial_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio = {"partial_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio = {"partial_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -6928,32 +6958,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_2partial_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_2partial_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_2partial_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_2partial_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -6990,15 +7020,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(102,0,__PYX_ERR(1, 102, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":103
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -7075,15 +7105,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -7093,23 +7123,23 @@
  * 
  * def partial_ratio_alignment(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment = {"partial_ratio_alignment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment = {"partial_ratio_alignment", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -7200,32 +7230,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_ratio_alignment", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_ratio_alignment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_4partial_ratio_alignment(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_4partial_ratio_alignment(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_4partial_ratio_alignment(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_4partial_ratio_alignment(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   rapidfuzz::ScoreAlignment<double>  __pyx_v_res;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
@@ -7272,15 +7302,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return None
  */
   __Pyx_TraceLine(114,0,__PYX_ERR(1, 114, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":115
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return None
  * 
@@ -7444,15 +7474,15 @@
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_ratio_alignment", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_ratio_alignment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -7462,23 +7492,23 @@
  * 
  * def token_sort_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio = {"token_sort_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio = {"token_sort_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -7569,32 +7599,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_6token_sort_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_6token_sort_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_6token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_6token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -7631,15 +7661,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(131,0,__PYX_ERR(1, 131, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":132
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -7716,15 +7746,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -7734,23 +7764,23 @@
  * 
  * def token_set_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio = {"token_set_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio = {"token_set_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -7841,32 +7871,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_8token_set_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_8token_set_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_8token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_8token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -7903,15 +7933,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(143,0,__PYX_ERR(1, 143, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":144
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -7988,15 +8018,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -8006,23 +8036,23 @@
  * 
  * def token_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio = {"token_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio = {"token_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -8113,32 +8143,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_10token_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_10token_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_10token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_10token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -8175,15 +8205,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(155,0,__PYX_ERR(1, 155, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":156
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -8260,15 +8290,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -8278,23 +8308,23 @@
  * 
  * def partial_token_sort_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio = {"partial_token_sort_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio = {"partial_token_sort_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -8385,32 +8415,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_12partial_token_sort_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_12partial_token_sort_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_12partial_token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_12partial_token_sort_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -8447,15 +8477,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(167,0,__PYX_ERR(1, 167, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":168
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -8532,15 +8562,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_sort_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -8550,23 +8580,23 @@
  * 
  * def partial_token_set_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio = {"partial_token_set_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio = {"partial_token_set_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -8657,32 +8687,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_14partial_token_set_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_14partial_token_set_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_14partial_token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_14partial_token_set_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -8719,15 +8749,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(179,0,__PYX_ERR(1, 179, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":180
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -8804,15 +8834,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_set_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -8822,23 +8852,23 @@
  * 
  * def partial_token_ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio = {"partial_token_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio = {"partial_token_ratio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -8929,32 +8959,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_16partial_token_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_16partial_token_ratio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_16partial_token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_16partial_token_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -8991,15 +9021,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(191,0,__PYX_ERR(1, 191, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":192
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -9076,15 +9106,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.partial_token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.partial_token_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9094,23 +9124,23 @@
  * 
  * def WRatio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_19WRatio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_19WRatio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_19WRatio = {"WRatio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_19WRatio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_19WRatio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_19WRatio = {"WRatio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_19WRatio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_19WRatio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -9201,32 +9231,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.WRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.WRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_18WRatio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_18WRatio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_18WRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_18WRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -9263,15 +9293,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(203,0,__PYX_ERR(1, 203, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":204
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -9348,15 +9378,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.WRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.WRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9366,23 +9396,23 @@
  * 
  * def QRatio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_21QRatio(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_21QRatio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_21QRatio = {"QRatio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_21QRatio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_sse2_21QRatio(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_21QRatio = {"QRatio", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_21QRatio, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9rapidfuzz_13fuzz_cpp_avx2_21QRatio(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_s1 = 0;
@@ -9473,32 +9503,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.QRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.QRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_20QRatio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
+  __pyx_r = __pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_20QRatio(__pyx_self, __pyx_v_s1, __pyx_v_s2, __pyx_v_processor, __pyx_v_score_cutoff);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_sse2_20QRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
+static PyObject *__pyx_pf_9rapidfuzz_13fuzz_cpp_avx2_20QRatio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2, PyObject *__pyx_v_processor, PyObject *__pyx_v_score_cutoff) {
   double __pyx_v_c_score_cutoff;
   RF_StringWrapper __pyx_v_s1_proc;
   RF_StringWrapper __pyx_v_s2_proc;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -9535,15 +9565,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  * 
  *     setupPandas()             # <<<<<<<<<<<<<<
  *     if is_none(s1) or is_none(s2):
  *         return 0
  */
   __Pyx_TraceLine(214,0,__PYX_ERR(1, 214, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":215
  * 
  *     setupPandas()
  *     if is_none(s1) or is_none(s2):             # <<<<<<<<<<<<<<
  *         return 0
  * 
@@ -9620,15 +9650,15 @@
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.QRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.QRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9637,15 +9667,15 @@
  * 
  * 
  * cdef bool GetScorerFlagsFuzz(const RF_Kwargs* self, RF_ScorerFlags* scorer_flags) except False nogil:             # <<<<<<<<<<<<<<
  *     scorer_flags.flags = RF_SCORER_FLAG_RESULT_F64 | RF_SCORER_FLAG_SYMMETRIC | RF_SCORER_NONE_IS_WORST_SCORE
  *     scorer_flags.optimal_score.f64 = 100
  */
 
-static bool __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz(CYTHON_UNUSED RF_Kwargs const *__pyx_v_self, RF_ScorerFlags *__pyx_v_scorer_flags) {
+static bool __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz(CYTHON_UNUSED RF_Kwargs const *__pyx_v_self, RF_ScorerFlags *__pyx_v_scorer_flags) {
   bool __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
@@ -9702,15 +9732,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   #ifdef WITH_THREAD
   __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.GetScorerFlagsFuzz", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.GetScorerFlagsFuzz", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
@@ -9720,15 +9750,15 @@
  *     return True
  * 
  * cdef bool GetScorerFlagsFuzzRatio(const RF_Kwargs* self, RF_ScorerFlags* scorer_flags) except False nogil:             # <<<<<<<<<<<<<<
  *     scorer_flags.flags = RF_SCORER_FLAG_RESULT_F64 | RF_SCORER_FLAG_SYMMETRIC | RF_SCORER_NONE_IS_WORST_SCORE
  *     if RatioMultiStringSupport(self):
  */
 
-static bool __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio(RF_Kwargs const *__pyx_v_self, RF_ScorerFlags *__pyx_v_scorer_flags) {
+static bool __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio(RF_Kwargs const *__pyx_v_self, RF_ScorerFlags *__pyx_v_scorer_flags) {
   bool __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
@@ -9816,15 +9846,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   #ifdef WITH_THREAD
   __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_sse2.GetScorerFlagsFuzzRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("rapidfuzz.fuzz_cpp_avx2.GetScorerFlagsFuzzRatio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
@@ -9886,15 +9916,15 @@
     {&__pyx_n_s_partial_ratio_alignment, __pyx_k_partial_ratio_alignment, sizeof(__pyx_k_partial_ratio_alignment), 0, 0, 1, 1},
     {&__pyx_n_s_partial_token_ratio, __pyx_k_partial_token_ratio, sizeof(__pyx_k_partial_token_ratio), 0, 0, 1, 1},
     {&__pyx_n_s_partial_token_set_ratio, __pyx_k_partial_token_set_ratio, sizeof(__pyx_k_partial_token_set_ratio), 0, 0, 1, 1},
     {&__pyx_n_s_partial_token_sort_ratio, __pyx_k_partial_token_sort_ratio, sizeof(__pyx_k_partial_token_sort_ratio), 0, 0, 1, 1},
     {&__pyx_n_s_processor, __pyx_k_processor, sizeof(__pyx_k_processor), 0, 0, 1, 1},
     {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-    {&__pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_k_rapidfuzz_fuzz_cpp_sse2, sizeof(__pyx_k_rapidfuzz_fuzz_cpp_sse2), 0, 0, 1, 1},
+    {&__pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_k_rapidfuzz_fuzz_cpp_avx2, sizeof(__pyx_k_rapidfuzz_fuzz_cpp_avx2), 0, 0, 1, 1},
     {&__pyx_n_s_ratio, __pyx_k_ratio, sizeof(__pyx_k_ratio), 0, 0, 1, 1},
     {&__pyx_n_s_res, __pyx_k_res, sizeof(__pyx_k_res), 0, 0, 1, 1},
     {&__pyx_n_s_s1, __pyx_k_s1, sizeof(__pyx_k_s1), 0, 0, 1, 1},
     {&__pyx_n_s_s1_proc, __pyx_k_s1_proc, sizeof(__pyx_k_s1_proc), 0, 0, 1, 1},
     {&__pyx_n_s_s2, __pyx_k_s2, sizeof(__pyx_k_s2), 0, 0, 1, 1},
     {&__pyx_n_s_s2_proc, __pyx_k_s2_proc, sizeof(__pyx_k_s2_proc), 0, 0, 1, 1},
     {&__pyx_n_s_score_cutoff, __pyx_k_score_cutoff, sizeof(__pyx_k_score_cutoff), 0, 0, 1, 1},
@@ -10101,23 +10131,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -10139,31 +10169,31 @@
   return 0;
 }
 
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_fuzz_cpp_sse2(PyObject* module); /*proto*/
+static int __pyx_pymod_exec_fuzz_cpp_avx2(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_fuzz_cpp_sse2},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_fuzz_cpp_avx2},
   {0, NULL}
 };
 #endif
 
 #ifdef __cplusplus
 namespace {
   struct PyModuleDef __pyx_moduledef =
   #else
   static struct PyModuleDef __pyx_moduledef =
   #endif
   {
       PyModuleDef_HEAD_INIT,
-      "fuzz_cpp_sse2",
+      "fuzz_cpp_avx2",
       0, /* m_doc */
     #if CYTHON_PEP489_MULTI_PHASE_INIT
       0, /* m_size */
     #elif CYTHON_USE_MODULE_STATE
       sizeof(__pyx_mstate), /* m_size */
     #else
       -1, /* m_size */
@@ -10203,19 +10233,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initfuzz_cpp_sse2(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initfuzz_cpp_sse2(void)
+__Pyx_PyMODINIT_FUNC initfuzz_cpp_avx2(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initfuzz_cpp_avx2(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_sse2(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_sse2(void)
+__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_avx2(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_avx2(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -10288,15 +10318,15 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_fuzz_cpp_sse2(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_fuzz_cpp_avx2(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   int stringtab_initialized = 0;
   #if CYTHON_USE_MODULE_STATE
   int pystate_addmodule_run = 0;
   #endif
@@ -10309,33 +10339,33 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'fuzz_cpp_sse2' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'fuzz_cpp_avx2' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("fuzz_cpp_sse2", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("fuzz_cpp_avx2", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(2, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "fuzz_cpp_sse2" pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "fuzz_cpp_avx2" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
@@ -10351,15 +10381,15 @@
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_sse2(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_avx2(void)", 0);
   if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(2, 1, __pyx_L1_error)
@@ -10389,22 +10419,22 @@
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitConstants() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_rapidfuzz__fuzz_cpp_sse2) {
+  if (__pyx_module_is_main_rapidfuzz__fuzz_cpp_avx2) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(2, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "rapidfuzz.fuzz_cpp_sse2")) {
-      if (unlikely((PyDict_SetItemString(modules, "rapidfuzz.fuzz_cpp_sse2", __pyx_m) < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "rapidfuzz.fuzz_cpp_avx2")) {
+      if (unlikely((PyDict_SetItemString(modules, "rapidfuzz.fuzz_cpp_avx2", __pyx_m) < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
@@ -10416,15 +10446,15 @@
   if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
-  __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_sse2(void)", __pyx_f[2], 1, 0, __PYX_ERR(2, 1, __pyx_L1_error));
+  __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_fuzz_cpp_avx2(void)", __pyx_f[2], 1, 0, __PYX_ERR(2, 1, __pyx_L1_error));
 
   /* "cpp_common.pxd":255
  *     void validate_string(object py_str, const char* err) except +
  * 
  * cdef inline bool hash_array(arr, RF_String* s_proc) except False:             # <<<<<<<<<<<<<<
  *     # TODO on Cpython this does not require any copies
  *     cdef Py_UCS4 typecode = <Py_UCS4>arr.typecode
@@ -10675,29 +10705,29 @@
  *             pandas_NA = pandas.NA
  * 
  * setupPandas()             # <<<<<<<<<<<<<<
  * 
  * cdef extern from "fuzz_cpp.hpp":
  */
   __Pyx_TraceLine(46,0,__PYX_ERR(1, 46, __pyx_L1_error))
-  __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_setupPandas();
+  __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_setupPandas();
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":86
  *     bool RatioMultiStringSupport(const RF_Kwargs*) nogil
  * 
  * def ratio(s1, s2, *, processor=None, score_cutoff=None):             # <<<<<<<<<<<<<<
  *     cdef double c_score_cutoff = 0.0 if score_cutoff is None else score_cutoff
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(86,0,__PYX_ERR(1, 86, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 86, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 86, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_1ratio, 0, __pyx_n_s_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 86, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_1ratio, 0, __pyx_n_s_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ratio, __pyx_t_2) < 0) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":98
@@ -10708,15 +10738,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(98,0,__PYX_ERR(1, 98, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 98, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 98, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_3partial_ratio, 0, __pyx_n_s_partial_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 98, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_3partial_ratio, 0, __pyx_n_s_partial_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_ratio, __pyx_t_3) < 0) __PYX_ERR(1, 98, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":110
@@ -10727,15 +10757,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(110,0,__PYX_ERR(1, 110, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 110, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 110, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_5partial_ratio_alignment, 0, __pyx_n_s_partial_ratio_alignment, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_5partial_ratio_alignment, 0, __pyx_n_s_partial_ratio_alignment, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_ratio_alignment, __pyx_t_2) < 0) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":127
@@ -10746,15 +10776,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(127,0,__PYX_ERR(1, 127, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 127, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 127, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_7token_sort_ratio, 0, __pyx_n_s_token_sort_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 127, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_7token_sort_ratio, 0, __pyx_n_s_token_sort_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_token_sort_ratio, __pyx_t_3) < 0) __PYX_ERR(1, 127, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":139
@@ -10765,15 +10795,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(139,0,__PYX_ERR(1, 139, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 139, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 139, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_9token_set_ratio, 0, __pyx_n_s_token_set_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 139, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_9token_set_ratio, 0, __pyx_n_s_token_set_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_token_set_ratio, __pyx_t_2) < 0) __PYX_ERR(1, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":151
@@ -10784,15 +10814,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(151,0,__PYX_ERR(1, 151, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_11token_ratio, 0, __pyx_n_s_token_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 151, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_11token_ratio, 0, __pyx_n_s_token_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_token_ratio, __pyx_t_3) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":163
@@ -10803,15 +10833,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(163,0,__PYX_ERR(1, 163, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 163, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 163, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_13partial_token_sort_ratio, 0, __pyx_n_s_partial_token_sort_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_13partial_token_sort_ratio, 0, __pyx_n_s_partial_token_sort_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_token_sort_ratio, __pyx_t_2) < 0) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":175
@@ -10822,15 +10852,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(175,0,__PYX_ERR(1, 175, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 175, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 175, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_15partial_token_set_ratio, 0, __pyx_n_s_partial_token_set_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 175, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_15partial_token_set_ratio, 0, __pyx_n_s_partial_token_set_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_token_set_ratio, __pyx_t_3) < 0) __PYX_ERR(1, 175, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":187
@@ -10841,15 +10871,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(187,0,__PYX_ERR(1, 187, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 187, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 187, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_17partial_token_ratio, 0, __pyx_n_s_partial_token_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 187, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_17partial_token_ratio, 0, __pyx_n_s_partial_token_ratio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_partial_token_ratio, __pyx_t_2) < 0) __PYX_ERR(1, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":199
@@ -10860,15 +10890,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(199,0,__PYX_ERR(1, 199, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 199, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_19WRatio, 0, __pyx_n_s_WRatio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_19WRatio, 0, __pyx_n_s_WRatio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_WRatio, __pyx_t_3) < 0) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":210
@@ -10879,15 +10909,15 @@
  *     cdef RF_StringWrapper s1_proc, s2_proc
  */
   __Pyx_TraceLine(210,0,__PYX_ERR(1, 210, __pyx_L1_error))
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_processor, Py_None) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_score_cutoff, Py_None) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_sse2_21QRatio, 0, __pyx_n_s_QRatio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_sse2, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 210, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidfuzz_13fuzz_cpp_avx2_21QRatio, 0, __pyx_n_s_QRatio, NULL, __pyx_n_s_rapidfuzz_fuzz_cpp_avx2, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_QRatio, __pyx_t_2) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":222
@@ -10914,16 +10944,16 @@
  *     return True
  * 
  * cdef RF_Scorer RatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, RatioInit, UncachedRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(ratio, fuzz_py.ratio, &RatioContext)
  * 
  */
   __Pyx_TraceLine(237,0,__PYX_ERR(1, 237, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio, RatioInit, UncachedRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 237, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_RatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio, RatioInit, UncachedRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 237, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_RatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":238
  * 
  * cdef RF_Scorer RatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, RatioInit, UncachedRatioFuncInit())
  * SetScorerAttrs(ratio, fuzz_py.ratio, &RatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer PartialRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit())
@@ -10932,28 +10962,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_RatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_RatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":240
  * SetScorerAttrs(ratio, fuzz_py.ratio, &RatioContext)
  * 
  * cdef RF_Scorer PartialRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(partial_ratio, fuzz_py.partial_ratio, &PartialRatioContext)
  * 
  */
   __Pyx_TraceLine(240,0,__PYX_ERR(1, 240, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 240, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 240, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":241
  * 
  * cdef RF_Scorer PartialRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialRatioInit, UncachedPartialRatioFuncInit())
  * SetScorerAttrs(partial_ratio, fuzz_py.partial_ratio, &PartialRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer TokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit())
@@ -10962,28 +10992,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_partial_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_partial_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 241, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":243
  * SetScorerAttrs(partial_ratio, fuzz_py.partial_ratio, &PartialRatioContext)
  * 
  * cdef RF_Scorer TokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(token_sort_ratio, fuzz_py.token_sort_ratio, &TokenSortRatioContext)
  * 
  */
   __Pyx_TraceLine(243,0,__PYX_ERR(1, 243, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 243, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSortRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 243, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSortRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":244
  * 
  * cdef RF_Scorer TokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, TokenSortRatioInit, UncachedTokenSortRatioFuncInit())
  * SetScorerAttrs(token_sort_ratio, fuzz_py.token_sort_ratio, &TokenSortRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer TokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit())
@@ -10992,28 +11022,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_token_sort_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_sort_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSortRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 244, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSortRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":246
  * SetScorerAttrs(token_sort_ratio, fuzz_py.token_sort_ratio, &TokenSortRatioContext)
  * 
  * cdef RF_Scorer TokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(token_set_ratio, fuzz_py.token_set_ratio, &TokenSetRatioContext)
  * 
  */
   __Pyx_TraceLine(246,0,__PYX_ERR(1, 246, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 246, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSetRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 246, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSetRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":247
  * 
  * cdef RF_Scorer TokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenSetRatioInit, UncachedTokenSetRatioFuncInit())
  * SetScorerAttrs(token_set_ratio, fuzz_py.token_set_ratio, &TokenSetRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer TokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit())
@@ -11022,28 +11052,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_token_set_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_set_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenSetRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 247, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenSetRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":249
  * SetScorerAttrs(token_set_ratio, fuzz_py.token_set_ratio, &TokenSetRatioContext)
  * 
  * cdef RF_Scorer TokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(token_ratio, fuzz_py.token_ratio, &TokenRatioContext)
  * 
  */
   __Pyx_TraceLine(249,0,__PYX_ERR(1, 249, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 249, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 249, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":250
  * 
  * cdef RF_Scorer TokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, TokenRatioInit, UncachedTokenRatioFuncInit())
  * SetScorerAttrs(token_ratio, fuzz_py.token_ratio, &TokenRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer PartialTokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit())
@@ -11052,28 +11082,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_token_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_token_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_TokenRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 250, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_TokenRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":252
  * SetScorerAttrs(token_ratio, fuzz_py.token_ratio, &TokenRatioContext)
  * 
  * cdef RF_Scorer PartialTokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(partial_token_sort_ratio, fuzz_py.partial_token_sort_ratio, &PartialTokenSortRatioContext)
  * 
  */
   __Pyx_TraceLine(252,0,__PYX_ERR(1, 252, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 252, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSortRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 252, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSortRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":253
  * 
  * cdef RF_Scorer PartialTokenSortRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSortRatioInit, UncachedPartialTokenSortRatioFuncInit())
  * SetScorerAttrs(partial_token_sort_ratio, fuzz_py.partial_token_sort_ratio, &PartialTokenSortRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer PartialTokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit())
@@ -11082,28 +11112,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_partial_token_sort_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_partial_token_sort_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSortRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 253, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSortRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":255
  * SetScorerAttrs(partial_token_sort_ratio, fuzz_py.partial_token_sort_ratio, &PartialTokenSortRatioContext)
  * 
  * cdef RF_Scorer PartialTokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(partial_token_set_ratio, fuzz_py.partial_token_set_ratio, &PartialTokenSetRatioContext)
  * 
  */
   __Pyx_TraceLine(255,0,__PYX_ERR(1, 255, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSetRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSetRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":256
  * 
  * cdef RF_Scorer PartialTokenSetRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenSetRatioInit, UncachedPartialTokenSetRatioFuncInit())
  * SetScorerAttrs(partial_token_set_ratio, fuzz_py.partial_token_set_ratio, &PartialTokenSetRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer PartialTokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit())
@@ -11112,28 +11142,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_partial_token_set_ratio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_partial_token_set_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenSetRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 256, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenSetRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 256, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":258
  * SetScorerAttrs(partial_token_set_ratio, fuzz_py.partial_token_set_ratio, &PartialTokenSetRatioContext)
  * 
  * cdef RF_Scorer PartialTokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(partial_token_ratio, fuzz_py.partial_token_ratio, &PartialTokenRatioContext)
  * 
  */
   __Pyx_TraceLine(258,0,__PYX_ERR(1, 258, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 258, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 258, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":259
  * 
  * cdef RF_Scorer PartialTokenRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, PartialTokenRatioInit, UncachedPartialTokenRatioFuncInit())
  * SetScorerAttrs(partial_token_ratio, fuzz_py.partial_token_ratio, &PartialTokenRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer WRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit())
@@ -11142,28 +11172,28 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_partial_token_ratio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_partial_token_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_PartialTokenRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 259, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_5, __pyx_t_3, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_PartialTokenRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":261
  * SetScorerAttrs(partial_token_ratio, fuzz_py.partial_token_ratio, &PartialTokenRatioContext)
  * 
  * cdef RF_Scorer WRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(WRatio, fuzz_py.WRatio, &WRatioContext)
  * 
  */
   __Pyx_TraceLine(261,0,__PYX_ERR(1, 261, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 261, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_WRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 261, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_WRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":262
  * 
  * cdef RF_Scorer WRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzz, WRatioInit, UncachedWRatioFuncInit())
  * SetScorerAttrs(WRatio, fuzz_py.WRatio, &WRatioContext)             # <<<<<<<<<<<<<<
  * 
  * cdef RF_Scorer QRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit())
@@ -11172,46 +11202,46 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_WRatio); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_WRatio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_WRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 262, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_3, __pyx_t_2, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_WRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 262, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":264
  * SetScorerAttrs(WRatio, fuzz_py.WRatio, &WRatioContext)
  * 
  * cdef RF_Scorer QRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit())             # <<<<<<<<<<<<<<
  * SetScorerAttrs(QRatio, fuzz_py.QRatio, &QRatioContext)
  */
   __Pyx_TraceLine(264,0,__PYX_ERR(1, 264, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_sse2_GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 264, __pyx_L1_error)
-  __pyx_v_9rapidfuzz_13fuzz_cpp_sse2_QRatioContext = __pyx_t_4;
+  __pyx_t_4 = __pyx_f_10cpp_common_CreateScorerContext(__pyx_f_10cpp_common_NoKwargsInit, __pyx_f_9rapidfuzz_13fuzz_cpp_avx2_GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit()); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 264, __pyx_L1_error)
+  __pyx_v_9rapidfuzz_13fuzz_cpp_avx2_QRatioContext = __pyx_t_4;
 
   /* "src/rapidfuzz/fuzz_cpp.pyx":265
  * 
  * cdef RF_Scorer QRatioContext = CreateScorerContext(NoKwargsInit, GetScorerFlagsFuzzRatio, QRatioInit, UncachedQRatioFuncInit())
  * SetScorerAttrs(QRatio, fuzz_py.QRatio, &QRatioContext)             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(265,0,__PYX_ERR(1, 265, __pyx_L1_error))
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_QRatio); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fuzz_py); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_QRatio); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_sse2_QRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 265, __pyx_L1_error)
+  __pyx_f_10cpp_common_SetScorerAttrs(__pyx_t_2, __pyx_t_5, (&__pyx_v_9rapidfuzz_13fuzz_cpp_avx2_QRatioContext)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "rapidfuzz/fuzz_cpp_sse2.pyx":1
+  /* "rapidfuzz/fuzz_cpp_avx2.pyx":1
  * # distutils: language=c++             # <<<<<<<<<<<<<<
  * # cython: language_level=3, binding=True, linetrace=True
  * 
  */
   __Pyx_TraceLine(1,0,__PYX_ERR(2, 1, __pyx_L1_error))
   __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -11224,29 +11254,29 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
-      __Pyx_AddTraceback("init rapidfuzz.fuzz_cpp_sse2", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init rapidfuzz.fuzz_cpp_avx2", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
     Py_DECREF(__pyx_m);
     if (pystate_addmodule_run) {
       PyObject *tp, *value, *tb;
       PyErr_Fetch(&tp, &value, &tb);
       PyState_RemoveModule(&__pyx_moduledef);
       PyErr_Restore(tp, value, tb);
     }
     #endif
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init rapidfuzz.fuzz_cpp_sse2");
+    PyErr_SetString(PyExc_ImportError, "init rapidfuzz.fuzz_cpp_avx2");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -13318,18 +13348,18 @@
 bad:
     Py_XDECREF(key);
     Py_XDECREF(value);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -13375,23 +13405,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/fuzz_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/fuzz_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/process.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/process.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/process_cpp.hpp` & `rapidfuzz-3.8.1/src/rapidfuzz/process_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/process_cpp.py` & `rapidfuzz-3.8.1/src/rapidfuzz/process_cpp.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/process_cpp_impl.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/process_cpp_impl.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -37,18 +37,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -132,14 +132,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -193,14 +195,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -254,60 +258,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -390,14 +417,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -3020,30 +3050,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Py3UpdateBases.proto */
 static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
 
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
@@ -3402,15 +3432,15 @@
 static CYTHON_INLINE __PYX_ENUM_CLASS_DECL MatrixType __pyx_f_9rapidfuzz_16process_cpp_impl_dtype_to_type_num_size_t(PyObject *); /*proto*/
 static CYTHON_INLINE __PYX_ENUM_CLASS_DECL MatrixType __pyx_f_9rapidfuzz_16process_cpp_impl_dtype_to_type_num_py(PyObject *, PyObject *, PyObject *); /*proto*/
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl_Matrix *__pyx_f_9rapidfuzz_16process_cpp_impl_cpdist_cpp(PyObject *, PyObject *, RF_Scorer *, RF_ScorerFlags const *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, int, RF_Kwargs const *); /*proto*/
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl_Matrix *__pyx_f_9rapidfuzz_16process_cpp_impl_cdist_two_lists(PyObject *, PyObject *, RF_Scorer *, RF_ScorerFlags const *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, int, RF_Kwargs const *); /*proto*/
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl_Matrix *__pyx_f_9rapidfuzz_16process_cpp_impl_cdist_single_list(PyObject *, RF_Scorer *, RF_ScorerFlags const *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, int, RF_Kwargs const *); /*proto*/
 static PyObject *__pyx_f_9rapidfuzz_16process_cpp_impl_cdist_py(PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *); /*proto*/
 static PyObject *__pyx_f_9rapidfuzz_16process_cpp_impl_cpdist_py(PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, PyObject *); /*proto*/
-static PyObject *__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(__PYX_ENUM_CLASS_DECL MatrixType); /*proto*/
+static PyObject *__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(__PYX_ENUM_CLASS_DECL MatrixType); /*proto*/
 static PyObject *__pyx_unpickle___Pyx_EnumMeta__set_state(struct __pyx_obj___Pyx_EnumMeta *, PyObject *); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "rapidfuzz.process_cpp_impl"
 extern int __pyx_module_is_main_rapidfuzz__process_cpp_impl;
 int __pyx_module_is_main_rapidfuzz__process_cpp_impl = 0;
 
@@ -5162,35 +5192,35 @@
 #define __pyx_codeobj__39 __pyx_mstate_global->__pyx_codeobj__39
 #define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
 #define __pyx_codeobj__42 __pyx_mstate_global->__pyx_codeobj__42
 /* #### Code section: module_code ### */
 
 /* "EnumTypeToPy":3
  * 
- * @cname("__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py")
- * cdef __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType c_val):             # <<<<<<<<<<<<<<
+ * @cname("__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py")
+ * cdef __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType c_val):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_enum
  *     __pyx_enum = MatrixType
  */
 
-static PyObject *__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(__PYX_ENUM_CLASS_DECL MatrixType __pyx_v_c_val) {
+static PyObject *__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(__PYX_ENUM_CLASS_DECL MatrixType __pyx_v_c_val) {
   PyObject *__pyx_v___pyx_enum = 0;
   int __pyx_v_underlying_c_val;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py", 1);
+  __Pyx_RefNannySetupContext("__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py", 1);
 
   /* "EnumTypeToPy":5
- * cdef __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType c_val):
+ * cdef __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType c_val):
  *     cdef object __pyx_enum
  *     __pyx_enum = MatrixType             # <<<<<<<<<<<<<<
  * 
  *     if 0:
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MatrixType); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -5587,25 +5617,25 @@
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(1, 33, __pyx_L1_error)
   }
 
   /* "EnumTypeToPy":3
  * 
- * @cname("__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py")
- * cdef __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType c_val):             # <<<<<<<<<<<<<<
+ * @cname("__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py")
+ * cdef __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType c_val):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_enum
  *     __pyx_enum = MatrixType
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_enum);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -11472,70 +11502,70 @@
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":20
  *         @property
- *         cdef inline double real(self):
+ *         cdef inline double real(self) noexcept:
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = __pyx_v_self->cval.real;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":24
  *         @property
- *         cdef inline double imag(self):
+ *         cdef inline double imag(self) noexcept:
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
  */
   __pyx_r = __pyx_v_self->cval.imag;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -34985,15 +35015,15 @@
  *     cdef Matrix matrix = Matrix()
  *     c_dtype = dtype_to_type_num_py(dtype, scorer, scorer_kwargs)             # <<<<<<<<<<<<<<
  *     matrix.matrix = RfMatrix(c_dtype, proc_queries.size(), proc_choices.size())
  * 
  */
   __Pyx_TraceLine(1968,0,__PYX_ERR(0, 1968, __pyx_L1_error))
   __pyx_t_3 = __pyx_f_9rapidfuzz_16process_cpp_impl_dtype_to_type_num_py(__pyx_v_dtype, __pyx_v_scorer, __pyx_v_scorer_kwargs); if (unlikely(__pyx_t_3 == ((__PYX_ENUM_CLASS_DECL MatrixType)MatrixType::UNDEFINED))) __PYX_ERR(0, 1968, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1968, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1968, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_c_dtype = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1969
  *     cdef Matrix matrix = Matrix()
  *     c_dtype = dtype_to_type_num_py(dtype, scorer, scorer_kwargs)
@@ -35770,15 +35800,15 @@
  *     cdef Matrix matrix = Matrix(vector_output=True)
  *     c_dtype = dtype_to_type_num_py(dtype, scorer, scorer_kwargs)             # <<<<<<<<<<<<<<
  *     matrix.matrix = RfMatrix(c_dtype, proc_queries.size(), 1)
  * 
  */
   __Pyx_TraceLine(2022,0,__PYX_ERR(0, 2022, __pyx_L1_error))
   __pyx_t_4 = __pyx_f_9rapidfuzz_16process_cpp_impl_dtype_to_type_num_py(__pyx_v_dtype, __pyx_v_scorer, __pyx_v_scorer_kwargs); if (unlikely(__pyx_t_4 == ((__PYX_ENUM_CLASS_DECL MatrixType)MatrixType::UNDEFINED))) __PYX_ERR(0, 2022, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2022, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2022, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_c_dtype = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":2023
  *     cdef Matrix matrix = Matrix(vector_output=True)
  *     c_dtype = dtype_to_type_num_py(dtype, scorer, scorer_kwargs)
@@ -36630,25 +36660,27 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter *__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter[8];
 static int __pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter[--__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -36690,15 +36722,15 @@
   Py_CLEAR(p->__pyx_v_query);
   Py_CLEAR(p->__pyx_v_score_cutoff);
   Py_CLEAR(p->__pyx_v_score_hint);
   Py_CLEAR(p->__pyx_v_scorer);
   Py_CLEAR(p->__pyx_v_scorer_capsule);
   Py_CLEAR(p->__pyx_v_scorer_kwargs);
   Py_CLEAR(p->__pyx_v_worst_score);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter)))) {
     __pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter[__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter++] = ((struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -36867,25 +36899,27 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64 *__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64[8];
 static int __pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64 = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64 *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64 > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64[--__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -36919,15 +36953,15 @@
   __Pyx_call_destructor(p->__pyx_v_query_proc);
   __Pyx_call_destructor(p->__pyx_v_scorer_func);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_v_choice);
   Py_CLEAR(p->__pyx_v_choice_key);
   Py_CLEAR(p->__pyx_v_proc_choice);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64 < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64)))) {
     __pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64[__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64++] = ((struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64 *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -37054,25 +37088,27 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64 *__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64[8];
 static int __pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64 = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64 *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64 > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64[--__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -37106,15 +37142,15 @@
   __Pyx_call_destructor(p->__pyx_v_query_proc);
   __Pyx_call_destructor(p->__pyx_v_scorer_func);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_v_choice);
   Py_CLEAR(p->__pyx_v_choice_key);
   Py_CLEAR(p->__pyx_v_proc_choice);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64 < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64)))) {
     __pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64[__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64++] = ((struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64 *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -37241,25 +37277,27 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t *__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t[8];
 static int __pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t[--__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -37293,15 +37331,15 @@
   __Pyx_call_destructor(p->__pyx_v_query_proc);
   __Pyx_call_destructor(p->__pyx_v_scorer_func);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_v_choice);
   Py_CLEAR(p->__pyx_v_choice_key);
   Py_CLEAR(p->__pyx_v_proc_choice);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t)))) {
     __pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t[__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t++] = ((struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_dict_size_t *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -37428,25 +37466,27 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64 *__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64[8];
 static int __pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64 = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64 *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64 > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64[--__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -37481,15 +37521,15 @@
   __Pyx_call_destructor(p->__pyx_v_scorer_func);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_v_choice);
   Py_CLEAR(p->__pyx_v_i);
   Py_CLEAR(p->__pyx_v_proc_choice);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_1);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64 < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64)))) {
     __pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64[__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64++] = ((struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_f64 *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -37619,25 +37659,27 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64 *__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64[8];
 static int __pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64 = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64 *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64 > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64[--__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -37672,15 +37714,15 @@
   __Pyx_call_destructor(p->__pyx_v_scorer_func);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_v_choice);
   Py_CLEAR(p->__pyx_v_i);
   Py_CLEAR(p->__pyx_v_proc_choice);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_1);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64 < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64)))) {
     __pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64[__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64++] = ((struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_extract_iter_list_i64 *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -37810,25 +37852,27 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t *__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t[8];
 static int __pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t[--__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -37863,15 +37907,15 @@
   __Pyx_call_destructor(p->__pyx_v_scorer_func);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_v_choice);
   Py_CLEAR(p->__pyx_v_i);
   Py_CLEAR(p->__pyx_v_proc_choice);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_1);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t)))) {
     __pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t[__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t++] = ((struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_extract_iter_list_size_t *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -38001,24 +38045,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict *__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict[8];
 static int __pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict[--__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -38043,15 +38089,15 @@
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_v_choice);
   Py_CLEAR(p->__pyx_v_choice_key);
   Py_CLEAR(p->__pyx_v_optimal_score);
   Py_CLEAR(p->__pyx_v_score);
   Py_CLEAR(p->__pyx_v_worst_score);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict)))) {
     __pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict[__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict++] = ((struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_7_py_extract_iter_dict *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -38184,24 +38230,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list *__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list[8];
 static int __pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list = 0;
+#endif
 
 static PyObject *__pyx_tp_new_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list)))) {
     o = (PyObject*)__pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list[--__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list];
     memset(o, 0, sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -38225,15 +38273,15 @@
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_v_choice);
   Py_CLEAR(p->__pyx_v_optimal_score);
   Py_CLEAR(p->__pyx_v_score);
   Py_CLEAR(p->__pyx_v_worst_score);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list)))) {
     __pyx_freelist_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list[__pyx_freecount_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list++] = ((struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_8_py_extract_iter_list *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -39368,31 +39416,31 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -41264,132 +41312,132 @@
  * 
  * 
  * FLOAT32 = MatrixType.FLOAT32             # <<<<<<<<<<<<<<
  * FLOAT64 = MatrixType.FLOAT64
  * INT8 = MatrixType.INT8
  */
   __Pyx_TraceLine(1651,0,__PYX_ERR(0, 1651, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::FLOAT32); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1651, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::FLOAT32); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FLOAT32, __pyx_t_13) < 0) __PYX_ERR(0, 1651, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1652
  * 
  * FLOAT32 = MatrixType.FLOAT32
  * FLOAT64 = MatrixType.FLOAT64             # <<<<<<<<<<<<<<
  * INT8 = MatrixType.INT8
  * INT16 = MatrixType.INT16
  */
   __Pyx_TraceLine(1652,0,__PYX_ERR(0, 1652, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::FLOAT64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1652, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::FLOAT64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1652, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FLOAT64, __pyx_t_13) < 0) __PYX_ERR(0, 1652, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1653
  * FLOAT32 = MatrixType.FLOAT32
  * FLOAT64 = MatrixType.FLOAT64
  * INT8 = MatrixType.INT8             # <<<<<<<<<<<<<<
  * INT16 = MatrixType.INT16
  * INT32 = MatrixType.INT32
  */
   __Pyx_TraceLine(1653,0,__PYX_ERR(0, 1653, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::INT8); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1653, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::INT8); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1653, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_INT8, __pyx_t_13) < 0) __PYX_ERR(0, 1653, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1654
  * FLOAT64 = MatrixType.FLOAT64
  * INT8 = MatrixType.INT8
  * INT16 = MatrixType.INT16             # <<<<<<<<<<<<<<
  * INT32 = MatrixType.INT32
  * INT64 = MatrixType.INT64
  */
   __Pyx_TraceLine(1654,0,__PYX_ERR(0, 1654, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::INT16); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1654, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::INT16); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_INT16, __pyx_t_13) < 0) __PYX_ERR(0, 1654, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1655
  * INT8 = MatrixType.INT8
  * INT16 = MatrixType.INT16
  * INT32 = MatrixType.INT32             # <<<<<<<<<<<<<<
  * INT64 = MatrixType.INT64
  * UINT8 = MatrixType.UINT8
  */
   __Pyx_TraceLine(1655,0,__PYX_ERR(0, 1655, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::INT32); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1655, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::INT32); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_INT32, __pyx_t_13) < 0) __PYX_ERR(0, 1655, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1656
  * INT16 = MatrixType.INT16
  * INT32 = MatrixType.INT32
  * INT64 = MatrixType.INT64             # <<<<<<<<<<<<<<
  * UINT8 = MatrixType.UINT8
  * UINT16 = MatrixType.UINT16
  */
   __Pyx_TraceLine(1656,0,__PYX_ERR(0, 1656, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::INT64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1656, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::INT64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1656, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_INT64, __pyx_t_13) < 0) __PYX_ERR(0, 1656, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1657
  * INT32 = MatrixType.INT32
  * INT64 = MatrixType.INT64
  * UINT8 = MatrixType.UINT8             # <<<<<<<<<<<<<<
  * UINT16 = MatrixType.UINT16
  * UINT32 = MatrixType.UINT32
  */
   __Pyx_TraceLine(1657,0,__PYX_ERR(0, 1657, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::UINT8); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1657, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::UINT8); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1657, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_UINT8, __pyx_t_13) < 0) __PYX_ERR(0, 1657, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1658
  * INT64 = MatrixType.INT64
  * UINT8 = MatrixType.UINT8
  * UINT16 = MatrixType.UINT16             # <<<<<<<<<<<<<<
  * UINT32 = MatrixType.UINT32
  * UINT64 = MatrixType.UINT64
  */
   __Pyx_TraceLine(1658,0,__PYX_ERR(0, 1658, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::UINT16); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1658, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::UINT16); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1658, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_UINT16, __pyx_t_13) < 0) __PYX_ERR(0, 1658, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1659
  * UINT8 = MatrixType.UINT8
  * UINT16 = MatrixType.UINT16
  * UINT32 = MatrixType.UINT32             # <<<<<<<<<<<<<<
  * UINT64 = MatrixType.UINT64
  * 
  */
   __Pyx_TraceLine(1659,0,__PYX_ERR(0, 1659, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::UINT32); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1659, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::UINT32); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_UINT32, __pyx_t_13) < 0) __PYX_ERR(0, 1659, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1660
  * UINT16 = MatrixType.UINT16
  * UINT32 = MatrixType.UINT32
  * UINT64 = MatrixType.UINT64             # <<<<<<<<<<<<<<
  * 
  * cdef inline vector[PyObjectWrapper] preprocess_py(queries, processor) except *:
  */
   __Pyx_TraceLine(1660,0,__PYX_ERR(0, 1660, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM_CLASS_DECL__space_MatrixType__etc_to_py(MatrixType::UINT64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1660, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_Enum_93c9ea__9rapidfuzz_16process_cpp_impl__dunder_PYX_ENUM__etc_to_py(MatrixType::UINT64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_UINT64, __pyx_t_13) < 0) __PYX_ERR(0, 1660, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
   /* "rapidfuzz/process_cpp_impl.pyx":1662
  * UINT64 = MatrixType.UINT64
  * 
@@ -47468,18 +47516,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -47525,23 +47573,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/process_cpp_impl.pyi` & `rapidfuzz-3.8.1/src/rapidfuzz/process_cpp_impl.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/process_cpp_impl.pyx` & `rapidfuzz-3.8.1/src/rapidfuzz/process_cpp_impl.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/process_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/process_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/rapidfuzz.h` & `rapidfuzz-3.8.1/src/rapidfuzz/rapidfuzz.h`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/unicodetype_db.h` & `rapidfuzz-3.8.1/src/rapidfuzz/unicodetype_db.h`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/utils.cpp` & `rapidfuzz-3.8.1/src/rapidfuzz/utils.cpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/utils.hpp` & `rapidfuzz-3.8.1/src/rapidfuzz/utils.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/utils_cpp.cxx` & `rapidfuzz-3.8.1/src/rapidfuzz/utils_cpp.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -20,18 +20,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +115,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -176,14 +178,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -237,60 +241,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -373,14 +400,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2221,30 +2251,30 @@
     const char* function_name);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -6708,23 +6738,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -9351,18 +9381,18 @@
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -9408,23 +9438,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/utils_cpp.hpp` & `rapidfuzz-3.8.1/src/rapidfuzz/utils_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/utils_cpp.pyx` & `rapidfuzz-3.8.1/src/rapidfuzz/utils_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz/utils_py.py` & `rapidfuzz-3.8.1/src/rapidfuzz/utils_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz.egg-info/PKG-INFO` & `rapidfuzz-3.8.1/src/rapidfuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidfuzz
-Version: 3.8.0
+Version: 3.8.1
 Summary: rapid fuzzy string matching
 Home-page: https://github.com/rapidfuzz/RapidFuzz
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidfuzz Version: 3.8.0 Summary: rapid fuzzy
+Metadata-Version: 2.1 Name: rapidfuzz Version: 3.8.1 Summary: rapid fuzzy
 string matching Home-page: https://github.com/rapidfuzz/RapidFuzz Author: Max
 Bachmann Author-email: pypi@maxbachmann.de License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
```

### Comparing `rapidfuzz-3.8.0/src/rapidfuzz.egg-info/SOURCES.txt` & `rapidfuzz-3.8.1/src/rapidfuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/common.py` & `rapidfuzz-3.8.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/common.py` & `rapidfuzz-3.8.1/tests/distance/common.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_DamerauLevenshtein.py` & `rapidfuzz-3.8.1/tests/distance/test_DamerauLevenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_Hamming.py` & `rapidfuzz-3.8.1/tests/distance/test_Hamming.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_Indel.py` & `rapidfuzz-3.8.1/tests/distance/test_Indel.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_Jaro.py` & `rapidfuzz-3.8.1/tests/distance/test_Jaro.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_JaroWinkler.py` & `rapidfuzz-3.8.1/tests/distance/test_JaroWinkler.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_LCSseq.py` & `rapidfuzz-3.8.1/tests/distance/test_LCSseq.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_Levenshtein.py` & `rapidfuzz-3.8.1/tests/distance/test_Levenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_OSA.py` & `rapidfuzz-3.8.1/tests/distance/test_OSA.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_Postfix.py` & `rapidfuzz-3.8.1/tests/distance/test_Postfix.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_Prefix.py` & `rapidfuzz-3.8.1/tests/distance/test_Prefix.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_distance.py` & `rapidfuzz-3.8.1/tests/distance/test_distance.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/distance/test_init.py` & `rapidfuzz-3.8.1/tests/distance/test_init.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/test_fuzz.py` & `rapidfuzz-3.8.1/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/test_hypothesis.py` & `rapidfuzz-3.8.1/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/test_process.py` & `rapidfuzz-3.8.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.8.0/tests/test_utils.py` & `rapidfuzz-3.8.1/tests/test_utils.py`

 * *Files identical despite different names*

