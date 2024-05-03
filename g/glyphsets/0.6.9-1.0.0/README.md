# Comparing `tmp/glyphsets-0.6.9.tar.gz` & `tmp/glyphsets-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glyphsets-0.6.9.tar", last modified: Fri Dec 15 14:17:58 2023, max compression
+gzip compressed data, was "glyphsets-1.0.0.tar", last modified: Fri May  3 09:49:32 2024, max compression
```

## Comparing `glyphsets-0.6.9.tar` & `glyphsets-1.0.0.tar`

### file list

```diff
@@ -1,530 +1,401 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.826099 glyphsets-0.6.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.722099 glyphsets-0.6.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.730099 glyphsets-0.6.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-12-15 14:17:45.000000 glyphsets-0.6.9/.github/workflows/publish-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-15 14:17:45.000000 glyphsets-0.6.9/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-15 14:17:45.000000 glyphsets-0.6.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.730099 glyphsets-0.6.9/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-15 14:17:45.000000 glyphsets-0.6.9/.vscode/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.722099 glyphsets-0.6.9/Archive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.734099 glyphsets-0.6.9/Archive/GF Glyph Sets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.734099 glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.734099 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    10080 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.722099 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.734099 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/historical_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_italic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs_smallcaps.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.738099 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/historical_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_italic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    18371 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    16079 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.738099 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     8571 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.722099 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/RECOMMENDED.md
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/TROUBLESHOOTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    75853 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   104148 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/locl.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/plus_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/pro_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_optional-glyphs_case-accents.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/pro_optional-glyphs_case-punctuation.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/plus_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/pro_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_either_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_either_19.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_either_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    43666 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/Info/
--rw-r--r--   0 runner    (1001) docker     (127)    89964 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (127)    35092 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/Directory.png
--rw-r--r--   0 runner    (1001) docker     (127)    98535 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/ListFilters.png
--rw-r--r--   0 runner    (1001) docker     (127)    84092 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png
--rw-r--r--   0 runner    (1001) docker     (127)    24052 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    71431 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-1.png
--rw-r--r--   0 runner    (1001) docker     (127)    33541 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-2.png
--rw-r--r--   0 runner    (1001) docker     (127)    45217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-3.png
--rw-r--r--   0 runner    (1001) docker     (127)    53065 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/list-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-12-15 14:17:45.000000 glyphsets-0.6.9/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/Arabic/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/Arabic/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/definitions/GF_Arabic_Core.stub.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    17968 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/Arabic/nam/
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Plus.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    21454 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist
--rw-r--r--   0 runner    (1001) docker     (127)    11221 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclItalic.nam
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclRoman.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.758099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Historical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclItalic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.758099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Historical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclItalic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.758099 glyphsets-0.6.9/GF_glyphsets/Greek/
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.758099 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    56423 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist
--rw-r--r--   0 runner    (1001) docker     (127)    30534 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    16742 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    15594 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    26352 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    28310 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Greek/nam/
--rw-r--r--   0 runner    (1001) docker     (127)    15006 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Expert.nam
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Greek/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Latin/
--rw-r--r--   0 runner    (1001) docker     (127)     8429 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Latin/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.766099 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    38119 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist
--rw-r--r--   0 runner    (1001) docker     (127)    62282 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    19144 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    16357 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    16570 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    18721 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    15064 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.766099 glyphsets-0.6.9/GF_glyphsets/Latin/nam/
--rw-r--r--   0 runner    (1001) docker     (127)    17738 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_African.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Latin/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.766099 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.770099 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.770099 glyphsets-0.6.9/GF_glyphsets/Phonetics/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.770099 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    19280 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    17764 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.770099 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAHistorical.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_SinoExt.nam
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_UPA.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_APA.txt
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAHistorical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_SinoExt.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_UPA.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_APA.txt
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAHistorical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_SinoExt.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_UPA.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    14581 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.730099 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Arabic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Arabic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/update-gs.sh
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-15 14:17:45.000000 glyphsets-0.6.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.730099 glyphsets-0.6.9/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.778099 glyphsets-0.6.9/Lib/glyphsets/
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16554 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/codepoints.py
--rw-r--r--   0 runner    (1001) docker     (127)   587834 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.778099 glyphsets-0.6.9/Lib/glyphsets/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/definitions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.778099 glyphsets-0.6.9/Lib/glyphsets/definitions/nam/
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Arabic_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Arabic_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Latin_Core.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.814099 glyphsets-0.6.9/Lib/glyphsets/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/adlam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ahom_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    20007 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    57487 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/arabic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/armenian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/avestan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/balinese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    22272 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/bamum_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/batak_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/bengali_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/braille_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/buginese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/buhid_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    25715 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/carian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chakma_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   284694 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   298348 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   241902 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/coptic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    46227 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/deseret_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/dogra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/duployan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    41018 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    33746 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/emoji_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    16949 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/georgian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/gothic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/grantha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    13891 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/greek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/hatran_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    91251 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/japanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/javanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kannada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kawi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    21734 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/khmer_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/khojki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    80178 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/korean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    37362 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/latin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/limbu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lisu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lycian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lydian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/makasar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/marchen_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   190939 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/math.nam
--rw-r--r--   0 runner    (1001) docker     (127)    95179 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/math_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/miao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/modi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mro_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/multani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    24495 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/music_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/newa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nko_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    13878 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nushu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ogham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/oriya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/osage_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/rejang_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/runic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sharada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/shavian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/siddham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    35208 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   118220 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/symbols_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/syriac_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/takri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tamil_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   212192 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tangut_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/telugu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/thaana_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/thai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/toto_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/vai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/wancho_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/wgl-latin.enc
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    30939 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/yi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.822099 glyphsets-0.6.9/Lib/glyphsets/slices/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  1087488 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/hongkong-chinese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   893039 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/japanese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   876086 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/korean_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   889189 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/simplified-chinese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   904276 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/traditional-chinese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/test_strings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.826099 glyphsets-0.6.9/Lib/glyphsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23873 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2023-12-15 14:17:58.826099 glyphsets-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2023-12-15 14:17:45.000000 glyphsets-0.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-15 14:17:45.000000 glyphsets-0.6.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.822099 glyphsets-0.6.9/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2023-12-15 14:17:45.000000 glyphsets-0.6.9/scripts/assemble_charactersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2023-12-15 14:17:45.000000 glyphsets-0.6.9/scripts/assemble_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-12-15 14:17:45.000000 glyphsets-0.6.9/scripts/create-glyphset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2023-12-15 14:17:45.000000 glyphsets-0.6.9/scripts/find_language_for_character.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 14:17:58.826099 glyphsets-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-12-15 14:17:45.000000 glyphsets-0.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.826099 glyphsets-0.6.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.826099 glyphsets-0.6.9/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    90712 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/data/MavenPro[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/test_glyphdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/test_glyphsets.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/test_teststrings.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/testcoverage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.253530 glyphsets-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.189530 glyphsets-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.197529 glyphsets-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-03 09:49:24.000000 glyphsets-1.0.0/.github/workflows/publish-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-03 09:49:24.000000 glyphsets-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 09:49:24.000000 glyphsets-1.0.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.197529 glyphsets-1.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 09:49:24.000000 glyphsets-1.0.0/.vscode/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.193529 glyphsets-1.0.0/Archive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.197529 glyphsets-1.0.0/Archive/GF Glyph Sets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.201530 glyphsets-1.0.0/Archive/GF Glyph Sets/Arabic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Arabic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.201530 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    10080 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.193529 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.201530 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/historical_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_italic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs_smallcaps.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.201530 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/historical_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_italic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    18371 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.205530 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.193529 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.205530 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.205530 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/RECOMMENDED.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/TROUBLESHOOTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.205530 glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.205530 glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    75853 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   104148 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/img/locl.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.209529 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.209529 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/plus_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/pro_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/plus_optional-glyphs_case-accents.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/pro_optional-glyphs_case-punctuation.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.209529 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/plus_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/pro_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.213529 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_either_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_either_19.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_either_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.213529 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.213529 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/Glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    43666 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.213529 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/Glyphs/Info/
+-rw-r--r--   0 runner    (1001) docker     (127)    89964 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.213529 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    35092 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/Directory.png
+-rw-r--r--   0 runner    (1001) docker     (127)    98535 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/ListFilters.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84092 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    71431 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/fix-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33541 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/fix-2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45217 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/fix-3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53065 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/list-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-05-03 09:49:24.000000 glyphsets-1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    98308 2024-05-03 09:49:24.000000 glyphsets-1.0.0/GLYPHSETS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 09:49:24.000000 glyphsets-1.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.193529 glyphsets-1.0.0/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.213529 glyphsets-1.0.0/Lib/glyphsets/
+-rw-r--r--   0 runner    (1001) docker     (127)    19424 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 09:49:32.000000 glyphsets-1.0.0/Lib/glyphsets/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.221530 glyphsets-1.0.0/Lib/glyphsets/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Arabic_Core.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Arabic_Plus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Cyrillic_Core.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Cyrillic_Historical.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Cyrillic_Plus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Cyrillic_Pro.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Greek_AncientMusicalSymbols.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Greek_Archaic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Greek_Coptic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Greek_Core.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Greek_Expert.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Greek_Plus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Greek_Pro.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Latin_African.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Latin_Beyond.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Latin_Core.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Latin_Kernel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Latin_Plus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Latin_PriAfrican.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Latin_Vietnamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Phonetics_APA.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Phonetics_DisorderedSpeech.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Phonetics_IPAHistorical.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Phonetics_IPAStandard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_Phonetics_SinoExt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_TransLatin_Arabic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/definitions/GF_TransLatin_Pinyin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.193529 glyphsets-1.0.0/Lib/glyphsets/results/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.225530 glyphsets-1.0.0/Lib/glyphsets/results/nam/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Arabic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Arabic_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Cyrillic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Cyrillic_Historical.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Cyrillic_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Cyrillic_Pro.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    15083 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_AncientMusicalSymbols.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Archaic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Coptic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Expert.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Pro.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    19925 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_African.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_Beyond.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_Kernel.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_PriAfrican.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_Vietnamese.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Phonetics_APA.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Phonetics_DisorderedSpeech.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Phonetics_IPAHistorical.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Phonetics_IPAStandard.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Phonetics_SinoExt.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_TransLatin_Arabic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_TransLatin_Pinyin.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.193529 glyphsets-1.0.0/Lib/glyphsets/results/txt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.229530 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Arabic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Arabic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Cyrillic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Cyrillic_Historical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Cyrillic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Cyrillic_Pro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Expert.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Pro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_African.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_Beyond.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_Kernel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_PriAfrican.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_Vietnamese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Phonetics_APA.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Phonetics_IPAHistorical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Phonetics_IPAStandard.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Phonetics_SinoExt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_TransLatin_Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-03 09:49:24.000000 glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_TransLatin_Pinyin.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.249530 glyphsets-1.0.0/Lib/glyphsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-03 09:49:32.000000 glyphsets-1.0.0/Lib/glyphsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18175 2024-05-03 09:49:32.000000 glyphsets-1.0.0/Lib/glyphsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:49:32.000000 glyphsets-1.0.0/Lib/glyphsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 09:49:32.000000 glyphsets-1.0.0/Lib/glyphsets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:49:32.000000 glyphsets-1.0.0/Lib/glyphsets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 09:49:32.000000 glyphsets-1.0.0/Lib/glyphsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 09:49:32.000000 glyphsets-1.0.0/Lib/glyphsets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-03 09:49:32.253530 glyphsets-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-05-03 09:49:24.000000 glyphsets-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 09:49:24.000000 glyphsets-1.0.0/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.229530 glyphsets-1.0.0/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.193529 glyphsets-1.0.0/data/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.233530 glyphsets-1.0.0/data/definitions/per_glyphset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Arabic_Core.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Cyrillic_Historical.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Cyrillic_Plus.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Cyrillic_Pro.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    20543 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Greek_AncientMusicalSymbols.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Greek_Archaic.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Greek_Coptic.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Greek_Core.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    26340 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Greek_Expert.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Greek_Plus.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Greek_Pro.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Latin_Beyond.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    14356 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Latin_Core.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Latin_Kernel.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    17506 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Latin_Plus.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Latin_PriAfrican.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    14707 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Latin_Vietnamese.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Phonetics_APA.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Phonetics_DisorderedSpeech.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Phonetics_IPAHistorical.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Phonetics_IPAStandard.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_Phonetics_SinoExt.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_TransLatin_Arabic.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    14899 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_glyphset/GF_TransLatin_Pinyin.stub.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.233530 glyphsets-1.0.0/data/definitions/per_language/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/definitions/per_language/ca_Latn.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/empty_font.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.193529 glyphsets-1.0.0/data/results/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.237530 glyphsets-1.0.0/data/results/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Arabic_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Arabic_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Cyrillic_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Cyrillic_Historical.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Cyrillic_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Cyrillic_Pro.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    20559 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Greek_AncientMusicalSymbols.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Greek_Archaic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Greek_Coptic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Greek_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    26497 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Greek_Expert.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    17507 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Greek_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Greek_Pro.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Latin_African.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Latin_Beyond.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    23739 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Latin_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Latin_Kernel.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    17565 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Latin_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Latin_PriAfrican.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    19823 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Latin_Vietnamese.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Phonetics_APA.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Phonetics_DisorderedSpeech.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Phonetics_IPAHistorical.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Phonetics_IPAStandard.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_Phonetics_SinoExt.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_TransLatin_Arabic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    14955 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/glyphs/GF_TransLatin_Pinyin.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.241530 glyphsets-1.0.0/data/results/nam/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Arabic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Arabic_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Cyrillic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Cyrillic_Historical.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Cyrillic_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Cyrillic_Pro.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    15083 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Greek_AncientMusicalSymbols.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Greek_Archaic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Greek_Coptic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Greek_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Greek_Expert.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Greek_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Greek_Pro.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    19925 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Latin_African.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Latin_Beyond.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Latin_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Latin_Kernel.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Latin_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Latin_PriAfrican.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Latin_Vietnamese.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Phonetics_APA.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Phonetics_DisorderedSpeech.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Phonetics_IPAHistorical.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Phonetics_IPAStandard.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_Phonetics_SinoExt.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_TransLatin_Arabic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/nam/GF_TransLatin_Pinyin.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.241530 glyphsets-1.0.0/data/results/plist/
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/plist/CustomFilter_GF_Arabic.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    11821 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/plist/CustomFilter_GF_Cyrillic.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    53788 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/plist/CustomFilter_GF_Greek.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    48017 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/plist/CustomFilter_GF_Latin.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/plist/CustomFilter_GF_Phonetics.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/plist/CustomFilter_GF_TransLatin.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.193529 glyphsets-1.0.0/data/results/txt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.245530 glyphsets-1.0.0/data/results/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Arabic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Arabic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Cyrillic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Cyrillic_Historical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Cyrillic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Cyrillic_Pro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Greek_Archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Greek_Coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Greek_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Greek_Expert.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Greek_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Greek_Pro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Latin_African.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Latin_Beyond.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Latin_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Latin_Kernel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Latin_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Latin_PriAfrican.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Latin_Vietnamese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Phonetics_APA.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Phonetics_IPAHistorical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Phonetics_IPAStandard.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_Phonetics_SinoExt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_TransLatin_Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/nice-names/GF_TransLatin_Pinyin.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.249530 glyphsets-1.0.0/data/results/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Arabic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Arabic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Cyrillic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Cyrillic_Historical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Cyrillic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Cyrillic_Pro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_Archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_Coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_Expert.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_Pro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_African.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_Beyond.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_Kernel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_PriAfrican.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_Vietnamese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Phonetics_APA.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Phonetics_IPAHistorical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Phonetics_IPAStandard.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_Phonetics_SinoExt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_TransLatin_Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-03 09:49:24.000000 glyphsets-1.0.0/data/results/txt/prod-names/GF_TransLatin_Pinyin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 09:49:24.000000 glyphsets-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-03 09:49:24.000000 glyphsets-1.0.0/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.249530 glyphsets-1.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-05-03 09:49:24.000000 glyphsets-1.0.0/scripts/assemble_charactersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-03 09:49:24.000000 glyphsets-1.0.0/scripts/assemble_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-03 09:49:24.000000 glyphsets-1.0.0/scripts/assemble_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-03 09:49:24.000000 glyphsets-1.0.0/scripts/find_language_for_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:49:32.253530 glyphsets-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-03 09:49:24.000000 glyphsets-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.249530 glyphsets-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:49:32.249530 glyphsets-1.0.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    90712 2024-05-03 09:49:24.000000 glyphsets-1.0.0/tests/data/MavenPro[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-03 09:49:24.000000 glyphsets-1.0.0/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-03 09:49:24.000000 glyphsets-1.0.0/tests/test_glyphsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 09:49:24.000000 glyphsets-1.0.0/tox.ini
```

### Comparing `glyphsets-0.6.9/.github/workflows/publish-release.yml` & `glyphsets-1.0.0/.github/workflows/publish-release.yml`

 * *Files 25% similar despite different names*

```diff
@@ -3,31 +3,30 @@
     tags:
       - "v*" # Push events to matching `v*` version srings. e.g. v1.0, v20.15.10
 
 name: Create and Publish Release
 
 jobs:
   build:
-    name: Create and Publish Release
+    name: Build distribution
     runs-on: ubuntu-latest
-
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
         with:
           submodules: recursive
           fetch-depth: 0
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v5
         with:
           python-version: '3.x'
 
       - name: Install release dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install --upgrade setuptools wheel twine
+          pip install --upgrade setuptools wheel build
 
       - name: Get release notes
         id: release_notes
         run: |
           # By default, GH Actions checkout will only fetch a single commit.
           # For us to extract the release notes, we need to fetch the tags
           # and tag annotations as well.
@@ -44,14 +43,38 @@
         with:
           tag_name: ${{ github.ref }}
           release_name: ${{ github.ref }}
           body_path: "${{ runner.temp }}/CHANGELOG.md"
           draft: false
           prerelease: false
 
-      - name: Build and publish to PyPI
-        env:
-          TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
-          TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-        run: |
-          python setup.py sdist bdist_wheel
-          twine upload dist/glyphsets*
+      - name: Build a binary wheel and a source tarball
+        run: python3 -m build
+      - name: Store the distribution packages
+        uses: actions/upload-artifact@v4
+        with:
+          name: python-package-distributions
+          path: dist/
+
+  publish-to-pypi:
+    name: >-
+      Publish Python 🐍 distribution 📦 to PyPI
+    if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
+    needs:
+      - build
+    runs-on: ubuntu-latest
+    environment:
+      name: pypi
+      url: https://pypi.org/p/glyphsets
+    permissions:
+      id-token: write  # IMPORTANT: mandatory for trusted publishing
+    steps:
+      - name: Download all the dists
+        uses: actions/download-artifact@v4
+        with:
+          name: python-package-distributions
+          path: dist/
+      - name: Publish distribution 📦 to PyPI
+        uses: pypa/gh-action-pypi-publish@v1.8.14
+        with:
+          # repository-url: https://test.pypi.org/legacy/ # for testing purposes
+          verify-metadata: false # twine previously didn't verify metadata when uploading
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/README.md` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Arabic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-core.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/README.md` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/README.md` & `glyphsets-1.0.0/Archive/GF Glyph Sets/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/RECOMMENDED.md` & `glyphsets-1.0.0/Archive/GF Glyph Sets/RECOMMENDED.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/TROUBLESHOOTING.md` & `glyphsets-1.0.0/Archive/GF Glyph Sets/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/README.md` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/locl.png` & `glyphsets-1.0.0/Archive/GF Glyph Sets/Vietnamese/img/locl.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt` & `glyphsets-1.0.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/README.md` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/Directory.png` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/Directory.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/ListFilters.png` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/ListFilters.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-1.png` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/fix-1.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-2.png` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/fix-2.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-3.png` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/fix-3.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/list-filter.png` & `glyphsets-1.0.0/Archive/GF Glyph Sets/tutorials/img/list-filter.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs` & `glyphsets-1.0.0/data/results/glyphs/GF_Latin_PriAfrican.glyphs`

 * *Files 26% similar despite different names*

```diff
@@ -1,600 +1,789 @@
 {
-.appVersion = "895";
-customParameters = (
+.appVersion = "3151";
+.formatVersion = 3;
+axes = (
 {
-name = Axes;
-value = (
-);
+name = Weight;
+tag = wght;
+},
+{
+name = Width;
+tag = wdth;
 }
 );
-familyName = GF_Arabic_Core;
+date = "2023-12-13 14:28:10 +0000";
+familyName = GF_Latin_PriAfrican;
 fontMaster = (
+{
+axesValues = (
+100,
+100
+);
+id = m01;
+metricValues = (
+{
+over = 16;
+pos = 800;
+},
+{
+over = 16;
+pos = 700;
+},
+{
+over = 16;
+pos = 500;
+},
+{
+over = -16;
+},
+{
+over = -16;
+pos = -200;
+},
+{
+over = -16;
+}
+);
+name = Regular;
+}
 );
 glyphs = (
 {
 glyphname = percent;
-unicode = 0025;
+unicode = 37;
+},
+{
+glyphname = ampersand;
+unicode = 38;
 },
 {
 glyphname = plus;
-unicode = 002B;
+unicode = 43;
 },
 {
-glyphname = less;
-unicode = 003C;
+glyphname = at;
+unicode = 64;
 },
 {
-glyphname = equal;
-unicode = 003D;
+glyphname = exclam;
+unicode = 33;
 },
 {
-glyphname = greater;
-unicode = 003E;
+glyphname = quotedbl;
+unicode = 34;
 },
 {
-glyphname = bar;
-unicode = 007C;
+glyphname = numbersign;
+unicode = 35;
 },
 {
-glyphname = multiply;
-unicode = 00D7;
+glyphname = quotesingle;
+unicode = 39;
 },
 {
-glyphname = divide;
-unicode = 00F7;
+glyphname = parenleft;
+unicode = 40;
 },
 {
-glyphname = "perthousand-ar";
-unicode = 0609;
+glyphname = parenright;
+unicode = 41;
 },
 {
-glyphname = "mark-ar";
-unicode = 061C;
+glyphname = asterisk;
+unicode = 42;
 },
 {
-glyphname = "percent-ar";
-unicode = 066A;
+glyphname = comma;
+unicode = 44;
 },
 {
-glyphname = minus;
-unicode = 2212;
+glyphname = hyphen;
+unicode = 45;
 },
 {
-glyphname = space;
-unicode = 0020;
+glyphname = period;
+unicode = 46;
 },
 {
-glyphname = nbspace;
-unicode = 00A0;
+glyphname = slash;
+unicode = 47;
 },
 {
-glyphname = lefttorightmark;
-unicode = 200E;
+glyphname = colon;
+unicode = 58;
 },
 {
-glyphname = exclam;
-unicode = 0021;
+glyphname = semicolon;
+unicode = 59;
 },
 {
-glyphname = quotedbl;
-unicode = 0022;
+glyphname = question;
+unicode = 63;
 },
 {
-glyphname = numbersign;
-unicode = 0023;
+glyphname = bracketleft;
+unicode = 91;
 },
 {
-glyphname = quotesingle;
-unicode = 0027;
+glyphname = bracketright;
+unicode = 93;
 },
 {
-glyphname = parenleft;
-unicode = 0028;
+glyphname = endash;
+unicode = 8211;
 },
 {
-glyphname = parenright;
-unicode = 0029;
+glyphname = emdash;
+unicode = 8212;
 },
 {
-glyphname = asterisk;
-unicode = 002A;
+glyphname = quoteleft;
+unicode = 8216;
 },
 {
-glyphname = comma;
-unicode = 002C;
+glyphname = quoteright;
+unicode = 8217;
 },
 {
-glyphname = hyphen;
-unicode = 002D;
+glyphname = quotedblleft;
+unicode = 8220;
 },
 {
-glyphname = period;
-unicode = 002E;
+glyphname = quotedblright;
+unicode = 8221;
 },
 {
-glyphname = slash;
-unicode = 002F;
+glyphname = ellipsis;
+unicode = 8230;
 },
 {
-glyphname = colon;
-unicode = 003A;
+glyphname = zero;
+unicode = 48;
 },
 {
-glyphname = bracketleft;
-unicode = 005B;
+glyphname = one;
+unicode = 49;
 },
 {
-glyphname = backslash;
-unicode = 005C;
+glyphname = two;
+unicode = 50;
 },
 {
-glyphname = bracketright;
-unicode = 005D;
+glyphname = three;
+unicode = 51;
 },
 {
-glyphname = braceleft;
-unicode = 007B;
+glyphname = four;
+unicode = 52;
 },
 {
-glyphname = braceright;
-unicode = 007D;
+glyphname = five;
+unicode = 53;
 },
 {
-glyphname = guillemetleft;
-unicode = 00AB;
+glyphname = six;
+unicode = 54;
 },
 {
-glyphname = guillemetright;
-unicode = 00BB;
+glyphname = seven;
+unicode = 55;
 },
 {
-glyphname = "comma-ar";
-unicode = 060C;
+glyphname = eight;
+unicode = 56;
 },
 {
-glyphname = "dateseparator-ar";
-unicode = 060D;
+glyphname = nine;
+unicode = 57;
 },
 {
-glyphname = "semicolon-ar";
-unicode = 061B;
+glyphname = dotbelowcomb;
+unicode = 803;
 },
 {
-glyphname = "question-ar";
-unicode = 061F;
+glyphname = apostrophemod;
+unicode = 700;
 },
 {
-glyphname = "asterisk-ar";
-unicode = 066D;
+glyphname = gravecomb;
+unicode = 768;
 },
 {
-glyphname = "fullstop-ar";
-unicode = 06D4;
+glyphname = acutecomb;
+unicode = 769;
 },
 {
-glyphname = endash;
-unicode = 2013;
+glyphname = circumflexcomb;
+unicode = 770;
 },
 {
-glyphname = emdash;
-unicode = 2014;
+glyphname = tildecomb;
+unicode = 771;
 },
 {
-glyphname = quoteleft;
-unicode = 2018;
+glyphname = macroncomb;
+unicode = 772;
 },
 {
-glyphname = quoteright;
-unicode = 2019;
+glyphname = brevecomb;
+unicode = 774;
 },
 {
-glyphname = quotedblleft;
-unicode = 201C;
+glyphname = dotaccentcomb;
+unicode = 775;
 },
 {
-glyphname = quotedblright;
-unicode = 201D;
+glyphname = dieresiscomb;
+unicode = 776;
 },
 {
-glyphname = ellipsis;
-unicode = 2026;
+glyphname = ringcomb;
+unicode = 778;
 },
 {
-glyphname = guilsinglleft;
-unicode = 2039;
+glyphname = cedillacomb;
+unicode = 807;
 },
 {
-glyphname = guilsinglright;
-unicode = 203A;
+glyphname = Eng;
+unicode = 330;
 },
 {
-glyphname = "parenleft-ar";
-unicode = FD3E;
+glyphname = eng;
+unicode = 331;
 },
 {
-glyphname = "parenright-ar";
-unicode = FD3F;
+glyphname = Bhook;
+unicode = 385;
 },
 {
-glyphname = zero;
-unicode = 0030;
+glyphname = Oopen;
+unicode = 390;
 },
 {
-glyphname = one;
-unicode = 0031;
+glyphname = Dhook;
+unicode = 394;
 },
 {
-glyphname = two;
-unicode = 0032;
+glyphname = Eopen;
+unicode = 400;
 },
 {
-glyphname = three;
-unicode = 0033;
+glyphname = Khook;
+unicode = 408;
 },
 {
-glyphname = four;
-unicode = 0034;
+glyphname = khook;
+unicode = 409;
 },
 {
-glyphname = five;
-unicode = 0035;
+glyphname = Nhookleft;
+unicode = 413;
 },
 {
-glyphname = six;
-unicode = 0036;
+glyphname = Yhook;
+unicode = 435;
 },
 {
-glyphname = seven;
-unicode = 0037;
+glyphname = yhook;
+unicode = 436;
 },
 {
-glyphname = eight;
-unicode = 0038;
+glyphname = Ngrave;
+unicode = 504;
 },
 {
-glyphname = nine;
-unicode = 0039;
+glyphname = ngrave;
+unicode = 505;
+},
+{
+glyphname = bhook;
+unicode = 595;
+},
+{
+glyphname = oopen;
+unicode = 596;
+},
+{
+glyphname = dhook;
+unicode = 599;
+},
+{
+glyphname = eopen;
+unicode = 603;
+},
+{
+glyphname = nhookleft;
+unicode = 626;
+},
+{
+glyphname = Macute;
+unicode = 7742;
+},
+{
+glyphname = macute;
+unicode = 7743;
+},
+{
+glyphname = Ndotaccent;
+unicode = 7748;
+},
+{
+glyphname = ndotaccent;
+unicode = 7749;
+},
+{
+glyphname = Sdotbelow;
+unicode = 7778;
+},
+{
+glyphname = sdotbelow;
+unicode = 7779;
+},
+{
+glyphname = Edotbelow;
+unicode = 7864;
+},
+{
+glyphname = edotbelow;
+unicode = 7865;
+},
+{
+glyphname = Idotbelow;
+unicode = 7882;
+},
+{
+glyphname = idotbelow;
+unicode = 7883;
+},
+{
+glyphname = Odotbelow;
+unicode = 7884;
 },
 {
-glyphname = "zero-ar";
-unicode = 0660;
+glyphname = odotbelow;
+unicode = 7885;
 },
 {
-glyphname = "one-ar";
-unicode = 0661;
+glyphname = Udotbelow;
+unicode = 7908;
 },
 {
-glyphname = "two-ar";
-unicode = 0662;
+glyphname = udotbelow;
+unicode = 7909;
 },
 {
-glyphname = "three-ar";
-unicode = 0663;
+glyphname = A;
+unicode = 65;
 },
 {
-glyphname = "four-ar";
-unicode = 0664;
+glyphname = B;
+unicode = 66;
 },
 {
-glyphname = "five-ar";
-unicode = 0665;
+glyphname = C;
+unicode = 67;
 },
 {
-glyphname = "six-ar";
-unicode = 0666;
+glyphname = D;
+unicode = 68;
 },
 {
-glyphname = "seven-ar";
-unicode = 0667;
+glyphname = E;
+unicode = 69;
 },
 {
-glyphname = "eight-ar";
-unicode = 0668;
+glyphname = F;
+unicode = 70;
 },
 {
-glyphname = "nine-ar";
-unicode = 0669;
+glyphname = G;
+unicode = 71;
 },
 {
-glyphname = "decimalseparator-ar";
-unicode = 066B;
+glyphname = H;
+unicode = 72;
 },
 {
-glyphname = "thousandseparator-ar";
-unicode = 066C;
+glyphname = I;
+unicode = 73;
 },
 {
-glyphname = "zero-persian";
-unicode = 06F0;
+glyphname = J;
+unicode = 74;
 },
 {
-glyphname = "one-persian";
-unicode = 06F1;
+glyphname = K;
+unicode = 75;
 },
 {
-glyphname = "two-persian";
-unicode = 06F2;
+glyphname = L;
+unicode = 76;
 },
 {
-glyphname = "three-persian";
-unicode = 06F3;
+glyphname = M;
+unicode = 77;
 },
 {
-glyphname = "four-persian";
-unicode = 06F4;
+glyphname = N;
+unicode = 78;
 },
 {
-glyphname = "five-persian";
-unicode = 06F5;
+glyphname = O;
+unicode = 79;
 },
 {
-glyphname = "six-persian";
-unicode = 06F6;
+glyphname = P;
+unicode = 80;
 },
 {
-glyphname = "seven-persian";
-unicode = 06F7;
+glyphname = Q;
+unicode = 81;
 },
 {
-glyphname = "eight-persian";
-unicode = 06F8;
+glyphname = R;
+unicode = 82;
 },
 {
-glyphname = "nine-persian";
-unicode = 06F9;
+glyphname = S;
+unicode = 83;
 },
 {
-glyphname = "fathatan-ar";
-unicode = 064B;
+glyphname = T;
+unicode = 84;
 },
 {
-glyphname = "dammatan-ar";
-unicode = 064C;
+glyphname = U;
+unicode = 85;
 },
 {
-glyphname = "kasratan-ar";
-unicode = 064D;
+glyphname = V;
+unicode = 86;
 },
 {
-glyphname = "fatha-ar";
-unicode = 064E;
+glyphname = W;
+unicode = 87;
 },
 {
-glyphname = "damma-ar";
-unicode = 064F;
+glyphname = X;
+unicode = 88;
 },
 {
-glyphname = "kasra-ar";
-unicode = 0650;
+glyphname = Y;
+unicode = 89;
 },
 {
-glyphname = "shadda-ar";
-unicode = 0651;
+glyphname = Z;
+unicode = 90;
 },
 {
-glyphname = "sukun-ar";
-unicode = 0652;
+glyphname = a;
+unicode = 97;
 },
 {
-glyphname = "madda-ar";
-unicode = 0653;
+glyphname = b;
+unicode = 98;
 },
 {
-glyphname = "hamzaabove-ar";
-unicode = 0654;
+glyphname = c;
+unicode = 99;
 },
 {
-glyphname = "hamzabelow-ar";
-unicode = 0655;
+glyphname = d;
+unicode = 100;
 },
 {
-glyphname = "alefabove-ar";
-unicode = 0670;
+glyphname = e;
+unicode = 101;
 },
 {
-glyphname = "hamza-ar";
-unicode = 0621;
+glyphname = f;
+unicode = 102;
 },
 {
-glyphname = "alefMadda-ar";
-unicode = 0622;
+glyphname = g;
+unicode = 103;
 },
 {
-glyphname = "alefHamzaabove-ar";
-unicode = 0623;
+glyphname = h;
+unicode = 104;
 },
 {
-glyphname = "wawHamzaabove-ar";
-unicode = 0624;
+glyphname = i;
+unicode = 105;
 },
 {
-glyphname = "alefHamzabelow-ar";
-unicode = 0625;
+glyphname = j;
+unicode = 106;
 },
 {
-glyphname = "yehHamzaabove-ar";
-unicode = 0626;
+glyphname = k;
+unicode = 107;
 },
 {
-glyphname = "alef-ar";
-unicode = 0627;
+glyphname = l;
+unicode = 108;
 },
 {
-glyphname = "beh-ar";
-unicode = 0628;
+glyphname = m;
+unicode = 109;
 },
 {
-glyphname = "tehMarbuta-ar";
-unicode = 0629;
+glyphname = n;
+unicode = 110;
 },
 {
-glyphname = "teh-ar";
-unicode = 062A;
+glyphname = o;
+unicode = 111;
 },
 {
-glyphname = "theh-ar";
-unicode = 062B;
+glyphname = p;
+unicode = 112;
 },
 {
-glyphname = "jeem-ar";
-unicode = 062C;
+glyphname = q;
+unicode = 113;
 },
 {
-glyphname = "hah-ar";
-unicode = 062D;
+glyphname = r;
+unicode = 114;
 },
 {
-glyphname = "khah-ar";
-unicode = 062E;
+glyphname = s;
+unicode = 115;
 },
 {
-glyphname = "dal-ar";
-unicode = 062F;
+glyphname = t;
+unicode = 116;
 },
 {
-glyphname = "thal-ar";
-unicode = 0630;
+glyphname = u;
+unicode = 117;
 },
 {
-glyphname = "reh-ar";
-unicode = 0631;
+glyphname = v;
+unicode = 118;
 },
 {
-glyphname = "zain-ar";
-unicode = 0632;
+glyphname = w;
+unicode = 119;
 },
 {
-glyphname = "seen-ar";
-unicode = 0633;
+glyphname = x;
+unicode = 120;
 },
 {
-glyphname = "sheen-ar";
-unicode = 0634;
+glyphname = y;
+unicode = 121;
 },
 {
-glyphname = "sad-ar";
-unicode = 0635;
+glyphname = z;
+unicode = 122;
 },
 {
-glyphname = "dad-ar";
-unicode = 0636;
+glyphname = Agrave;
+unicode = 192;
 },
 {
-glyphname = "tah-ar";
-unicode = 0637;
+glyphname = Aacute;
+unicode = 193;
 },
 {
-glyphname = "zah-ar";
-unicode = 0638;
+glyphname = Adieresis;
+unicode = 196;
 },
 {
-glyphname = "ain-ar";
-unicode = 0639;
+glyphname = Egrave;
+unicode = 200;
 },
 {
-glyphname = "ghain-ar";
-unicode = 063A;
+glyphname = Eacute;
+unicode = 201;
 },
 {
-glyphname = "kashida-ar";
-unicode = 0640;
+glyphname = Ecircumflex;
+unicode = 202;
 },
 {
-glyphname = "feh-ar";
-unicode = 0641;
+glyphname = Edieresis;
+unicode = 203;
 },
 {
-glyphname = "qaf-ar";
-unicode = 0642;
+glyphname = Igrave;
+unicode = 204;
 },
 {
-glyphname = "kaf-ar";
-unicode = 0643;
+glyphname = Iacute;
+unicode = 205;
 },
 {
-glyphname = "lam-ar";
-unicode = 0644;
+glyphname = Icircumflex;
+unicode = 206;
 },
 {
-glyphname = "meem-ar";
-unicode = 0645;
+glyphname = Idieresis;
+unicode = 207;
 },
 {
-glyphname = "noon-ar";
-unicode = 0646;
+glyphname = Ntilde;
+unicode = 209;
 },
 {
-glyphname = "heh-ar";
-unicode = 0647;
+glyphname = Ograve;
+unicode = 210;
 },
 {
-glyphname = "waw-ar";
-unicode = 0648;
+glyphname = Oacute;
+unicode = 211;
 },
 {
-glyphname = "alefMaksura-ar";
-unicode = 0649;
+glyphname = Ocircumflex;
+unicode = 212;
 },
 {
-glyphname = "yeh-ar";
-unicode = 064A;
+glyphname = Odieresis;
+unicode = 214;
 },
 {
-glyphname = "tteh-ar";
-unicode = 0679;
+glyphname = Ugrave;
+unicode = 217;
 },
 {
-glyphname = "peh-ar";
-unicode = 067E;
+glyphname = Uacute;
+unicode = 218;
 },
 {
-glyphname = "tcheh-ar";
-unicode = 0686;
+glyphname = Ucircumflex;
+unicode = 219;
 },
 {
-glyphname = "ddal-ar";
-unicode = 0688;
+glyphname = Udieresis;
+unicode = 220;
 },
 {
-glyphname = "rreh-ar";
-unicode = 0691;
+glyphname = Yacute;
+unicode = 221;
 },
 {
-glyphname = "jeh-ar";
-unicode = 0698;
+glyphname = agrave;
+unicode = 224;
 },
 {
-glyphname = "keheh-ar";
-unicode = 06A9;
+glyphname = aacute;
+unicode = 225;
 },
 {
-glyphname = "gaf-ar";
-unicode = 06AF;
+glyphname = adieresis;
+unicode = 228;
 },
 {
-glyphname = "hehDoachashmee-ar";
-unicode = 06BE;
+glyphname = egrave;
+unicode = 232;
 },
 {
-glyphname = "hehgoal-ar";
-unicode = 06C1;
+glyphname = eacute;
+unicode = 233;
 },
 {
-glyphname = "yeh-farsi";
-unicode = 06CC;
+glyphname = ecircumflex;
+unicode = 234;
 },
 {
-glyphname = "yehbarree-ar";
-unicode = 06D2;
+glyphname = edieresis;
+unicode = 235;
 },
 {
-glyphname = "kehehThreedotsabove-ar";
-unicode = 0763;
+glyphname = igrave;
+unicode = 236;
+},
+{
+glyphname = iacute;
+unicode = 237;
+},
+{
+glyphname = icircumflex;
+unicode = 238;
+},
+{
+glyphname = idieresis;
+unicode = 239;
+},
+{
+glyphname = ntilde;
+unicode = 241;
+},
+{
+glyphname = ograve;
+unicode = 242;
+},
+{
+glyphname = oacute;
+unicode = 243;
+},
+{
+glyphname = ocircumflex;
+unicode = 244;
+},
+{
+glyphname = odieresis;
+unicode = 246;
+},
+{
+glyphname = ugrave;
+unicode = 249;
+},
+{
+glyphname = uacute;
+unicode = 250;
+},
+{
+glyphname = ucircumflex;
+unicode = 251;
+},
+{
+glyphname = udieresis;
+unicode = 252;
+},
+{
+glyphname = yacute;
+unicode = 253;
+},
+{
+glyphname = Nacute;
+unicode = 323;
+},
+{
+glyphname = nacute;
+unicode = 324;
 }
 );
 instances = (
 );
+kerningLTR = {
+};
+metrics = (
+{
+type = ascender;
+},
+{
+type = "cap height";
+},
+{
+type = "x-height";
+},
+{
+type = baseline;
+},
+{
+type = descender;
+},
+{
+type = "italic angle";
+}
+);
+stems = (
+);
 unitsPerEm = 1000;
 versionMajor = 1;
 versionMinor = 0;
 }
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs` & `glyphsets-1.0.0/data/results/glyphs/GF_Cyrillic_Core.glyphs`

 * *Files 16% similar despite different names*

```diff
@@ -1,536 +1,621 @@
 {
-.appVersion = "895";
-customParameters = (
+.appVersion = "3151";
+.formatVersion = 3;
+axes = (
 {
-name = Axes;
-value = (
-);
+name = Weight;
+tag = wght;
+},
+{
+name = Width;
+tag = wdth;
 }
 );
-familyName = GF_Arabic_Plus;
+date = "2023-12-13 14:28:10 +0000";
+familyName = GF_Cyrillic_Core;
 fontMaster = (
+{
+axesValues = (
+100,
+100
 );
-glyphs = (
+id = m01;
+metricValues = (
 {
-glyphname = percent;
-unicode = 0025;
+over = 16;
+pos = 800;
 },
 {
-glyphname = plus;
-unicode = 002B;
+over = 16;
+pos = 700;
 },
 {
-glyphname = "perthousand-ar";
-unicode = 0609;
+over = 16;
+pos = 500;
 },
 {
-glyphname = "percent-ar";
-unicode = 066A;
+over = -16;
 },
 {
-glyphname = "sindhipostpositionmen-ar";
-unicode = 06FE;
+over = -16;
+pos = -200;
 },
 {
-glyphname = minus;
-unicode = 2212;
+over = -16;
+}
+);
+name = Regular;
+}
+);
+glyphs = (
+{
+glyphname = percent;
+unicode = 37;
 },
 {
-glyphname = lefttorightmark;
-unicode = 200E;
+glyphname = ampersand;
+unicode = 38;
 },
 {
-glyphname = righttoleftmark;
-unicode = 200F;
+glyphname = plus;
+unicode = 43;
+},
+{
+glyphname = at;
+unicode = 64;
+},
+{
+glyphname = numero;
+unicode = 8470;
 },
 {
 glyphname = exclam;
-unicode = 0021;
+unicode = 33;
+},
+{
+glyphname = quotedbl;
+unicode = 34;
+},
+{
+glyphname = numbersign;
+unicode = 35;
 },
 {
 glyphname = quotesingle;
-unicode = 0027;
+unicode = 39;
 },
 {
 glyphname = parenleft;
-unicode = 0028;
+unicode = 40;
 },
 {
 glyphname = parenright;
-unicode = 0029;
+unicode = 41;
+},
+{
+glyphname = asterisk;
+unicode = 42;
 },
 {
 glyphname = comma;
-unicode = 002C;
+unicode = 44;
 },
 {
 glyphname = hyphen;
-unicode = 002D;
+unicode = 45;
 },
 {
 glyphname = period;
-unicode = 002E;
+unicode = 46;
 },
 {
 glyphname = slash;
-unicode = 002F;
+unicode = 47;
 },
 {
 glyphname = colon;
-unicode = 003A;
+unicode = 58;
 },
 {
 glyphname = semicolon;
-unicode = 003B;
+unicode = 59;
+},
+{
+glyphname = question;
+unicode = 63;
 },
 {
 glyphname = bracketleft;
-unicode = 005B;
+unicode = 91;
+},
+{
+glyphname = backslash;
+unicode = 92;
 },
 {
 glyphname = bracketright;
-unicode = 005D;
+unicode = 93;
+},
+{
+glyphname = guillemetleft;
+unicode = 171;
 },
 {
-glyphname = "comma-ar";
-unicode = 060C;
+glyphname = guillemetright;
+unicode = 187;
 },
 {
-glyphname = "fullstop-ar";
-unicode = 06D4;
+glyphname = endash;
+unicode = 8211;
 },
 {
-glyphname = "sindhiampersand-ar";
-unicode = 06FD;
+glyphname = emdash;
+unicode = 8212;
 },
 {
 glyphname = quoteleft;
-unicode = 2018;
+unicode = 8216;
+},
+{
+glyphname = quoteright;
+unicode = 8217;
+},
+{
+glyphname = quotesinglbase;
+unicode = 8218;
+},
+{
+glyphname = quotedblleft;
+unicode = 8220;
+},
+{
+glyphname = quotedblbase;
+unicode = 8222;
+},
+{
+glyphname = ellipsis;
+unicode = 8230;
 },
 {
 glyphname = zero;
-unicode = 0030;
+unicode = 48;
 },
 {
 glyphname = one;
-unicode = 0031;
+unicode = 49;
 },
 {
 glyphname = two;
-unicode = 0032;
+unicode = 50;
 },
 {
 glyphname = three;
-unicode = 0033;
+unicode = 51;
 },
 {
 glyphname = four;
-unicode = 0034;
+unicode = 52;
 },
 {
 glyphname = five;
-unicode = 0035;
+unicode = 53;
 },
 {
 glyphname = six;
-unicode = 0036;
+unicode = 54;
 },
 {
 glyphname = seven;
-unicode = 0037;
+unicode = 55;
 },
 {
 glyphname = eight;
-unicode = 0038;
+unicode = 56;
 },
 {
 glyphname = nine;
-unicode = 0039;
+unicode = 57;
 },
 {
-glyphname = "zero-ar";
-unicode = 0660;
+glyphname = apostrophemod;
+unicode = 700;
 },
 {
-glyphname = "one-ar";
-unicode = 0661;
+glyphname = gravecomb;
+unicode = 768;
 },
 {
-glyphname = "two-ar";
-unicode = 0662;
+glyphname = acutecomb;
+unicode = 769;
 },
 {
-glyphname = "three-ar";
-unicode = 0663;
+glyphname = brevecomb;
+unicode = 774;
 },
 {
-glyphname = "four-ar";
-unicode = 0664;
+glyphname = dieresiscomb;
+unicode = 776;
 },
 {
-glyphname = "five-ar";
-unicode = 0665;
+glyphname = "Io-cy";
+unicode = 1025;
 },
 {
-glyphname = "six-ar";
-unicode = 0666;
+glyphname = "Dje-cy";
+unicode = 1026;
 },
 {
-glyphname = "seven-ar";
-unicode = 0667;
+glyphname = "E-cy";
+unicode = 1028;
 },
 {
-glyphname = "eight-ar";
-unicode = 0668;
+glyphname = "I-cy";
+unicode = 1030;
 },
 {
-glyphname = "nine-ar";
-unicode = 0669;
+glyphname = "Yi-cy";
+unicode = 1031;
 },
 {
-glyphname = "decimalseparator-ar";
-unicode = 066B;
+glyphname = "Je-cy";
+unicode = 1032;
 },
 {
-glyphname = "thousandseparator-ar";
-unicode = 066C;
+glyphname = "Lje-cy";
+unicode = 1033;
 },
 {
-glyphname = "zero-persian";
-unicode = 06F0;
+glyphname = "Nje-cy";
+unicode = 1034;
 },
 {
-glyphname = "one-persian";
-unicode = 06F1;
+glyphname = "Tshe-cy";
+unicode = 1035;
 },
 {
-glyphname = "two-persian";
-unicode = 06F2;
+glyphname = "Ushort-cy";
+unicode = 1038;
 },
 {
-glyphname = "three-persian";
-unicode = 06F3;
+glyphname = "Dzhe-cy";
+unicode = 1039;
 },
 {
-glyphname = "four-persian";
-unicode = 06F4;
+glyphname = "A-cy";
+unicode = 1040;
 },
 {
-glyphname = "five-persian";
-unicode = 06F5;
+glyphname = "Be-cy";
+unicode = 1041;
 },
 {
-glyphname = "six-persian";
-unicode = 06F6;
+glyphname = "Ve-cy";
+unicode = 1042;
 },
 {
-glyphname = "seven-persian";
-unicode = 06F7;
+glyphname = "Ge-cy";
+unicode = 1043;
 },
 {
-glyphname = "eight-persian";
-unicode = 06F8;
+glyphname = "De-cy";
+unicode = 1044;
 },
 {
-glyphname = "nine-persian";
-unicode = 06F9;
+glyphname = "Ie-cy";
+unicode = 1045;
 },
 {
-glyphname = "fathatan-ar";
-unicode = 064B;
+glyphname = "Zhe-cy";
+unicode = 1046;
 },
 {
-glyphname = "dammatan-ar";
-unicode = 064C;
+glyphname = "Ze-cy";
+unicode = 1047;
 },
 {
-glyphname = "kasratan-ar";
-unicode = 064D;
+glyphname = "Ii-cy";
+unicode = 1048;
 },
 {
-glyphname = "fatha-ar";
-unicode = 064E;
+glyphname = "Iishort-cy";
+unicode = 1049;
 },
 {
-glyphname = "damma-ar";
-unicode = 064F;
+glyphname = "Ka-cy";
+unicode = 1050;
 },
 {
-glyphname = "kasra-ar";
-unicode = 0650;
+glyphname = "El-cy";
+unicode = 1051;
 },
 {
-glyphname = "shadda-ar";
-unicode = 0651;
+glyphname = "Em-cy";
+unicode = 1052;
 },
 {
-glyphname = "sukun-ar";
-unicode = 0652;
+glyphname = "En-cy";
+unicode = 1053;
 },
 {
-glyphname = "hamzaabove-ar";
-unicode = 0654;
+glyphname = "O-cy";
+unicode = 1054;
 },
 {
-glyphname = "alefabove-ar";
-unicode = 0670;
+glyphname = "Pe-cy";
+unicode = 1055;
 },
 {
-glyphname = "hamza-ar";
-unicode = 0621;
+glyphname = "Er-cy";
+unicode = 1056;
 },
 {
-glyphname = "alefMadda-ar";
-unicode = 0622;
+glyphname = "Es-cy";
+unicode = 1057;
 },
 {
-glyphname = "alefHamzaabove-ar";
-unicode = 0623;
+glyphname = "Te-cy";
+unicode = 1058;
 },
 {
-glyphname = "wawHamzaabove-ar";
-unicode = 0624;
+glyphname = "U-cy";
+unicode = 1059;
 },
 {
-glyphname = "yehHamzaabove-ar";
-unicode = 0626;
+glyphname = "Ef-cy";
+unicode = 1060;
 },
 {
-glyphname = "alef-ar";
-unicode = 0627;
+glyphname = "Ha-cy";
+unicode = 1061;
 },
 {
-glyphname = "beh-ar";
-unicode = 0628;
+glyphname = "Tse-cy";
+unicode = 1062;
 },
 {
-glyphname = "tehMarbuta-ar";
-unicode = 0629;
+glyphname = "Che-cy";
+unicode = 1063;
 },
 {
-glyphname = "teh-ar";
-unicode = 062A;
+glyphname = "Sha-cy";
+unicode = 1064;
 },
 {
-glyphname = "theh-ar";
-unicode = 062B;
+glyphname = "Shcha-cy";
+unicode = 1065;
 },
 {
-glyphname = "jeem-ar";
-unicode = 062C;
+glyphname = "Hardsign-cy";
+unicode = 1066;
 },
 {
-glyphname = "hah-ar";
-unicode = 062D;
+glyphname = "Yeru-cy";
+unicode = 1067;
 },
 {
-glyphname = "khah-ar";
-unicode = 062E;
+glyphname = "Softsign-cy";
+unicode = 1068;
 },
 {
-glyphname = "dal-ar";
-unicode = 062F;
+glyphname = "Ereversed-cy";
+unicode = 1069;
 },
 {
-glyphname = "thal-ar";
-unicode = 0630;
+glyphname = "Yu-cy";
+unicode = 1070;
 },
 {
-glyphname = "reh-ar";
-unicode = 0631;
+glyphname = "Ya-cy";
+unicode = 1071;
 },
 {
-glyphname = "zain-ar";
-unicode = 0632;
+glyphname = "a-cy";
+unicode = 1072;
 },
 {
-glyphname = "seen-ar";
-unicode = 0633;
+glyphname = "be-cy";
+unicode = 1073;
 },
 {
-glyphname = "sheen-ar";
-unicode = 0634;
+glyphname = "ve-cy";
+unicode = 1074;
 },
 {
-glyphname = "sad-ar";
-unicode = 0635;
+glyphname = "ge-cy";
+unicode = 1075;
 },
 {
-glyphname = "dad-ar";
-unicode = 0636;
+glyphname = "de-cy";
+unicode = 1076;
 },
 {
-glyphname = "tah-ar";
-unicode = 0637;
+glyphname = "ie-cy";
+unicode = 1077;
 },
 {
-glyphname = "zah-ar";
-unicode = 0638;
+glyphname = "zhe-cy";
+unicode = 1078;
 },
 {
-glyphname = "ain-ar";
-unicode = 0639;
+glyphname = "ze-cy";
+unicode = 1079;
 },
 {
-glyphname = "ghain-ar";
-unicode = 063A;
+glyphname = "ii-cy";
+unicode = 1080;
 },
 {
-glyphname = "feh-ar";
-unicode = 0641;
+glyphname = "iishort-cy";
+unicode = 1081;
 },
 {
-glyphname = "qaf-ar";
-unicode = 0642;
+glyphname = "ka-cy";
+unicode = 1082;
 },
 {
-glyphname = "kaf-ar";
-unicode = 0643;
+glyphname = "el-cy";
+unicode = 1083;
 },
 {
-glyphname = "lam-ar";
-unicode = 0644;
+glyphname = "em-cy";
+unicode = 1084;
 },
 {
-glyphname = "meem-ar";
-unicode = 0645;
+glyphname = "en-cy";
+unicode = 1085;
 },
 {
-glyphname = "noon-ar";
-unicode = 0646;
+glyphname = "o-cy";
+unicode = 1086;
 },
 {
-glyphname = "heh-ar";
-unicode = 0647;
+glyphname = "pe-cy";
+unicode = 1087;
 },
 {
-glyphname = "waw-ar";
-unicode = 0648;
+glyphname = "er-cy";
+unicode = 1088;
 },
 {
-glyphname = "alefMaksura-ar";
-unicode = 0649;
+glyphname = "es-cy";
+unicode = 1089;
 },
 {
-glyphname = "yeh-ar";
-unicode = 064A;
+glyphname = "te-cy";
+unicode = 1090;
 },
 {
-glyphname = "tehRing-ar";
-unicode = 067C;
+glyphname = "u-cy";
+unicode = 1091;
 },
 {
-glyphname = "peh-ar";
-unicode = 067E;
+glyphname = "ef-cy";
+unicode = 1092;
 },
 {
-glyphname = "hahHamzaabove-ar";
-unicode = 0681;
+glyphname = "ha-cy";
+unicode = 1093;
 },
 {
-glyphname = "hahThreedotsabove-ar";
-unicode = 0685;
+glyphname = "tse-cy";
+unicode = 1094;
 },
 {
-glyphname = "tcheh-ar";
-unicode = 0686;
+glyphname = "che-cy";
+unicode = 1095;
 },
 {
-glyphname = "dalRing-ar";
-unicode = 0689;
+glyphname = "sha-cy";
+unicode = 1096;
 },
 {
-glyphname = "rehRing-ar";
-unicode = 0693;
+glyphname = "shcha-cy";
+unicode = 1097;
 },
 {
-glyphname = "rehVbelow-ar";
-unicode = 0695;
+glyphname = "hardsign-cy";
+unicode = 1098;
 },
 {
-glyphname = "rehDotbelowdotabove-ar";
-unicode = 0696;
+glyphname = "yeru-cy";
+unicode = 1099;
 },
 {
-glyphname = "jeh-ar";
-unicode = 0698;
+glyphname = "softsign-cy";
+unicode = 1100;
 },
 {
-glyphname = "seenDotbelowDotabove-ar";
-unicode = 069A;
+glyphname = "ereversed-cy";
+unicode = 1101;
 },
 {
-glyphname = "veh-ar";
-unicode = 06A4;
+glyphname = "yu-cy";
+unicode = 1102;
 },
 {
-glyphname = "keheh-ar";
-unicode = 06A9;
+glyphname = "ya-cy";
+unicode = 1103;
 },
 {
-glyphname = "kafRing-ar";
-unicode = 06AB;
+glyphname = "io-cy";
+unicode = 1105;
 },
 {
-glyphname = "ng-ar";
-unicode = 06AD;
+glyphname = "dje-cy";
+unicode = 1106;
 },
 {
-glyphname = "gaf-ar";
-unicode = 06AF;
+glyphname = "e-cy";
+unicode = 1108;
 },
 {
-glyphname = "lamVabove-ar";
-unicode = 06B5;
+glyphname = "i-cy";
+unicode = 1110;
 },
 {
-glyphname = "noonRing-ar";
-unicode = 06BC;
+glyphname = "yi-cy";
+unicode = 1111;
 },
 {
-glyphname = "hehDoachashmee-ar";
-unicode = 06BE;
+glyphname = "je-cy";
+unicode = 1112;
 },
 {
-glyphname = "oe-ar";
-unicode = 06C6;
+glyphname = "lje-cy";
+unicode = 1113;
 },
 {
-glyphname = "u-ar";
-unicode = 06C7;
+glyphname = "nje-cy";
+unicode = 1114;
 },
 {
-glyphname = "yu-ar";
-unicode = 06C8;
+glyphname = "tshe-cy";
+unicode = 1115;
 },
 {
-glyphname = "ve-ar";
-unicode = 06CB;
+glyphname = "ushort-cy";
+unicode = 1118;
 },
 {
-glyphname = "yeh-farsi";
-unicode = 06CC;
+glyphname = "dzhe-cy";
+unicode = 1119;
 },
 {
-glyphname = "yehTail-ar";
-unicode = 06CD;
+glyphname = "Geupturn-cy";
+unicode = 1168;
 },
 {
-glyphname = "yehVabove-ar";
-unicode = 06CE;
+glyphname = "geupturn-cy";
+unicode = 1169;
+}
+);
+instances = (
+);
+kerningLTR = {
+};
+metrics = (
+{
+type = ascender;
 },
 {
-glyphname = "e-ar";
-unicode = 06D0;
+type = "cap height";
 },
 {
-glyphname = "ae-ar";
-unicode = 06D5;
+type = "x-height";
+},
+{
+type = baseline;
+},
+{
+type = descender;
+},
+{
+type = "italic angle";
 }
 );
-instances = (
+stems = (
 );
 unitsPerEm = 1000;
 versionMajor = 1;
 versionMinor = 0;
 }
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Arabic_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Arabic_Plus.nam`

 * *Files 18% similar despite different names*

```diff
@@ -79,31 +79,49 @@
 0x0667 ARABIC-INDIC DIGIT SEVEN
 0x0668 ARABIC-INDIC DIGIT EIGHT
 0x0669 ARABIC-INDIC DIGIT NINE
 0x066A ARABIC PERCENT SIGN
 0x066B ARABIC DECIMAL SEPARATOR
 0x066C ARABIC THOUSANDS SEPARATOR
 0x0670 ARABIC LETTER SUPERSCRIPT ALEF
+0x067A ARABIC LETTER TTEHEH
+0x067B ARABIC LETTER BEEH
 0x067C ARABIC LETTER TEH WITH RING
+0x067D ARABIC LETTER TEH WITH THREE DOTS ABOVE DOWNWARDS
 0x067E ARABIC LETTER PEH
+0x067F ARABIC LETTER TEHEH
+0x0680 ARABIC LETTER BEHEH
 0x0681 ARABIC LETTER HAH WITH HAMZA ABOVE
+0x0683 ARABIC LETTER NYEH
+0x0684 ARABIC LETTER DYEH
 0x0685 ARABIC LETTER HAH WITH THREE DOTS ABOVE
 0x0686 ARABIC LETTER TCHEH
+0x0687 ARABIC LETTER TCHEHEH
 0x0689 ARABIC LETTER DAL WITH RING
+0x068A ARABIC LETTER DAL WITH DOT BELOW
+0x068C ARABIC LETTER DAHAL
+0x068D ARABIC LETTER DDAHAL
+0x068F ARABIC LETTER DAL WITH THREE DOTS ABOVE DOWNWARDS
 0x0693 ARABIC LETTER REH WITH RING
 0x0695 ARABIC LETTER REH WITH SMALL V BELOW
 0x0696 ARABIC LETTER REH WITH DOT BELOW AND DOT ABOVE
 0x0698 ARABIC LETTER JEH
+0x0699 ARABIC LETTER REH WITH FOUR DOTS ABOVE
 0x069A ARABIC LETTER SEEN WITH DOT BELOW AND DOT ABOVE
 0x06A4 ARABIC LETTER VEH
+0x06A6 ARABIC LETTER PEHEH
 0x06A9 ARABIC LETTER KEHEH
+0x06AA ARABIC LETTER SWASH KAF
 0x06AB ARABIC LETTER KAF WITH RING
 0x06AD ARABIC LETTER NG
 0x06AF ARABIC LETTER GAF
+0x06B1 ARABIC LETTER NGOEH
+0x06B3 ARABIC LETTER GUEH
 0x06B5 ARABIC LETTER LAM WITH SMALL V
+0x06BB ARABIC LETTER RNOON
 0x06BC ARABIC LETTER NOON WITH RING
 0x06BE ARABIC LETTER HEH DOACHASHMEE
 0x06C6 ARABIC LETTER OE
 0x06C7 ARABIC LETTER U
 0x06C8 ARABIC LETTER YU
 0x06CB ARABIC LETTER VE
 0x06CC ARABIC LETTER FARSI YEH
@@ -123,8 +141,10 @@
 0x06F8 EXTENDED ARABIC-INDIC DIGIT EIGHT
 0x06F9 EXTENDED ARABIC-INDIC DIGIT NINE
 0x06FD ARABIC SIGN SINDHI AMPERSAND
 0x06FE ARABIC SIGN SINDHI POSTPOSITION MEN
 0x200E LEFT-TO-RIGHT MARK
 0x200F RIGHT-TO-LEFT MARK
 0x2018 LEFT SINGLE QUOTATION MARK
-0x2212 MINUS SIGN
+0x204F REVERSED SEMICOLON
+0x2212 MINUS SIGN
+0x2E41 REVERSED COMMA
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Arabic_Core.txt`

 * *Files 19% similar despite different names*

```diff
@@ -113,27 +113,27 @@
 ddal-ar
 rreh-ar
 jeh-ar
 keheh-ar
 gaf-ar
 hehDoachashmee-ar
 hehgoal-ar
-yeh-farsi
+yehFarsi-ar
 yehbarree-ar
 fullstop-ar
-zero-persian
-one-persian
-two-persian
-three-persian
-four-persian
-five-persian
-six-persian
-seven-persian
-eight-persian
-nine-persian
+zeroFarsi-ar
+oneFarsi-ar
+twoFarsi-ar
+threeFarsi-ar
+fourFarsi-ar
+fiveFarsi-ar
+sixFarsi-ar
+sevenFarsi-ar
+eightFarsi-ar
+nineFarsi-ar
 kehehThreedotsabove-ar
 lefttorightmark
 endash
 emdash
 quoteleft
 quoteright
 quotedblleft
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt` & `glyphsets-1.0.0/data/results/txt/nice-names/GF_Arabic_Core.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # This file is auto-generated; do not edit. See /README.md for instructions.
+space
 exclam
+quotedbl
+numbersign
 percent
 quotesingle
 parenleft
 parenright
+asterisk
 plus
 comma
 hyphen
 period
 slash
 zero
 one
@@ -16,23 +20,39 @@
 four
 five
 six
 seven
 eight
 nine
 colon
-semicolon
+less
+equal
+greater
 bracketleft
+backslash
 bracketright
+braceleft
+bar
+braceright
+nbspace
+guillemetleft
+guillemetright
+multiply
+divide
 perthousand-ar
 comma-ar
+dateseparator-ar
+semicolon-ar
+mark-ar
+question-ar
 hamza-ar
 alefMadda-ar
 alefHamzaabove-ar
 wawHamzaabove-ar
+alefHamzabelow-ar
 yehHamzaabove-ar
 alef-ar
 beh-ar
 tehMarbuta-ar
 teh-ar
 theh-ar
 jeem-ar
@@ -46,14 +66,15 @@
 sheen-ar
 sad-ar
 dad-ar
 tah-ar
 zah-ar
 ain-ar
 ghain-ar
+kashida-ar
 feh-ar
 qaf-ar
 kaf-ar
 lam-ar
 meem-ar
 noon-ar
 heh-ar
@@ -64,67 +85,62 @@
 dammatan-ar
 kasratan-ar
 fatha-ar
 damma-ar
 kasra-ar
 shadda-ar
 sukun-ar
+madda-ar
 hamzaabove-ar
+hamzabelow-ar
 zero-ar
 one-ar
 two-ar
 three-ar
 four-ar
 five-ar
 six-ar
 seven-ar
 eight-ar
 nine-ar
 percent-ar
 decimalseparator-ar
 thousandseparator-ar
+asterisk-ar
 alefabove-ar
-tehRing-ar
+tteh-ar
 peh-ar
-hahHamzaabove-ar
-hahThreedotsabove-ar
 tcheh-ar
-dalRing-ar
-rehRing-ar
-rehVbelow-ar
-rehDotbelowdotabove-ar
+ddal-ar
+rreh-ar
 jeh-ar
-seenDotbelowDotabove-ar
-veh-ar
 keheh-ar
-kafRing-ar
-ng-ar
 gaf-ar
-lamVabove-ar
-noonRing-ar
 hehDoachashmee-ar
-oe-ar
-u-ar
-yu-ar
-ve-ar
-yeh-farsi
-yehTail-ar
-yehVabove-ar
-e-ar
+hehgoal-ar
+yehFarsi-ar
+yehbarree-ar
 fullstop-ar
-ae-ar
-zero-persian
-one-persian
-two-persian
-three-persian
-four-persian
-five-persian
-six-persian
-seven-persian
-eight-persian
-nine-persian
-sindhiampersand-ar
-sindhipostpositionmen-ar
+zeroFarsi-ar
+oneFarsi-ar
+twoFarsi-ar
+threeFarsi-ar
+fourFarsi-ar
+fiveFarsi-ar
+sixFarsi-ar
+sevenFarsi-ar
+eightFarsi-ar
+nineFarsi-ar
+kehehThreedotsabove-ar
 lefttorightmark
-righttoleftmark
+endash
+emdash
 quoteleft
-minus
+quoteright
+quotedblleft
+quotedblright
+ellipsis
+guilsinglleft
+guilsinglright
+minus
+parenleft-ar
+parenright-ar
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Arabic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Plus.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Arabic_Plus.txt`

 * *Files 24% similar despite different names*

```diff
@@ -79,31 +79,49 @@
 uni0667
 uni0668
 uni0669
 uni066A
 uni066B
 uni066C
 uni0670
+uni067A
+uni067B
 uni067C
+uni067D
 uni067E
+uni067F
+uni0680
 uni0681
+uni0683
+uni0684
 uni0685
 uni0686
+uni0687
 uni0689
+uni068A
+uni068C
+uni068D
+uni068F
 uni0693
 uni0695
 uni0696
 uni0698
+uni0699
 uni069A
 uni06A4
+uni06A6
 uni06A9
+uni06AA
 uni06AB
 uni06AD
 uni06AF
+uni06B1
+uni06B3
 uni06B5
+uni06BB
 uni06BC
 uni06BE
 uni06C6
 uni06C7
 uni06C8
 uni06CB
 uni06CC
@@ -123,8 +141,10 @@
 uni06F8
 uni06F9
 uni06FD
 uni06FE
 uni200E
 uni200F
 quoteleft
-minus
+uni204F
+minus
+uni2E41
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs` & `glyphsets-1.0.0/data/definitions/per_glyphset/GF_Latin_Vietnamese.stub.glyphs`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,28 @@
 {
-.appVersion = "3124";
+.appVersion = "3257";
 .formatVersion = 3;
-date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Cyrillic Plus";
-featurePrefixes = (
-{
-automatic = 1;
-code = "languagesystem DFLT dflt;
-
-languagesystem latn dflt;
-languagesystem latn AZE;
-languagesystem latn CRT;
-languagesystem latn KAZ;
-languagesystem latn TAT;
-languagesystem latn TRK;
-languagesystem latn ROM;
-languagesystem latn MOL;
-languagesystem latn CAT;
-";
-name = Languagesystems;
-}
-);
-features = (
-{
-automatic = 1;
-code = "feature locl;
-feature ordn;
-feature case;
-";
-tag = aalt;
-},
-{
-automatic = 1;
-code = "lookup ccmp_Other_1 {
-	@CombiningTopAccents = [acutecomb brevecomb caroncomb circumflexcomb commaturnedabovecomb dieresiscomb dotaccentcomb gravecomb hungarumlautcomb macroncomb ringcomb tildecomb];
-	@CombiningNonTopAccents = [cedillacomb ogonekcomb];
-	sub [i j]' @CombiningTopAccents by [idotless jdotless];
-	sub [i j]' @CombiningNonTopAccents @CombiningTopAccents by [idotless jdotless];
-} ccmp_Other_1;
-";
-tag = ccmp;
-},
-{
-automatic = 1;
-code = "lookup locl_latn_0 {
-	script latn;
-	language AZE;
-	sub i by idotaccent;
-	language CRT;
-	sub i by idotaccent;
-	language KAZ;
-	sub i by idotaccent;
-	language TAT;
-	sub i by idotaccent;
-	language TRK;
-	sub i by idotaccent;
-} locl_latn_0;
-
-lookup locl_latn_1 {
-	script latn;
-	language ROM;
-	sub Scedilla by Scommaaccent;
-	sub scedilla by scommaaccent;
-	language MOL;
-	sub Scedilla by Scommaaccent;
-	sub scedilla by scommaaccent;
-} locl_latn_1;
-
-lookup locl_latn_2 {
-	script latn;
-	language CAT;
-	sub l periodcentered' l by periodcentered.loclCAT;
-	sub L periodcentered' L by periodcentered.loclCAT.case;
-} locl_latn_2;
-";
-tag = locl;
-},
-{
-automatic = 1;
-code = "sub [zero one two three four five six seven eight nine] [A a]' by ordfeminine;
-sub [zero one two three four five six seven eight nine] [O o]' by ordmasculine;
-";
-tag = ordn;
-},
-{
-automatic = 1;
-code = "sub periodcentered.loclCAT by periodcentered.loclCAT.case;
-";
-tag = case;
+axes = (
+{
+name = Weight;
+tag = wght;
+},
+{
+name = Width;
+tag = wdth;
 }
 );
+date = "2023-12-13 14:28:10 +0000";
+familyName = "Neue Schrift";
 fontMaster = (
 {
+axesValues = (
+100,
+100
+);
 id = m01;
 metricValues = (
 {
 over = 16;
 pos = 800;
 },
 {
@@ -110,959 +37,1180 @@
 over = -16;
 },
 {
 over = -16;
 pos = -200;
 },
 {
-over = -16;
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-glyphname = "Gedescender-cy";
+glyphname = Abreveacute;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7854;
+},
+{
+glyphname = Abrevedotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7862;
+},
+{
+glyphname = Abrevegrave;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7856;
+},
+{
+glyphname = Abrevehookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7858;
+},
+{
+glyphname = Abrevetilde;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7860;
+},
+{
+glyphname = Acircumflexacute;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7844;
+},
+{
+glyphname = Acircumflexdotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7852;
+},
+{
+glyphname = Acircumflexgrave;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7846;
+},
+{
+glyphname = Acircumflexhookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7848;
+},
+{
+glyphname = Acircumflextilde;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7850;
+},
+{
+glyphname = Adotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7840;
+},
+{
+glyphname = Ahookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7842;
+},
+{
+glyphname = Ecircumflexacute;
+lastChange = "2024-04-10 11:00:19 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 7870;
+},
+{
+glyphname = Ecircumflexdotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1270;
+unicode = 7878;
 },
 {
-glyphname = "Gestroke-cy";
+glyphname = Ecircumflexgrave;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1170;
+unicode = 7872;
 },
 {
-glyphname = "Gemiddlehook-cy";
+glyphname = Ecircumflexhookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1172;
+unicode = 7874;
 },
 {
-glyphname = "Yat-cy";
+glyphname = Ecircumflextilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1122;
+unicode = 7876;
 },
 {
-glyphname = "Yusbig-cy";
+glyphname = Edotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1130;
+unicode = 7864;
 },
 {
-glyphname = "Fita-cy";
+glyphname = Ehookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1138;
+unicode = 7866;
 },
 {
-glyphname = "Izhitsa-cy";
+glyphname = Etilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1140;
+unicode = 7868;
 },
 {
-glyphname = "Zhedescender-cy";
+glyphname = Idotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1174;
+unicode = 7882;
 },
 {
-glyphname = "Zedescender-cy";
+glyphname = Ihookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1176;
+unicode = 7880;
 },
 {
-glyphname = "Kadescender-cy";
+glyphname = Itilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1178;
+unicode = 296;
 },
 {
-glyphname = "Kaverticalstroke-cy";
+glyphname = Ocircumflexacute;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1180;
+unicode = 7888;
 },
 {
-glyphname = "Kabashkir-cy";
+glyphname = Ocircumflexdotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1184;
+unicode = 7896;
 },
 {
-glyphname = "Endescender-cy";
+glyphname = Ocircumflexgrave;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1186;
+unicode = 7890;
 },
 {
-glyphname = "EnGe-cy";
+glyphname = Ocircumflexhookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1188;
+unicode = 7892;
 },
 {
-glyphname = "Esdescender-cy";
+glyphname = Ocircumflextilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1194;
+unicode = 7894;
 },
 {
-glyphname = "Ustraight-cy";
+glyphname = Odotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1198;
+unicode = 7884;
 },
 {
-glyphname = "Ustraightstroke-cy";
+glyphname = Ohookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1200;
+unicode = 7886;
 },
 {
-glyphname = "Hadescender-cy";
+glyphname = Ohorn;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1202;
+unicode = 416;
 },
 {
-glyphname = "Chedescender-cy";
+glyphname = Ohornacute;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1206;
+unicode = 7898;
 },
 {
-glyphname = "Cheverticalstroke-cy";
+glyphname = Ohorndotbelow;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1208;
+unicode = 7906;
 },
 {
-glyphname = "Shha-cy";
+glyphname = Ohorngrave;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1210;
+unicode = 7900;
 },
 {
-glyphname = "Palochka-cy";
+glyphname = Ohornhookabove;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1216;
+unicode = 7902;
 },
 {
-glyphname = "Zhebreve-cy";
+glyphname = Ohorntilde;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1217;
+unicode = 7904;
 },
 {
-glyphname = "Chekhakassian-cy";
+glyphname = Udotbelow;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1227;
+unicode = 7908;
 },
 {
-glyphname = "Abreve-cy";
+glyphname = Uhookabove;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1232;
+unicode = 7910;
 },
 {
-glyphname = "Adieresis-cy";
+glyphname = Uhorn;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1234;
+unicode = 431;
 },
 {
-glyphname = "Aie-cy";
+glyphname = Uhornacute;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1236;
+unicode = 7912;
 },
 {
-glyphname = "Iebreve-cy";
+glyphname = Uhorndotbelow;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1238;
+unicode = 7920;
 },
 {
-glyphname = "Schwa-cy";
+glyphname = Uhorngrave;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1240;
+unicode = 7914;
 },
 {
-glyphname = "Zhedieresis-cy";
+glyphname = Uhornhookabove;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1244;
+unicode = 7916;
 },
 {
-glyphname = "Zedieresis-cy";
+glyphname = Uhorntilde;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1246;
+unicode = 7918;
 },
 {
-glyphname = "Imacron-cy";
+glyphname = Utilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1250;
+unicode = 360;
 },
 {
-glyphname = "Idieresis-cy";
+glyphname = Ydotbelow;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1252;
+unicode = 7924;
 },
 {
-glyphname = "Odieresis-cy";
+glyphname = Yhookabove;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1254;
+unicode = 7926;
 },
 {
-glyphname = "Obarred-cy";
+glyphname = Ytilde;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1256;
+unicode = 7928;
 },
 {
-glyphname = "Umacron-cy";
+glyphname = abreveacute;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1262;
+unicode = 7855;
 },
 {
-glyphname = "Udieresis-cy";
+glyphname = abrevedotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1264;
+unicode = 7863;
 },
 {
-glyphname = "Uhungarumlaut-cy";
+glyphname = abrevegrave;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1266;
+unicode = 7857;
 },
 {
-glyphname = "Chedieresis-cy";
+glyphname = abrevehookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1268;
+unicode = 7859;
 },
 {
-glyphname = "Yerudieresis-cy";
+glyphname = abrevetilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1272;
+unicode = 7861;
 },
 {
-glyphname = "Qa-cy";
+glyphname = acircumflexacute;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1306;
+unicode = 7845;
 },
 {
-glyphname = "We-cy";
+glyphname = acircumflexdotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1308;
+unicode = 7853;
 },
 {
-glyphname = "gedescender-cy";
+glyphname = acircumflexgrave;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1271;
+unicode = 7847;
 },
 {
-glyphname = "gestroke-cy";
+glyphname = acircumflexhookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1171;
+unicode = 7849;
 },
 {
-glyphname = "gemiddlehook-cy";
+glyphname = acircumflextilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1173;
+unicode = 7851;
 },
 {
-glyphname = "yat-cy";
+glyphname = adotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1123;
+unicode = 7841;
 },
 {
-glyphname = "yusbig-cy";
+glyphname = ahookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1131;
+unicode = 7843;
 },
 {
-glyphname = "fita-cy";
+glyphname = ecircumflexacute;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1139;
+unicode = 7871;
 },
 {
-glyphname = "izhitsa-cy";
+glyphname = ecircumflexdotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1141;
+unicode = 7879;
 },
 {
-glyphname = "zhedescender-cy";
+glyphname = ecircumflexgrave;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1175;
+unicode = 7873;
 },
 {
-glyphname = "zedescender-cy";
+glyphname = ecircumflexhookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1177;
+unicode = 7875;
 },
 {
-glyphname = "kadescender-cy";
+glyphname = ecircumflextilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1179;
+unicode = 7877;
 },
 {
-glyphname = "kaverticalstroke-cy";
+glyphname = edotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1181;
+unicode = 7865;
 },
 {
-glyphname = "kabashkir-cy";
+glyphname = ehookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1185;
+unicode = 7867;
 },
 {
-glyphname = "endescender-cy";
+glyphname = etilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1187;
+unicode = 7869;
 },
 {
-glyphname = "enge-cy";
+glyphname = idotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1189;
+unicode = 7883;
 },
 {
-glyphname = "esdescender-cy";
+glyphname = ihookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1195;
+unicode = 7881;
 },
 {
-glyphname = "ustraight-cy";
+glyphname = itilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1199;
+unicode = 297;
 },
 {
-glyphname = "ustraightstroke-cy";
+glyphname = ocircumflexacute;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1201;
+unicode = 7889;
 },
 {
-glyphname = "hadescender-cy";
+glyphname = ocircumflexdotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1203;
+unicode = 7897;
 },
 {
-glyphname = "chedescender-cy";
+glyphname = ocircumflexgrave;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1207;
+unicode = 7891;
 },
 {
-glyphname = "cheverticalstroke-cy";
+glyphname = ocircumflexhookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1209;
+unicode = 7893;
 },
 {
-glyphname = "shha-cy";
+glyphname = ocircumflextilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1211;
+unicode = 7895;
 },
 {
-glyphname = "palochka-cy";
+glyphname = odotbelow;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1231;
+unicode = 7885;
 },
 {
-glyphname = "zhebreve-cy";
+glyphname = ohookabove;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1218;
+unicode = 7887;
 },
 {
-glyphname = "chekhakassian-cy";
+glyphname = ohorn;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1228;
+unicode = 417;
 },
 {
-glyphname = "abreve-cy";
+glyphname = ohornacute;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1233;
+unicode = 7899;
 },
 {
-glyphname = "adieresis-cy";
+glyphname = ohorndotbelow;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1235;
+unicode = 7907;
 },
 {
-glyphname = "aie-cy";
+glyphname = ohorngrave;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1237;
+unicode = 7901;
 },
 {
-glyphname = "iebreve-cy";
+glyphname = ohornhookabove;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1239;
+unicode = 7903;
 },
 {
-glyphname = "schwa-cy";
+glyphname = ohorntilde;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1241;
+unicode = 7905;
 },
 {
-glyphname = "zhedieresis-cy";
+glyphname = udotbelow;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1245;
+unicode = 7909;
 },
 {
-glyphname = "zedieresis-cy";
+glyphname = uhookabove;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1247;
+unicode = 7911;
 },
 {
-glyphname = "imacron-cy";
+glyphname = uhorn;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1251;
+unicode = 432;
 },
 {
-glyphname = "idieresis-cy";
+glyphname = uhornacute;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1253;
+unicode = 7913;
 },
 {
-glyphname = "odieresis-cy";
+glyphname = uhorndotbelow;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1255;
+unicode = 7921;
 },
 {
-glyphname = "obarred-cy";
+glyphname = uhorngrave;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1257;
+unicode = 7915;
 },
 {
-glyphname = "umacron-cy";
+glyphname = uhornhookabove;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1263;
+unicode = 7917;
 },
 {
-glyphname = "udieresis-cy";
+glyphname = uhorntilde;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1265;
+unicode = 7919;
 },
 {
-glyphname = "uhungarumlaut-cy";
+glyphname = utilde;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1267;
+unicode = 361;
 },
 {
-glyphname = "chedieresis-cy";
+glyphname = ydotbelow;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1269;
+unicode = 7925;
 },
 {
-glyphname = "yerudieresis-cy";
+glyphname = yhookabove;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1273;
+unicode = 7927;
 },
 {
-glyphname = "qa-cy";
+glyphname = ytilde;
+lastChange = "2024-04-10 11:00:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1307;
+unicode = 7929;
 },
 {
-glyphname = "we-cy";
+glyphname = hookabovecomb;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1309;
+unicode = 777;
 },
 {
-glyphname = hryvnia;
+glyphname = horncomb;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8372;
+unicode = 795;
 },
 {
-glyphname = tenge;
+glyphname = dotbelowcomb;
+lastChange = "2024-04-10 11:00:19 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8376;
+unicode = 803;
 },
 {
-glyphname = tugrik;
+glyphname = brevecomb_acutecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8366;
 },
 {
-glyphname = "brevecomb-cy";
+glyphname = brevecomb_gravecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
 },
 {
-glyphname = dieresiscomb;
+glyphname = brevecomb_hookabovecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 776;
 },
 {
-glyphname = gravecomb;
+glyphname = brevecomb_tildecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 768;
 },
 {
-glyphname = acutecomb;
+glyphname = circumflexcomb_acutecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 769;
 },
 {
-glyphname = hungarumlautcomb;
+glyphname = circumflexcomb_gravecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 779;
 },
 {
-glyphname = macroncomb;
+glyphname = circumflexcomb_hookabovecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 772;
 },
 {
-glyphname = apostrophemod;
+glyphname = circumflexcomb_tildecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 700;
 }
 );
 metrics = (
 {
 type = ascender;
 },
 {
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Cyrillic_Pro.nam`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,57 @@
-0x0400 CYRILLIC CAPITAL LETTER IE WITH GRAVE
-0x0401 CYRILLIC CAPITAL LETTER IO
-0x0402 CYRILLIC CAPITAL LETTER DJE
-0x0403 CYRILLIC CAPITAL LETTER GJE
-0x0404 CYRILLIC CAPITAL LETTER UKRAINIAN IE
-0x0405 CYRILLIC CAPITAL LETTER DZE
-0x0406 CYRILLIC CAPITAL LETTER BYELORUSSIAN-UKRAINIAN I
-0x0407 CYRILLIC CAPITAL LETTER YI
-0x0408 CYRILLIC CAPITAL LETTER JE
-0x0409 CYRILLIC CAPITAL LETTER LJE
-0x040A CYRILLIC CAPITAL LETTER NJE
-0x040B CYRILLIC CAPITAL LETTER TSHE
-0x040C CYRILLIC CAPITAL LETTER KJE
-0x040D CYRILLIC CAPITAL LETTER I WITH GRAVE
-0x040E CYRILLIC CAPITAL LETTER SHORT U
-0x040F CYRILLIC CAPITAL LETTER DZHE
-0x0410 CYRILLIC CAPITAL LETTER A
-0x0411 CYRILLIC CAPITAL LETTER BE
-0x0412 CYRILLIC CAPITAL LETTER VE
-0x0413 CYRILLIC CAPITAL LETTER GHE
-0x0414 CYRILLIC CAPITAL LETTER DE
-0x0415 CYRILLIC CAPITAL LETTER IE
-0x0416 CYRILLIC CAPITAL LETTER ZHE
-0x0417 CYRILLIC CAPITAL LETTER ZE
-0x0418 CYRILLIC CAPITAL LETTER I
-0x0419 CYRILLIC CAPITAL LETTER SHORT I
-0x041A CYRILLIC CAPITAL LETTER KA
-0x041B CYRILLIC CAPITAL LETTER EL
-0x041C CYRILLIC CAPITAL LETTER EM
-0x041D CYRILLIC CAPITAL LETTER EN
-0x041E CYRILLIC CAPITAL LETTER O
-0x041F CYRILLIC CAPITAL LETTER PE
-0x0420 CYRILLIC CAPITAL LETTER ER
-0x0421 CYRILLIC CAPITAL LETTER ES
-0x0422 CYRILLIC CAPITAL LETTER TE
-0x0423 CYRILLIC CAPITAL LETTER U
-0x0424 CYRILLIC CAPITAL LETTER EF
-0x0425 CYRILLIC CAPITAL LETTER HA
-0x0426 CYRILLIC CAPITAL LETTER TSE
-0x0427 CYRILLIC CAPITAL LETTER CHE
-0x0428 CYRILLIC CAPITAL LETTER SHA
-0x0429 CYRILLIC CAPITAL LETTER SHCHA
-0x042A CYRILLIC CAPITAL LETTER HARD SIGN
-0x042B CYRILLIC CAPITAL LETTER YERU
-0x042C CYRILLIC CAPITAL LETTER SOFT SIGN
-0x042D CYRILLIC CAPITAL LETTER E
-0x042E CYRILLIC CAPITAL LETTER YU
-0x042F CYRILLIC CAPITAL LETTER YA
-0x0430 CYRILLIC SMALL LETTER A
-0x0431 CYRILLIC SMALL LETTER BE
-0x0432 CYRILLIC SMALL LETTER VE
-0x0433 CYRILLIC SMALL LETTER GHE
-0x0434 CYRILLIC SMALL LETTER DE
-0x0435 CYRILLIC SMALL LETTER IE
-0x0436 CYRILLIC SMALL LETTER ZHE
-0x0437 CYRILLIC SMALL LETTER ZE
-0x0438 CYRILLIC SMALL LETTER I
-0x0439 CYRILLIC SMALL LETTER SHORT I
-0x043A CYRILLIC SMALL LETTER KA
-0x043B CYRILLIC SMALL LETTER EL
-0x043C CYRILLIC SMALL LETTER EM
-0x043D CYRILLIC SMALL LETTER EN
-0x043E CYRILLIC SMALL LETTER O
-0x043F CYRILLIC SMALL LETTER PE
-0x0440 CYRILLIC SMALL LETTER ER
-0x0441 CYRILLIC SMALL LETTER ES
-0x0442 CYRILLIC SMALL LETTER TE
-0x0443 CYRILLIC SMALL LETTER U
-0x0444 CYRILLIC SMALL LETTER EF
-0x0445 CYRILLIC SMALL LETTER HA
-0x0446 CYRILLIC SMALL LETTER TSE
-0x0447 CYRILLIC SMALL LETTER CHE
-0x0448 CYRILLIC SMALL LETTER SHA
-0x0449 CYRILLIC SMALL LETTER SHCHA
-0x044A CYRILLIC SMALL LETTER HARD SIGN
-0x044B CYRILLIC SMALL LETTER YERU
-0x044C CYRILLIC SMALL LETTER SOFT SIGN
-0x044D CYRILLIC SMALL LETTER E
-0x044E CYRILLIC SMALL LETTER YU
-0x044F CYRILLIC SMALL LETTER YA
-0x0450 CYRILLIC SMALL LETTER IE WITH GRAVE
-0x0451 CYRILLIC SMALL LETTER IO
-0x0452 CYRILLIC SMALL LETTER DJE
-0x0453 CYRILLIC SMALL LETTER GJE
-0x0454 CYRILLIC SMALL LETTER UKRAINIAN IE
-0x0455 CYRILLIC SMALL LETTER DZE
-0x0456 CYRILLIC SMALL LETTER BYELORUSSIAN-UKRAINIAN I
-0x0457 CYRILLIC SMALL LETTER YI
-0x0458 CYRILLIC SMALL LETTER JE
-0x0459 CYRILLIC SMALL LETTER LJE
-0x045A CYRILLIC SMALL LETTER NJE
-0x045B CYRILLIC SMALL LETTER TSHE
-0x045C CYRILLIC SMALL LETTER KJE
-0x045D CYRILLIC SMALL LETTER I WITH GRAVE
-0x045E CYRILLIC SMALL LETTER SHORT U
-0x045F CYRILLIC SMALL LETTER DZHE
-0x0490 CYRILLIC CAPITAL LETTER GHE WITH UPTURN
-0x0491 CYRILLIC SMALL LETTER GHE WITH UPTURN
-0x2116 NUMERO SIGN
+# This file is auto-generated; do not edit. See /README.md for instructions.
+0x048A CYRILLIC CAPITAL LETTER SHORT I WITH TAIL
+0x048B CYRILLIC SMALL LETTER SHORT I WITH TAIL
+0x048C CYRILLIC CAPITAL LETTER SEMISOFT SIGN
+0x048D CYRILLIC SMALL LETTER SEMISOFT SIGN
+0x048E CYRILLIC CAPITAL LETTER ER WITH TICK
+0x048F CYRILLIC SMALL LETTER ER WITH TICK
+0x0494 CYRILLIC CAPITAL LETTER GHE WITH MIDDLE HOOK
+0x0495 CYRILLIC SMALL LETTER GHE WITH MIDDLE HOOK
+0x049E CYRILLIC CAPITAL LETTER KA WITH STROKE
+0x049F CYRILLIC SMALL LETTER KA WITH STROKE
+0x04A8 CYRILLIC CAPITAL LETTER ABKHASIAN HA
+0x04A9 CYRILLIC SMALL LETTER ABKHASIAN HA
+0x04AC CYRILLIC CAPITAL LETTER TE WITH DESCENDER
+0x04AD CYRILLIC SMALL LETTER TE WITH DESCENDER
+0x04B4 CYRILLIC CAPITAL LIGATURE TE TSE
+0x04B5 CYRILLIC SMALL LIGATURE TE TSE
+0x04BC CYRILLIC CAPITAL LETTER ABKHASIAN CHE
+0x04BD CYRILLIC SMALL LETTER ABKHASIAN CHE
+0x04BE CYRILLIC CAPITAL LETTER ABKHASIAN CHE WITH DESCENDER
+0x04BF CYRILLIC SMALL LETTER ABKHASIAN CHE WITH DESCENDER
+0x04C3 CYRILLIC CAPITAL LETTER KA WITH HOOK
+0x04C4 CYRILLIC SMALL LETTER KA WITH HOOK
+0x04C5 CYRILLIC CAPITAL LETTER EL WITH TAIL
+0x04C6 CYRILLIC SMALL LETTER EL WITH TAIL
+0x04C7 CYRILLIC CAPITAL LETTER EN WITH HOOK
+0x04C8 CYRILLIC SMALL LETTER EN WITH HOOK
+0x04C9 CYRILLIC CAPITAL LETTER EN WITH TAIL
+0x04CA CYRILLIC SMALL LETTER EN WITH TAIL
+0x04CD CYRILLIC CAPITAL LETTER EM WITH TAIL
+0x04CE CYRILLIC SMALL LETTER EM WITH TAIL
+0x04DA CYRILLIC CAPITAL LETTER SCHWA WITH DIAERESIS
+0x04DB CYRILLIC SMALL LETTER SCHWA WITH DIAERESIS
+0x04E0 CYRILLIC CAPITAL LETTER ABKHASIAN DZE
+0x04E1 CYRILLIC SMALL LETTER ABKHASIAN DZE
+0x04EA CYRILLIC CAPITAL LETTER BARRED O WITH DIAERESIS
+0x04EB CYRILLIC SMALL LETTER BARRED O WITH DIAERESIS
+0x04EC CYRILLIC CAPITAL LETTER E WITH DIAERESIS
+0x04ED CYRILLIC SMALL LETTER E WITH DIAERESIS
+0x04FA CYRILLIC CAPITAL LETTER GHE WITH STROKE AND HOOK
+0x04FB CYRILLIC SMALL LETTER GHE WITH STROKE AND HOOK
+0x04FC CYRILLIC CAPITAL LETTER HA WITH HOOK
+0x04FD CYRILLIC SMALL LETTER HA WITH HOOK
+0x04FE CYRILLIC CAPITAL LETTER HA WITH STROKE
+0x04FF CYRILLIC SMALL LETTER HA WITH STROKE
+0x0510 CYRILLIC CAPITAL LETTER REVERSED ZE
+0x0511 CYRILLIC SMALL LETTER REVERSED ZE
+0x0512 CYRILLIC CAPITAL LETTER EL WITH HOOK
+0x0513 CYRILLIC SMALL LETTER EL WITH HOOK
+0x0524 CYRILLIC CAPITAL LETTER PE WITH DESCENDER
+0x0525 CYRILLIC SMALL LETTER PE WITH DESCENDER
+0x0526 CYRILLIC CAPITAL LETTER SHHA WITH DESCENDER
+0x0527 CYRILLIC SMALL LETTER SHHA WITH DESCENDER
+0x0528 CYRILLIC CAPITAL LETTER EN WITH LEFT HOOK
+0x0529 CYRILLIC SMALL LETTER EN WITH LEFT HOOK
+0x052E CYRILLIC CAPITAL LETTER EL WITH DESCENDER
+0x052F CYRILLIC SMALL LETTER EL WITH DESCENDER
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Cyrillic_Historical.nam`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x0460 CYRILLIC CAPITAL LETTER OMEGA
 0x0461 CYRILLIC SMALL LETTER OMEGA
 0x0464 CYRILLIC CAPITAL LETTER IOTIFIED E
 0x0465 CYRILLIC SMALL LETTER IOTIFIED E
 0x0466 CYRILLIC CAPITAL LETTER LITTLE YUS
 0x0467 CYRILLIC SMALL LETTER LITTLE YUS
 0x0468 CYRILLIC CAPITAL LETTER IOTIFIED LITTLE YUS
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Cyrillic_Plus.nam`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x02BC MODIFIER LETTER APOSTROPHE
 0x0300 COMBINING GRAVE ACCENT
 0x0301 COMBINING ACUTE ACCENT
 0x0304 COMBINING MACRON
 0x0308 COMBINING DIAERESIS
 0x030B COMBINING DOUBLE ACUTE ACCENT
 0x0462 CYRILLIC CAPITAL LETTER YAT
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam` & `glyphsets-1.0.0/data/results/nam/GF_Cyrillic_Pro.nam`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x048A CYRILLIC CAPITAL LETTER SHORT I WITH TAIL
 0x048B CYRILLIC SMALL LETTER SHORT I WITH TAIL
 0x048C CYRILLIC CAPITAL LETTER SEMISOFT SIGN
 0x048D CYRILLIC SMALL LETTER SEMISOFT SIGN
 0x048E CYRILLIC CAPITAL LETTER ER WITH TICK
 0x048F CYRILLIC SMALL LETTER ER WITH TICK
 0x0494 CYRILLIC CAPITAL LETTER GHE WITH MIDDLE HOOK
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Cyrillic_Core.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,136 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+exclam
+quotedbl
+numbersign
+percent
+ampersand
+quotesingle
+parenleft
+parenright
+asterisk
+plus
+comma
+hyphen
+period
+slash
+zero
+one
+two
+three
+four
+five
+six
+seven
+eight
+nine
+colon
+semicolon
+question
+at
+bracketleft
+backslash
+bracketright
+guillemetleft
+guillemetright
+apostrophemod
+gravecomb
+acutecomb
+brevecomb
+dieresiscomb
+Io-cy
+Dje-cy
+E-cy
+I-cy
+Yi-cy
+Je-cy
+Lje-cy
+Nje-cy
+Tshe-cy
+Ushort-cy
+Dzhe-cy
 A-cy
 Be-cy
 Ve-cy
 Ge-cy
-Gje-cy
-Geupturn-cy
 De-cy
 Ie-cy
-Iegrave-cy
-Io-cy
 Zhe-cy
 Ze-cy
 Ii-cy
 Iishort-cy
-Iigrave-cy
 Ka-cy
-Kje-cy
 El-cy
 Em-cy
 En-cy
 O-cy
 Pe-cy
 Er-cy
 Es-cy
 Te-cy
 U-cy
-Ushort-cy
 Ef-cy
 Ha-cy
-Che-cy
 Tse-cy
+Che-cy
 Sha-cy
 Shcha-cy
-Dzhe-cy
-Softsign-cy
-Yeru-cy
 Hardsign-cy
-Lje-cy
-Nje-cy
-Dze-cy
-E-cy
+Yeru-cy
+Softsign-cy
 Ereversed-cy
-I-cy
-Yi-cy
-Je-cy
-Tshe-cy
 Yu-cy
 Ya-cy
-Dje-cy
 a-cy
 be-cy
 ve-cy
 ge-cy
-gje-cy
-geupturn-cy
 de-cy
 ie-cy
-iegrave-cy
-io-cy
 zhe-cy
 ze-cy
 ii-cy
 iishort-cy
-iigrave-cy
 ka-cy
-kje-cy
 el-cy
 em-cy
 en-cy
 o-cy
 pe-cy
 er-cy
 es-cy
 te-cy
 u-cy
-ushort-cy
 ef-cy
 ha-cy
-che-cy
 tse-cy
+che-cy
 sha-cy
 shcha-cy
-dzhe-cy
-softsign-cy
-yeru-cy
 hardsign-cy
-lje-cy
-nje-cy
-dze-cy
-e-cy
+yeru-cy
+softsign-cy
 ereversed-cy
+yu-cy
+ya-cy
+io-cy
+dje-cy
+e-cy
 i-cy
 yi-cy
 je-cy
+lje-cy
+nje-cy
 tshe-cy
-yu-cy
-ya-cy
-dje-cy
+ushort-cy
+dzhe-cy
+Geupturn-cy
+geupturn-cy
+endash
+emdash
+quoteleft
+quoteright
+quotesinglbase
+quotedblleft
+quotedblbase
+ellipsis
 numero
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Cyrillic_Plus.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,130 @@
-Gedescender-cy
-Gestroke-cy
-Gemiddlehook-cy
+# This file is auto-generated; do not edit. See /README.md for instructions.
+apostrophemod
+gravecomb
+acutecomb
+macroncomb
+dieresiscomb
+hungarumlautcomb
 Yat-cy
+yat-cy
 Yusbig-cy
+yusbig-cy
 Fita-cy
+fita-cy
 Izhitsa-cy
+izhitsa-cy
+Ghestroke-cy
+ghestroke-cy
+Ghemiddlehook-cy
+ghemiddlehook-cy
 Zhedescender-cy
+zhedescender-cy
 Zedescender-cy
+zedescender-cy
 Kadescender-cy
+kadescender-cy
 Kaverticalstroke-cy
+kaverticalstroke-cy
 Kabashkir-cy
+kabashkir-cy
 Endescender-cy
-EnGe-cy
+endescender-cy
+Enghe-cy
+enghe-cy
 Esdescender-cy
+esdescender-cy
 Ustraight-cy
+ustraight-cy
 Ustraightstroke-cy
+ustraightstroke-cy
 Hadescender-cy
+hadescender-cy
 Chedescender-cy
+chedescender-cy
 Cheverticalstroke-cy
+cheverticalstroke-cy
 Shha-cy
+shha-cy
 Palochka-cy
 Zhebreve-cy
-Chekhakassian-cy
-Abreve-cy
-Adieresis-cy
-Aie-cy
-Iebreve-cy
-Schwa-cy
-Zhedieresis-cy
-Zedieresis-cy
-Imacron-cy
-Idieresis-cy
-Odieresis-cy
-Obarred-cy
-Umacron-cy
-Udieresis-cy
-Uhungarumlaut-cy
-Chedieresis-cy
-Yerudieresis-cy
-Qa-cy
-We-cy
-gedescender-cy
-gestroke-cy
-gemiddlehook-cy
-yat-cy
-yusbig-cy
-fita-cy
-izhitsa-cy
-zhedescender-cy
-zedescender-cy
-kadescender-cy
-kaverticalstroke-cy
-kabashkir-cy
-endescender-cy
-enge-cy
-esdescender-cy
-ustraight-cy
-ustraightstroke-cy
-hadescender-cy
-chedescender-cy
-cheverticalstroke-cy
-shha-cy
-palochka-cy
 zhebreve-cy
+Chekhakassian-cy
 chekhakassian-cy
+palochka-cy
+Abreve-cy
 abreve-cy
+Adieresis-cy
 adieresis-cy
+Aie-cy
 aie-cy
+Iebreve-cy
 iebreve-cy
+Schwa-cy
 schwa-cy
+Zhedieresis-cy
 zhedieresis-cy
+Zedieresis-cy
 zedieresis-cy
+Imacron-cy
 imacron-cy
+Idieresis-cy
 idieresis-cy
+Odieresis-cy
 odieresis-cy
+Obarred-cy
 obarred-cy
+Umacron-cy
 umacron-cy
+Udieresis-cy
 udieresis-cy
+Uhungarumlaut-cy
 uhungarumlaut-cy
+Chedieresis-cy
 chedieresis-cy
+Gedescender-cy
+gedescender-cy
+Yerudieresis-cy
 yerudieresis-cy
+Qa-cy
 qa-cy
+We-cy
 we-cy
+tugrik
 hryvnia
 tenge
-tugrik
 brevecomb-cy
-dieresiscomb
-gravecomb
-acutecomb
-hungarumlautcomb
-macroncomb
-apostrophemod
+gestroke-cy.loclBSH
+yu-cy.loclBGR
+Gestroke-cy.loclBSH
+De-cy.loclBGR
+Ii-cy.loclBGR
+Iishort-cy.loclBGR
+Iigrave-cy.loclBGR
+El-cy.loclBGR
+Ef-cy.loclBGR
+Zedescender-cy.loclBSH
+Esdescender-cy.loclBSH
+Esdescender-cy.loclCHU
+ve-cy.loclBGR
+ge-cy.loclBGR
+de-cy.loclBGR
+zhe-cy.loclBGR
+ze-cy.loclBGR
+ii-cy.loclBGR
+iishort-cy.loclBGR
+iigrave-cy.loclBGR
+ka-cy.loclBGR
+el-cy.loclBGR
+en-cy.loclBGR
+pe-cy.loclBGR
+te-cy.loclBGR
+che-cy.loclBGR
+tse-cy.loclBGR
+sha-cy.loclBGR
+shcha-cy.loclBGR
+softsign-cy.loclBGR
+hardsign-cy.loclBGR
+zedescender-cy.loclBSH
+esdescender-cy.loclBSH
+esdescender-cy.loclCHU
+be-cy.loclSRB
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Cyrillic_Pro.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-Gemiddlehook-cy
-gemiddlehook-cy
+# This file is auto-generated; do not edit. See /README.md for instructions.
 Iishorttail-cy
-Kastroke-cy
-Pedescender-cy
-Haabkhasian-cy
-Tedescender-cy
-Tetse-cy
-Shhadescender-cy
-Cheabkhasian-cy
-Chedescenderabkhasian-cy
-Kahook-cy
-Eltail-cy
-Enhook-cy
-Entail-cy
-Emtail-cy
-Schwadieresis-cy
-Dzeabkhasian-cy
-Obarreddieresis-cy
-Edieresis-cy
-Gestrokehook-cy
-Hahook-cy
-Hastroke-cy
-Reversedze-cy
-Elhook-cy
+iishorttail-cy
 Semisoftsign-cy
+semisoftsign-cy
 Ertick-cy
-EnLeftHook-cy
-Eldescender-cy
-iishorttail-cy
+ertick-cy
+Ghemiddlehook-cy
+ghemiddlehook-cy
+Kastroke-cy
 kastroke-cy
-pedescender-cy
+Haabkhasian-cy
 haabkhasian-cy
+Tedescender-cy
 tedescender-cy
+Tetse-cy
 tetse-cy
-shhadescender-cy
+Cheabkhasian-cy
 cheabkhasian-cy
+Chedescenderabkhasian-cy
 chedescenderabkhasian-cy
+Kahook-cy
 kahook-cy
+Eltail-cy
 eltail-cy
+Enhook-cy
 enhook-cy
+Entail-cy
 entail-cy
+Emtail-cy
 emtail-cy
+Schwadieresis-cy
 schwadieresis-cy
+Dzeabkhasian-cy
 dzeabkhasian-cy
+Obarreddieresis-cy
 obarreddieresis-cy
+Edieresis-cy
 edieresis-cy
+Gestrokehook-cy
 gestrokehook-cy
+Hahook-cy
 hahook-cy
+Hastroke-cy
 hastroke-cy
+Reversedze-cy
 reversedze-cy
+Elhook-cy
 elhook-cy
-semisoftsign-cy
-ertick-cy
+Pedescender-cy
+pedescender-cy
+Shhadescender-cy
+shhadescender-cy
+EnLeftHook-cy
 enlefthook-cy
+Eldescender-cy
 eldescender-cy
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs` & `glyphsets-1.0.0/data/results/glyphs/GF_Latin_Plus.glyphs`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,28 @@
 {
-.appVersion = "3124";
+.appVersion = "3257";
 .formatVersion = 3;
-date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Greek Archaic";
-featurePrefixes = (
-{
-automatic = 1;
-code = "languagesystem DFLT dflt;
-
-languagesystem latn dflt;
-languagesystem latn AZE;
-languagesystem latn CRT;
-languagesystem latn KAZ;
-languagesystem latn TAT;
-languagesystem latn TRK;
-languagesystem latn ROM;
-languagesystem latn MOL;
-languagesystem latn CAT;
-";
-name = Languagesystems;
-}
-);
-features = (
-{
-automatic = 1;
-code = "feature locl;
-feature ordn;
-feature case;
-";
-tag = aalt;
-},
-{
-automatic = 1;
-code = "lookup ccmp_Other_1 {
-	@CombiningTopAccents = [acutecomb brevecomb caroncomb circumflexcomb commaturnedabovecomb dieresiscomb dotaccentcomb gravecomb hungarumlautcomb macroncomb ringcomb tildecomb];
-	@CombiningNonTopAccents = [cedillacomb ogonekcomb];
-	sub [i j]' @CombiningTopAccents by [idotless jdotless];
-	sub [i j]' @CombiningNonTopAccents @CombiningTopAccents by [idotless jdotless];
-} ccmp_Other_1;
-";
-tag = ccmp;
-},
-{
-automatic = 1;
-code = "lookup locl_latn_0 {
-	script latn;
-	language AZE;
-	sub i by idotaccent;
-	language CRT;
-	sub i by idotaccent;
-	language KAZ;
-	sub i by idotaccent;
-	language TAT;
-	sub i by idotaccent;
-	language TRK;
-	sub i by idotaccent;
-} locl_latn_0;
-
-lookup locl_latn_1 {
-	script latn;
-	language ROM;
-	sub Scedilla by Scommaaccent;
-	sub scedilla by scommaaccent;
-	language MOL;
-	sub Scedilla by Scommaaccent;
-	sub scedilla by scommaaccent;
-} locl_latn_1;
-
-lookup locl_latn_2 {
-	script latn;
-	language CAT;
-	sub l periodcentered' l by periodcentered.loclCAT;
-	sub L periodcentered' L by periodcentered.loclCAT.case;
-} locl_latn_2;
-";
-tag = locl;
-},
-{
-automatic = 1;
-code = "sub [zero one two three four five six seven eight nine] [A a]' by ordfeminine;
-sub [zero one two three four five six seven eight nine] [O o]' by ordmasculine;
-";
-tag = ordn;
-},
-{
-automatic = 1;
-code = "sub periodcentered.loclCAT by periodcentered.loclCAT.case;
-";
-tag = case;
+axes = (
+{
+name = Weight;
+tag = wght;
+},
+{
+name = Width;
+tag = wdth;
 }
 );
+date = "2023-12-13 14:28:10 +0000";
+familyName = GF_Latin_Plus;
 fontMaster = (
 {
+axesValues = (
+100,
+100
+);
 id = m01;
 metricValues = (
 {
 over = 16;
 pos = 800;
 },
 {
@@ -110,1452 +37,1504 @@
 over = -16;
 },
 {
 over = -16;
 pos = -200;
 },
 {
-over = -16;
+over = 0;
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-glyphname = Heta;
+glyphname = baht;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 880;
+unicode = 3647;
 },
 {
-glyphname = Archaicsampi;
+glyphname = minute;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 882;
+unicode = 8242;
 },
 {
-glyphname = Pamphyliandigamma;
+glyphname = second;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 886;
+unicode = 8243;
 },
 {
-glyphname = KoppaArchaic;
+glyphname = brokenbar;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 984;
+unicode = 166;
 },
 {
-glyphname = UpsilonhookSymbol;
+glyphname = dagger;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 978;
+unicode = 8224;
 },
 {
-glyphname = UpsilonacutehookSymbol;
+glyphname = literSign;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 979;
+unicode = 8467;
 },
 {
-glyphname = UpsilondieresishookSymbol;
+glyphname = daggerdbl;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 980;
+unicode = 8225;
 },
 {
-glyphname = ThetaSymbol;
+glyphname = estimated;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1012;
+unicode = 8494;
 },
 {
-glyphname = Sho;
+glyphname = numero;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1015;
+unicode = 8470;
 },
 {
-glyphname = SigmaLunateSymbol;
+glyphname = bitcoin;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1017;
+unicode = 8383;
 },
 {
-glyphname = San;
+glyphname = cedi;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1018;
+unicode = 8373;
 },
 {
-glyphname = SigmaLunateReversedSymbol;
+glyphname = colonsign;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1021;
+unicode = 8353;
 },
 {
-glyphname = SigmaLunateDottedSymbol;
+glyphname = dong;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1022;
+unicode = 8363;
 },
 {
-glyphname = SigmaLunateDottedReversedSymbol;
+glyphname = guarani;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1023;
+unicode = 8370;
 },
 {
-glyphname = heta;
+glyphname = hryvnia;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 881;
+unicode = 8372;
 },
 {
-glyphname = archaicsampi;
+glyphname = kip;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 883;
+unicode = 8365;
 },
 {
-glyphname = pamphyliandigamma;
+glyphname = lari;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 887;
+unicode = 8382;
 },
 {
-glyphname = sigmaLunateReversedSymbol;
+glyphname = liraTurkish;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 891;
+unicode = 8378;
 },
 {
-glyphname = sigmaLunateDottedSymbol;
+glyphname = manat;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 892;
+unicode = 8380;
 },
 {
-glyphname = sigmaLunateDottedReversedSymbol;
+glyphname = naira;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 893;
+unicode = 8358;
 },
 {
-glyphname = koppaArchaic;
+glyphname = peso;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 985;
+unicode = 8369;
 },
 {
-glyphname = betaSymbol;
+glyphname = ruble;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 976;
+unicode = 8381;
 },
 {
-glyphname = thetaSymbol;
+glyphname = rupee;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 977;
+unicode = 8360;
 },
 {
-glyphname = phiSymbol;
+glyphname = rupeeIndian;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 981;
+unicode = 8377;
 },
 {
-glyphname = piSymbol;
+glyphname = sheqel;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 982;
+unicode = 8362;
 },
 {
-glyphname = kappaSymbol;
+glyphname = tenge;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1008;
+unicode = 8376;
 },
 {
-glyphname = rhoSymbol;
+glyphname = tugrik;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1009;
+unicode = 8366;
 },
 {
-glyphname = sigmaLunateSymbol;
+glyphname = won;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1010;
+unicode = 8361;
 },
 {
-glyphname = yot;
+glyphname = notequal;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1011;
+unicode = 8800;
 },
 {
-glyphname = epsilonLunateSymbol;
+glyphname = greaterequal;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1013;
+unicode = 8805;
 },
 {
-glyphname = sho;
+glyphname = lessequal;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1016;
+unicode = 8804;
 },
 {
-glyphname = san;
+glyphname = plusminus;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1019;
+unicode = 177;
 },
 {
-glyphname = rhoStrokeSymbol;
+glyphname = approxequal;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1020;
+unicode = 8776;
 },
 {
-glyphname = "onequarter-atticGreek";
+glyphname = logicalnot;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65856;
+unicode = 172;
 },
 {
-glyphname = "onehalf-atticGreek";
+glyphname = emptyset;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65857;
+unicode = 8709;
 },
 {
-glyphname = "onedrachma-atticGreek";
+glyphname = "infinity";
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65858;
+unicode = 8734;
 },
 {
-glyphname = "five-atticGreek";
+glyphname = integral;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65859;
+unicode = 8747;
 },
 {
-glyphname = "fifty-atticGreek";
+glyphname = Ohm;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65860;
+unicode = 8486;
 },
 {
-glyphname = "fivehundred-atticGreek";
+glyphname = increment;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65861;
+unicode = 8710;
 },
 {
-glyphname = "fivethousand-atticGreek";
+glyphname = product;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65862;
+unicode = 8719;
 },
 {
-glyphname = "fiftythousand-atticGreek";
+glyphname = summation;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65863;
+unicode = 8721;
 },
 {
-glyphname = "fivetalents-atticGreek";
+glyphname = radical;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65864;
+unicode = 8730;
 },
 {
-glyphname = "tentalents-atticGreek";
+glyphname = micro;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65865;
+unicode = 181;
 },
 {
-glyphname = "fiftytalents-atticGreek";
+glyphname = partialdiff;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65866;
+unicode = 8706;
 },
 {
-glyphname = "onehundredtalents-atticGreek";
+glyphname = perthousand;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65867;
+unicode = 8240;
 },
 {
-glyphname = "fivehundredtalents-atticGreek";
+glyphname = upArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65868;
+unicode = 8593;
 },
 {
-glyphname = "onethousandtalents-atticGreek";
+glyphname = northEastArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65869;
+unicode = 8599;
 },
 {
-glyphname = "fivethousandtalents-atticGreek";
+glyphname = rightArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65870;
+unicode = 8594;
 },
 {
-glyphname = "fivestaters-atticGreek";
+glyphname = southEastArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65871;
+unicode = 8600;
 },
 {
-glyphname = "tenstaters-atticGreek";
+glyphname = downArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65872;
+unicode = 8595;
 },
 {
-glyphname = "fiftystaters-atticGreek";
+glyphname = southWestArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65873;
+unicode = 8601;
 },
 {
-glyphname = "onehundredstaters-atticGreek";
+glyphname = leftArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65874;
+unicode = 8592;
 },
 {
-glyphname = "fivehundredstaters-atticGreek";
+glyphname = northWestArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65875;
+unicode = 8598;
 },
 {
-glyphname = "onethousandstaters-atticGreek";
+glyphname = leftRightArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65876;
+unicode = 8596;
 },
 {
-glyphname = "tenthousandstaters-atticGreek";
+glyphname = upDownArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65877;
+unicode = 8597;
 },
 {
-glyphname = "fiftythousandstaters-atticGreek";
+glyphname = blackCircle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65878;
+unicode = 9679;
 },
 {
-glyphname = "tenmnas-atticGreek";
+glyphname = whiteCircle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65879;
+unicode = 9675;
 },
 {
-glyphname = "heraeumoneplethron-ancientGreek";
+glyphname = whiteBullet;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65880;
+unicode = 9702;
 },
 {
-glyphname = "thespianone-ancientGreek";
+glyphname = blackDiamond;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65881;
+unicode = 9670;
 },
 {
-glyphname = "hermionianone-ancientGreek";
+glyphname = whiteDiamond;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65882;
+unicode = 9671;
 },
 {
-glyphname = "epidaureantwo-ancientGreek";
+glyphname = lozenge;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65883;
+unicode = 9674;
 },
 {
-glyphname = "thespiantwo-ancientGreek";
+glyphname = blackSquare;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65884;
+unicode = 9632;
 },
 {
-glyphname = "cyrenaictwodrachmas-ancientGreek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65885;
-},
-{
-glyphname = "epidaureantwodrachmas-ancientGreek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65886;
-},
-{
-glyphname = "troezenianfive-ancientGreek";
+glyphname = whiteSquare;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65887;
+unicode = 9633;
 },
 {
-glyphname = "troezenianten-ancientGreek";
+glyphname = blackSmallSquare;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65888;
+unicode = 9642;
 },
 {
-glyphname = "troezeniantenalternateform-ancientGreek";
+glyphname = whiteSmallSquare;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65889;
+unicode = 9643;
 },
 {
-glyphname = "hermionianten-ancientGreek";
+glyphname = upBlackTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65890;
+unicode = 9650;
 },
 {
-glyphname = "messenianten-ancientGreek";
+glyphname = rightBlackTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65891;
+unicode = 9654;
 },
 {
-glyphname = "thespianten-ancientGreek";
+glyphname = downBlackTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65892;
+unicode = 9660;
 },
 {
-glyphname = "thespianthirty-ancientGreek";
+glyphname = leftBlackTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65893;
+unicode = 9664;
 },
 {
-glyphname = "troezenianfifty-ancientGreek";
+glyphname = upWhiteTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65894;
+unicode = 9651;
 },
 {
-glyphname = "troezenianfiftyalternateform-ancientGreek";
+glyphname = rightWhiteTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65895;
+unicode = 9655;
 },
 {
-glyphname = "hermionianfifty-ancientGreek";
+glyphname = downWhiteTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65896;
+unicode = 9661;
 },
 {
-glyphname = "thespianfifty-ancientGreek";
+glyphname = leftWhiteTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65897;
+unicode = 9665;
 },
 {
-glyphname = "thespianonehundred-ancientGreek";
+glyphname = upBlackSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65898;
+unicode = 9652;
 },
 {
-glyphname = "thespianthreehundred-ancientGreek";
+glyphname = rightBlackSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65899;
+unicode = 9656;
 },
 {
-glyphname = "epidaureanfivehundred-ancientGreek";
+glyphname = downBlackSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65900;
+unicode = 9662;
 },
 {
-glyphname = "troezenianfivehundred-ancientGreek";
+glyphname = leftBlackSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65901;
+unicode = 9666;
 },
 {
-glyphname = "thespianfivehundred-ancientGreek";
+glyphname = upWhiteSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65902;
+unicode = 9653;
 },
 {
-glyphname = "carystianfivehundred-ancientGreek";
+glyphname = rightWhiteSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65903;
+unicode = 9657;
 },
 {
-glyphname = "naxianfivehundred-ancientGreek";
+glyphname = downWhiteSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65904;
+unicode = 9663;
 },
 {
-glyphname = "thespianonethousand-ancientGreek";
+glyphname = leftWhiteSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65905;
+unicode = 9667;
 },
 {
-glyphname = "thespianfivethousand-ancientGreek";
+glyphname = "leftanglebracket-math";
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65906;
+unicode = 10216;
 },
 {
-glyphname = "delphicfivemnas-ancientGreek";
+glyphname = "rightanglebracket-math";
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65907;
+unicode = 10217;
 },
 {
-glyphname = "stratianfiftymnas-ancientGreek";
+glyphname = dblverticalbar;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65908;
+unicode = 8214;
 },
 {
-glyphname = "onehalf-greek";
+glyphname = zero.zero;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65909;
 },
 {
-glyphname = "onehalfAlternate-greek";
+glyphname = zero.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65910;
 },
 {
-glyphname = "twothirds-greek";
+glyphname = one.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65911;
 },
 {
-glyphname = "threequarters-greek";
+glyphname = two.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65912;
 },
 {
-glyphname = "zero-greek";
+glyphname = three.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65930;
 },
 {
-glyphname = "year-greek";
+glyphname = four.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65913;
 },
 {
-glyphname = "talent-greek";
+glyphname = five.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65914;
 },
 {
-glyphname = "drachma-greek";
+glyphname = six.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65915;
 },
 {
-glyphname = "obol-greek";
+glyphname = seven.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65916;
 },
 {
-glyphname = "twoObols-greek";
+glyphname = eight.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65917;
 },
 {
-glyphname = "threeObols-greek";
+glyphname = nine.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65918;
 },
 {
-glyphname = "fourObols-greek";
+glyphname = zero.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65919;
 },
 {
-glyphname = "fiveObols-greek";
+glyphname = one.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65920;
 },
 {
-glyphname = "metretes-greek";
+glyphname = two.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65921;
 },
 {
-glyphname = "kyathosBase-greek";
+glyphname = three.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65922;
 },
 {
-glyphname = "litra-greek";
+glyphname = four.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65923;
 },
 {
-glyphname = "ounkia-greek";
+glyphname = five.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65924;
 },
 {
-glyphname = "xestes-greek";
+glyphname = six.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65925;
 },
 {
-glyphname = "artabe-greek";
+glyphname = seven.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65926;
 },
 {
-glyphname = "aroura-greek";
+glyphname = eight.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65927;
 },
 {
-glyphname = "gramma-greek";
+glyphname = nine.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65928;
 },
 {
-glyphname = "tryblionBase-greek";
+glyphname = zero.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65929;
 },
 {
-glyphname = epsilonLunateReversedSymbol;
+glyphname = one.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1014;
 },
 {
-glyphname = sunSymbol;
+glyphname = two.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9737;
 },
 {
-glyphname = blackstar;
+glyphname = three.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9733;
 },
 {
-glyphname = ascendingNode;
+glyphname = four.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9738;
 },
 {
-glyphname = descendingNode;
+glyphname = five.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9739;
 },
 {
-glyphname = conjunction;
+glyphname = six.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9740;
 },
 {
-glyphname = opposition;
+glyphname = seven.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9741;
 },
 {
-glyphname = constantineCross;
+glyphname = eight.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9767;
 },
 {
-glyphname = jerusalemCross;
+glyphname = nine.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9769;
 },
 {
-glyphname = firstQuarterMoon;
+glyphname = fraction;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9789;
+unicode = 8260;
 },
 {
-glyphname = lastQuarterMoon;
+glyphname = onehalf;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9790;
+unicode = 189;
 },
 {
-glyphname = mercury;
+glyphname = onethird;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9791;
+unicode = 8531;
 },
 {
-glyphname = venus;
+glyphname = twothirds;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9792;
+unicode = 8532;
 },
 {
-glyphname = earth;
+glyphname = onequarter;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9793;
+unicode = 188;
 },
 {
-glyphname = mars;
+glyphname = threequarters;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9794;
+unicode = 190;
 },
 {
-glyphname = jupiter;
+glyphname = oneinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9795;
+unicode = 8321;
 },
 {
-glyphname = saturn;
+glyphname = twoinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9796;
+unicode = 8322;
 },
 {
-glyphname = uranus;
+glyphname = threeinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9797;
+unicode = 8323;
 },
 {
-glyphname = neptune;
+glyphname = fourinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9798;
+unicode = 8324;
 },
 {
-glyphname = pluto;
+glyphname = fiveinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9799;
+unicode = 8325;
 },
 {
-glyphname = aries;
+glyphname = sixinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9800;
+unicode = 8326;
 },
 {
-glyphname = taurus;
+glyphname = seveninferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9801;
+unicode = 8327;
 },
 {
-glyphname = gemini;
+glyphname = eightinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9802;
+unicode = 8328;
 },
 {
-glyphname = cancer;
+glyphname = nineinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9803;
+unicode = 8329;
 },
 {
-glyphname = leo;
+glyphname = onesuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9804;
+unicode = 185;
 },
 {
-glyphname = virgo;
+glyphname = twosuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9805;
+unicode = 178;
 },
 {
-glyphname = libra;
+glyphname = threesuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9806;
+unicode = 179;
 },
 {
-glyphname = scorpius;
+glyphname = foursuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9807;
+unicode = 8308;
 },
 {
-glyphname = sagittarius;
+glyphname = fivesuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9808;
+unicode = 8309;
 },
 {
-glyphname = capricorn;
+glyphname = sixsuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9809;
+unicode = 8310;
 },
 {
-glyphname = aquarius;
+glyphname = sevensuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9810;
+unicode = 8311;
 },
 {
-glyphname = pisces;
+glyphname = eightsuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 9811;
+unicode = 8312;
 },
 {
-glyphname = threeDimensionalAngle;
+glyphname = ninesuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 10176;
+unicode = 8313;
 },
 {
-glyphname = whitetrianglecontainingwhitetriangle;
+glyphname = pi;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 10177;
-},
-{
-glyphname = whiteSquare;
-layers = (
-{
-layerId = m01;
-width = 600;
+unicode = 960;
 }
 );
-unicode = 9633;
-}
+instances = (
 );
+kerningLTR = {
+};
 metrics = (
 {
 type = ascender;
 },
 {
 type = "cap height";
 },
@@ -1568,11 +1547,13 @@
 {
 type = descender;
 },
 {
 type = "italic angle";
 }
 );
+stems = (
+);
 unitsPerEm = 1000;
 versionMajor = 1;
 versionMinor = 0;
 }
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs` & `glyphsets-1.0.0/data/definitions/per_glyphset/GF_Greek_Plus.stub.glyphs`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 {
-.appVersion = "3124";
+.appVersion = "3239";
 .formatVersion = 3;
+axes = (
+{
+name = Weight;
+tag = wght;
+},
+{
+name = Width;
+tag = wdth;
+}
+);
 date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Greek Coptic";
+familyName = "GF Greek Plus";
 featurePrefixes = (
 {
 automatic = 1;
 code = "languagesystem DFLT dflt;
 
 languagesystem latn dflt;
 languagesystem latn AZE;
@@ -88,14 +98,18 @@
 code = "sub periodcentered.loclCAT by periodcentered.loclCAT.case;
 ";
 tag = case;
 }
 );
 fontMaster = (
 {
+axesValues = (
+100,
+100
+);
 id = m01;
 metricValues = (
 {
 over = 16;
 pos = 800;
 },
 {
@@ -110,1380 +124,1221 @@
 over = -16;
 },
 {
 over = -16;
 pos = -200;
 },
 {
-over = -16;
+over = 0;
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-glyphname = "Alfa-coptic";
-layers = (
+glyphname = perispomenicomb;
+unicode = 834;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11392;
+glyphname = koroniscomb;
+unicode = 835;
 },
 {
-glyphname = "Vida-coptic";
-layers = (
+glyphname = dialytikatonoscomb;
+unicode = 836;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11394;
+glyphname = ypogegrammenicomb;
+unicode = 837;
 },
 {
-glyphname = "Gamma-coptic";
-layers = (
+glyphname = koronis;
+unicode = 8125;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11396;
+glyphname = psili;
+unicode = 8127;
 },
 {
-glyphname = "Dalda-coptic";
-layers = (
+glyphname = perispomeni;
+unicode = 8128;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11398;
+glyphname = dialytikaperispomeni;
+unicode = 8129;
 },
 {
-glyphname = "Eie-coptic";
-layers = (
+glyphname = psilivaria;
+unicode = 8141;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11400;
+glyphname = psilioxia;
+unicode = 8142;
 },
 {
-glyphname = "Sou-coptic";
-layers = (
+glyphname = psiliperispomeni;
+unicode = 8143;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11402;
+glyphname = dasiavaria;
+unicode = 8157;
 },
 {
-glyphname = "Zata-coptic";
-layers = (
+glyphname = dasiaoxia;
+unicode = 8158;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11404;
+glyphname = dasiaperispomeni;
+unicode = 8159;
 },
 {
-glyphname = "Hate-coptic";
-layers = (
+glyphname = dialytikavaria;
+unicode = 8173;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11406;
+glyphname = dialytikaoxia;
+unicode = 8174;
 },
 {
-glyphname = "Thethe-coptic";
-layers = (
+glyphname = varia;
+unicode = 8175;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11408;
+glyphname = oxia;
+unicode = 8189;
 },
 {
-glyphname = "Iauda-coptic";
+glyphname = dasia;
+unicode = 8190;
+},
+{
+glyphname = Alphaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11410;
 },
 {
-glyphname = "Kapa-coptic";
+glyphname = Alphapsiliprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11412;
 },
 {
-glyphname = "Laula-coptic";
+glyphname = Alphadasiaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11414;
 },
 {
-glyphname = "Mi-coptic";
+glyphname = Alphapsilivariaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11416;
 },
 {
-glyphname = "Ni-coptic";
+glyphname = Alphadasiavariaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11418;
 },
 {
-glyphname = "Ksi-coptic";
+glyphname = Alphapsilioxiaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11420;
 },
 {
-glyphname = "O-coptic";
+glyphname = Alphadasiaoxiaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11422;
 },
 {
-glyphname = "Pi-coptic";
+glyphname = Alphapsiliperispomeniprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11424;
 },
 {
-glyphname = "Ro-coptic";
+glyphname = Alphadasiaperispomeniprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11426;
 },
 {
-glyphname = "Sima-coptic";
+glyphname = Etaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11428;
 },
 {
-glyphname = "Tau-coptic";
+glyphname = Etapsiliprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11430;
 },
 {
-glyphname = "Ua-coptic";
+glyphname = Etadasiaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11432;
 },
 {
-glyphname = "Fi-coptic";
+glyphname = Etapsilivariaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11434;
 },
 {
-glyphname = "Khi-coptic";
+glyphname = Etadasiavariaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11436;
 },
 {
-glyphname = "Psi-coptic";
+glyphname = Etapsilioxiaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11438;
 },
 {
-glyphname = "Oou-coptic";
+glyphname = Etadasiaoxiaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11440;
 },
 {
-glyphname = "Cryptogrammiceie-coptic";
+glyphname = Etapsiliperispomeniprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11446;
 },
 {
-glyphname = "dialectPkapa-coptic";
+glyphname = Etadasiaperispomeniprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11448;
 },
 {
-glyphname = "dialectPni-coptic";
+glyphname = Omegaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11450;
 },
 {
-glyphname = "Cryptogrammicni-coptic";
+glyphname = Omegapsiliprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11452;
 },
 {
-glyphname = "OouOld-coptic";
+glyphname = Omegadasiaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11454;
 },
 {
-glyphname = "Sampi-coptic";
+glyphname = Omegapsilivariaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11456;
 },
 {
-glyphname = "Shei-coptic";
+glyphname = Omegadasiavariaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 994;
 },
 {
-glyphname = "SheiCryptogrammic-coptic";
+glyphname = Omegapsilioxiaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11499;
 },
 {
-glyphname = "SheiCrossed-coptic";
+glyphname = Omegadasiaoxiaprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11458;
 },
 {
-glyphname = "SheiOld-coptic";
+glyphname = Omegapsiliperispomeniprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11460;
 },
 {
-glyphname = "EshOld-coptic";
+glyphname = Omegadasiaperispomeniprosgegrammeni.ss01;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11462;
 },
 {
-glyphname = "Fei-coptic";
-layers = (
+glyphname = ypogegrammeni;
+unicode = 890;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 996;
+glyphname = alphapsili;
+unicode = 7936;
 },
 {
-glyphname = "Khei-coptic";
-layers = (
+glyphname = alphadasia;
+unicode = 7937;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 998;
+glyphname = alphapsilivaria;
+unicode = 7938;
 },
 {
-glyphname = "KheiBohairic-coptic";
-layers = (
+glyphname = alphadasiavaria;
+unicode = 7939;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11506;
+glyphname = alphapsilioxia;
+unicode = 7940;
 },
 {
-glyphname = "KheiAkhmimic-coptic";
-layers = (
+glyphname = alphadasiaoxia;
+unicode = 7941;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11464;
+glyphname = alphapsiliperispomeni;
+unicode = 7942;
 },
 {
-glyphname = "Hori-coptic";
-layers = (
+glyphname = alphadasiaperispomeni;
+unicode = 7943;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1000;
+glyphname = Alphapsili;
+unicode = 7944;
 },
 {
-glyphname = "HoriDialectP-coptic";
-layers = (
+glyphname = Alphadasia;
+unicode = 7945;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11466;
+glyphname = Alphapsilivaria;
+unicode = 7946;
 },
 {
-glyphname = "HoriOld-coptic";
-layers = (
+glyphname = Alphadasiavaria;
+unicode = 7947;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11468;
+glyphname = Alphapsilioxia;
+unicode = 7948;
 },
 {
-glyphname = "HaOld-coptic";
-layers = (
+glyphname = Alphadasiaoxia;
+unicode = 7949;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11470;
+glyphname = Alphapsiliperispomeni;
+unicode = 7950;
 },
 {
-glyphname = "HaLshaped-coptic";
-layers = (
+glyphname = Alphadasiaperispomeni;
+unicode = 7951;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11472;
+glyphname = epsilonpsili;
+unicode = 7952;
 },
 {
-glyphname = "HeiOld-coptic";
-layers = (
+glyphname = epsilondasia;
+unicode = 7953;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11474;
+glyphname = epsilonpsilivaria;
+unicode = 7954;
 },
 {
-glyphname = "HatOld-coptic";
-layers = (
+glyphname = epsilondasiavaria;
+unicode = 7955;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11476;
+glyphname = epsilonpsilioxia;
+unicode = 7956;
 },
 {
-glyphname = "Gangia-coptic";
-layers = (
+glyphname = epsilondasiaoxia;
+unicode = 7957;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1002;
+glyphname = Epsilonpsili;
+unicode = 7960;
 },
 {
-glyphname = "GangiaCryptogrammic-coptic";
-layers = (
+glyphname = Epsilondasia;
+unicode = 7961;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11501;
+glyphname = Epsilonpsilivaria;
+unicode = 7962;
 },
 {
-glyphname = "GangiaOld-coptic";
-layers = (
+glyphname = Epsilondasiavaria;
+unicode = 7963;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11478;
+glyphname = Epsilonpsilioxia;
+unicode = 7964;
 },
 {
-glyphname = "Shima-coptic";
-layers = (
+glyphname = Epsilondasiaoxia;
+unicode = 7965;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1004;
+glyphname = etapsili;
+unicode = 7968;
 },
 {
-glyphname = "DjaOld-coptic";
-layers = (
+glyphname = etadasia;
+unicode = 7969;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11480;
+glyphname = etapsilivaria;
+unicode = 7970;
 },
 {
-glyphname = "ShimaOld-coptic";
-layers = (
+glyphname = etadasiavaria;
+unicode = 7971;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11482;
+glyphname = etapsilioxia;
+unicode = 7972;
 },
 {
-glyphname = "Dei-coptic";
-layers = (
+glyphname = etadasiaoxia;
+unicode = 7973;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1006;
+glyphname = etapsiliperispomeni;
+unicode = 7974;
 },
 {
-glyphname = "AlefDialectP-coptic";
-layers = (
+glyphname = etadasiaperispomeni;
+unicode = 7975;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11442;
+glyphname = Etapsili;
+unicode = 7976;
 },
 {
-glyphname = "AinOld-coptic";
-layers = (
+glyphname = Etadasia;
+unicode = 7977;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11444;
+glyphname = Etapsilivaria;
+unicode = 7978;
 },
 {
-glyphname = "alfa-coptic";
-layers = (
+glyphname = Etadasiavaria;
+unicode = 7979;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11393;
+glyphname = Etapsilioxia;
+unicode = 7980;
 },
 {
-glyphname = "vida-coptic";
-layers = (
+glyphname = Etadasiaoxia;
+unicode = 7981;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11395;
+glyphname = Etapsiliperispomeni;
+unicode = 7982;
 },
 {
-glyphname = "gamma-coptic";
-layers = (
+glyphname = Etadasiaperispomeni;
+unicode = 7983;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11397;
+glyphname = iotapsili;
+unicode = 7984;
 },
 {
-glyphname = "dalda-coptic";
-layers = (
+glyphname = iotadasia;
+unicode = 7985;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11399;
+glyphname = iotapsilivaria;
+unicode = 7986;
 },
 {
-glyphname = "eie-coptic";
-layers = (
+glyphname = iotadasiavaria;
+unicode = 7987;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11401;
+glyphname = iotapsilioxia;
+unicode = 7988;
 },
 {
-glyphname = "sou-coptic";
-layers = (
+glyphname = iotadasiaoxia;
+unicode = 7989;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11403;
+glyphname = iotapsiliperispomeni;
+unicode = 7990;
 },
 {
-glyphname = "zata-coptic";
-layers = (
+glyphname = iotadasiaperispomeni;
+unicode = 7991;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11405;
+glyphname = Iotapsili;
+unicode = 7992;
 },
 {
-glyphname = "hate-coptic";
-layers = (
+glyphname = Iotadasia;
+unicode = 7993;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11407;
+glyphname = Iotapsilivaria;
+unicode = 7994;
 },
 {
-glyphname = "thethe-coptic";
-layers = (
+glyphname = Iotadasiavaria;
+unicode = 7995;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11409;
+glyphname = Iotapsilioxia;
+unicode = 7996;
 },
 {
-glyphname = "iauda-coptic";
-layers = (
+glyphname = Iotadasiaoxia;
+unicode = 7997;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11411;
+glyphname = Iotapsiliperispomeni;
+unicode = 7998;
 },
 {
-glyphname = "kapa-coptic";
-layers = (
+glyphname = Iotadasiaperispomeni;
+unicode = 7999;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11413;
+glyphname = omicronpsili;
+unicode = 8000;
 },
 {
-glyphname = "laula-coptic";
-layers = (
+glyphname = omicrondasia;
+unicode = 8001;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11415;
+glyphname = omicronpsilivaria;
+unicode = 8002;
 },
 {
-glyphname = "mi-coptic";
-layers = (
+glyphname = omicrondasiavaria;
+unicode = 8003;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11417;
+glyphname = omicronpsilioxia;
+unicode = 8004;
 },
 {
-glyphname = "ni-coptic";
-layers = (
+glyphname = omicrondasiaoxia;
+unicode = 8005;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11419;
+glyphname = Omicronpsili;
+unicode = 8008;
 },
 {
-glyphname = "ksi-coptic";
-layers = (
+glyphname = Omicrondasia;
+unicode = 8009;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11421;
+glyphname = Omicronpsilivaria;
+unicode = 8010;
 },
 {
-glyphname = "o-coptic";
-layers = (
+glyphname = Omicrondasiavaria;
+unicode = 8011;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11423;
+glyphname = Omicronpsilioxia;
+unicode = 8012;
 },
 {
-glyphname = "pi-coptic";
-layers = (
+glyphname = Omicrondasiaoxia;
+unicode = 8013;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11425;
+glyphname = upsilonpsili;
+unicode = 8016;
 },
 {
-glyphname = "ro-coptic";
-layers = (
+glyphname = upsilondasia;
+unicode = 8017;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11427;
+glyphname = upsilonpsilivaria;
+unicode = 8018;
 },
 {
-glyphname = "sima-coptic";
-layers = (
+glyphname = upsilondasiavaria;
+unicode = 8019;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11429;
+glyphname = upsilonpsilioxia;
+unicode = 8020;
 },
 {
-glyphname = "tau-coptic";
-layers = (
+glyphname = upsilondasiaoxia;
+unicode = 8021;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11431;
+glyphname = upsilonpsiliperispomeni;
+unicode = 8022;
 },
 {
-glyphname = "ua-coptic";
-layers = (
+glyphname = upsilondasiaperispomeni;
+unicode = 8023;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11433;
+glyphname = Upsilondasia;
+unicode = 8025;
 },
 {
-glyphname = "fi-coptic";
-layers = (
+glyphname = Upsilondasiavaria;
+unicode = 8027;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11435;
+glyphname = Upsilondasiaoxia;
+unicode = 8029;
 },
 {
-glyphname = "khi-coptic";
-layers = (
+glyphname = Upsilondasiaperispomeni;
+unicode = 8031;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11437;
+glyphname = omegapsili;
+unicode = 8032;
 },
 {
-glyphname = "psi-coptic";
-layers = (
+glyphname = omegadasia;
+unicode = 8033;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11439;
+glyphname = omegapsilivaria;
+unicode = 8034;
 },
 {
-glyphname = "oou-coptic";
-layers = (
+glyphname = omegadasiavaria;
+unicode = 8035;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11441;
+glyphname = omegapsilioxia;
+unicode = 8036;
 },
 {
-glyphname = "cryptogrammiceie-coptic";
-layers = (
+glyphname = omegadasiaoxia;
+unicode = 8037;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11447;
+glyphname = omegapsiliperispomeni;
+unicode = 8038;
 },
 {
-glyphname = "dialectpkapa-coptic";
-layers = (
+glyphname = omegadasiaperispomeni;
+unicode = 8039;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11449;
+glyphname = Omegapsili;
+unicode = 8040;
 },
 {
-glyphname = "dialectpni-coptic";
-layers = (
+glyphname = Omegadasia;
+unicode = 8041;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11451;
+glyphname = Omegapsilivaria;
+unicode = 8042;
 },
 {
-glyphname = "cryptogrammicni-coptic";
-layers = (
+glyphname = Omegadasiavaria;
+unicode = 8043;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11453;
+glyphname = Omegapsilioxia;
+unicode = 8044;
 },
 {
-glyphname = "oouOld-coptic";
-layers = (
+glyphname = Omegadasiaoxia;
+unicode = 8045;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11455;
+glyphname = Omegapsiliperispomeni;
+unicode = 8046;
 },
 {
-glyphname = "sampi-coptic";
-layers = (
+glyphname = Omegadasiaperispomeni;
+unicode = 8047;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11457;
+glyphname = alphavaria;
+unicode = 8048;
 },
 {
-glyphname = "shei-coptic";
-layers = (
+glyphname = alphaoxia;
+unicode = 8049;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 995;
+glyphname = epsilonvaria;
+unicode = 8050;
 },
 {
-glyphname = "sheiCryptogrammic-coptic";
-layers = (
+glyphname = epsilonoxia;
+unicode = 8051;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11500;
+glyphname = etavaria;
+unicode = 8052;
 },
 {
-glyphname = "sheiCrossed-coptic";
-layers = (
+glyphname = etaoxia;
+unicode = 8053;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11459;
+glyphname = iotavaria;
+unicode = 8054;
 },
 {
-glyphname = "sheiOld-coptic";
-layers = (
+glyphname = iotaoxia;
+unicode = 8055;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11461;
+glyphname = omicronvaria;
+unicode = 8056;
 },
 {
-glyphname = "eshOld-coptic";
-layers = (
+glyphname = omicronoxia;
+unicode = 8057;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11463;
+glyphname = upsilonvaria;
+unicode = 8058;
 },
 {
-glyphname = "fei-coptic";
-layers = (
+glyphname = upsilonoxia;
+unicode = 8059;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 997;
+glyphname = omegavaria;
+unicode = 8060;
 },
 {
-glyphname = "khei-coptic";
-layers = (
+glyphname = omegaoxia;
+unicode = 8061;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 999;
+glyphname = alphapsiliypogegrammeni;
+unicode = 8064;
 },
 {
-glyphname = "kheiBohairic-coptic";
-layers = (
+glyphname = alphadasiaypogegrammeni;
+unicode = 8065;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11507;
+glyphname = alphapsilivariaypogegrammeni;
+unicode = 8066;
 },
 {
-glyphname = "kheiAkhmimic-coptic";
-layers = (
+glyphname = alphadasiavariaypogegrammeni;
+unicode = 8067;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11465;
+glyphname = alphapsilioxiaypogegrammeni;
+unicode = 8068;
 },
 {
-glyphname = "hori-coptic";
-layers = (
+glyphname = alphadasiaoxiaypogegrammeni;
+unicode = 8069;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1001;
+glyphname = alphapsiliperispomeniypogegrammeni;
+unicode = 8070;
 },
 {
-glyphname = "horiDialectP-coptic";
-layers = (
+glyphname = alphadasiaperispomeniypogegrammeni;
+unicode = 8071;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11467;
+glyphname = Alphapsiliprosgegrammeni;
+unicode = 8072;
 },
 {
-glyphname = "horiOld-coptic";
-layers = (
+glyphname = Alphadasiaprosgegrammeni;
+unicode = 8073;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11469;
+glyphname = Alphapsilivariaprosgegrammeni;
+unicode = 8074;
 },
 {
-glyphname = "haOld-coptic";
-layers = (
+glyphname = Alphadasiavariaprosgegrammeni;
+unicode = 8075;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11471;
+glyphname = Alphapsilioxiaprosgegrammeni;
+unicode = 8076;
 },
 {
-glyphname = "haLshaped-coptic";
-layers = (
+glyphname = Alphadasiaoxiaprosgegrammeni;
+unicode = 8077;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11473;
+glyphname = Alphapsiliperispomeniprosgegrammeni;
+unicode = 8078;
 },
 {
-glyphname = "heiOld-coptic";
-layers = (
+glyphname = Alphadasiaperispomeniprosgegrammeni;
+unicode = 8079;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11475;
+glyphname = etapsiliypogegrammeni;
+unicode = 8080;
 },
 {
-glyphname = "hatOld-coptic";
-layers = (
+glyphname = etadasiaypogegrammeni;
+unicode = 8081;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11477;
+glyphname = etapsilivariaypogegrammeni;
+unicode = 8082;
 },
 {
-glyphname = "gangia-coptic";
-layers = (
+glyphname = etadasiavariaypogegrammeni;
+unicode = 8083;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1003;
+glyphname = etapsilioxiaypogegrammeni;
+unicode = 8084;
 },
 {
-glyphname = "gangiaCryptogrammic-coptic";
-layers = (
+glyphname = etadasiaoxiaypogegrammeni;
+unicode = 8085;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11502;
+glyphname = etapsiliperispomeniypogegrammeni;
+unicode = 8086;
 },
 {
-glyphname = "gangiaOld-coptic";
-layers = (
+glyphname = etadasiaperispomeniypogegrammeni;
+unicode = 8087;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11479;
+glyphname = Etapsiliprosgegrammeni;
+unicode = 8088;
 },
 {
-glyphname = "shima-coptic";
-layers = (
+glyphname = Etadasiaprosgegrammeni;
+unicode = 8089;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1005;
+glyphname = Etapsilivariaprosgegrammeni;
+unicode = 8090;
 },
 {
-glyphname = "djaOld-coptic";
-layers = (
+glyphname = Etadasiavariaprosgegrammeni;
+unicode = 8091;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11481;
+glyphname = Etapsilioxiaprosgegrammeni;
+unicode = 8092;
 },
 {
-glyphname = "shimaOld-coptic";
-layers = (
+glyphname = Etadasiaoxiaprosgegrammeni;
+unicode = 8093;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11483;
+glyphname = Etapsiliperispomeniprosgegrammeni;
+unicode = 8094;
 },
 {
-glyphname = "dei-coptic";
-layers = (
+glyphname = Etadasiaperispomeniprosgegrammeni;
+unicode = 8095;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1007;
+glyphname = omegapsiliypogegrammeni;
+unicode = 8096;
 },
 {
-glyphname = "alefDialectP-coptic";
-layers = (
+glyphname = omegadasiaypogegrammeni;
+unicode = 8097;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11443;
+glyphname = omegapsilivariaypogegrammeni;
+unicode = 8098;
 },
 {
-glyphname = "ainOld-coptic";
-layers = (
+glyphname = omegadasiavariaypogegrammeni;
+unicode = 8099;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11445;
+glyphname = omegapsilioxiaypogegrammeni;
+unicode = 8100;
 },
 {
-glyphname = "onehalf-coptic";
-layers = (
+glyphname = omegadasiaoxiaypogegrammeni;
+unicode = 8101;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11517;
+glyphname = omegapsiliperispomeniypogegrammeni;
+unicode = 8102;
 },
 {
-glyphname = "fullstop-coptic";
-layers = (
+glyphname = omegadasiaperispomeniypogegrammeni;
+unicode = 8103;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11518;
+glyphname = Omegapsiliprosgegrammeni;
+unicode = 8104;
 },
 {
-glyphname = "morphologicaldivider-coptic";
-layers = (
+glyphname = Omegadasiaprosgegrammeni;
+unicode = 8105;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11519;
+glyphname = Omegapsilivariaprosgegrammeni;
+unicode = 8106;
 },
 {
-glyphname = "kai-coptic";
-layers = (
+glyphname = Omegadasiavariaprosgegrammeni;
+unicode = 8107;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11492;
+glyphname = Omegapsilioxiaprosgegrammeni;
+unicode = 8108;
 },
 {
-glyphname = "miro-coptic";
-layers = (
+glyphname = Omegadasiaoxiaprosgegrammeni;
+unicode = 8109;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11493;
+glyphname = Omegapsiliperispomeniprosgegrammeni;
+unicode = 8110;
 },
 {
-glyphname = "piro-coptic";
-layers = (
+glyphname = Omegadasiaperispomeniprosgegrammeni;
+unicode = 8111;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11494;
+glyphname = alphavrachy;
+unicode = 8112;
 },
 {
-glyphname = "stauros-coptic";
-layers = (
+glyphname = alphamacron;
+unicode = 8113;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11495;
+glyphname = alphavariaypogegrammeni;
+unicode = 8114;
 },
 {
-glyphname = "tauro-coptic";
-layers = (
+glyphname = alphaypogegrammeni;
+unicode = 8115;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11496;
+glyphname = alphaoxiaypogegrammeni;
+unicode = 8116;
 },
 {
-glyphname = "khiro-coptic";
-layers = (
+glyphname = alphaperispomeni;
+unicode = 8118;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11497;
+glyphname = alphaperispomeniypogegrammeni;
+unicode = 8119;
 },
 {
-glyphname = "shimasima-coptic";
-layers = (
+glyphname = Alphavrachy;
+unicode = 8120;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11498;
+glyphname = Alphamacron;
+unicode = 8121;
 },
 {
-glyphname = uni2CEF;
-layers = (
+glyphname = Alphavaria;
+unicode = 8122;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11503;
+glyphname = Alphaoxia;
+unicode = 8123;
 },
 {
-glyphname = uni2CF0;
-layers = (
+glyphname = Alphaprosgegrammeni;
+unicode = 8124;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11504;
+glyphname = prosgegrammeni;
+unicode = 8126;
 },
 {
-glyphname = uni2CF1;
-layers = (
+glyphname = etavariaypogegrammeni;
+unicode = 8130;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 11505;
+glyphname = etaypogegrammeni;
+unicode = 8131;
 },
 {
-glyphname = "oldNgi-nubian-coptic";
-layers = (
+glyphname = etaoxiaypogegrammeni;
+unicode = 8132;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = etaperispomeni;
+unicode = 8134;
 },
 {
-glyphname = "oldNyi-nubian-coptic";
-layers = (
+glyphname = etaperispomeniypogegrammeni;
+unicode = 8135;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = Epsilonvaria;
+unicode = 8136;
 },
 {
-glyphname = "oldShima-nubian-coptic";
-layers = (
+glyphname = Epsilonoxia;
+unicode = 8137;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = Etavaria;
+unicode = 8138;
 },
 {
-glyphname = "oldWau-nubian-coptic";
-layers = (
+glyphname = Etaoxia;
+unicode = 8139;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = Etaprosgegrammeni;
+unicode = 8140;
 },
 {
-glyphname = "olddirectquestion-nubian-coptic";
-layers = (
+glyphname = iotavrachy;
+unicode = 8144;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = iotamacron;
+unicode = 8145;
 },
 {
-glyphname = "oldfullstop-nubian-coptic";
-layers = (
+glyphname = iotadialytikavaria;
+unicode = 8146;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = iotadialytikaoxia;
+unicode = 8147;
 },
 {
-glyphname = "oldindirectquestion-nubian-coptic";
-layers = (
+glyphname = iotaperispomeni;
+unicode = 8150;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = iotadialytikaperispomeni;
+unicode = 8151;
 },
 {
-glyphname = "oldngi-nubian-coptic";
-layers = (
+glyphname = Iotavrachy;
+unicode = 8152;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = Iotamacron;
+unicode = 8153;
 },
 {
-glyphname = "oldnyi-nubian-coptic";
-layers = (
+glyphname = Iotavaria;
+unicode = 8154;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = Iotaoxia;
+unicode = 8155;
 },
 {
-glyphname = "oldshima-nubian-coptic";
-layers = (
+glyphname = upsilonvrachy;
+unicode = 8160;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = upsilonmacron;
+unicode = 8161;
 },
 {
-glyphname = "oldversedivider-nubian-coptic";
-layers = (
+glyphname = upsilondialytikavaria;
+unicode = 8162;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
+glyphname = upsilondialytikaoxia;
+unicode = 8163;
 },
 {
-glyphname = "oldwau-nubian-coptic";
-layers = (
+glyphname = rhopsili;
+unicode = 8164;
+},
 {
-layerId = m01;
-width = 600;
+glyphname = rhodasia;
+unicode = 8165;
+},
+{
+glyphname = upsilonperispomeni;
+unicode = 8166;
+},
+{
+glyphname = upsilondialytikaperispomeni;
+unicode = 8167;
+},
+{
+glyphname = Upsilonvrachy;
+unicode = 8168;
+},
+{
+glyphname = Upsilonmacron;
+unicode = 8169;
+},
+{
+glyphname = Upsilonvaria;
+unicode = 8170;
+},
+{
+glyphname = Upsilonoxia;
+unicode = 8171;
+},
+{
+glyphname = Rhodasia;
+unicode = 8172;
+},
+{
+glyphname = omegavariaypogegrammeni;
+unicode = 8178;
+},
+{
+glyphname = omegaypogegrammeni;
+unicode = 8179;
+},
+{
+glyphname = omegaoxiaypogegrammeni;
+unicode = 8180;
+},
+{
+glyphname = omegaperispomeni;
+unicode = 8182;
+},
+{
+glyphname = omegaperispomeniypogegrammeni;
+unicode = 8183;
+},
+{
+glyphname = Omicronvaria;
+unicode = 8184;
+},
+{
+glyphname = Omicronoxia;
+unicode = 8185;
+},
+{
+glyphname = Omegavaria;
+unicode = 8186;
+},
+{
+glyphname = Omegaoxia;
+unicode = 8187;
+},
+{
+glyphname = Omegaprosgegrammeni;
+unicode = 8188;
 }
 );
-}
+instances = (
 );
+kerningLTR = {
+};
 metrics = (
 {
 type = ascender;
 },
 {
 type = "cap height";
 },
@@ -1496,11 +1351,13 @@
 {
 type = descender;
 },
 {
 type = "italic angle";
 }
 );
+stems = (
+);
 unitsPerEm = 1000;
 versionMajor = 1;
 versionMinor = 0;
 }
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs` & `glyphsets-1.0.0/data/results/glyphs/GF_Greek_Expert.glyphs`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 {
-.appVersion = "3124";
+.appVersion = "3239";
 .formatVersion = 3;
+axes = (
+{
+name = Weight;
+tag = wght;
+},
+{
+name = Width;
+tag = wdth;
+}
+);
 date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Greek Expert";
+familyName = GF_Greek_Expert;
 featurePrefixes = (
 {
 automatic = 1;
 code = "languagesystem DFLT dflt;
 
 languagesystem latn dflt;
 languagesystem latn AZE;
@@ -88,14 +98,18 @@
 code = "sub periodcentered.loclCAT by periodcentered.loclCAT.case;
 ";
 tag = case;
 }
 );
 fontMaster = (
 {
+axesValues = (
+100,
+100
+);
 id = m01;
 metricValues = (
 {
 over = 16;
 pos = 800;
 },
 {
@@ -110,22 +124,76 @@
 over = -16;
 },
 {
 over = -16;
 pos = -200;
 },
 {
-over = -16;
+over = 0;
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
+glyphname = "numeral-greek.sc";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
+glyphname = "lowernumeral-greek.sc";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
+glyphname = anoteleia.sc;
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
+glyphname = questiongreek.sc;
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
+glyphname = tonos.sc;
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
+glyphname = dieresistonos.sc;
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
 glyphname = gamma_gamma;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
@@ -2600,70 +2668,20 @@
 glyphname = omega.sups;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-},
-{
-glyphname = anoteleia.sc;
-layers = (
-{
-layerId = m01;
-width = 600;
 }
 );
-},
-{
-glyphname = questiongreek.sc;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-},
-{
-glyphname = "numeral-greek.sc";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-},
-{
-glyphname = "lowernumeral-greek.sc";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-},
-{
-glyphname = tonos.sc;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-},
-{
-glyphname = dieresistonos.sc;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-}
+instances = (
 );
+kerningLTR = {
+};
 metrics = (
 {
 type = ascender;
 },
 {
 type = "cap height";
 },
@@ -2676,11 +2694,13 @@
 {
 type = descender;
 },
 {
 type = "italic angle";
 }
 );
+stems = (
+);
 unitsPerEm = 1000;
 versionMajor = 1;
 versionMinor = 0;
 }
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_AncientMusicalSymbols.nam`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x1D000 BYZANTINE MUSICAL SYMBOL PSILI
 0x1D001 BYZANTINE MUSICAL SYMBOL DASEIA
 0x1D002 BYZANTINE MUSICAL SYMBOL PERISPOMENI
 0x1D003 BYZANTINE MUSICAL SYMBOL OXEIA EKFONITIKON
 0x1D004 BYZANTINE MUSICAL SYMBOL OXEIA DIPLI
 0x1D005 BYZANTINE MUSICAL SYMBOL VAREIA EKFONITIKON
 0x1D006 BYZANTINE MUSICAL SYMBOL VAREIA DIPLI
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Archaic.nam`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x0370 GREEK CAPITAL LETTER HETA
 0x0371 GREEK SMALL LETTER HETA
 0x0372 GREEK CAPITAL LETTER ARCHAIC SAMPI
 0x0373 GREEK SMALL LETTER ARCHAIC SAMPI
 0x0376 GREEK CAPITAL LETTER PAMPHYLIAN DIGAMMA
 0x0377 GREEK SMALL LETTER PAMPHYLIAN DIGAMMA
 0x037B GREEK SMALL REVERSED LUNATE SIGMA SYMBOL
@@ -28,14 +29,48 @@
 0x03F9 GREEK CAPITAL LUNATE SIGMA SYMBOL
 0x03FA GREEK CAPITAL LETTER SAN
 0x03FB GREEK SMALL LETTER SAN
 0x03FC GREEK RHO WITH STROKE SYMBOL
 0x03FD GREEK CAPITAL REVERSED LUNATE SIGMA SYMBOL
 0x03FE GREEK CAPITAL DOTTED LUNATE SIGMA SYMBOL
 0x03FF GREEK CAPITAL REVERSED DOTTED LUNATE SIGMA SYMBOL
+0x25A1 WHITE SQUARE
+0x2605 BLACK STAR
+0x2609 SUN
+0x260A ASCENDING NODE
+0x260B DESCENDING NODE
+0x260C CONJUNCTION
+0x260D OPPOSITION
+0x2627 CHI RHO
+0x2629 CROSS OF JERUSALEM
+0x263D FIRST QUARTER MOON
+0x263E LAST QUARTER MOON
+0x263F MERCURY
+0x2640 FEMALE SIGN
+0x2641 EARTH
+0x2642 MALE SIGN
+0x2643 JUPITER
+0x2644 SATURN
+0x2645 URANUS
+0x2646 NEPTUNE
+0x2647 PLUTO
+0x2648 ARIES
+0x2649 TAURUS
+0x264A GEMINI
+0x264B CANCER
+0x264C LEO
+0x264D VIRGO
+0x264E LIBRA
+0x264F SCORPIUS
+0x2650 SAGITTARIUS
+0x2651 CAPRICORN
+0x2652 AQUARIUS
+0x2653 PISCES
+0x27C0 THREE DIMENSIONAL ANGLE
+0x27C1 WHITE TRIANGLE CONTAINING SMALL WHITE TRIANGLE
 0x10140 GREEK ACROPHONIC ATTIC ONE QUARTER
 0x10141 GREEK ACROPHONIC ATTIC ONE HALF
 0x10142 GREEK ACROPHONIC ATTIC ONE DRACHMA
 0x10143 GREEK ACROPHONIC ATTIC FIVE
 0x10144 GREEK ACROPHONIC ATTIC FIFTY
 0x10145 GREEK ACROPHONIC ATTIC FIVE HUNDRED
 0x10146 GREEK ACROPHONIC ATTIC FIVE THOUSAND
@@ -102,42 +137,8 @@
 0x10183 GREEK LITRA SIGN
 0x10184 GREEK OUNKIA SIGN
 0x10185 GREEK XESTES SIGN
 0x10186 GREEK ARTABE SIGN
 0x10187 GREEK AROURA SIGN
 0x10188 GREEK GRAMMA SIGN
 0x10189 GREEK TRYBLION BASE SIGN
-0x1018A GREEK ZERO SIGN
-0x25A1 WHITE SQUARE
-0x2605 BLACK STAR
-0x2609 SUN
-0x260A ASCENDING NODE
-0x260B DESCENDING NODE
-0x260C CONJUNCTION
-0x260D OPPOSITION
-0x2627 CHI RHO
-0x2629 CROSS OF JERUSALEM
-0x263D FIRST QUARTER MOON
-0x263E LAST QUARTER MOON
-0x263F MERCURY
-0x2640 FEMALE SIGN
-0x2641 EARTH
-0x2642 MALE SIGN
-0x2643 JUPITER
-0x2644 SATURN
-0x2645 URANUS
-0x2646 NEPTUNE
-0x2647 PLUTO
-0x2648 ARIES
-0x2649 TAURUS
-0x264A GEMINI
-0x264B CANCER
-0x264C LEO
-0x264D VIRGO
-0x264E LIBRA
-0x264F SCORPIUS
-0x2650 SAGITTARIUS
-0x2651 CAPRICORN
-0x2652 AQUARIUS
-0x2653 PISCES
-0x27C0 THREE DIMENSIONAL ANGLE
-0x27C1 WHITE TRIANGLE CONTAINING SMALL WHITE TRIANGLE
+0x1018A GREEK ZERO SIGN
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Coptic.nam`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x03E2 COPTIC CAPITAL LETTER SHEI
 0x03E3 COPTIC SMALL LETTER SHEI
 0x03E4 COPTIC CAPITAL LETTER FEI
 0x03E5 COPTIC SMALL LETTER FEI
 0x03E6 COPTIC CAPITAL LETTER KHEI
 0x03E7 COPTIC SMALL LETTER KHEI
 0x03E8 COPTIC CAPITAL LETTER HORI
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Core.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Core.nam`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+0x0021 EXCLAMATION MARK
+0x0022 QUOTATION MARK
+0x0025 PERCENT SIGN
+0x0026 AMPERSAND
+0x0028 LEFT PARENTHESIS
+0x0029 RIGHT PARENTHESIS
+0x002A ASTERISK
+0x002B PLUS SIGN
+0x002C COMMA
+0x002D HYPHEN-MINUS
+0x002E FULL STOP
+0x002F SOLIDUS
+0x0030 DIGIT ZERO
+0x0031 DIGIT ONE
+0x0032 DIGIT TWO
+0x0033 DIGIT THREE
+0x0034 DIGIT FOUR
+0x0035 DIGIT FIVE
+0x0036 DIGIT SIX
+0x0037 DIGIT SEVEN
+0x0038 DIGIT EIGHT
+0x0039 DIGIT NINE
+0x003A COLON
+0x003B SEMICOLON
+0x0040 COMMERCIAL AT
+0x005B LEFT SQUARE BRACKET
+0x005C REVERSE SOLIDUS
+0x005D RIGHT SQUARE BRACKET
+0x00AB LEFT-POINTING DOUBLE ANGLE QUOTATION MARK
+0x00BB RIGHT-POINTING DOUBLE ANGLE QUOTATION MARK
+0x0301 COMBINING ACUTE ACCENT
+0x0308 COMBINING DIAERESIS
 0x0374 GREEK NUMERAL SIGN
 0x0375 GREEK LOWER NUMERAL SIGN
 0x037E GREEK QUESTION MARK
 0x0384 GREEK TONOS
 0x0385 GREEK DIALYTIKA TONOS
 0x0386 GREEK CAPITAL LETTER ALPHA WITH TONOS
 0x0387 GREEK ANO TELEIA
@@ -70,8 +103,11 @@
 0x03C9 GREEK SMALL LETTER OMEGA
 0x03CA GREEK SMALL LETTER IOTA WITH DIALYTIKA
 0x03CB GREEK SMALL LETTER UPSILON WITH DIALYTIKA
 0x03CC GREEK SMALL LETTER OMICRON WITH TONOS
 0x03CD GREEK SMALL LETTER UPSILON WITH TONOS
 0x03CE GREEK SMALL LETTER OMEGA WITH TONOS
 0x03CF GREEK CAPITAL KAI SYMBOL
-0x03D7 GREEK KAI SYMBOL
+0x03D7 GREEK KAI SYMBOL
+0x2013 EN DASH
+0x2014 EM DASH
+0x2026 HORIZONTAL ELLIPSIS
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Plus.nam`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x0342 COMBINING GREEK PERISPOMENI
 0x0343 COMBINING GREEK KORONIS
 0x0344 COMBINING GREEK DIALYTIKA TONOS
 0x0345 COMBINING GREEK YPOGEGRAMMENI
 0x037A GREEK YPOGEGRAMMENI
 0x1F00 GREEK SMALL LETTER ALPHA WITH PSILI
 0x1F01 GREEK SMALL LETTER ALPHA WITH DASIA
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Greek_Pro.nam`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x02D9 DOT ABOVE
 0x0305 COMBINING OVERLINE
 0x0323 COMBINING DOT BELOW
 0x0359 COMBINING ASTERISK BELOW
 0x035C COMBINING DOUBLE BREVE BELOW
 0x03DA GREEK LETTER STIGMA
 0x03DB GREEK SMALL LETTER STIGMA
 0x03DC GREEK LETTER DIGAMMA
 0x03DD GREEK SMALL LETTER DIGAMMA
 0x03DE GREEK LETTER KOPPA
 0x03DF GREEK SMALL LETTER KOPPA
 0x03E0 GREEK LETTER SAMPI
 0x03E1 GREEK SMALL LETTER SAMPI
-0x1D459 MATHEMATICAL ITALIC SMALL L
-0x1D510 MATHEMATICAL FRAKTUR CAPITAL M
-0x1D513 MATHEMATICAL FRAKTUR CAPITAL P
-0x1D516 MATHEMATICAL FRAKTUR CAPITAL S
-0x1D52D MATHEMATICAL FRAKTUR SMALL P
 0x2016 DOUBLE VERTICAL LINE
 0x203B REFERENCE MARK
 0x203F UNDERTIE
 0x2042 ASTERISM
 0x2056 THREE DOT PUNCTUATION
 0x2058 FOUR DOT PUNCTUATION
 0x2059 FIVE DOT PUNCTUATION
@@ -75,8 +71,13 @@
 0x3008 LEFT ANGLE BRACKET
 0x3009 RIGHT ANGLE BRACKET
 0x300A LEFT DOUBLE ANGLE BRACKET
 0x300B RIGHT DOUBLE ANGLE BRACKET
 0x300C LEFT CORNER BRACKET
 0x300D RIGHT CORNER BRACKET
 0x301A LEFT WHITE SQUARE BRACKET
-0x301B RIGHT WHITE SQUARE BRACKET
+0x301B RIGHT WHITE SQUARE BRACKET
+0x1D459 MATHEMATICAL ITALIC SMALL L
+0x1D510 MATHEMATICAL FRAKTUR CAPITAL M
+0x1D513 MATHEMATICAL FRAKTUR CAPITAL P
+0x1D516 MATHEMATICAL FRAKTUR CAPITAL S
+0x1D52D MATHEMATICAL FRAKTUR SMALL P
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Archaic.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,76 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 Heta
-Archaicsampi
-Pamphyliandigamma
-KoppaArchaic
-UpsilonhookSymbol
-UpsilonacutehookSymbol
-UpsilondieresishookSymbol
-ThetaSymbol
-Sho
-SigmaLunateSymbol
-San
-SigmaLunateReversedSymbol
-SigmaLunateDottedSymbol
-SigmaLunateDottedReversedSymbol
 heta
+Archaicsampi
 archaicsampi
+Pamphyliandigamma
 pamphyliandigamma
 sigmaLunateReversedSymbol
 sigmaLunateDottedSymbol
 sigmaLunateDottedReversedSymbol
-koppaArchaic
 betaSymbol
 thetaSymbol
+UpsilonhookSymbol
+UpsilonacutehookSymbol
+UpsilondieresishookSymbol
 phiSymbol
 piSymbol
+KoppaArchaic
+koppaArchaic
 kappaSymbol
 rhoSymbol
 sigmaLunateSymbol
 yot
+ThetaSymbol
 epsilonLunateSymbol
+epsilonLunateReversedSymbol
+Sho
 sho
+SigmaLunateSymbol
+San
 san
 rhoStrokeSymbol
+SigmaLunateReversedSymbol
+SigmaLunateDottedSymbol
+SigmaLunateDottedReversedSymbol
+whiteSquare
+blackstar
+sunSymbol
+ascendingNode
+descendingNode
+conjunction
+opposition
+constantineCross
+jerusalemCross
+firstQuarterMoon
+lastQuarterMoon
+mercury
+venus
+earth
+mars
+jupiter
+saturn
+uranus
+neptune
+pluto
+aries
+taurus
+gemini
+cancer
+leo
+virgo
+libra
+scorpius
+sagittarius
+capricorn
+aquarius
+pisces
+threeDimensionalAngle
+whitetrianglecontainingwhitetriangle
 onequarter-atticGreek
 onehalf-atticGreek
 onedrachma-atticGreek
 five-atticGreek
 fifty-atticGreek
 fivehundred-atticGreek
 fivethousand-atticGreek
@@ -84,15 +120,14 @@
 thespianfivethousand-ancientGreek
 delphicfivemnas-ancientGreek
 stratianfiftymnas-ancientGreek
 onehalf-greek
 onehalfAlternate-greek
 twothirds-greek
 threequarters-greek
-zero-greek
 year-greek
 talent-greek
 drachma-greek
 obol-greek
 twoObols-greek
 threeObols-greek
 fourObols-greek
@@ -102,42 +137,8 @@
 litra-greek
 ounkia-greek
 xestes-greek
 artabe-greek
 aroura-greek
 gramma-greek
 tryblionBase-greek
-epsilonLunateReversedSymbol
-sunSymbol
-blackstar
-ascendingNode
-descendingNode
-conjunction
-opposition
-constantineCross
-jerusalemCross
-firstQuarterMoon
-lastQuarterMoon
-mercury
-venus
-earth
-mars
-jupiter
-saturn
-uranus
-neptune
-pluto
-aries
-taurus
-gemini
-cancer
-leo
-virgo
-libra
-scorpius
-sagittarius
-capricorn
-aquarius
-pisces
-threeDimensionalAngle
-whitetrianglecontainingwhitetriangle
-whiteSquare
+zero-greek
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Coptic.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,132 +1,133 @@
-Alfa-coptic
-Vida-coptic
-Gamma-coptic
-Dalda-coptic
-Eie-coptic
-Sou-coptic
-Zata-coptic
-Hate-coptic
-Thethe-coptic
-Iauda-coptic
-Kapa-coptic
-Laula-coptic
-Mi-coptic
-Ni-coptic
-Ksi-coptic
-O-coptic
-Pi-coptic
-Ro-coptic
-Sima-coptic
-Tau-coptic
-Ua-coptic
-Fi-coptic
-Khi-coptic
-Psi-coptic
-Oou-coptic
-Cryptogrammiceie-coptic
-dialectPkapa-coptic
-dialectPni-coptic
-Cryptogrammicni-coptic
-OouOld-coptic
-Sampi-coptic
+# This file is auto-generated; do not edit. See /README.md for instructions.
 Shei-coptic
-SheiCryptogrammic-coptic
-SheiCrossed-coptic
-SheiOld-coptic
-EshOld-coptic
+shei-coptic
 Fei-coptic
+fei-coptic
 Khei-coptic
-KheiBohairic-coptic
-KheiAkhmimic-coptic
+khei-coptic
 Hori-coptic
-HoriDialectP-coptic
-HoriOld-coptic
-HaOld-coptic
-HaLshaped-coptic
-HeiOld-coptic
-HatOld-coptic
+hori-coptic
 Gangia-coptic
-GangiaCryptogrammic-coptic
-GangiaOld-coptic
+gangia-coptic
 Shima-coptic
-DjaOld-coptic
-ShimaOld-coptic
+shima-coptic
 Dei-coptic
-AlefDialectP-coptic
-AinOld-coptic
+dei-coptic
+Alfa-coptic
 alfa-coptic
+Vida-coptic
 vida-coptic
+Gamma-coptic
 gamma-coptic
+Dalda-coptic
 dalda-coptic
+Eie-coptic
 eie-coptic
+Sou-coptic
 sou-coptic
+Zata-coptic
 zata-coptic
+Hate-coptic
 hate-coptic
+Thethe-coptic
 thethe-coptic
+Iauda-coptic
 iauda-coptic
+Kapa-coptic
 kapa-coptic
+Laula-coptic
 laula-coptic
+Mi-coptic
 mi-coptic
+Ni-coptic
 ni-coptic
+Ksi-coptic
 ksi-coptic
+O-coptic
 o-coptic
+Pi-coptic
 pi-coptic
+Ro-coptic
 ro-coptic
+Sima-coptic
 sima-coptic
+Tau-coptic
 tau-coptic
+Ua-coptic
 ua-coptic
+Fi-coptic
 fi-coptic
+Khi-coptic
 khi-coptic
+Psi-coptic
 psi-coptic
+Oou-coptic
 oou-coptic
+AlefDialectP-coptic
+alefDialectP-coptic
+AinOld-coptic
+ainOld-coptic
+Cryptogrammiceie-coptic
 cryptogrammiceie-coptic
+dialectPkapa-coptic
 dialectpkapa-coptic
+dialectPni-coptic
 dialectpni-coptic
+Cryptogrammicni-coptic
 cryptogrammicni-coptic
+OouOld-coptic
 oouOld-coptic
+Sampi-coptic
 sampi-coptic
-shei-coptic
-sheiCryptogrammic-coptic
+SheiCrossed-coptic
 sheiCrossed-coptic
+SheiOld-coptic
 sheiOld-coptic
+EshOld-coptic
 eshOld-coptic
-fei-coptic
-khei-coptic
-kheiBohairic-coptic
+KheiAkhmimic-coptic
 kheiAkhmimic-coptic
-hori-coptic
+HoriDialectP-coptic
 horiDialectP-coptic
+HoriOld-coptic
 horiOld-coptic
+HaOld-coptic
 haOld-coptic
+HaLshaped-coptic
 haLshaped-coptic
+HeiOld-coptic
 heiOld-coptic
+HatOld-coptic
 hatOld-coptic
-gangia-coptic
-gangiaCryptogrammic-coptic
+GangiaOld-coptic
 gangiaOld-coptic
-shima-coptic
+DjaOld-coptic
 djaOld-coptic
+ShimaOld-coptic
 shimaOld-coptic
-dei-coptic
-alefDialectP-coptic
-ainOld-coptic
-onehalf-coptic
-fullstop-coptic
-morphologicaldivider-coptic
 kai-coptic
 miro-coptic
 piro-coptic
 stauros-coptic
 tauro-coptic
 khiro-coptic
 shimasima-coptic
+SheiCryptogrammic-coptic
+sheiCryptogrammic-coptic
+GangiaCryptogrammic-coptic
+gangiaCryptogrammic-coptic
 uni2CEF
 uni2CF0
 uni2CF1
+KheiBohairic-coptic
+kheiBohairic-coptic
+onehalf-coptic
+fullstop-coptic
+morphologicaldivider-coptic
 oldNgi-nubian-coptic
 oldNyi-nubian-coptic
 oldShima-nubian-coptic
 oldWau-nubian-coptic
 olddirectquestion-nubian-coptic
 oldfullstop-nubian-coptic
 oldindirectquestion-nubian-coptic
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Expert.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+numeral-greek.sc
+lowernumeral-greek.sc
+anoteleia.sc
+questiongreek.sc
+tonos.sc
+dieresistonos.sc
 gamma_gamma
 lambda_lambda
 alpha.sc
 beta.sc
 gamma.sc
 delta.sc
 epsilon.sc
@@ -269,14 +276,8 @@
 sigmafinal.sups
 sigma.sups
 tau.sups
 upsilon.sups
 phi.sups
 chi.sups
 psi.sups
-omega.sups
-anoteleia.sc
-questiongreek.sc
-numeral-greek.sc
-lowernumeral-greek.sc
-tonos.sc
-dieresistonos.sc
+omega.sups
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Plus.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,265 +1,266 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+perispomenicomb
+koroniscomb
+dialytikatonoscomb
+ypogegrammenicomb
+ypogegrammeni
+alphapsili
+alphadasia
+alphapsilivaria
+alphadasiavaria
+alphapsilioxia
+alphadasiaoxia
+alphapsiliperispomeni
+alphadasiaperispomeni
 Alphapsili
 Alphadasia
 Alphapsilivaria
 Alphadasiavaria
 Alphapsilioxia
 Alphadasiaoxia
 Alphapsiliperispomeni
 Alphadasiaperispomeni
-Alphavaria
-Alphaoxia
-Alphavrachy
-Alphamacron
-Alphaprosgegrammeni
-Alphapsiliprosgegrammeni
-Alphadasiaprosgegrammeni
-Alphapsilivariaprosgegrammeni
-Alphadasiavariaprosgegrammeni
-Alphapsilioxiaprosgegrammeni
-Alphadasiaoxiaprosgegrammeni
-Alphapsiliperispomeniprosgegrammeni
-Alphadasiaperispomeniprosgegrammeni
+epsilonpsili
+epsilondasia
+epsilonpsilivaria
+epsilondasiavaria
+epsilonpsilioxia
+epsilondasiaoxia
 Epsilonpsili
 Epsilondasia
 Epsilonpsilivaria
 Epsilondasiavaria
 Epsilonpsilioxia
 Epsilondasiaoxia
-Epsilonvaria
-Epsilonoxia
+etapsili
+etadasia
+etapsilivaria
+etadasiavaria
+etapsilioxia
+etadasiaoxia
+etapsiliperispomeni
+etadasiaperispomeni
 Etapsili
 Etadasia
 Etapsilivaria
 Etadasiavaria
 Etapsilioxia
 Etadasiaoxia
 Etapsiliperispomeni
 Etadasiaperispomeni
-Etavaria
-Etaoxia
-Etaprosgegrammeni
-Etapsiliprosgegrammeni
-Etadasiaprosgegrammeni
-Etapsilivariaprosgegrammeni
-Etadasiavariaprosgegrammeni
-Etapsilioxiaprosgegrammeni
-Etadasiaoxiaprosgegrammeni
-Etapsiliperispomeniprosgegrammeni
-Etadasiaperispomeniprosgegrammeni
+iotapsili
+iotadasia
+iotapsilivaria
+iotadasiavaria
+iotapsilioxia
+iotadasiaoxia
+iotapsiliperispomeni
+iotadasiaperispomeni
 Iotapsili
 Iotadasia
 Iotapsilivaria
 Iotadasiavaria
 Iotapsilioxia
 Iotadasiaoxia
 Iotapsiliperispomeni
 Iotadasiaperispomeni
-Iotavaria
-Iotaoxia
-Iotavrachy
-Iotamacron
+omicronpsili
+omicrondasia
+omicronpsilivaria
+omicrondasiavaria
+omicronpsilioxia
+omicrondasiaoxia
 Omicronpsili
 Omicrondasia
 Omicronpsilivaria
 Omicrondasiavaria
 Omicronpsilioxia
 Omicrondasiaoxia
-Omicronvaria
-Omicronoxia
-Rhodasia
+upsilonpsili
+upsilondasia
+upsilonpsilivaria
+upsilondasiavaria
+upsilonpsilioxia
+upsilondasiaoxia
+upsilonpsiliperispomeni
+upsilondasiaperispomeni
 Upsilondasia
 Upsilondasiavaria
 Upsilondasiaoxia
 Upsilondasiaperispomeni
-Upsilonvaria
-Upsilonoxia
-Upsilonvrachy
-Upsilonmacron
+omegapsili
+omegadasia
+omegapsilivaria
+omegadasiavaria
+omegapsilioxia
+omegadasiaoxia
+omegapsiliperispomeni
+omegadasiaperispomeni
 Omegapsili
 Omegadasia
 Omegapsilivaria
 Omegadasiavaria
 Omegapsilioxia
 Omegadasiaoxia
 Omegapsiliperispomeni
 Omegadasiaperispomeni
-Omegavaria
-Omegaoxia
-Omegaprosgegrammeni
-Omegapsiliprosgegrammeni
-Omegadasiaprosgegrammeni
-Omegapsilivariaprosgegrammeni
-Omegadasiavariaprosgegrammeni
-Omegapsilioxiaprosgegrammeni
-Omegadasiaoxiaprosgegrammeni
-Omegapsiliperispomeniprosgegrammeni
-Omegadasiaperispomeniprosgegrammeni
-Alphaprosgegrammeni.ss01
-Alphapsiliprosgegrammeni.ss01
-Alphadasiaprosgegrammeni.ss01
-Alphapsilivariaprosgegrammeni.ss01
-Alphadasiavariaprosgegrammeni.ss01
-Alphapsilioxiaprosgegrammeni.ss01
-Alphadasiaoxiaprosgegrammeni.ss01
-Alphapsiliperispomeniprosgegrammeni.ss01
-Alphadasiaperispomeniprosgegrammeni.ss01
-Etaprosgegrammeni.ss01
-Etapsiliprosgegrammeni.ss01
-Etadasiaprosgegrammeni.ss01
-Etapsilivariaprosgegrammeni.ss01
-Etadasiavariaprosgegrammeni.ss01
-Etapsilioxiaprosgegrammeni.ss01
-Etadasiaoxiaprosgegrammeni.ss01
-Etapsiliperispomeniprosgegrammeni.ss01
-Etadasiaperispomeniprosgegrammeni.ss01
-Omegaprosgegrammeni.ss01
-Omegapsiliprosgegrammeni.ss01
-Omegadasiaprosgegrammeni.ss01
-Omegapsilivariaprosgegrammeni.ss01
-Omegadasiavariaprosgegrammeni.ss01
-Omegapsilioxiaprosgegrammeni.ss01
-Omegadasiaoxiaprosgegrammeni.ss01
-Omegapsiliperispomeniprosgegrammeni.ss01
-Omegadasiaperispomeniprosgegrammeni.ss01
-alphapsili
-alphadasia
-alphapsilivaria
-alphadasiavaria
-alphapsilioxia
-alphadasiaoxia
-alphapsiliperispomeni
-alphadasiaperispomeni
 alphavaria
 alphaoxia
-alphaperispomeni
-alphavrachy
-alphamacron
-alphaypogegrammeni
-alphavariaypogegrammeni
-alphaoxiaypogegrammeni
+epsilonvaria
+epsilonoxia
+etavaria
+etaoxia
+iotavaria
+iotaoxia
+omicronvaria
+omicronoxia
+upsilonvaria
+upsilonoxia
+omegavaria
+omegaoxia
 alphapsiliypogegrammeni
 alphadasiaypogegrammeni
 alphapsilivariaypogegrammeni
 alphadasiavariaypogegrammeni
 alphapsilioxiaypogegrammeni
 alphadasiaoxiaypogegrammeni
 alphapsiliperispomeniypogegrammeni
 alphadasiaperispomeniypogegrammeni
-alphaperispomeniypogegrammeni
-epsilonpsili
-epsilondasia
-epsilonpsilivaria
-epsilondasiavaria
-epsilonpsilioxia
-epsilondasiaoxia
-epsilonvaria
-epsilonoxia
-etapsili
-etadasia
-etapsilivaria
-etadasiavaria
-etapsilioxia
-etadasiaoxia
-etapsiliperispomeni
-etadasiaperispomeni
-etavaria
-etaoxia
-etaperispomeni
-etaypogegrammeni
-etavariaypogegrammeni
-etaoxiaypogegrammeni
+Alphapsiliprosgegrammeni
+Alphadasiaprosgegrammeni
+Alphapsilivariaprosgegrammeni
+Alphadasiavariaprosgegrammeni
+Alphapsilioxiaprosgegrammeni
+Alphadasiaoxiaprosgegrammeni
+Alphapsiliperispomeniprosgegrammeni
+Alphadasiaperispomeniprosgegrammeni
 etapsiliypogegrammeni
 etadasiaypogegrammeni
 etapsilivariaypogegrammeni
 etadasiavariaypogegrammeni
 etapsilioxiaypogegrammeni
 etadasiaoxiaypogegrammeni
 etapsiliperispomeniypogegrammeni
 etadasiaperispomeniypogegrammeni
-etaperispomeniypogegrammeni
-iotapsili
-iotadasia
-iotapsilivaria
-iotadasiavaria
-iotapsilioxia
-iotadasiaoxia
-iotapsiliperispomeni
-iotadasiaperispomeni
-iotavaria
-iotaoxia
-iotaperispomeni
-iotavrachy
-iotamacron
-iotadialytikavaria
-iotadialytikaoxia
-iotadialytikaperispomeni
-omicronpsili
-omicrondasia
-omicronpsilivaria
-omicrondasiavaria
-omicronpsilioxia
-omicrondasiaoxia
-omicronvaria
-omicronoxia
-rhopsili
-rhodasia
-upsilonpsili
-upsilondasia
-upsilonpsilivaria
-upsilondasiavaria
-upsilonpsilioxia
-upsilondasiaoxia
-upsilonpsiliperispomeni
-upsilondasiaperispomeni
-upsilonvaria
-upsilonoxia
-upsilonperispomeni
-upsilonvrachy
-upsilonmacron
-upsilondialytikavaria
-upsilondialytikaoxia
-upsilondialytikaperispomeni
-omegapsili
-omegadasia
-omegapsilivaria
-omegadasiavaria
-omegapsilioxia
-omegadasiaoxia
-omegapsiliperispomeni
-omegadasiaperispomeni
-omegavaria
-omegaoxia
-omegaperispomeni
-omegaypogegrammeni
-omegavariaypogegrammeni
-omegaoxiaypogegrammeni
+Etapsiliprosgegrammeni
+Etadasiaprosgegrammeni
+Etapsilivariaprosgegrammeni
+Etadasiavariaprosgegrammeni
+Etapsilioxiaprosgegrammeni
+Etadasiaoxiaprosgegrammeni
+Etapsiliperispomeniprosgegrammeni
+Etadasiaperispomeniprosgegrammeni
 omegapsiliypogegrammeni
 omegadasiaypogegrammeni
 omegapsilivariaypogegrammeni
 omegadasiavariaypogegrammeni
 omegapsilioxiaypogegrammeni
 omegadasiaoxiaypogegrammeni
 omegapsiliperispomeniypogegrammeni
 omegadasiaperispomeniypogegrammeni
-omegaperispomeniypogegrammeni
+Omegapsiliprosgegrammeni
+Omegadasiaprosgegrammeni
+Omegapsilivariaprosgegrammeni
+Omegadasiavariaprosgegrammeni
+Omegapsilioxiaprosgegrammeni
+Omegadasiaoxiaprosgegrammeni
+Omegapsiliperispomeniprosgegrammeni
+Omegadasiaperispomeniprosgegrammeni
+alphavrachy
+alphamacron
+alphavariaypogegrammeni
+alphaypogegrammeni
+alphaoxiaypogegrammeni
+alphaperispomeni
+alphaperispomeniypogegrammeni
+Alphavrachy
+Alphamacron
+Alphavaria
+Alphaoxia
+Alphaprosgegrammeni
+koronis
 prosgegrammeni
-ypogegrammeni
-perispomenicomb
-koroniscomb
-dialytikatonoscomb
-ypogegrammenicomb
 psili
-koronis
-dasia
+perispomeni
+dialytikaperispomeni
+etavariaypogegrammeni
+etaypogegrammeni
+etaoxiaypogegrammeni
+etaperispomeni
+etaperispomeniypogegrammeni
+Epsilonvaria
+Epsilonoxia
+Etavaria
+Etaoxia
+Etaprosgegrammeni
 psilivaria
-dasiavaria
 psilioxia
-dasiaoxia
 psiliperispomeni
+iotavrachy
+iotamacron
+iotadialytikavaria
+iotadialytikaoxia
+iotaperispomeni
+iotadialytikaperispomeni
+Iotavrachy
+Iotamacron
+Iotavaria
+Iotaoxia
+dasiavaria
+dasiaoxia
 dasiaperispomeni
+upsilonvrachy
+upsilonmacron
+upsilondialytikavaria
+upsilondialytikaoxia
+rhopsili
+rhodasia
+upsilonperispomeni
+upsilondialytikaperispomeni
+Upsilonvrachy
+Upsilonmacron
+Upsilonvaria
+Upsilonoxia
+Rhodasia
 dialytikavaria
 dialytikaoxia
-dialytikaperispomeni
 varia
+omegavariaypogegrammeni
+omegaypogegrammeni
+omegaoxiaypogegrammeni
+omegaperispomeni
+omegaperispomeniypogegrammeni
+Omicronvaria
+Omicronoxia
+Omegavaria
+Omegaoxia
+Omegaprosgegrammeni
 oxia
-perispomeni
+dasia
+Alphaprosgegrammeni.ss01
+Alphapsiliprosgegrammeni.ss01
+Alphadasiaprosgegrammeni.ss01
+Alphapsilivariaprosgegrammeni.ss01
+Alphadasiavariaprosgegrammeni.ss01
+Alphapsilioxiaprosgegrammeni.ss01
+Alphadasiaoxiaprosgegrammeni.ss01
+Alphapsiliperispomeniprosgegrammeni.ss01
+Alphadasiaperispomeniprosgegrammeni.ss01
+Etaprosgegrammeni.ss01
+Etapsiliprosgegrammeni.ss01
+Etadasiaprosgegrammeni.ss01
+Etapsilivariaprosgegrammeni.ss01
+Etadasiavariaprosgegrammeni.ss01
+Etapsilioxiaprosgegrammeni.ss01
+Etadasiaoxiaprosgegrammeni.ss01
+Etapsiliperispomeniprosgegrammeni.ss01
+Etadasiaperispomeniprosgegrammeni.ss01
+Omegaprosgegrammeni.ss01
+Omegapsiliprosgegrammeni.ss01
+Omegadasiaprosgegrammeni.ss01
+Omegapsilivariaprosgegrammeni.ss01
+Omegadasiavariaprosgegrammeni.ss01
+Omegapsilioxiaprosgegrammeni.ss01
+Omegadasiaoxiaprosgegrammeni.ss01
+Omegapsiliperispomeniprosgegrammeni.ss01
+Omegadasiaperispomeniprosgegrammeni.ss01
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Greek_Pro.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,83 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+dotaccent
+overlinecomb
+dotbelowcomb
+asteriskbelowcomb
+doublebrevebelowcomb
 Stigma
-Digamma
-Koppa
-Sampi
 stigma
+Digamma
 digamma
+Koppa
 koppa
+Sampi
 sampi
-M-fraktur
-P-fraktur
-S-fraktur
-p-fraktur
-litalic-math
-asterism
 dblverticalbar
-dottedcross
-dottedobelos
-dottedrightpointingangle
-dottedtranspositionmarker
-downancora
-editorialcoronis
+referencemark
+undertie
+asterism
+threedotpunctuation
+fourdotpunctuation
 fivedotpunctuation
-forkedparagraphos
+twodotpunctuation
 fourdotmark
-fourdotpunctuation
-hypodiastole
-leftdottedsubstitutionbracket
-leftraisedomissionbracket
+dottedcross
+tricolon
+verticalfourdots
+plussuperior
+minussuperior
+equalsuperior
+plusinferior
+minusinferior
+equalinferior
+alephsymbol
+betsymbol
+multiply.circled
+ellipsisvertical
+metricalbreve
+metricallongovershort
+metricalshortoverlong
+metricallongovertwoshorts
+metricaltwoshortsoverlong
+metricaltwoshortsjoined
+metricaltriseme
+metricaltetraseme
+metricalpentaseme
+doubleSolidusOperator
+rightanglesubstitutionmarker
+rightangledottedsubstitutionmarker
 leftsubstitutionbracket
-lefttranspositionbracket
-paragraphos
-raiseddottedinterpolationmarker
+rightsubstitutionbracket
+leftdottedsubstitutionbracket
+rightdottedsubstitutionbracket
 raisedinterpolationmarker
+raiseddottedinterpolationmarker
+dottedtranspositionmarker
+lefttranspositionbracket
+righttranspositionbracket
 raisedsquare
-referencemark
-reversedforkedparagraphos
-rightangledottedsubstitutionmarker
-rightanglesubstitutionmarker
-rightdottedsubstitutionbracket
+leftraisedomissionbracket
 rightraisedomissionbracket
-rightsubstitutionbracket
-righttranspositionbracket
-threedotpunctuation
-tricolon
-twodotpunctuation
-undertie
+editorialcoronis
+paragraphos
+forkedparagraphos
+reversedforkedparagraphos
+hypodiastole
+dottedobelos
+downancora
 upancora
-verticalfourdots
+dottedrightpointingangle
 doubleobliquehyphen
 anglebracketleft
 anglebracketright
-cornerbracketleft
-cornerbracketright
 dblanglebracketleft
 dblanglebracketright
+cornerbracketleft
+cornerbracketright
 whitesquarebracketleft
 whitesquarebracketright
-metricalbreve
-metricallongovershort
-metricallongovertwoshorts
-metricalpentaseme
-metricalshortoverlong
-metricaltetraseme
-metricaltriseme
-metricaltwoshortsjoined
-metricaltwoshortsoverlong
-alephsymbol
-betsymbol
-doubleSolidusOperator
-ellipsisvertical
-equalinferior
-equalsuperior
-minusinferior
-minussuperior
-plusinferior
-plussuperior
-multiply.circled
-overlinecomb
-dotbelowcomb
-asteriskbelowcomb
-doublebrevebelowcomb
-dotaccent
+litalic-math
+M-fraktur
+P-fraktur
+S-fraktur
+p-fraktur
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_Archaic.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,76 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 uni0370
-uni0372
-uni0376
-uni03D8
-uni03D2
-uni03D3
-uni03D4
-uni03F4
-uni03F7
-uni03F9
-uni03FA
-uni03FD
-uni03FE
-uni03FF
 uni0371
+uni0372
 uni0373
+uni0376
 uni0377
 uni037B
 uni037C
 uni037D
-uni03D9
 uni03D0
 uni03D1
+uni03D2
+uni03D3
+uni03D4
 uni03D5
 uni03D6
+uni03D8
+uni03D9
 uni03F0
 uni03F1
 uni03F2
 uni03F3
+uni03F4
 uni03F5
+uni03F6
+uni03F7
 uni03F8
+uni03F9
+uni03FA
 uni03FB
 uni03FC
+uni03FD
+uni03FE
+uni03FF
+uni25A1
+uni2605
+uni2609
+uni260A
+uni260B
+uni260C
+uni260D
+uni2627
+uni2629
+uni263D
+uni263E
+uni263F
+female
+uni2641
+male
+uni2643
+uni2644
+uni2645
+uni2646
+uni2647
+uni2648
+uni2649
+uni264A
+uni264B
+uni264C
+uni264D
+uni264E
+uni264F
+uni2650
+uni2651
+uni2652
+uni2653
+uni27C0
+uni27C1
 u10140
 u10141
 u10142
 u10143
 u10144
 u10145
 u10146
@@ -84,15 +120,14 @@
 u10172
 u10173
 u10174
 u10175
 u10176
 u10177
 u10178
-u1018A
 u10179
 u1017A
 u1017B
 u1017C
 u1017D
 u1017E
 u1017F
@@ -102,42 +137,8 @@
 u10183
 u10184
 u10185
 u10186
 u10187
 u10188
 u10189
-uni03F6
-uni2609
-uni2605
-uni260A
-uni260B
-uni260C
-uni260D
-uni2627
-uni2629
-uni263D
-uni263E
-uni263F
-female
-uni2641
-male
-uni2643
-uni2644
-uni2645
-uni2646
-uni2647
-uni2648
-uni2649
-uni264A
-uni264B
-uni264C
-uni264D
-uni264E
-uni264F
-uni2650
-uni2651
-uni2652
-uni2653
-uni27C0
-uni27C1
-uni25A1
+u1018A
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_Expert.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+uni0374.sc
+uni0375.sc
+anoteleia.sc
+uni037E.sc
+tonos.sc
+dieresistonos.sc
 gamma_gamma
 lambda_lambda
 alpha.sc
 beta.sc
 gamma.sc
 delta.sc
 epsilon.sc
@@ -269,14 +276,8 @@
 uni03C2.sups
 sigma.sups
 tau.sups
 upsilon.sups
 phi.sups
 chi.sups
 psi.sups
-omega.sups
-anoteleia.sc
-uni037E.sc
-uni0374.sc
-uni0375.sc
-tonos.sc
-dieresistonos.sc
+omega.sups
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Greek_Plus.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,265 +1,266 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+uni0342
+uni0343
+uni0344
+uni0345
+uni037A
+uni1F00
+uni1F01
+uni1F02
+uni1F03
+uni1F04
+uni1F05
+uni1F06
+uni1F07
 uni1F08
 uni1F09
 uni1F0A
 uni1F0B
 uni1F0C
 uni1F0D
 uni1F0E
 uni1F0F
-uni1FBA
-uni1FBB
-uni1FB8
-uni1FB9
-uni1FBC
-uni1F88
-uni1F89
-uni1F8A
-uni1F8B
-uni1F8C
-uni1F8D
-uni1F8E
-uni1F8F
+uni1F10
+uni1F11
+uni1F12
+uni1F13
+uni1F14
+uni1F15
 uni1F18
 uni1F19
 uni1F1A
 uni1F1B
 uni1F1C
 uni1F1D
-uni1FC8
-uni1FC9
+uni1F20
+uni1F21
+uni1F22
+uni1F23
+uni1F24
+uni1F25
+uni1F26
+uni1F27
 uni1F28
 uni1F29
 uni1F2A
 uni1F2B
 uni1F2C
 uni1F2D
 uni1F2E
 uni1F2F
-uni1FCA
-uni1FCB
-uni1FCC
-uni1F98
-uni1F99
-uni1F9A
-uni1F9B
-uni1F9C
-uni1F9D
-uni1F9E
-uni1F9F
+uni1F30
+uni1F31
+uni1F32
+uni1F33
+uni1F34
+uni1F35
+uni1F36
+uni1F37
 uni1F38
 uni1F39
 uni1F3A
 uni1F3B
 uni1F3C
 uni1F3D
 uni1F3E
 uni1F3F
-uni1FDA
-uni1FDB
-uni1FD8
-uni1FD9
+uni1F40
+uni1F41
+uni1F42
+uni1F43
+uni1F44
+uni1F45
 uni1F48
 uni1F49
 uni1F4A
 uni1F4B
 uni1F4C
 uni1F4D
-uni1FF8
-uni1FF9
-uni1FEC
+uni1F50
+uni1F51
+uni1F52
+uni1F53
+uni1F54
+uni1F55
+uni1F56
+uni1F57
 uni1F59
 uni1F5B
 uni1F5D
 uni1F5F
-uni1FEA
-uni1FEB
-uni1FE8
-uni1FE9
+uni1F60
+uni1F61
+uni1F62
+uni1F63
+uni1F64
+uni1F65
+uni1F66
+uni1F67
 uni1F68
 uni1F69
 uni1F6A
 uni1F6B
 uni1F6C
 uni1F6D
 uni1F6E
 uni1F6F
-uni1FFA
-uni1FFB
-uni1FFC
-uni1FA8
-uni1FA9
-uni1FAA
-uni1FAB
-uni1FAC
-uni1FAD
-uni1FAE
-uni1FAF
-uni1FBC.ss01
-uni1F88.ss01
-uni1F89.ss01
-uni1F8A.ss01
-uni1F8B.ss01
-uni1F8C.ss01
-uni1F8D.ss01
-uni1F8E.ss01
-uni1F8F.ss01
-uni1FCC.ss01
-uni1F98.ss01
-uni1F99.ss01
-uni1F9A.ss01
-uni1F9B.ss01
-uni1F9C.ss01
-uni1F9D.ss01
-uni1F9E.ss01
-uni1F9F.ss01
-uni1FFC.ss01
-uni1FA8.ss01
-uni1FA9.ss01
-uni1FAA.ss01
-uni1FAB.ss01
-uni1FAC.ss01
-uni1FAD.ss01
-uni1FAE.ss01
-uni1FAF.ss01
-uni1F00
-uni1F01
-uni1F02
-uni1F03
-uni1F04
-uni1F05
-uni1F06
-uni1F07
 uni1F70
 uni1F71
-uni1FB6
-uni1FB0
-uni1FB1
-uni1FB3
-uni1FB2
-uni1FB4
+uni1F72
+uni1F73
+uni1F74
+uni1F75
+uni1F76
+uni1F77
+uni1F78
+uni1F79
+uni1F7A
+uni1F7B
+uni1F7C
+uni1F7D
 uni1F80
 uni1F81
 uni1F82
 uni1F83
 uni1F84
 uni1F85
 uni1F86
 uni1F87
-uni1FB7
-uni1F10
-uni1F11
-uni1F12
-uni1F13
-uni1F14
-uni1F15
-uni1F72
-uni1F73
-uni1F20
-uni1F21
-uni1F22
-uni1F23
-uni1F24
-uni1F25
-uni1F26
-uni1F27
-uni1F74
-uni1F75
-uni1FC6
-uni1FC3
-uni1FC2
-uni1FC4
+uni1F88
+uni1F89
+uni1F8A
+uni1F8B
+uni1F8C
+uni1F8D
+uni1F8E
+uni1F8F
 uni1F90
 uni1F91
 uni1F92
 uni1F93
 uni1F94
 uni1F95
 uni1F96
 uni1F97
-uni1FC7
-uni1F30
-uni1F31
-uni1F32
-uni1F33
-uni1F34
-uni1F35
-uni1F36
-uni1F37
-uni1F76
-uni1F77
-uni1FD6
-uni1FD0
-uni1FD1
-uni1FD2
-uni1FD3
-uni1FD7
-uni1F40
-uni1F41
-uni1F42
-uni1F43
-uni1F44
-uni1F45
-uni1F78
-uni1F79
-uni1FE4
-uni1FE5
-uni1F50
-uni1F51
-uni1F52
-uni1F53
-uni1F54
-uni1F55
-uni1F56
-uni1F57
-uni1F7A
-uni1F7B
-uni1FE6
-uni1FE0
-uni1FE1
-uni1FE2
-uni1FE3
-uni1FE7
-uni1F60
-uni1F61
-uni1F62
-uni1F63
-uni1F64
-uni1F65
-uni1F66
-uni1F67
-uni1F7C
-uni1F7D
-uni1FF6
-uni1FF3
-uni1FF2
-uni1FF4
+uni1F98
+uni1F99
+uni1F9A
+uni1F9B
+uni1F9C
+uni1F9D
+uni1F9E
+uni1F9F
 uni1FA0
 uni1FA1
 uni1FA2
 uni1FA3
 uni1FA4
 uni1FA5
 uni1FA6
 uni1FA7
-uni1FF7
+uni1FA8
+uni1FA9
+uni1FAA
+uni1FAB
+uni1FAC
+uni1FAD
+uni1FAE
+uni1FAF
+uni1FB0
+uni1FB1
+uni1FB2
+uni1FB3
+uni1FB4
+uni1FB6
+uni1FB7
+uni1FB8
+uni1FB9
+uni1FBA
+uni1FBB
+uni1FBC
+uni1FBD
 uni1FBE
-uni037A
-uni0342
-uni0343
-uni0344
-uni0345
 uni1FBF
-uni1FBD
-uni1FFE
+uni1FC0
+uni1FC1
+uni1FC2
+uni1FC3
+uni1FC4
+uni1FC6
+uni1FC7
+uni1FC8
+uni1FC9
+uni1FCA
+uni1FCB
+uni1FCC
 uni1FCD
-uni1FDD
 uni1FCE
-uni1FDE
 uni1FCF
+uni1FD0
+uni1FD1
+uni1FD2
+uni1FD3
+uni1FD6
+uni1FD7
+uni1FD8
+uni1FD9
+uni1FDA
+uni1FDB
+uni1FDD
+uni1FDE
 uni1FDF
+uni1FE0
+uni1FE1
+uni1FE2
+uni1FE3
+uni1FE4
+uni1FE5
+uni1FE6
+uni1FE7
+uni1FE8
+uni1FE9
+uni1FEA
+uni1FEB
+uni1FEC
 uni1FED
 uni1FEE
-uni1FC1
 uni1FEF
+uni1FF2
+uni1FF3
+uni1FF4
+uni1FF6
+uni1FF7
+uni1FF8
+uni1FF9
+uni1FFA
+uni1FFB
+uni1FFC
 uni1FFD
-uni1FC0
+uni1FFE
+uni1FBC.ss01
+uni1F88.ss01
+uni1F89.ss01
+uni1F8A.ss01
+uni1F8B.ss01
+uni1F8C.ss01
+uni1F8D.ss01
+uni1F8E.ss01
+uni1F8F.ss01
+uni1FCC.ss01
+uni1F98.ss01
+uni1F99.ss01
+uni1F9A.ss01
+uni1F9B.ss01
+uni1F9C.ss01
+uni1F9D.ss01
+uni1F9E.ss01
+uni1F9F.ss01
+uni1FFC.ss01
+uni1FA8.ss01
+uni1FA9.ss01
+uni1FAA.ss01
+uni1FAB.ss01
+uni1FAC.ss01
+uni1FAD.ss01
+uni1FAE.ss01
+uni1FAF.ss01
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs` & `glyphsets-1.0.0/data/definitions/per_glyphset/GF_Latin_Plus.stub.glyphs`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 {
-.appVersion = "3151";
+.appVersion = "3257";
 .formatVersion = 3;
-date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Latin Minorities";
+axes = (
+{
+name = Weight;
+tag = wght;
+},
+{
+name = Width;
+tag = wdth;
+}
+);
+date = "2023-12-13 14:28:10 +0000";
+familyName = "Neue Schrift";
 fontMaster = (
 {
+axesValues = (
+100,
+100
+);
 id = m01;
 metricValues = (
 {
 over = 16;
 pos = 800;
 },
 {
@@ -23,1589 +37,1497 @@
 over = -16;
 },
 {
 over = -16;
 pos = -200;
 },
 {
-over = -16;
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-glyphname = Acaron;
+glyphname = pi;
+lastChange = "2024-04-10 10:50:35 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 960;
+},
+{
+glyphname = zero.zero;
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
+glyphname = zero.tf;
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
+glyphname = one.tf;
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
+glyphname = two.tf;
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+},
+{
+glyphname = three.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 461;
 },
 {
-color = 3;
-glyphname = Astroke;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = four.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 570;
 },
 {
-glyphname = Ccircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = five.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 264;
 },
 {
-color = 3;
-glyphname = Cstroke;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = six.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 571;
 },
 {
-color = 3;
-glyphname = Emacronacute;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = seven.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7702;
 },
 {
-color = 3;
-glyphname = Emacrongrave;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = eight.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7700;
 },
 {
-color = 3;
-glyphname = Eopen;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = nine.tf;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 400;
 },
 {
-glyphname = Etilde;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = zero.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7868;
 },
 {
-glyphname = Schwa;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = one.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 399;
 },
 {
-glyphname = Ezh;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = two.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 439;
 },
 {
-glyphname = Ezhcaron;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = three.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 494;
 },
 {
-glyphname = Gcaron;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = four.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 486;
 },
 {
-glyphname = Gcircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = five.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 284;
 },
 {
-color = 3;
-glyphname = Glottalstop;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = six.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 577;
 },
 {
-glyphname = Gmacron;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = seven.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7712;
 },
 {
-glyphname = Gstroke;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = eight.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 484;
 },
 {
-glyphname = Hcircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = nine.dnom;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 292;
 },
 {
-color = 3;
-glyphname = Hdotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = zero.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7716;
 },
 {
-color = 3;
-glyphname = Icaron;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = one.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 463;
 },
 {
-color = 3;
-glyphname = Idotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = two.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7882;
 },
 {
-color = 3;
-glyphname = Istroke;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = three.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 407;
 },
 {
-glyphname = Itilde;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = four.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 296;
 },
 {
-glyphname = Jcircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = five.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 308;
 },
 {
-color = 3;
-glyphname = Kacute;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = six.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7728;
 },
 {
-glyphname = Kcaron;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = seven.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 488;
 },
 {
-color = 3;
-glyphname = Kdotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = eight.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7730;
 },
 {
-color = 3;
-glyphname = Kmacronbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = nine.numr;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7732;
 },
 {
-color = 3;
-glyphname = Lbar;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = fraction;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 573;
+unicode = 8260;
 },
 {
-color = 3;
-glyphname = Ldotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = onehalf;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7734;
+unicode = 189;
 },
 {
-color = 3;
-glyphname = Lmiddletilde;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = onethird;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11362;
+unicode = 8531;
 },
 {
-color = 3;
-glyphname = Mdotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = twothirds;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7746;
+unicode = 8532;
 },
 {
-color = 3;
-glyphname = Ndotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = onequarter;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7750;
+unicode = 188;
 },
 {
-color = 3;
-glyphname = Nmacronbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = threequarters;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7752;
+unicode = 190;
 },
 {
-color = 3;
-glyphname = Ocaron;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = oneinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 465;
+unicode = 8321;
 },
 {
-color = 3;
-glyphname = Omacronacute;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = twoinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7762;
+unicode = 8322;
 },
 {
-color = 3;
-glyphname = Omacrongrave;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = threeinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7760;
+unicode = 8323;
 },
 {
-color = 3;
-glyphname = Oogonek;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = fourinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 490;
+unicode = 8324;
 },
 {
-color = 3;
-glyphname = Oogonekmacron;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = fiveinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 492;
+unicode = 8325;
 },
 {
-color = 3;
-glyphname = Oopen;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = sixinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 390;
+unicode = 8326;
 },
 {
-glyphname = Saltillo;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = seveninferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 42891;
+unicode = 8327;
 },
 {
-glyphname = Scircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = eightinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 348;
+unicode = 8328;
 },
 {
-color = 3;
-glyphname = Sdotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = nineinferior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7778;
+unicode = 8329;
 },
 {
-glyphname = Tbar;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = onesuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 358;
+unicode = 185;
 },
 {
-glyphname = Tcedilla;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = twosuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 354;
+unicode = 178;
 },
 {
-color = 3;
-glyphname = Tdiagonalstroke;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = threesuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 574;
+unicode = 179;
 },
 {
-color = 3;
-glyphname = Tmacronbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = foursuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7790;
+unicode = 8308;
 },
 {
-color = 3;
-glyphname = Ucaron;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = fivesuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 467;
+unicode = 8309;
 },
 {
-color = 3;
-glyphname = "Upsilon-latin";
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = sixsuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 433;
+unicode = 8310;
 },
 {
-glyphname = Utilde;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = sevensuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 360;
+unicode = 8311;
 },
 {
-color = 3;
-glyphname = "Gamma-latin";
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = eightsuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 404;
+unicode = 8312;
 },
 {
-glyphname = Ytilde;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = ninesuperior;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7928;
+unicode = 8313;
 },
 {
-color = 3;
-glyphname = Zcircumflex;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = "leftanglebracket-math";
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7824;
+unicode = 10216;
 },
 {
-color = 3;
-glyphname = Zmacronbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = "rightanglebracket-math";
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7828;
+unicode = 10217;
 },
 {
-color = 3;
-glyphname = Ismall;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = dblverticalbar;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 618;
+unicode = 8214;
 },
 {
-glyphname = acaron;
+glyphname = baht;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 462;
+unicode = 3647;
 },
 {
-color = 3;
-glyphname = astroke;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = minute;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11365;
+unicode = 8242;
 },
 {
-glyphname = ccircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = second;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 265;
+unicode = 8243;
 },
 {
-color = 3;
-glyphname = "chi-latin";
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = brokenbar;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 43859;
+unicode = 166;
 },
 {
-color = 3;
-glyphname = cstroke;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = dagger;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 572;
+unicode = 8224;
 },
 {
-color = 3;
-glyphname = emacronacute;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = literSign;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7703;
+unicode = 8467;
 },
 {
-color = 3;
-glyphname = emacrongrave;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = daggerdbl;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7701;
+unicode = 8225;
 },
 {
-color = 3;
-glyphname = eopen;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = estimated;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 603;
+unicode = 8494;
 },
 {
-glyphname = etilde;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = numero;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7869;
+unicode = 8470;
 },
 {
-glyphname = schwa;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = bitcoin;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 601;
+unicode = 8383;
 },
 {
-glyphname = ezh;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = cedi;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 658;
+unicode = 8373;
 },
 {
-glyphname = ezhcaron;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = colonsign;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 495;
+unicode = 8353;
 },
 {
-color = 3;
-glyphname = "gamma-latin";
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = dong;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 611;
+unicode = 8363;
 },
 {
-glyphname = gcaron;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = guarani;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 487;
+unicode = 8370;
 },
 {
-glyphname = gcircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = hryvnia;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 285;
+unicode = 8372;
 },
 {
-color = 3;
-glyphname = glottalstop;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = kip;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 660;
+unicode = 8365;
 },
 {
-color = 3;
-glyphname = glottalstopreversed;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = lari;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 661;
+unicode = 8382;
 },
 {
-glyphname = gmacron;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = liraTurkish;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7713;
+unicode = 8378;
 },
 {
-glyphname = gstroke;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = manat;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 485;
+unicode = 8380;
 },
 {
-glyphname = hcircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = naira;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 293;
+unicode = 8358;
 },
 {
-color = 3;
-glyphname = hdotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = peso;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7717;
+unicode = 8369;
 },
 {
-color = 3;
-glyphname = idotless_ogonek;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = ruble;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
+unicode = 8381;
 },
 {
-color = 3;
-glyphname = icaron;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = rupee;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 464;
+unicode = 8360;
 },
 {
-color = 3;
-glyphname = idotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = rupeeIndian;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7883;
+unicode = 8377;
 },
 {
-color = 3;
-glyphname = "iota-latin";
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = sheqel;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 617;
+unicode = 8362;
 },
 {
-color = 3;
-glyphname = istroke;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = tenge;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 616;
+unicode = 8376;
 },
 {
-glyphname = itilde;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = tugrik;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 297;
+unicode = 8366;
 },
 {
-color = 3;
-glyphname = jcaron;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = won;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 496;
+unicode = 8361;
 },
 {
-glyphname = jcircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = notequal;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 309;
+unicode = 8800;
 },
 {
-color = 3;
-glyphname = kacute;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = greaterequal;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7729;
+unicode = 8805;
 },
 {
-glyphname = kcaron;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = lessequal;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 489;
+unicode = 8804;
 },
 {
-color = 3;
-glyphname = kdotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = plusminus;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7731;
+unicode = 177;
 },
 {
-glyphname = kgreenlandic;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = approxequal;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 312;
+unicode = 8776;
 },
 {
-color = 3;
-glyphname = kmacronbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = logicalnot;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7733;
+unicode = 172;
 },
 {
-color = 3;
-glyphname = lambdastroke;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = emptyset;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 411;
+unicode = 8709;
 },
 {
-color = 3;
-glyphname = lbar;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = infinity;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 410;
+unicode = 8734;
 },
 {
-color = 3;
-glyphname = lbelt;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = integral;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 620;
+unicode = 8747;
 },
 {
-color = 3;
-glyphname = ldotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = Ohm;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7735;
+unicode = 8486;
 },
 {
-color = 3;
-glyphname = lmiddletilde;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = increment;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 619;
+unicode = 8710;
 },
 {
-color = 3;
-glyphname = mdotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = product;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7747;
+unicode = 8719;
 },
 {
-color = 3;
-glyphname = ndotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = summation;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7751;
+unicode = 8721;
 },
 {
-color = 3;
-glyphname = nmacronbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = radical;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7753;
+unicode = 8730;
 },
 {
-color = 3;
-glyphname = ocaron;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = micro;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 466;
+unicode = 181;
 },
 {
-color = 3;
-glyphname = omacronacute;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = partialdiff;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7763;
+unicode = 8706;
 },
 {
-color = 3;
-glyphname = omacrongrave;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = perthousand;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7761;
+unicode = 8240;
 },
 {
-color = 3;
-glyphname = oogonek;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = upArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 491;
+unicode = 8593;
 },
 {
-color = 3;
-glyphname = oogonekmacron;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = northEastArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 493;
+unicode = 8599;
 },
 {
-color = 3;
-glyphname = oopen;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = rightArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 596;
+unicode = 8594;
 },
 {
-glyphname = saltillo;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = southEastArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 42892;
+unicode = 8600;
 },
 {
-glyphname = scircumflex;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = downArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 349;
+unicode = 8595;
 },
 {
-color = 3;
-glyphname = sdotbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = southWestArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7779;
+unicode = 8601;
 },
 {
-glyphname = tbar;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = leftArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 359;
+unicode = 8592;
 },
 {
-glyphname = tcedilla;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = northWestArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 355;
+unicode = 8598;
 },
 {
-color = 3;
-glyphname = tdiagonalstroke;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = leftRightArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 11366;
+unicode = 8596;
 },
 {
-color = 3;
-glyphname = tmacronbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = upDownArrow;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7791;
+unicode = 8597;
 },
 {
-color = 3;
-glyphname = ucaron;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = blackCircle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 468;
+unicode = 9679;
 },
 {
-color = 3;
-glyphname = "upsilon-latin";
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = whiteCircle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 650;
+unicode = 9675;
 },
 {
-glyphname = utilde;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = whiteBullet;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 361;
+unicode = 9702;
 },
 {
-glyphname = ytilde;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = blackDiamond;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7929;
+unicode = 9670;
 },
 {
-color = 3;
-glyphname = zcircumflex;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = whiteDiamond;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7825;
+unicode = 9671;
 },
 {
-color = 3;
-glyphname = zmacronbelow;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = lozenge;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7829;
+unicode = 9674;
 },
 {
-color = 3;
-glyphname = wmod;
-lastChange = "2022-09-14 13:29:37 +0000";
+glyphname = blackSquare;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 695;
+unicode = 9632;
 },
 {
-color = 3;
-glyphname = ymod;
-lastChange = "2022-09-14 13:29:37 +0000";
+glyphname = whiteSquare;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 696;
+unicode = 9633;
 },
 {
-color = 3;
-glyphname = clickalveolar;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = blackSmallSquare;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 450;
+unicode = 9642;
 },
 {
-color = 3;
-glyphname = lambda;
-lastChange = "2022-09-14 12:59:32 +0000";
+glyphname = whiteSmallSquare;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 955;
+unicode = 9643;
 },
 {
-color = 3;
-glyphname = chi;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = upBlackTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 967;
+unicode = 9650;
 },
 {
-color = 3;
-glyphname = thetamod;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = rightBlackTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7615;
+unicode = 9654;
 },
 {
-color = 3;
-glyphname = zmod;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = downBlackTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7611;
+unicode = 9660;
 },
 {
-glyphname = degree;
+glyphname = leftBlackTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 176;
+unicode = 9664;
 },
 {
-color = 3;
-glyphname = YturnedSansSerif;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = upWhiteTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8516;
+unicode = 9651;
 },
 {
-color = 3;
-glyphname = commaabovecomb;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = rightWhiteTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 787;
+unicode = 9655;
 },
 {
-color = 3;
-glyphname = commaaboverightcomb;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = downWhiteTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 789;
+unicode = 9661;
 },
 {
-color = 3;
-glyphname = dotbelowcomb;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = leftWhiteTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 803;
+unicode = 9665;
 },
 {
-color = 3;
-glyphname = macronbelowcomb;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = upBlackSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 817;
+unicode = 9652;
 },
 {
-color = 3;
-glyphname = lowlinecomb;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = rightBlackSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 818;
+unicode = 9656;
 },
 {
-glyphname = strokeshortcomb;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = downBlackSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 821;
+unicode = 9662;
 },
 {
-glyphname = apostrophemod;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = leftBlackSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 700;
+unicode = 9666;
 },
 {
-glyphname = commaturnedmod;
-lastChange = "2023-03-17 14:37:04 +0000";
+glyphname = upWhiteSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 699;
+unicode = 9653;
 },
 {
-color = 3;
-glyphname = glottalstopmod;
-lastChange = "2022-09-14 12:57:10 +0000";
+glyphname = rightWhiteSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 704;
+unicode = 9657;
 },
 {
-glyphname = primemod;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = downWhiteSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 697;
+unicode = 9663;
 },
 {
-glyphname = verticallinemod;
-lastChange = "2022-04-27 12:15:07 +0000";
+glyphname = leftWhiteSmallTriangle;
+lastChange = "2024-04-10 10:50:35 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 712;
+unicode = 9667;
 }
 );
 metrics = (
 {
 type = ascender;
 },
 {
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_African.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_African.nam`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,233 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+0x0021 EXCLAMATION MARK
+0x0022 QUOTATION MARK
+0x0023 NUMBER SIGN
+0x0025 PERCENT SIGN
+0x0026 AMPERSAND
+0x0027 APOSTROPHE
+0x0028 LEFT PARENTHESIS
+0x0029 RIGHT PARENTHESIS
+0x002A ASTERISK
+0x002B PLUS SIGN
+0x002C COMMA
+0x002D HYPHEN-MINUS
+0x002E FULL STOP
+0x002F SOLIDUS
+0x0030 DIGIT ZERO
+0x0031 DIGIT ONE
+0x0032 DIGIT TWO
+0x0033 DIGIT THREE
+0x0034 DIGIT FOUR
+0x0035 DIGIT FIVE
+0x0036 DIGIT SIX
+0x0037 DIGIT SEVEN
+0x0038 DIGIT EIGHT
+0x0039 DIGIT NINE
+0x003A COLON
+0x003B SEMICOLON
+0x003F QUESTION MARK
+0x0040 COMMERCIAL AT
+0x0041 LATIN CAPITAL LETTER A
+0x0042 LATIN CAPITAL LETTER B
+0x0043 LATIN CAPITAL LETTER C
+0x0044 LATIN CAPITAL LETTER D
+0x0045 LATIN CAPITAL LETTER E
+0x0046 LATIN CAPITAL LETTER F
+0x0047 LATIN CAPITAL LETTER G
+0x0048 LATIN CAPITAL LETTER H
+0x0049 LATIN CAPITAL LETTER I
+0x004A LATIN CAPITAL LETTER J
+0x004B LATIN CAPITAL LETTER K
+0x004C LATIN CAPITAL LETTER L
+0x004D LATIN CAPITAL LETTER M
+0x004E LATIN CAPITAL LETTER N
+0x004F LATIN CAPITAL LETTER O
+0x0050 LATIN CAPITAL LETTER P
+0x0051 LATIN CAPITAL LETTER Q
+0x0052 LATIN CAPITAL LETTER R
+0x0053 LATIN CAPITAL LETTER S
+0x0054 LATIN CAPITAL LETTER T
+0x0055 LATIN CAPITAL LETTER U
+0x0056 LATIN CAPITAL LETTER V
+0x0057 LATIN CAPITAL LETTER W
+0x0058 LATIN CAPITAL LETTER X
+0x0059 LATIN CAPITAL LETTER Y
+0x005A LATIN CAPITAL LETTER Z
+0x005B LEFT SQUARE BRACKET
+0x005D RIGHT SQUARE BRACKET
+0x0061 LATIN SMALL LETTER A
+0x0062 LATIN SMALL LETTER B
+0x0063 LATIN SMALL LETTER C
+0x0064 LATIN SMALL LETTER D
+0x0065 LATIN SMALL LETTER E
+0x0066 LATIN SMALL LETTER F
+0x0067 LATIN SMALL LETTER G
+0x0068 LATIN SMALL LETTER H
+0x0069 LATIN SMALL LETTER I
+0x006A LATIN SMALL LETTER J
+0x006B LATIN SMALL LETTER K
+0x006C LATIN SMALL LETTER L
+0x006D LATIN SMALL LETTER M
+0x006E LATIN SMALL LETTER N
+0x006F LATIN SMALL LETTER O
+0x0070 LATIN SMALL LETTER P
+0x0071 LATIN SMALL LETTER Q
+0x0072 LATIN SMALL LETTER R
+0x0073 LATIN SMALL LETTER S
+0x0074 LATIN SMALL LETTER T
+0x0075 LATIN SMALL LETTER U
+0x0076 LATIN SMALL LETTER V
+0x0077 LATIN SMALL LETTER W
+0x0078 LATIN SMALL LETTER X
+0x0079 LATIN SMALL LETTER Y
+0x007A LATIN SMALL LETTER Z
+0x00AA FEMININE ORDINAL INDICATOR
+0x00AB LEFT-POINTING DOUBLE ANGLE QUOTATION MARK
+0x00BA MASCULINE ORDINAL INDICATOR
+0x00BB RIGHT-POINTING DOUBLE ANGLE QUOTATION MARK
+0x00C0 LATIN CAPITAL LETTER A WITH GRAVE
+0x00C1 LATIN CAPITAL LETTER A WITH ACUTE
+0x00C2 LATIN CAPITAL LETTER A WITH CIRCUMFLEX
+0x00C3 LATIN CAPITAL LETTER A WITH TILDE
+0x00C4 LATIN CAPITAL LETTER A WITH DIAERESIS
+0x00C5 LATIN CAPITAL LETTER A WITH RING ABOVE
+0x00C6 LATIN CAPITAL LETTER AE
+0x00C7 LATIN CAPITAL LETTER C WITH CEDILLA
+0x00C8 LATIN CAPITAL LETTER E WITH GRAVE
+0x00C9 LATIN CAPITAL LETTER E WITH ACUTE
+0x00CA LATIN CAPITAL LETTER E WITH CIRCUMFLEX
+0x00CB LATIN CAPITAL LETTER E WITH DIAERESIS
+0x00CC LATIN CAPITAL LETTER I WITH GRAVE
+0x00CD LATIN CAPITAL LETTER I WITH ACUTE
+0x00CE LATIN CAPITAL LETTER I WITH CIRCUMFLEX
+0x00CF LATIN CAPITAL LETTER I WITH DIAERESIS
+0x00D1 LATIN CAPITAL LETTER N WITH TILDE
+0x00D2 LATIN CAPITAL LETTER O WITH GRAVE
+0x00D3 LATIN CAPITAL LETTER O WITH ACUTE
+0x00D4 LATIN CAPITAL LETTER O WITH CIRCUMFLEX
+0x00D5 LATIN CAPITAL LETTER O WITH TILDE
+0x00D6 LATIN CAPITAL LETTER O WITH DIAERESIS
+0x00D8 LATIN CAPITAL LETTER O WITH STROKE
+0x00D9 LATIN CAPITAL LETTER U WITH GRAVE
+0x00DA LATIN CAPITAL LETTER U WITH ACUTE
+0x00DB LATIN CAPITAL LETTER U WITH CIRCUMFLEX
+0x00DC LATIN CAPITAL LETTER U WITH DIAERESIS
+0x00DD LATIN CAPITAL LETTER Y WITH ACUTE
+0x00E0 LATIN SMALL LETTER A WITH GRAVE
+0x00E1 LATIN SMALL LETTER A WITH ACUTE
+0x00E2 LATIN SMALL LETTER A WITH CIRCUMFLEX
+0x00E3 LATIN SMALL LETTER A WITH TILDE
+0x00E4 LATIN SMALL LETTER A WITH DIAERESIS
+0x00E5 LATIN SMALL LETTER A WITH RING ABOVE
+0x00E6 LATIN SMALL LETTER AE
+0x00E7 LATIN SMALL LETTER C WITH CEDILLA
+0x00E8 LATIN SMALL LETTER E WITH GRAVE
+0x00E9 LATIN SMALL LETTER E WITH ACUTE
+0x00EA LATIN SMALL LETTER E WITH CIRCUMFLEX
+0x00EB LATIN SMALL LETTER E WITH DIAERESIS
+0x00EC LATIN SMALL LETTER I WITH GRAVE
+0x00ED LATIN SMALL LETTER I WITH ACUTE
+0x00EE LATIN SMALL LETTER I WITH CIRCUMFLEX
+0x00EF LATIN SMALL LETTER I WITH DIAERESIS
+0x00F1 LATIN SMALL LETTER N WITH TILDE
+0x00F2 LATIN SMALL LETTER O WITH GRAVE
+0x00F3 LATIN SMALL LETTER O WITH ACUTE
+0x00F4 LATIN SMALL LETTER O WITH CIRCUMFLEX
+0x00F5 LATIN SMALL LETTER O WITH TILDE
+0x00F6 LATIN SMALL LETTER O WITH DIAERESIS
+0x00F8 LATIN SMALL LETTER O WITH STROKE
+0x00F9 LATIN SMALL LETTER U WITH GRAVE
+0x00FA LATIN SMALL LETTER U WITH ACUTE
+0x00FB LATIN SMALL LETTER U WITH CIRCUMFLEX
+0x00FC LATIN SMALL LETTER U WITH DIAERESIS
+0x00FD LATIN SMALL LETTER Y WITH ACUTE
+0x00FF LATIN SMALL LETTER Y WITH DIAERESIS
+0x0100 LATIN CAPITAL LETTER A WITH MACRON
+0x0101 LATIN SMALL LETTER A WITH MACRON
+0x0102 LATIN CAPITAL LETTER A WITH BREVE
+0x0103 LATIN SMALL LETTER A WITH BREVE
+0x0104 LATIN CAPITAL LETTER A WITH OGONEK
+0x0105 LATIN SMALL LETTER A WITH OGONEK
+0x0108 LATIN CAPITAL LETTER C WITH CIRCUMFLEX
+0x0109 LATIN SMALL LETTER C WITH CIRCUMFLEX
+0x010C LATIN CAPITAL LETTER C WITH CARON
+0x010D LATIN SMALL LETTER C WITH CARON
+0x0110 LATIN CAPITAL LETTER D WITH STROKE
+0x0111 LATIN SMALL LETTER D WITH STROKE
+0x0112 LATIN CAPITAL LETTER E WITH MACRON
+0x0113 LATIN SMALL LETTER E WITH MACRON
+0x0116 LATIN CAPITAL LETTER E WITH DOT ABOVE
+0x0117 LATIN SMALL LETTER E WITH DOT ABOVE
+0x0118 LATIN CAPITAL LETTER E WITH OGONEK
+0x0119 LATIN SMALL LETTER E WITH OGONEK
+0x011A LATIN CAPITAL LETTER E WITH CARON
+0x011B LATIN SMALL LETTER E WITH CARON
+0x0124 LATIN CAPITAL LETTER H WITH CIRCUMFLEX
+0x0125 LATIN SMALL LETTER H WITH CIRCUMFLEX
+0x0126 LATIN CAPITAL LETTER H WITH STROKE
+0x0127 LATIN SMALL LETTER H WITH STROKE
 0x0128 LATIN CAPITAL LETTER I WITH TILDE
 0x0129 LATIN SMALL LETTER I WITH TILDE
+0x012A LATIN CAPITAL LETTER I WITH MACRON
+0x012B LATIN SMALL LETTER I WITH MACRON
+0x012E LATIN CAPITAL LETTER I WITH OGONEK
+0x012F LATIN SMALL LETTER I WITH OGONEK
+0x0139 LATIN CAPITAL LETTER L WITH ACUTE
+0x013A LATIN SMALL LETTER L WITH ACUTE
+0x0143 LATIN CAPITAL LETTER N WITH ACUTE
+0x0144 LATIN SMALL LETTER N WITH ACUTE
+0x0147 LATIN CAPITAL LETTER N WITH CARON
+0x0148 LATIN SMALL LETTER N WITH CARON
+0x014A LATIN CAPITAL LETTER ENG
+0x014B LATIN SMALL LETTER ENG
+0x014C LATIN CAPITAL LETTER O WITH MACRON
+0x014D LATIN SMALL LETTER O WITH MACRON
+0x0150 LATIN CAPITAL LETTER O WITH DOUBLE ACUTE
+0x0151 LATIN SMALL LETTER O WITH DOUBLE ACUTE
+0x0152 LATIN CAPITAL LIGATURE OE
+0x0153 LATIN SMALL LIGATURE OE
+0x0154 LATIN CAPITAL LETTER R WITH ACUTE
+0x0155 LATIN SMALL LETTER R WITH ACUTE
+0x0156 LATIN CAPITAL LETTER R WITH CEDILLA
+0x0157 LATIN SMALL LETTER R WITH CEDILLA
+0x0158 LATIN CAPITAL LETTER R WITH CARON
+0x0159 LATIN SMALL LETTER R WITH CARON
+0x015A LATIN CAPITAL LETTER S WITH ACUTE
+0x015B LATIN SMALL LETTER S WITH ACUTE
+0x015C LATIN CAPITAL LETTER S WITH CIRCUMFLEX
+0x015D LATIN SMALL LETTER S WITH CIRCUMFLEX
+0x015E LATIN CAPITAL LETTER S WITH CEDILLA
+0x015F LATIN SMALL LETTER S WITH CEDILLA
+0x0160 LATIN CAPITAL LETTER S WITH CARON
+0x0161 LATIN SMALL LETTER S WITH CARON
+0x0162 LATIN CAPITAL LETTER T WITH CEDILLA
+0x0163 LATIN SMALL LETTER T WITH CEDILLA
+0x0166 LATIN CAPITAL LETTER T WITH STROKE
+0x0167 LATIN SMALL LETTER T WITH STROKE
 0x0168 LATIN CAPITAL LETTER U WITH TILDE
 0x0169 LATIN SMALL LETTER U WITH TILDE
-0x0180 LATIN SMALL LETTER B WITH STROKE
+0x016A LATIN CAPITAL LETTER U WITH MACRON
+0x016B LATIN SMALL LETTER U WITH MACRON
+0x0170 LATIN CAPITAL LETTER U WITH DOUBLE ACUTE
+0x0171 LATIN SMALL LETTER U WITH DOUBLE ACUTE
+0x0172 LATIN CAPITAL LETTER U WITH OGONEK
+0x0173 LATIN SMALL LETTER U WITH OGONEK
+0x0174 LATIN CAPITAL LETTER W WITH CIRCUMFLEX
+0x0175 LATIN SMALL LETTER W WITH CIRCUMFLEX
+0x0176 LATIN CAPITAL LETTER Y WITH CIRCUMFLEX
+0x0177 LATIN SMALL LETTER Y WITH CIRCUMFLEX
+0x0178 LATIN CAPITAL LETTER Y WITH DIAERESIS
+0x017B LATIN CAPITAL LETTER Z WITH DOT ABOVE
+0x017C LATIN SMALL LETTER Z WITH DOT ABOVE
+0x017D LATIN CAPITAL LETTER Z WITH CARON
+0x017E LATIN SMALL LETTER Z WITH CARON
 0x0181 LATIN CAPITAL LETTER B WITH HOOK
+0x0182 LATIN CAPITAL LETTER B WITH TOPBAR
+0x0183 LATIN SMALL LETTER B WITH TOPBAR
 0x0186 LATIN CAPITAL LETTER OPEN O
 0x0187 LATIN CAPITAL LETTER C WITH HOOK
 0x0188 LATIN SMALL LETTER C WITH HOOK
 0x0189 LATIN CAPITAL LETTER AFRICAN D
 0x018A LATIN CAPITAL LETTER D WITH HOOK
 0x018E LATIN CAPITAL LETTER REVERSED E
 0x018F LATIN CAPITAL LETTER SCHWA
@@ -16,32 +236,27 @@
 0x0192 LATIN SMALL LETTER F WITH HOOK
 0x0193 LATIN CAPITAL LETTER G WITH HOOK
 0x0194 LATIN CAPITAL LETTER GAMMA
 0x0196 LATIN CAPITAL LETTER IOTA
 0x0197 LATIN CAPITAL LETTER I WITH STROKE
 0x0198 LATIN CAPITAL LETTER K WITH HOOK
 0x0199 LATIN SMALL LETTER K WITH HOOK
-0x019A LATIN SMALL LETTER L WITH BAR
-0x019B LATIN SMALL LETTER LAMBDA WITH STROKE
 0x019C LATIN CAPITAL LETTER TURNED M
 0x019D LATIN CAPITAL LETTER N WITH LEFT HOOK
-0x019E LATIN SMALL LETTER N WITH LONG RIGHT LEG
 0x019F LATIN CAPITAL LETTER O WITH MIDDLE TILDE
 0x01A4 LATIN CAPITAL LETTER P WITH HOOK
 0x01A5 LATIN SMALL LETTER P WITH HOOK
 0x01A9 LATIN CAPITAL LETTER ESH
 0x01AC LATIN CAPITAL LETTER T WITH HOOK
 0x01AD LATIN SMALL LETTER T WITH HOOK
 0x01AE LATIN CAPITAL LETTER T WITH RETROFLEX HOOK
 0x01B1 LATIN CAPITAL LETTER UPSILON
 0x01B2 LATIN CAPITAL LETTER V WITH HOOK
 0x01B3 LATIN CAPITAL LETTER Y WITH HOOK
 0x01B4 LATIN SMALL LETTER Y WITH HOOK
-0x01B5 LATIN CAPITAL LETTER Z WITH STROKE
-0x01B6 LATIN SMALL LETTER Z WITH STROKE
 0x01B7 LATIN CAPITAL LETTER EZH
 0x01B8 LATIN CAPITAL LETTER EZH REVERSED
 0x01B9 LATIN SMALL LETTER EZH REVERSED
 0x01C0 LATIN LETTER DENTAL CLICK
 0x01C1 LATIN LETTER LATERAL CLICK
 0x01C2 LATIN LETTER ALVEOLAR CLICK
 0x01C3 LATIN LETTER RETROFLEX CLICK
@@ -49,320 +264,210 @@
 0x01CE LATIN SMALL LETTER A WITH CARON
 0x01CF LATIN CAPITAL LETTER I WITH CARON
 0x01D0 LATIN SMALL LETTER I WITH CARON
 0x01D1 LATIN CAPITAL LETTER O WITH CARON
 0x01D2 LATIN SMALL LETTER O WITH CARON
 0x01D3 LATIN CAPITAL LETTER U WITH CARON
 0x01D4 LATIN SMALL LETTER U WITH CARON
-0x01D5 LATIN CAPITAL LETTER U WITH DIAERESIS AND MACRON
-0x01D6 LATIN SMALL LETTER U WITH DIAERESIS AND MACRON
 0x01D7 LATIN CAPITAL LETTER U WITH DIAERESIS AND ACUTE
 0x01D8 LATIN SMALL LETTER U WITH DIAERESIS AND ACUTE
-0x01D9 LATIN CAPITAL LETTER U WITH DIAERESIS AND CARON
-0x01DA LATIN SMALL LETTER U WITH DIAERESIS AND CARON
-0x01DB LATIN CAPITAL LETTER U WITH DIAERESIS AND GRAVE
-0x01DC LATIN SMALL LETTER U WITH DIAERESIS AND GRAVE
 0x01DD LATIN SMALL LETTER TURNED E
-0x01DE LATIN CAPITAL LETTER A WITH DIAERESIS AND MACRON
-0x01DF LATIN SMALL LETTER A WITH DIAERESIS AND MACRON
-0x01E0 LATIN CAPITAL LETTER A WITH DOT ABOVE AND MACRON
-0x01E1 LATIN SMALL LETTER A WITH DOT ABOVE AND MACRON
 0x01E2 LATIN CAPITAL LETTER AE WITH MACRON
 0x01E3 LATIN SMALL LETTER AE WITH MACRON
-0x01E4 LATIN CAPITAL LETTER G WITH STROKE
-0x01E5 LATIN SMALL LETTER G WITH STROKE
 0x01E6 LATIN CAPITAL LETTER G WITH CARON
 0x01E7 LATIN SMALL LETTER G WITH CARON
-0x01E8 LATIN CAPITAL LETTER K WITH CARON
-0x01E9 LATIN SMALL LETTER K WITH CARON
 0x01EA LATIN CAPITAL LETTER O WITH OGONEK
 0x01EB LATIN SMALL LETTER O WITH OGONEK
-0x01EC LATIN CAPITAL LETTER O WITH OGONEK AND MACRON
-0x01ED LATIN SMALL LETTER O WITH OGONEK AND MACRON
-0x01EE LATIN CAPITAL LETTER EZH WITH CARON
-0x01EF LATIN SMALL LETTER EZH WITH CARON
-0x01F4 LATIN CAPITAL LETTER G WITH ACUTE
-0x01F5 LATIN SMALL LETTER G WITH ACUTE
+0x01F0 LATIN SMALL LETTER J WITH CARON
 0x01F8 LATIN CAPITAL LETTER N WITH GRAVE
 0x01F9 LATIN SMALL LETTER N WITH GRAVE
+0x01FC LATIN CAPITAL LETTER AE WITH ACUTE
+0x01FD LATIN SMALL LETTER AE WITH ACUTE
 0x01FE LATIN CAPITAL LETTER O WITH STROKE AND ACUTE
 0x01FF LATIN SMALL LETTER O WITH STROKE AND ACUTE
 0x0200 LATIN CAPITAL LETTER A WITH DOUBLE GRAVE
 0x0201 LATIN SMALL LETTER A WITH DOUBLE GRAVE
-0x0202 LATIN CAPITAL LETTER A WITH INVERTED BREVE
-0x0203 LATIN SMALL LETTER A WITH INVERTED BREVE
 0x0204 LATIN CAPITAL LETTER E WITH DOUBLE GRAVE
 0x0205 LATIN SMALL LETTER E WITH DOUBLE GRAVE
-0x0206 LATIN CAPITAL LETTER E WITH INVERTED BREVE
-0x0207 LATIN SMALL LETTER E WITH INVERTED BREVE
 0x0208 LATIN CAPITAL LETTER I WITH DOUBLE GRAVE
 0x0209 LATIN SMALL LETTER I WITH DOUBLE GRAVE
-0x020A LATIN CAPITAL LETTER I WITH INVERTED BREVE
-0x020B LATIN SMALL LETTER I WITH INVERTED BREVE
 0x020C LATIN CAPITAL LETTER O WITH DOUBLE GRAVE
 0x020D LATIN SMALL LETTER O WITH DOUBLE GRAVE
-0x020E LATIN CAPITAL LETTER O WITH INVERTED BREVE
-0x020F LATIN SMALL LETTER O WITH INVERTED BREVE
-0x0210 LATIN CAPITAL LETTER R WITH DOUBLE GRAVE
-0x0211 LATIN SMALL LETTER R WITH DOUBLE GRAVE
 0x0212 LATIN CAPITAL LETTER R WITH INVERTED BREVE
 0x0213 LATIN SMALL LETTER R WITH INVERTED BREVE
 0x0214 LATIN CAPITAL LETTER U WITH DOUBLE GRAVE
 0x0215 LATIN SMALL LETTER U WITH DOUBLE GRAVE
-0x0216 LATIN CAPITAL LETTER U WITH INVERTED BREVE
-0x0217 LATIN SMALL LETTER U WITH INVERTED BREVE
-0x021E LATIN CAPITAL LETTER H WITH CARON
-0x021F LATIN SMALL LETTER H WITH CARON
-0x0220 LATIN CAPITAL LETTER N WITH LONG RIGHT LEG
-0x0222 LATIN CAPITAL LETTER OU
-0x0223 LATIN SMALL LETTER OU
 0x0226 LATIN CAPITAL LETTER A WITH DOT ABOVE
 0x0227 LATIN SMALL LETTER A WITH DOT ABOVE
 0x0228 LATIN CAPITAL LETTER E WITH CEDILLA
 0x0229 LATIN SMALL LETTER E WITH CEDILLA
-0x022A LATIN CAPITAL LETTER O WITH DIAERESIS AND MACRON
-0x022B LATIN SMALL LETTER O WITH DIAERESIS AND MACRON
-0x022C LATIN CAPITAL LETTER O WITH TILDE AND MACRON
-0x022D LATIN SMALL LETTER O WITH TILDE AND MACRON
-0x022E LATIN CAPITAL LETTER O WITH DOT ABOVE
-0x022F LATIN SMALL LETTER O WITH DOT ABOVE
-0x0230 LATIN CAPITAL LETTER O WITH DOT ABOVE AND MACRON
-0x0231 LATIN SMALL LETTER O WITH DOT ABOVE AND MACRON
 0x0232 LATIN CAPITAL LETTER Y WITH MACRON
 0x0233 LATIN SMALL LETTER Y WITH MACRON
-0x023A LATIN CAPITAL LETTER A WITH STROKE
-0x023B LATIN CAPITAL LETTER C WITH STROKE
-0x023C LATIN SMALL LETTER C WITH STROKE
-0x023D LATIN CAPITAL LETTER L WITH BAR
-0x023E LATIN CAPITAL LETTER T WITH DIAGONAL STROKE
 0x0241 LATIN CAPITAL LETTER GLOTTAL STOP
 0x0242 LATIN SMALL LETTER GLOTTAL STOP
-0x0243 LATIN CAPITAL LETTER B WITH STROKE
 0x0244 LATIN CAPITAL LETTER U BAR
 0x0245 LATIN CAPITAL LETTER TURNED V
-0x0246 LATIN CAPITAL LETTER E WITH STROKE
-0x0247 LATIN SMALL LETTER E WITH STROKE
 0x0248 LATIN CAPITAL LETTER J WITH STROKE
 0x0249 LATIN SMALL LETTER J WITH STROKE
-0x024A LATIN CAPITAL LETTER SMALL Q WITH HOOK TAIL
-0x024B LATIN SMALL LETTER Q WITH HOOK TAIL
 0x024C LATIN CAPITAL LETTER R WITH STROKE
 0x024D LATIN SMALL LETTER R WITH STROKE
-0x024E LATIN CAPITAL LETTER Y WITH STROKE
-0x024F LATIN SMALL LETTER Y WITH STROKE
+0x0250 LATIN SMALL LETTER TURNED A
 0x0251 LATIN SMALL LETTER ALPHA
 0x0253 LATIN SMALL LETTER B WITH HOOK
 0x0254 LATIN SMALL LETTER OPEN O
 0x0256 LATIN SMALL LETTER D WITH TAIL
 0x0257 LATIN SMALL LETTER D WITH HOOK
 0x0259 LATIN SMALL LETTER SCHWA
 0x025B LATIN SMALL LETTER OPEN E
 0x0260 LATIN SMALL LETTER G WITH HOOK
 0x0263 LATIN SMALL LETTER GAMMA
+0x0264 LATIN SMALL LETTER RAMS HORN
 0x0265 LATIN SMALL LETTER TURNED H
 0x0266 LATIN SMALL LETTER H WITH HOOK
 0x0268 LATIN SMALL LETTER I WITH STROKE
 0x0269 LATIN SMALL LETTER IOTA
 0x026A LATIN LETTER SMALL CAPITAL I
-0x026B LATIN SMALL LETTER L WITH MIDDLE TILDE
-0x026C LATIN SMALL LETTER L WITH BELT
 0x026F LATIN SMALL LETTER TURNED M
 0x0272 LATIN SMALL LETTER N WITH LEFT HOOK
 0x0275 LATIN SMALL LETTER BARRED O
 0x027D LATIN SMALL LETTER R WITH TAIL
-0x027E LATIN SMALL LETTER R WITH FISHHOOK
 0x0283 LATIN SMALL LETTER ESH
 0x0288 LATIN SMALL LETTER T WITH RETROFLEX HOOK
 0x0289 LATIN SMALL LETTER U BAR
 0x028A LATIN SMALL LETTER UPSILON
 0x028B LATIN SMALL LETTER V WITH HOOK
 0x028C LATIN SMALL LETTER TURNED V
 0x0292 LATIN SMALL LETTER EZH
 0x0294 LATIN LETTER GLOTTAL STOP
-0x0295 LATIN LETTER PHARYNGEAL VOICED FRICATIVE
 0x0298 LATIN LETTER BILABIAL CLICK
 0x029D LATIN SMALL LETTER J WITH CROSSED-TAIL
-0x02B0 MODIFIER LETTER SMALL H
 0x02B7 MODIFIER LETTER SMALL W
-0x02BB MODIFIER LETTER TURNED COMMA
 0x02BC MODIFIER LETTER APOSTROPHE
-0x02BE MODIFIER LETTER RIGHT HALF RING
-0x02BF MODIFIER LETTER LEFT HALF RING
 0x02C0 MODIFIER LETTER GLOTTAL STOP
-0x02CA MODIFIER LETTER ACUTE ACCENT
-0x02CB MODIFIER LETTER GRAVE ACCENT
+0x02C6 MODIFIER LETTER CIRCUMFLEX ACCENT
+0x02C8 MODIFIER LETTER VERTICAL LINE
 0x02D7 MODIFIER LETTER MINUS SIGN
 0x02EE MODIFIER LETTER DOUBLE APOSTROPHE
+0x0300 COMBINING GRAVE ACCENT
+0x0301 COMBINING ACUTE ACCENT
+0x0302 COMBINING CIRCUMFLEX ACCENT
+0x0303 COMBINING TILDE
+0x0304 COMBINING MACRON
+0x0306 COMBINING BREVE
+0x0307 COMBINING DOT ABOVE
+0x0308 COMBINING DIAERESIS
+0x030A COMBINING RING ABOVE
+0x030B COMBINING DOUBLE ACUTE ACCENT
+0x030C COMBINING CARON
 0x030D COMBINING VERTICAL LINE ABOVE
 0x030F COMBINING DOUBLE GRAVE ACCENT
-0x0310 COMBINING CANDRABINDU
 0x0311 COMBINING INVERTED BREVE
-0x0313 COMBINING COMMA ABOVE
+0x0323 COMBINING DOT BELOW
+0x0324 COMBINING DIAERESIS BELOW
 0x0325 COMBINING RING BELOW
-0x0329 COMBINING VERTICAL LINE BELOW
+0x0327 COMBINING CEDILLA
+0x0328 COMBINING OGONEK
 0x032D COMBINING CIRCUMFLEX ACCENT BELOW
 0x032F COMBINING INVERTED BREVE BELOW
 0x0330 COMBINING TILDE BELOW
 0x0331 COMBINING MACRON BELOW
-0x0332 COMBINING LOW LINE
-0x0334 COMBINING TILDE OVERLAY
-0x0358 COMBINING DOT ABOVE RIGHT
+0x035F COMBINING DOUBLE MACRON BELOW
+0x1D43 MODIFIER LETTER SMALL A
+0x1D49 MODIFIER LETTER SMALL E
+0x1D4B MODIFIER LETTER SMALL OPEN E
+0x1D52 MODIFIER LETTER SMALL O
+0x1D53 MODIFIER LETTER SMALL OPEN O
 0x1D58 MODIFIER LETTER SMALL U
-0x1D5B MODIFIER LETTER SMALL V
 0x1D7D LATIN SMALL LETTER P WITH STROKE
-0x1DBB MODIFIER LETTER SMALL Z
+0x1DA4 MODIFIER LETTER SMALL I WITH STROKE
+0x1DB6 MODIFIER LETTER SMALL U BAR
 0x1DC4 COMBINING MACRON-ACUTE
 0x1DC5 COMBINING GRAVE-MACRON
 0x1DC6 COMBINING MACRON-GRAVE
 0x1DC7 COMBINING ACUTE-MACRON
-0x1DCA COMBINING LATIN SMALL LETTER R BELOW
-0x1E00 LATIN CAPITAL LETTER A WITH RING BELOW
-0x1E01 LATIN SMALL LETTER A WITH RING BELOW
-0x1E02 LATIN CAPITAL LETTER B WITH DOT ABOVE
-0x1E03 LATIN SMALL LETTER B WITH DOT ABOVE
 0x1E04 LATIN CAPITAL LETTER B WITH DOT BELOW
 0x1E05 LATIN SMALL LETTER B WITH DOT BELOW
 0x1E06 LATIN CAPITAL LETTER B WITH LINE BELOW
 0x1E07 LATIN SMALL LETTER B WITH LINE BELOW
-0x1E08 LATIN CAPITAL LETTER C WITH CEDILLA AND ACUTE
-0x1E09 LATIN SMALL LETTER C WITH CEDILLA AND ACUTE
 0x1E0A LATIN CAPITAL LETTER D WITH DOT ABOVE
 0x1E0B LATIN SMALL LETTER D WITH DOT ABOVE
 0x1E0C LATIN CAPITAL LETTER D WITH DOT BELOW
 0x1E0D LATIN SMALL LETTER D WITH DOT BELOW
 0x1E0E LATIN CAPITAL LETTER D WITH LINE BELOW
 0x1E0F LATIN SMALL LETTER D WITH LINE BELOW
-0x1E10 LATIN CAPITAL LETTER D WITH CEDILLA
-0x1E11 LATIN SMALL LETTER D WITH CEDILLA
 0x1E12 LATIN CAPITAL LETTER D WITH CIRCUMFLEX BELOW
 0x1E13 LATIN SMALL LETTER D WITH CIRCUMFLEX BELOW
 0x1E14 LATIN CAPITAL LETTER E WITH MACRON AND GRAVE
 0x1E15 LATIN SMALL LETTER E WITH MACRON AND GRAVE
-0x1E16 LATIN CAPITAL LETTER E WITH MACRON AND ACUTE
-0x1E17 LATIN SMALL LETTER E WITH MACRON AND ACUTE
-0x1E18 LATIN CAPITAL LETTER E WITH CIRCUMFLEX BELOW
-0x1E19 LATIN SMALL LETTER E WITH CIRCUMFLEX BELOW
 0x1E1A LATIN CAPITAL LETTER E WITH TILDE BELOW
 0x1E1B LATIN SMALL LETTER E WITH TILDE BELOW
-0x1E1C LATIN CAPITAL LETTER E WITH CEDILLA AND BREVE
-0x1E1D LATIN SMALL LETTER E WITH CEDILLA AND BREVE
-0x1E1E LATIN CAPITAL LETTER F WITH DOT ABOVE
-0x1E1F LATIN SMALL LETTER F WITH DOT ABOVE
-0x1E20 LATIN CAPITAL LETTER G WITH MACRON
-0x1E21 LATIN SMALL LETTER G WITH MACRON
 0x1E22 LATIN CAPITAL LETTER H WITH DOT ABOVE
 0x1E23 LATIN SMALL LETTER H WITH DOT ABOVE
 0x1E24 LATIN CAPITAL LETTER H WITH DOT BELOW
 0x1E25 LATIN SMALL LETTER H WITH DOT BELOW
-0x1E26 LATIN CAPITAL LETTER H WITH DIAERESIS
-0x1E27 LATIN SMALL LETTER H WITH DIAERESIS
-0x1E28 LATIN CAPITAL LETTER H WITH CEDILLA
-0x1E29 LATIN SMALL LETTER H WITH CEDILLA
-0x1E2A LATIN CAPITAL LETTER H WITH BREVE BELOW
-0x1E2B LATIN SMALL LETTER H WITH BREVE BELOW
 0x1E2C LATIN CAPITAL LETTER I WITH TILDE BELOW
 0x1E2D LATIN SMALL LETTER I WITH TILDE BELOW
 0x1E2E LATIN CAPITAL LETTER I WITH DIAERESIS AND ACUTE
 0x1E2F LATIN SMALL LETTER I WITH DIAERESIS AND ACUTE
-0x1E30 LATIN CAPITAL LETTER K WITH ACUTE
-0x1E31 LATIN SMALL LETTER K WITH ACUTE
 0x1E32 LATIN CAPITAL LETTER K WITH DOT BELOW
 0x1E33 LATIN SMALL LETTER K WITH DOT BELOW
 0x1E34 LATIN CAPITAL LETTER K WITH LINE BELOW
 0x1E35 LATIN SMALL LETTER K WITH LINE BELOW
 0x1E36 LATIN CAPITAL LETTER L WITH DOT BELOW
 0x1E37 LATIN SMALL LETTER L WITH DOT BELOW
-0x1E38 LATIN CAPITAL LETTER L WITH DOT BELOW AND MACRON
-0x1E39 LATIN SMALL LETTER L WITH DOT BELOW AND MACRON
-0x1E3A LATIN CAPITAL LETTER L WITH LINE BELOW
-0x1E3B LATIN SMALL LETTER L WITH LINE BELOW
 0x1E3C LATIN CAPITAL LETTER L WITH CIRCUMFLEX BELOW
 0x1E3D LATIN SMALL LETTER L WITH CIRCUMFLEX BELOW
 0x1E3E LATIN CAPITAL LETTER M WITH ACUTE
 0x1E3F LATIN SMALL LETTER M WITH ACUTE
-0x1E40 LATIN CAPITAL LETTER M WITH DOT ABOVE
-0x1E41 LATIN SMALL LETTER M WITH DOT ABOVE
 0x1E42 LATIN CAPITAL LETTER M WITH DOT BELOW
 0x1E43 LATIN SMALL LETTER M WITH DOT BELOW
 0x1E44 LATIN CAPITAL LETTER N WITH DOT ABOVE
 0x1E45 LATIN SMALL LETTER N WITH DOT ABOVE
 0x1E46 LATIN CAPITAL LETTER N WITH DOT BELOW
 0x1E47 LATIN SMALL LETTER N WITH DOT BELOW
 0x1E48 LATIN CAPITAL LETTER N WITH LINE BELOW
 0x1E49 LATIN SMALL LETTER N WITH LINE BELOW
 0x1E4A LATIN CAPITAL LETTER N WITH CIRCUMFLEX BELOW
 0x1E4B LATIN SMALL LETTER N WITH CIRCUMFLEX BELOW
 0x1E4C LATIN CAPITAL LETTER O WITH TILDE AND ACUTE
 0x1E4D LATIN SMALL LETTER O WITH TILDE AND ACUTE
-0x1E4E LATIN CAPITAL LETTER O WITH TILDE AND DIAERESIS
-0x1E4F LATIN SMALL LETTER O WITH TILDE AND DIAERESIS
-0x1E50 LATIN CAPITAL LETTER O WITH MACRON AND GRAVE
-0x1E51 LATIN SMALL LETTER O WITH MACRON AND GRAVE
-0x1E52 LATIN CAPITAL LETTER O WITH MACRON AND ACUTE
-0x1E53 LATIN SMALL LETTER O WITH MACRON AND ACUTE
 0x1E54 LATIN CAPITAL LETTER P WITH ACUTE
 0x1E55 LATIN SMALL LETTER P WITH ACUTE
-0x1E56 LATIN CAPITAL LETTER P WITH DOT ABOVE
-0x1E57 LATIN SMALL LETTER P WITH DOT ABOVE
-0x1E58 LATIN CAPITAL LETTER R WITH DOT ABOVE
-0x1E59 LATIN SMALL LETTER R WITH DOT ABOVE
 0x1E5A LATIN CAPITAL LETTER R WITH DOT BELOW
 0x1E5B LATIN SMALL LETTER R WITH DOT BELOW
-0x1E5C LATIN CAPITAL LETTER R WITH DOT BELOW AND MACRON
-0x1E5D LATIN SMALL LETTER R WITH DOT BELOW AND MACRON
-0x1E5E LATIN CAPITAL LETTER R WITH LINE BELOW
-0x1E5F LATIN SMALL LETTER R WITH LINE BELOW
 0x1E60 LATIN CAPITAL LETTER S WITH DOT ABOVE
 0x1E61 LATIN SMALL LETTER S WITH DOT ABOVE
 0x1E62 LATIN CAPITAL LETTER S WITH DOT BELOW
 0x1E63 LATIN SMALL LETTER S WITH DOT BELOW
-0x1E64 LATIN CAPITAL LETTER S WITH ACUTE AND DOT ABOVE
-0x1E65 LATIN SMALL LETTER S WITH ACUTE AND DOT ABOVE
-0x1E66 LATIN CAPITAL LETTER S WITH CARON AND DOT ABOVE
-0x1E67 LATIN SMALL LETTER S WITH CARON AND DOT ABOVE
-0x1E68 LATIN CAPITAL LETTER S WITH DOT BELOW AND DOT ABOVE
-0x1E69 LATIN SMALL LETTER S WITH DOT BELOW AND DOT ABOVE
 0x1E6A LATIN CAPITAL LETTER T WITH DOT ABOVE
 0x1E6B LATIN SMALL LETTER T WITH DOT ABOVE
 0x1E6C LATIN CAPITAL LETTER T WITH DOT BELOW
 0x1E6D LATIN SMALL LETTER T WITH DOT BELOW
 0x1E6E LATIN CAPITAL LETTER T WITH LINE BELOW
 0x1E6F LATIN SMALL LETTER T WITH LINE BELOW
 0x1E70 LATIN CAPITAL LETTER T WITH CIRCUMFLEX BELOW
 0x1E71 LATIN SMALL LETTER T WITH CIRCUMFLEX BELOW
 0x1E72 LATIN CAPITAL LETTER U WITH DIAERESIS BELOW
 0x1E73 LATIN SMALL LETTER U WITH DIAERESIS BELOW
 0x1E74 LATIN CAPITAL LETTER U WITH TILDE BELOW
 0x1E75 LATIN SMALL LETTER U WITH TILDE BELOW
-0x1E76 LATIN CAPITAL LETTER U WITH CIRCUMFLEX BELOW
-0x1E77 LATIN SMALL LETTER U WITH CIRCUMFLEX BELOW
 0x1E78 LATIN CAPITAL LETTER U WITH TILDE AND ACUTE
 0x1E79 LATIN SMALL LETTER U WITH TILDE AND ACUTE
-0x1E7A LATIN CAPITAL LETTER U WITH MACRON AND DIAERESIS
-0x1E7B LATIN SMALL LETTER U WITH MACRON AND DIAERESIS
 0x1E7C LATIN CAPITAL LETTER V WITH TILDE
 0x1E7D LATIN SMALL LETTER V WITH TILDE
 0x1E7E LATIN CAPITAL LETTER V WITH DOT BELOW
 0x1E7F LATIN SMALL LETTER V WITH DOT BELOW
-0x1E86 LATIN CAPITAL LETTER W WITH DOT ABOVE
-0x1E87 LATIN SMALL LETTER W WITH DOT ABOVE
-0x1E88 LATIN CAPITAL LETTER W WITH DOT BELOW
-0x1E89 LATIN SMALL LETTER W WITH DOT BELOW
+0x1E84 LATIN CAPITAL LETTER W WITH DIAERESIS
+0x1E85 LATIN SMALL LETTER W WITH DIAERESIS
 0x1E8A LATIN CAPITAL LETTER X WITH DOT ABOVE
 0x1E8B LATIN SMALL LETTER X WITH DOT ABOVE
-0x1E8C LATIN CAPITAL LETTER X WITH DIAERESIS
-0x1E8D LATIN SMALL LETTER X WITH DIAERESIS
-0x1E8E LATIN CAPITAL LETTER Y WITH DOT ABOVE
-0x1E8F LATIN SMALL LETTER Y WITH DOT ABOVE
-0x1E90 LATIN CAPITAL LETTER Z WITH CIRCUMFLEX
-0x1E91 LATIN SMALL LETTER Z WITH CIRCUMFLEX
 0x1E92 LATIN CAPITAL LETTER Z WITH DOT BELOW
 0x1E93 LATIN SMALL LETTER Z WITH DOT BELOW
-0x1E94 LATIN CAPITAL LETTER Z WITH LINE BELOW
-0x1E95 LATIN SMALL LETTER Z WITH LINE BELOW
+0x1E96 LATIN SMALL LETTER H WITH LINE BELOW
+0x1EA0 LATIN CAPITAL LETTER A WITH DOT BELOW
 0x1EA1 LATIN SMALL LETTER A WITH DOT BELOW
 0x1EAC LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND DOT BELOW
 0x1EAD LATIN SMALL LETTER A WITH CIRCUMFLEX AND DOT BELOW
 0x1EB8 LATIN CAPITAL LETTER E WITH DOT BELOW
 0x1EB9 LATIN SMALL LETTER E WITH DOT BELOW
 0x1EBC LATIN CAPITAL LETTER E WITH TILDE
 0x1EBD LATIN SMALL LETTER E WITH TILDE
@@ -372,42 +477,44 @@
 0x1ECB LATIN SMALL LETTER I WITH DOT BELOW
 0x1ECC LATIN CAPITAL LETTER O WITH DOT BELOW
 0x1ECD LATIN SMALL LETTER O WITH DOT BELOW
 0x1ED8 LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND DOT BELOW
 0x1ED9 LATIN SMALL LETTER O WITH CIRCUMFLEX AND DOT BELOW
 0x1EE4 LATIN CAPITAL LETTER U WITH DOT BELOW
 0x1EE5 LATIN SMALL LETTER U WITH DOT BELOW
-0x207F SUPERSCRIPT LATIN SMALL LETTER N
-0x20AD KIP SIGN
-0x2C60 LATIN CAPITAL LETTER L WITH DOUBLE BAR
-0x2C61 LATIN SMALL LETTER L WITH DOUBLE BAR
-0x2C62 LATIN CAPITAL LETTER L WITH MIDDLE TILDE
+0x1EF2 LATIN CAPITAL LETTER Y WITH GRAVE
+0x1EF3 LATIN SMALL LETTER Y WITH GRAVE
+0x1EF8 LATIN CAPITAL LETTER Y WITH TILDE
+0x1EF9 LATIN SMALL LETTER Y WITH TILDE
+0x2013 EN DASH
+0x2014 EM DASH
+0x2018 LEFT SINGLE QUOTATION MARK
+0x2019 RIGHT SINGLE QUOTATION MARK
+0x201C LEFT DOUBLE QUOTATION MARK
+0x201D RIGHT DOUBLE QUOTATION MARK
+0x2026 HORIZONTAL ELLIPSIS
+0x2039 SINGLE LEFT-POINTING ANGLE QUOTATION MARK
+0x203A SINGLE RIGHT-POINTING ANGLE QUOTATION MARK
+0x2071 SUPERSCRIPT LATIN SMALL LETTER I
+0x24B6 CIRCLED LATIN CAPITAL LETTER A
+0x24D0 CIRCLED LATIN SMALL LETTER A
 0x2C63 LATIN CAPITAL LETTER P WITH STROKE
 0x2C64 LATIN CAPITAL LETTER R WITH TAIL
-0x2C65 LATIN SMALL LETTER A WITH STROKE
-0x2C66 LATIN SMALL LETTER T WITH DIAGONAL STROKE
 0x2C6D LATIN CAPITAL LETTER ALPHA
+0x2C6F LATIN CAPITAL LETTER TURNED A
 0x2C72 LATIN CAPITAL LETTER W WITH HOOK
 0x2C73 LATIN SMALL LETTER W WITH HOOK
-0xA726 LATIN CAPITAL LETTER HENG
-0xA727 LATIN SMALL LETTER HENG
-0xA740 LATIN CAPITAL LETTER K WITH STROKE
-0xA741 LATIN SMALL LETTER K WITH STROKE
 0xA789 MODIFIER LETTER COLON
 0xA78A MODIFIER LETTER SHORT EQUALS SIGN
 0xA78B LATIN CAPITAL LETTER SALTILLO
 0xA78C LATIN SMALL LETTER SALTILLO
 0xA78D LATIN CAPITAL LETTER TURNED H
-0xA7A8 LATIN CAPITAL LETTER S WITH OBLIQUE STROKE
-0xA7A9 LATIN SMALL LETTER S WITH OBLIQUE STROKE
 0xA7AA LATIN CAPITAL LETTER H WITH HOOK
-0xA7AD LATIN CAPITAL LETTER L WITH BELT
 0xA7AE LATIN CAPITAL LETTER SMALL CAPITAL I
 0xA7B2 LATIN CAPITAL LETTER J WITH CROSSED-TAIL
-0xA7B3 LATIN CAPITAL LETTER CHI
 0xA7B4 LATIN CAPITAL LETTER BETA
 0xA7B5 LATIN SMALL LETTER BETA
 0xA7B6 LATIN CAPITAL LETTER OMEGA
 0xA7B7 LATIN SMALL LETTER OMEGA
-0xA7B8 LATIN CAPITAL LETTER U WITH STROKE
-0xA7B9 LATIN SMALL LETTER U WITH STROKE
-0xAB53 LATIN SMALL LETTER CHI
+0xA7C7 LATIN CAPITAL LETTER D WITH SHORT STROKE OVERLAY
+0xA7C8 LATIN SMALL LETTER D WITH SHORT STROKE OVERLAY
+0xA7CB
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_Beyond.nam`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x00B0 DEGREE SIGN
 0x0108 LATIN CAPITAL LETTER C WITH CIRCUMFLEX
 0x0109 LATIN SMALL LETTER C WITH CIRCUMFLEX
 0x011C LATIN CAPITAL LETTER G WITH CIRCUMFLEX
 0x011D LATIN SMALL LETTER G WITH CIRCUMFLEX
 0x0124 LATIN CAPITAL LETTER H WITH CIRCUMFLEX
 0x0125 LATIN SMALL LETTER H WITH CIRCUMFLEX
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Core.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_Core.nam`

 * *Files 2% similar despite different names*

```diff
@@ -206,16 +206,14 @@
 0x011F LATIN SMALL LETTER G WITH BREVE
 0x0120 LATIN CAPITAL LETTER G WITH DOT ABOVE
 0x0121 LATIN SMALL LETTER G WITH DOT ABOVE
 0x0122 LATIN CAPITAL LETTER G WITH CEDILLA
 0x0123 LATIN SMALL LETTER G WITH CEDILLA
 0x0126 LATIN CAPITAL LETTER H WITH STROKE
 0x0127 LATIN SMALL LETTER H WITH STROKE
-0x0128 LATIN CAPITAL LETTER I WITH TILDE
-0x0129 LATIN SMALL LETTER I WITH TILDE
 0x012A LATIN CAPITAL LETTER I WITH MACRON
 0x012B LATIN SMALL LETTER I WITH MACRON
 0x012E LATIN CAPITAL LETTER I WITH OGONEK
 0x012F LATIN SMALL LETTER I WITH OGONEK
 0x0130 LATIN CAPITAL LETTER I WITH DOT ABOVE
 0x0131 LATIN SMALL LETTER DOTLESS I
 0x0136 LATIN CAPITAL LETTER K WITH CEDILLA
@@ -246,16 +244,14 @@
 0x015B LATIN SMALL LETTER S WITH ACUTE
 0x015E LATIN CAPITAL LETTER S WITH CEDILLA
 0x015F LATIN SMALL LETTER S WITH CEDILLA
 0x0160 LATIN CAPITAL LETTER S WITH CARON
 0x0161 LATIN SMALL LETTER S WITH CARON
 0x0164 LATIN CAPITAL LETTER T WITH CARON
 0x0165 LATIN SMALL LETTER T WITH CARON
-0x0168 LATIN CAPITAL LETTER U WITH TILDE
-0x0169 LATIN SMALL LETTER U WITH TILDE
 0x016A LATIN CAPITAL LETTER U WITH MACRON
 0x016B LATIN SMALL LETTER U WITH MACRON
 0x016E LATIN CAPITAL LETTER U WITH RING ABOVE
 0x016F LATIN SMALL LETTER U WITH RING ABOVE
 0x0170 LATIN CAPITAL LETTER U WITH DOUBLE ACUTE
 0x0171 LATIN SMALL LETTER U WITH DOUBLE ACUTE
 0x0172 LATIN CAPITAL LETTER U WITH OGONEK
@@ -272,15 +268,14 @@
 0x017D LATIN CAPITAL LETTER Z WITH CARON
 0x017E LATIN SMALL LETTER Z WITH CARON
 0x0218 LATIN CAPITAL LETTER S WITH COMMA BELOW
 0x0219 LATIN SMALL LETTER S WITH COMMA BELOW
 0x021A LATIN CAPITAL LETTER T WITH COMMA BELOW
 0x021B LATIN SMALL LETTER T WITH COMMA BELOW
 0x0237 LATIN SMALL LETTER DOTLESS J
-0x02BC MODIFIER LETTER APOSTROPHE
 0x02C6 MODIFIER LETTER CIRCUMFLEX ACCENT
 0x02C7 CARON
 0x02D8 BREVE
 0x02D9 DOT ABOVE
 0x02DA RING ABOVE
 0x02DB OGONEK
 0x02DC SMALL TILDE
@@ -302,20 +297,16 @@
 0x1E80 LATIN CAPITAL LETTER W WITH GRAVE
 0x1E81 LATIN SMALL LETTER W WITH GRAVE
 0x1E82 LATIN CAPITAL LETTER W WITH ACUTE
 0x1E83 LATIN SMALL LETTER W WITH ACUTE
 0x1E84 LATIN CAPITAL LETTER W WITH DIAERESIS
 0x1E85 LATIN SMALL LETTER W WITH DIAERESIS
 0x1E9E LATIN CAPITAL LETTER SHARP S
-0x1EBC LATIN CAPITAL LETTER E WITH TILDE
-0x1EBD LATIN SMALL LETTER E WITH TILDE
 0x1EF2 LATIN CAPITAL LETTER Y WITH GRAVE
 0x1EF3 LATIN SMALL LETTER Y WITH GRAVE
-0x1EF8 LATIN CAPITAL LETTER Y WITH TILDE
-0x1EF9 LATIN SMALL LETTER Y WITH TILDE
 0x2013 EN DASH
 0x2014 EM DASH
 0x2018 LEFT SINGLE QUOTATION MARK
 0x2019 RIGHT SINGLE QUOTATION MARK
 0x201A SINGLE LOW-9 QUOTATION MARK
 0x201C LEFT DOUBLE QUOTATION MARK
 0x201D RIGHT DOUBLE QUOTATION MARK
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_Kernel.nam`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x0020 SPACE
 0x0021 EXCLAMATION MARK
 0x0022 QUOTATION MARK
 0x0023 NUMBER SIGN
 0x0024 DOLLAR SIGN
 0x0025 PERCENT SIGN
 0x0026 AMPERSAND
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_Plus.nam`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x00A6 BROKEN BAR
 0x00AC NOT SIGN
 0x00B1 PLUS-MINUS SIGN
 0x00B2 SUPERSCRIPT TWO
 0x00B3 SUPERSCRIPT THREE
 0x00B5 MICRO SIGN
 0x00B9 SUPERSCRIPT ONE
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam` & `glyphsets-1.0.0/data/results/nam/GF_Latin_Beyond.nam`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,135 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+0x00B0 DEGREE SIGN
+0x0108 LATIN CAPITAL LETTER C WITH CIRCUMFLEX
+0x0109 LATIN SMALL LETTER C WITH CIRCUMFLEX
+0x011C LATIN CAPITAL LETTER G WITH CIRCUMFLEX
+0x011D LATIN SMALL LETTER G WITH CIRCUMFLEX
+0x0124 LATIN CAPITAL LETTER H WITH CIRCUMFLEX
+0x0125 LATIN SMALL LETTER H WITH CIRCUMFLEX
 0x0128 LATIN CAPITAL LETTER I WITH TILDE
 0x0129 LATIN SMALL LETTER I WITH TILDE
+0x0134 LATIN CAPITAL LETTER J WITH CIRCUMFLEX
+0x0135 LATIN SMALL LETTER J WITH CIRCUMFLEX
+0x0138 LATIN SMALL LETTER KRA
+0x015C LATIN CAPITAL LETTER S WITH CIRCUMFLEX
+0x015D LATIN SMALL LETTER S WITH CIRCUMFLEX
+0x0162 LATIN CAPITAL LETTER T WITH CEDILLA
+0x0163 LATIN SMALL LETTER T WITH CEDILLA
+0x0166 LATIN CAPITAL LETTER T WITH STROKE
+0x0167 LATIN SMALL LETTER T WITH STROKE
 0x0168 LATIN CAPITAL LETTER U WITH TILDE
 0x0169 LATIN SMALL LETTER U WITH TILDE
-0x01A0 LATIN CAPITAL LETTER O WITH HORN
-0x01A1 LATIN SMALL LETTER O WITH HORN
-0x01AF LATIN CAPITAL LETTER U WITH HORN
-0x01B0 LATIN SMALL LETTER U WITH HORN
-0x0309 COMBINING HOOK ABOVE
-0x031B COMBINING HORN
+0x0186 LATIN CAPITAL LETTER OPEN O
+0x018F LATIN CAPITAL LETTER SCHWA
+0x0190 LATIN CAPITAL LETTER OPEN E
+0x0194 LATIN CAPITAL LETTER GAMMA
+0x0197 LATIN CAPITAL LETTER I WITH STROKE
+0x019A LATIN SMALL LETTER L WITH BAR
+0x019B LATIN SMALL LETTER LAMBDA WITH STROKE
+0x01B1 LATIN CAPITAL LETTER UPSILON
+0x01B7 LATIN CAPITAL LETTER EZH
+0x01C2 LATIN LETTER ALVEOLAR CLICK
+0x01CD LATIN CAPITAL LETTER A WITH CARON
+0x01CE LATIN SMALL LETTER A WITH CARON
+0x01CF LATIN CAPITAL LETTER I WITH CARON
+0x01D0 LATIN SMALL LETTER I WITH CARON
+0x01D1 LATIN CAPITAL LETTER O WITH CARON
+0x01D2 LATIN SMALL LETTER O WITH CARON
+0x01D3 LATIN CAPITAL LETTER U WITH CARON
+0x01D4 LATIN SMALL LETTER U WITH CARON
+0x01E4 LATIN CAPITAL LETTER G WITH STROKE
+0x01E5 LATIN SMALL LETTER G WITH STROKE
+0x01E6 LATIN CAPITAL LETTER G WITH CARON
+0x01E7 LATIN SMALL LETTER G WITH CARON
+0x01E8 LATIN CAPITAL LETTER K WITH CARON
+0x01E9 LATIN SMALL LETTER K WITH CARON
+0x01EA LATIN CAPITAL LETTER O WITH OGONEK
+0x01EB LATIN SMALL LETTER O WITH OGONEK
+0x01EC LATIN CAPITAL LETTER O WITH OGONEK AND MACRON
+0x01ED LATIN SMALL LETTER O WITH OGONEK AND MACRON
+0x01EE LATIN CAPITAL LETTER EZH WITH CARON
+0x01EF LATIN SMALL LETTER EZH WITH CARON
+0x01F0 LATIN SMALL LETTER J WITH CARON
+0x023A LATIN CAPITAL LETTER A WITH STROKE
+0x023B LATIN CAPITAL LETTER C WITH STROKE
+0x023C LATIN SMALL LETTER C WITH STROKE
+0x023D LATIN CAPITAL LETTER L WITH BAR
+0x023E LATIN CAPITAL LETTER T WITH DIAGONAL STROKE
+0x0241 LATIN CAPITAL LETTER GLOTTAL STOP
+0x0254 LATIN SMALL LETTER OPEN O
+0x0259 LATIN SMALL LETTER SCHWA
+0x025B LATIN SMALL LETTER OPEN E
+0x0263 LATIN SMALL LETTER GAMMA
+0x0268 LATIN SMALL LETTER I WITH STROKE
+0x0269 LATIN SMALL LETTER IOTA
+0x026A LATIN LETTER SMALL CAPITAL I
+0x026B LATIN SMALL LETTER L WITH MIDDLE TILDE
+0x026C LATIN SMALL LETTER L WITH BELT
+0x028A LATIN SMALL LETTER UPSILON
+0x0292 LATIN SMALL LETTER EZH
+0x0294 LATIN LETTER GLOTTAL STOP
+0x0295 LATIN LETTER PHARYNGEAL VOICED FRICATIVE
+0x02B7 MODIFIER LETTER SMALL W
+0x02B8 MODIFIER LETTER SMALL Y
+0x02B9 MODIFIER LETTER PRIME
+0x02BB MODIFIER LETTER TURNED COMMA
+0x02BC MODIFIER LETTER APOSTROPHE
+0x02C0 MODIFIER LETTER GLOTTAL STOP
+0x02C8 MODIFIER LETTER VERTICAL LINE
+0x0313 COMBINING COMMA ABOVE
+0x0315 COMBINING COMMA ABOVE RIGHT
 0x0323 COMBINING DOT BELOW
-0x1EA0 LATIN CAPITAL LETTER A WITH DOT BELOW
-0x1EA1 LATIN SMALL LETTER A WITH DOT BELOW
-0x1EA2 LATIN CAPITAL LETTER A WITH HOOK ABOVE
-0x1EA3 LATIN SMALL LETTER A WITH HOOK ABOVE
-0x1EA4 LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND ACUTE
-0x1EA5 LATIN SMALL LETTER A WITH CIRCUMFLEX AND ACUTE
-0x1EA6 LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND GRAVE
-0x1EA7 LATIN SMALL LETTER A WITH CIRCUMFLEX AND GRAVE
-0x1EA8 LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND HOOK ABOVE
-0x1EA9 LATIN SMALL LETTER A WITH CIRCUMFLEX AND HOOK ABOVE
-0x1EAA LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND TILDE
-0x1EAB LATIN SMALL LETTER A WITH CIRCUMFLEX AND TILDE
-0x1EAC LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND DOT BELOW
-0x1EAD LATIN SMALL LETTER A WITH CIRCUMFLEX AND DOT BELOW
-0x1EAE LATIN CAPITAL LETTER A WITH BREVE AND ACUTE
-0x1EAF LATIN SMALL LETTER A WITH BREVE AND ACUTE
-0x1EB0 LATIN CAPITAL LETTER A WITH BREVE AND GRAVE
-0x1EB1 LATIN SMALL LETTER A WITH BREVE AND GRAVE
-0x1EB2 LATIN CAPITAL LETTER A WITH BREVE AND HOOK ABOVE
-0x1EB3 LATIN SMALL LETTER A WITH BREVE AND HOOK ABOVE
-0x1EB4 LATIN CAPITAL LETTER A WITH BREVE AND TILDE
-0x1EB5 LATIN SMALL LETTER A WITH BREVE AND TILDE
-0x1EB6 LATIN CAPITAL LETTER A WITH BREVE AND DOT BELOW
-0x1EB7 LATIN SMALL LETTER A WITH BREVE AND DOT BELOW
-0x1EB8 LATIN CAPITAL LETTER E WITH DOT BELOW
-0x1EB9 LATIN SMALL LETTER E WITH DOT BELOW
-0x1EBA LATIN CAPITAL LETTER E WITH HOOK ABOVE
-0x1EBB LATIN SMALL LETTER E WITH HOOK ABOVE
+0x0331 COMBINING MACRON BELOW
+0x0332 COMBINING LOW LINE
+0x0335 COMBINING SHORT STROKE OVERLAY
+0x03BB GREEK SMALL LETTER LAMDA
+0x03C7 GREEK SMALL LETTER CHI
+0x1DBB MODIFIER LETTER SMALL Z
+0x1DBF MODIFIER LETTER SMALL THETA
+0x1E14 LATIN CAPITAL LETTER E WITH MACRON AND GRAVE
+0x1E15 LATIN SMALL LETTER E WITH MACRON AND GRAVE
+0x1E16 LATIN CAPITAL LETTER E WITH MACRON AND ACUTE
+0x1E17 LATIN SMALL LETTER E WITH MACRON AND ACUTE
+0x1E20 LATIN CAPITAL LETTER G WITH MACRON
+0x1E21 LATIN SMALL LETTER G WITH MACRON
+0x1E24 LATIN CAPITAL LETTER H WITH DOT BELOW
+0x1E25 LATIN SMALL LETTER H WITH DOT BELOW
+0x1E30 LATIN CAPITAL LETTER K WITH ACUTE
+0x1E31 LATIN SMALL LETTER K WITH ACUTE
+0x1E32 LATIN CAPITAL LETTER K WITH DOT BELOW
+0x1E33 LATIN SMALL LETTER K WITH DOT BELOW
+0x1E34 LATIN CAPITAL LETTER K WITH LINE BELOW
+0x1E35 LATIN SMALL LETTER K WITH LINE BELOW
+0x1E36 LATIN CAPITAL LETTER L WITH DOT BELOW
+0x1E37 LATIN SMALL LETTER L WITH DOT BELOW
+0x1E42 LATIN CAPITAL LETTER M WITH DOT BELOW
+0x1E43 LATIN SMALL LETTER M WITH DOT BELOW
+0x1E46 LATIN CAPITAL LETTER N WITH DOT BELOW
+0x1E47 LATIN SMALL LETTER N WITH DOT BELOW
+0x1E48 LATIN CAPITAL LETTER N WITH LINE BELOW
+0x1E49 LATIN SMALL LETTER N WITH LINE BELOW
+0x1E50 LATIN CAPITAL LETTER O WITH MACRON AND GRAVE
+0x1E51 LATIN SMALL LETTER O WITH MACRON AND GRAVE
+0x1E52 LATIN CAPITAL LETTER O WITH MACRON AND ACUTE
+0x1E53 LATIN SMALL LETTER O WITH MACRON AND ACUTE
+0x1E62 LATIN CAPITAL LETTER S WITH DOT BELOW
+0x1E63 LATIN SMALL LETTER S WITH DOT BELOW
+0x1E6E LATIN CAPITAL LETTER T WITH LINE BELOW
+0x1E6F LATIN SMALL LETTER T WITH LINE BELOW
+0x1E90 LATIN CAPITAL LETTER Z WITH CIRCUMFLEX
+0x1E91 LATIN SMALL LETTER Z WITH CIRCUMFLEX
+0x1E94 LATIN CAPITAL LETTER Z WITH LINE BELOW
+0x1E95 LATIN SMALL LETTER Z WITH LINE BELOW
 0x1EBC LATIN CAPITAL LETTER E WITH TILDE
 0x1EBD LATIN SMALL LETTER E WITH TILDE
-0x1EBE LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND ACUTE
-0x1EBF LATIN SMALL LETTER E WITH CIRCUMFLEX AND ACUTE
-0x1EC0 LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND GRAVE
-0x1EC1 LATIN SMALL LETTER E WITH CIRCUMFLEX AND GRAVE
-0x1EC2 LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND HOOK ABOVE
-0x1EC3 LATIN SMALL LETTER E WITH CIRCUMFLEX AND HOOK ABOVE
-0x1EC4 LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND TILDE
-0x1EC5 LATIN SMALL LETTER E WITH CIRCUMFLEX AND TILDE
-0x1EC6 LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND DOT BELOW
-0x1EC7 LATIN SMALL LETTER E WITH CIRCUMFLEX AND DOT BELOW
-0x1EC8 LATIN CAPITAL LETTER I WITH HOOK ABOVE
-0x1EC9 LATIN SMALL LETTER I WITH HOOK ABOVE
 0x1ECA LATIN CAPITAL LETTER I WITH DOT BELOW
 0x1ECB LATIN SMALL LETTER I WITH DOT BELOW
-0x1ECC LATIN CAPITAL LETTER O WITH DOT BELOW
-0x1ECD LATIN SMALL LETTER O WITH DOT BELOW
-0x1ECE LATIN CAPITAL LETTER O WITH HOOK ABOVE
-0x1ECF LATIN SMALL LETTER O WITH HOOK ABOVE
-0x1ED0 LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND ACUTE
-0x1ED1 LATIN SMALL LETTER O WITH CIRCUMFLEX AND ACUTE
-0x1ED2 LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND GRAVE
-0x1ED3 LATIN SMALL LETTER O WITH CIRCUMFLEX AND GRAVE
-0x1ED4 LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND HOOK ABOVE
-0x1ED5 LATIN SMALL LETTER O WITH CIRCUMFLEX AND HOOK ABOVE
-0x1ED6 LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND TILDE
-0x1ED7 LATIN SMALL LETTER O WITH CIRCUMFLEX AND TILDE
-0x1ED8 LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND DOT BELOW
-0x1ED9 LATIN SMALL LETTER O WITH CIRCUMFLEX AND DOT BELOW
-0x1EDA LATIN CAPITAL LETTER O WITH HORN AND ACUTE
-0x1EDB LATIN SMALL LETTER O WITH HORN AND ACUTE
-0x1EDC LATIN CAPITAL LETTER O WITH HORN AND GRAVE
-0x1EDD LATIN SMALL LETTER O WITH HORN AND GRAVE
-0x1EDE LATIN CAPITAL LETTER O WITH HORN AND HOOK ABOVE
-0x1EDF LATIN SMALL LETTER O WITH HORN AND HOOK ABOVE
-0x1EE0 LATIN CAPITAL LETTER O WITH HORN AND TILDE
-0x1EE1 LATIN SMALL LETTER O WITH HORN AND TILDE
-0x1EE2 LATIN CAPITAL LETTER O WITH HORN AND DOT BELOW
-0x1EE3 LATIN SMALL LETTER O WITH HORN AND DOT BELOW
-0x1EE4 LATIN CAPITAL LETTER U WITH DOT BELOW
-0x1EE5 LATIN SMALL LETTER U WITH DOT BELOW
-0x1EE6 LATIN CAPITAL LETTER U WITH HOOK ABOVE
-0x1EE7 LATIN SMALL LETTER U WITH HOOK ABOVE
-0x1EE8 LATIN CAPITAL LETTER U WITH HORN AND ACUTE
-0x1EE9 LATIN SMALL LETTER U WITH HORN AND ACUTE
-0x1EEA LATIN CAPITAL LETTER U WITH HORN AND GRAVE
-0x1EEB LATIN SMALL LETTER U WITH HORN AND GRAVE
-0x1EEC LATIN CAPITAL LETTER U WITH HORN AND HOOK ABOVE
-0x1EED LATIN SMALL LETTER U WITH HORN AND HOOK ABOVE
-0x1EEE LATIN CAPITAL LETTER U WITH HORN AND TILDE
-0x1EEF LATIN SMALL LETTER U WITH HORN AND TILDE
-0x1EF0 LATIN CAPITAL LETTER U WITH HORN AND DOT BELOW
-0x1EF1 LATIN SMALL LETTER U WITH HORN AND DOT BELOW
-0x1EF4 LATIN CAPITAL LETTER Y WITH DOT BELOW
-0x1EF5 LATIN SMALL LETTER Y WITH DOT BELOW
-0x1EF6 LATIN CAPITAL LETTER Y WITH HOOK ABOVE
-0x1EF7 LATIN SMALL LETTER Y WITH HOOK ABOVE
 0x1EF8 LATIN CAPITAL LETTER Y WITH TILDE
-0x1EF9 LATIN SMALL LETTER Y WITH TILDE
+0x1EF9 LATIN SMALL LETTER Y WITH TILDE
+0x2144 TURNED SANS-SERIF CAPITAL Y
+0x2C62 LATIN CAPITAL LETTER L WITH MIDDLE TILDE
+0x2C65 LATIN SMALL LETTER A WITH STROKE
+0x2C66 LATIN SMALL LETTER T WITH DIAGONAL STROKE
+0xA78B LATIN CAPITAL LETTER SALTILLO
+0xA78C LATIN SMALL LETTER SALTILLO
+0xAB53 LATIN SMALL LETTER CHI
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_African.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,417 +1,520 @@
-apostrophemod
-Acaron
-Acircumflexdotbelow
-Adblgrave
-Adieresismacron
-Adotaccent
-Adotmacron
-Ainvertedbreve
-Alpha-latin
-Aringbelow
-Astroke
-AEmacron
-Bdotaccent
-Bdotbelow
-Beta-latin
+# This file is auto-generated; do not edit. See /README.md for instructions.
+exclam
+quotedbl
+numbersign
+percent
+ampersand
+quotesingle
+parenleft
+parenright
+asterisk
+plus
+comma
+hyphen
+period
+slash
+zero
+one
+two
+three
+four
+five
+six
+seven
+eight
+nine
+colon
+semicolon
+question
+at
+A
+B
+C
+D
+E
+F
+G
+H
+I
+J
+K
+L
+M
+N
+O
+P
+Q
+R
+S
+T
+U
+V
+W
+X
+Y
+Z
+bracketleft
+bracketright
+a
+b
+c
+d
+e
+f
+g
+h
+i
+j
+k
+l
+m
+n
+o
+p
+q
+r
+s
+t
+u
+v
+w
+x
+y
+z
+ordfeminine
+guillemetleft
+ordmasculine
+guillemetright
+Agrave
+Aacute
+Acircumflex
+Atilde
+Adieresis
+Aring
+AE
+Ccedilla
+Egrave
+Eacute
+Ecircumflex
+Edieresis
+Igrave
+Iacute
+Icircumflex
+Idieresis
+Ntilde
+Ograve
+Oacute
+Ocircumflex
+Otilde
+Odieresis
+Oslash
+Ugrave
+Uacute
+Ucircumflex
+Udieresis
+Yacute
+agrave
+aacute
+acircumflex
+atilde
+adieresis
+aring
+ae
+ccedilla
+egrave
+eacute
+ecircumflex
+edieresis
+igrave
+iacute
+icircumflex
+idieresis
+ntilde
+ograve
+oacute
+ocircumflex
+otilde
+odieresis
+oslash
+ugrave
+uacute
+ucircumflex
+udieresis
+yacute
+ydieresis
+Amacron
+amacron
+Abreve
+abreve
+Aogonek
+aogonek
+Ccircumflex
+ccircumflex
+Ccaron
+ccaron
+Dcroat
+dcroat
+Emacron
+emacron
+Edotaccent
+edotaccent
+Eogonek
+eogonek
+Ecaron
+ecaron
+Hcircumflex
+hcircumflex
+Hbar
+hbar
+Itilde
+itilde
+Imacron
+imacron
+Iogonek
+iogonek
+Lacute
+lacute
+Nacute
+nacute
+Ncaron
+ncaron
+Eng
+eng
+Omacron
+omacron
+Ohungarumlaut
+ohungarumlaut
+OE
+oe
+Racute
+racute
+Rcommaaccent
+rcommaaccent
+Rcaron
+rcaron
+Sacute
+sacute
+Scircumflex
+scircumflex
+Scedilla
+scedilla
+Scaron
+scaron
+Tcedilla
+tcedilla
+Tbar
+tbar
+Utilde
+utilde
+Umacron
+umacron
+Uhungarumlaut
+uhungarumlaut
+Uogonek
+uogonek
+Wcircumflex
+wcircumflex
+Ycircumflex
+ycircumflex
+Ydieresis
+Zdotaccent
+zdotaccent
+Zcaron
+zcaron
 Bhook
-Bmacronbelow
-Bstroke
-Ccedillaacute
-Chi-latin
+Btopbar
+btopbar
+Oopen
 Chook
-Cstroke
-Dcedilla
-Dcircumflexbelow
-Ddotaccent
-Ddotbelow
-Dhook
-Dmacronbelow
+chook
 Dtail
-Ecedilla
-Ecedillabreve
-Ecircumflexbelow
-Ecircumflexdotbelow
-Edblgrave
-Edotbelow
-Einvertedbreve
-Emacronacute
-Emacrongrave
-Eopen
-Ereversed
-Esh
-Estroke
-Etilde
-Etildebelow
+Dhook
+Eturned
 Schwa
-Ezh
-Ezhcaron
-Ezhreversed
-Fdotaccent
+Eopen
 Fhook
-Gacute
-Gcaron
+florin
 Ghook
-Glottalstop
-Gmacron
-Gstroke
-Hbrevebelow
-Hcaron
-Hcedilla
-Hdieresis
-Hdotaccent
-Hdotbelow
-Heng
-Hhook
-Hturned
-Icaron
-Idblgrave
-Idieresisacute
-Idotbelow
-Iinvertedbreve
+Gamma-latin
 Iota-latin
 Istroke
-Itilde
-Itildebelow
-Jcrossedtail
-Jstroke
-Kacute
-Kcaron
-Kdotbelow
 Khook
-Kmacronbelow
-Kstroke
-Lbar
-Lbelt
-Lcircumflexbelow
-Ldotbelow
-Ldotbelowmacron
-Ldoublebar
-Lmacronbelow
-Lmiddletilde
-Macute
-Mdotaccent
-Mdotbelow
+khook
 Mturned
-Ncircumflexbelow
-Ndotaccent
-Ndotbelow
-Ngrave
 Nhookleft
-Nlongrightleg
-Nmacronbelow
-OU
-Ocaron
-Ocenteredtilde
-Ocircumflexdotbelow
-Odblgrave
-Odieresismacron
-Odotaccent
-Odotaccentmacron
-Odotbelow
-Oinvertedbreve
-Omacronacute
-Omacrongrave
-Omega-latin
-Oogonek
-Oogonekmacron
-Oopen
-Oslashacute
-Otildeacute
-Otildedieresis
-Otildemacron
-Pacute
-Pdotaccent
+Obarred
 Phook
-Pstroke
-Qhooktail
-Rdblgrave
-Rdotaccent
-Rdotbelow
-Rdotbelowmacron
-Rinvertedbreve
-Rmacronbelow
-Rstroke
-Rtail
-Sacutedotaccent
-Saltillo
-Scarondotaccent
-Sdotaccent
-Sdotbelow
-Sdotbelowdotaccent
-Sobliquestroke
-Tcircumflexbelow
-Tdiagonalstroke
-Tdotaccent
-Tdotbelow
+phook
+Esh
 Thook
-Tmacronbelow
+thook
 Tretroflexhook
-Ubar
-Ucaron
-Ucircumflexbelow
-Udblgrave
-Udieresisacute
-Udieresisbelow
-Udieresiscaron
-Udieresisgrave
-Udieresismacron
-Udotbelow
-Uinvertedbreve
-Umacrondieresis
 Upsilon-latin
-Utilde
-Utildeacute
-Utildebelow
-Gamma-latin
-Vdotbelow
 Vhook
-Vtilde
-Vturned
-Wdotaccent
-Wdotbelow
-Whook
-Xdieresis
-Xdotaccent
-Ydotaccent
 Yhook
-Ymacron
-Ystroke
-Zcircumflex
-Zdotbelow
-Zmacronbelow
-Zstroke
-Ismall
+yhook
+Ezh
+Ezhreversed
+ezhreversed
+clickdental
+clicklateral
+clickalveolar
+clickretroflex
+Acaron
 acaron
-acircumflexdotbelow
+Icaron
+icaron
+Ocaron
+ocaron
+Ucaron
+ucaron
+Udieresisacute
+udieresisacute
+eturned
+AEmacron
+aemacron
+Gcaron
+gcaron
+Oogonek
+oogonek
+jcaron
+Ngrave
+ngrave
+AEacute
+aeacute
+Oslashacute
+oslashacute
+Adblgrave
 adblgrave
-adieresismacron
+Edblgrave
+edblgrave
+Idblgrave
+idblgrave
+Odblgrave
+odblgrave
+Rinvertedbreve
+rinvertedbreve
+Udblgrave
+udblgrave
+Adotaccent
 adotaccent
-adotbelow
-adotmacron
-ainvertedbreve
+Ecedilla
+ecedilla
+Ymacron
+ymacron
+Glottalstopsmall
+glottalstopsmall
+Ubar
+Vturned
+Jstroke
+jstroke
+Rstroke
+rstroke
+aturned
 alpha-latin
-aringbelow
-astroke
-aemacron
-bdotaccent
-bdotbelow
-beta-latin
 bhook
+oopen
+dtail
+dhook
+schwa
+eopen
+ghook
+gamma-latin
+ramshorn
+hturned
+hhook
+istroke
+iota-latin
+Ismall
+mturned
+nhookleft
+obarred
+rtail
+esh
+tretroflexhook
+ubar
+upsilon-latin
+vhook
+vturned
+ezh
+glottalstop
 bilabialclick
+jcrossedtail
+wmod
+apostrophemod
+glottalstopmod
+circumflex
+verticallinemod
+minusmod
+doubleapostrophemod
+gravecomb
+acutecomb
+circumflexcomb
+tildecomb
+macroncomb
+brevecomb
+dotaccentcomb
+dieresiscomb
+ringcomb
+hungarumlautcomb
+caroncomb
+verticallineabovecomb
+dblgravecomb
+breveinvertedcomb
+dotbelowcomb
+dieresisbelowcomb
+ringbelowcomb
+cedillacomb
+ogonekcomb
+circumflexbelowcomb
+breveinvertedbelowcomb
+tildebelowcomb
+macronbelowcomb
+doublemacronbelowcomb
+amod
+emod
+eOpenmod
+omod
+oOpenmod
+umod
+pstroke
+istrokemod
+ubarmod
+macronacutecomb
+gravemacroncomb
+macrongravecomb
+acutemacroncomb
+Bdotbelow
+bdotbelow
+Bmacronbelow
 bmacronbelow
-bstroke
-ccedillaacute
-chi-latin
-chook
-cstroke
-dcedilla
-dcircumflexbelow
+Ddotaccent
 ddotaccent
+Ddotbelow
 ddotbelow
-dhook
+Dmacronbelow
 dmacronbelow
-dtail
-ecedilla
-ecedillabreve
-ecircumflexbelow
-ecircumflexdotbelow
-edblgrave
-edotbelow
-einvertedbreve
-emacronacute
+Dcircumflexbelow
+dcircumflexbelow
+Emacrongrave
 emacrongrave
-eopen
-esh
-estroke
-etilde
+Etildebelow
 etildebelow
-eturned
-schwa
-ezh
-ezhcaron
-ezhreversed
-fdotaccent
-gacute
-gamma-latin
-gcaron
-ghook
-glottalstop
-glottalstopreversed
-glottalstopsmall
-gmacron
-gstroke
-hbrevebelow
-hcaron
-hcedilla
-hdieresis
+Hdotaccent
 hdotaccent
+Hdotbelow
 hdotbelow
-heng
-hhook
-hturned
-icaron
-idblgrave
-idieresisacute
-idotbelow
-iinvertedbreve
-iota-latin
-istroke
-itilde
+Itildebelow
 itildebelow
-jcrossedtail
-jstroke
-kacute
-kcaron
+Idieresisacute
+idieresisacute
+Kdotbelow
 kdotbelow
-khook
+Kmacronbelow
 kmacronbelow
-kstroke
-lambdastroke
-lbar
-lbelt
-lcircumflexbelow
+Ldotbelow
 ldotbelow
-ldotbelowmacron
-ldoublebar
-lmacronbelow
-lmiddletilde
+Lcircumflexbelow
+lcircumflexbelow
+Macute
 macute
-mdotaccent
+Mdotbelow
 mdotbelow
-mturned
-ncircumflexbelow
+Ndotaccent
 ndotaccent
+Ndotbelow
 ndotbelow
-ngrave
-nhookleft
-nlegrightlong
+Nmacronbelow
 nmacronbelow
-obarred
-ocaron
-ocircumflexdotbelow
-odblgrave
-odieresismacron
-odotaccent
-odotaccentmacron
-odotbelow
-oinvertedbreve
-omacronacute
-omacrongrave
-omega-latin
-oogonek
-oogonekmacron
-oopen
-oslashacute
+Ncircumflexbelow
+ncircumflexbelow
+Otildeacute
 otildeacute
-otildedieresis
-otildemacron
-ou
+Pacute
 pacute
-pdotaccent
-phook
-pstroke
-qhooktail
-rdblgrave
-rdotaccent
+Rdotbelow
 rdotbelow
-rdotbelowmacron
-rfishhook
-rinvertedbreve
-rmacronbelow
-rstroke
-rtail
-sacutedotaccent
-saltillo
-scarondotaccent
+Sdotaccent
 sdotaccent
+Sdotbelow
 sdotbelow
-sdotbelowdotaccent
-sobliquestroke
-tcircumflexbelow
-tdiagonalstroke
+Tdotaccent
 tdotaccent
+Tdotbelow
 tdotbelow
-thook
+Tmacronbelow
 tmacronbelow
-tretroflexhook
-ubar
-ucaron
-ucircumflexbelow
-udblgrave
-udieresisacute
+Tcircumflexbelow
+tcircumflexbelow
+Udieresisbelow
 udieresisbelow
-udieresiscaron
-udieresisgrave
-udieresismacron
-udotbelow
-uinvertedbreve
-umacrondieresis
-upsilon-latin
-utilde
-utildeacute
+Utildebelow
 utildebelow
-vdotbelow
-vhook
+Utildeacute
+utildeacute
+Vtilde
 vtilde
-vturned
-wdotaccent
-wdotbelow
-whook
-xdieresis
+Vdotbelow
+vdotbelow
+Wdieresis
+wdieresis
+Xdotaccent
 xdotaccent
-ydotaccent
-yhook
-ymacron
-ystroke
-zcircumflex
+Zdotbelow
 zdotbelow
-zmacronbelow
-zstroke
-hmod
-nmod
-wmod
-clickalveolar
-clickdental
-clicklateral
-clickretroflex
-umod
-vmod
-zmod
-florin
+hmacronbelow
+Adotbelow
+adotbelow
+Acircumflexdotbelow
+acircumflexdotbelow
+Edotbelow
+edotbelow
+Etilde
+etilde
+Ecircumflexdotbelow
+ecircumflexdotbelow
+Idotbelow
+idotbelow
+Odotbelow
+odotbelow
+Ocircumflexdotbelow
+ocircumflexdotbelow
+Udotbelow
+udotbelow
+Ygrave
+ygrave
+Ytilde
+ytilde
+endash
+emdash
+quoteleft
+quoteright
+quotedblleft
+quotedblright
+ellipsis
+guilsinglleft
+guilsinglright
+imod
+A.circled
+a.circled
+Pstroke
+Rtail
+Alpha-latin
+Aturned
+Whook
+whook
 colonmod
-doubleapostrophemod
-minusmod
 shortequalmod
-kip
-rbelowcomb
-gravecomb_macroncomb
-acutecomb_macroncomb
-macroncomb_gravecomb
-macroncomb_acutecomb
-verticallineabovecomb
-dblgravecomb
-candraBinducomb
-breveinvertedcomb
-commaabovecomb
-ringbelowcomb
-verticallinebelowcomb
-circumflexbelowcomb
-breveinvertedbelowcomb
-tildebelowcomb
-macronbelowcomb
-lowlinecomb
-tildeoverlaycomb
-dotaboverightcomb
-acutemacroncomb
-gravemacroncomb
-macronacutecomb
-macrongravecomb
-secondtonechinese
-fourthtonechinese
-commaturnedmod
-glottalstopmod
-ringhalfleft
-ringhalfright
+Saltillo
+saltillo
+Hturned
+Hhook
 uniA7AE
-uniA7B8
-uniA7B9
+Jcrossedtail
+Beta-latin
+beta-latin
+Omega-latin
+omega-latin
+uniA7C7
+uniA7C8
+uniA7CB
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_Core.txt`

 * *Files 4% similar despite different names*

```diff
@@ -206,16 +206,14 @@
 gbreve
 Gdotaccent
 gdotaccent
 Gcommaaccent
 gcommaaccent
 Hbar
 hbar
-Itilde
-itilde
 Imacron
 imacron
 Iogonek
 iogonek
 Idotaccent
 idotless
 Kcommaaccent
@@ -246,16 +244,14 @@
 sacute
 Scedilla
 scedilla
 Scaron
 scaron
 Tcaron
 tcaron
-Utilde
-utilde
 Umacron
 umacron
 Uring
 uring
 Uhungarumlaut
 uhungarumlaut
 Uogonek
@@ -272,15 +268,14 @@
 Zcaron
 zcaron
 Scommaaccent
 scommaaccent
 Tcommaaccent
 tcommaaccent
 jdotless
-apostrophemod
 circumflex
 caron
 breve
 dotaccent
 ring
 ogonek
 tilde
@@ -302,20 +297,16 @@
 Wgrave
 wgrave
 Wacute
 wacute
 Wdieresis
 wdieresis
 Germandbls
-Etilde
-etilde
 Ygrave
 ygrave
-Ytilde
-ytilde
 endash
 emdash
 quoteleft
 quoteright
 quotesinglbase
 quotedblleft
 quotedblright
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_Kernel.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,41 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+space
+exclam
+quotedbl
+numbersign
+dollar
+percent
+ampersand
+quotesingle
+parenleft
+parenright
+asterisk
+plus
+comma
+hyphen
+period
+slash
 zero
 one
 two
 three
 four
 five
 six
 seven
 eight
 nine
-space
-nbspace
-period
 colon
-ellipsis
-exclam
-asterisk
-numbersign
-slash
-backslash
-hyphen
-parenleft
-parenright
-braceleft
-braceright
-bracketleft
-bracketright
-quotedblleft
-quotedblright
-quoteleft
-quoteright
-quotedbl
-quotesingle
-bar
-plus
-multiply
-divide
+semicolon
+less
 equal
 greater
-less
-percent
-degree
+question
+at
 A
 B
 C
 D
 E
 F
 G
@@ -62,14 +54,20 @@
 T
 U
 V
 W
 X
 Y
 Z
+bracketleft
+backslash
+bracketright
+asciicircum
+underscore
+grave
 a
 b
 c
 d
 e
 f
 g
@@ -88,30 +86,32 @@
 t
 u
 v
 w
 x
 y
 z
-.notdef
-comma
-semicolon
-question
+braceleft
+bar
+braceright
+asciitilde
+uni00A0
+cent
+sterling
+yen
+copyright
+registered
+degree
 periodcentered
-bullet
+multiply
+divide
 endash
 emdash
-underscore
-at
-ampersand
-copyright
-registered
+quoteleft
+quoteright
+quotedblleft
+quotedblright
+bullet
+ellipsis
+Euro
 trademark
-cent
-dollar
-euro
-sterling
-yen
-minus
-asciitilde
-asciicircum
-grave
+minus
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Latin_Plus.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,140 +1,141 @@
-numero
-hryvnia
-tenge
-tugrik
-whiteSquare
+# This file is auto-generated; do not edit. See /README.md for instructions.
+brokenbar
+logicalnot
+plusminus
+twosuperior
+threesuperior
+micro
+onesuperior
+onequarter
+onehalf
+threequarters
 pi
+baht
 dblverticalbar
-kip
-zero.zero
-zero.tf
-one.tf
-two.tf
-three.tf
-four.tf
-five.tf
-six.tf
-seven.tf
-eight.tf
-nine.tf
-zero.dnom
-one.dnom
-two.dnom
-three.dnom
-four.dnom
-five.dnom
-six.dnom
-seven.dnom
-eight.dnom
-nine.dnom
-zero.numr
-one.numr
-two.numr
-three.numr
-four.numr
-five.numr
-six.numr
-seven.numr
-eight.numr
-nine.numr
+dagger
+daggerdbl
+perthousand
+minute
+second
 fraction
-onehalf
-onethird
-twothirds
-onequarter
-threequarters
+foursuperior
+fivesuperior
+sixsuperior
+sevensuperior
+eightsuperior
+ninesuperior
 oneinferior
 twoinferior
 threeinferior
 fourinferior
 fiveinferior
 sixinferior
 seveninferior
 eightinferior
 nineinferior
-onesuperior
-twosuperior
-threesuperior
-foursuperior
-fivesuperior
-sixsuperior
-sevensuperior
-eightsuperior
-ninesuperior
-leftanglebracket-math
-rightanglebracket-math
-baht
-minute
-second
-brokenbar
-dagger
-literSign
-daggerdbl
-estimated
-bitcoin
-cedi
 colonsign
+naira
+rupee
+won
+sheqel
 dong
+kip
+tugrik
+peso
 guarani
-lari
+hryvnia
+cedi
+tenge
+rupeeIndian
 liraTurkish
 manat
-naira
-peso
 ruble
-rupee
-rupeeIndian
-sheqel
-won
-notequal
-greaterequal
-lessequal
-plusminus
-approxequal
-logicalnot
-emptyset
-infinity
-integral
+lari
+bitcoin
+literSign
+numero
 Ohm
-increment
-product
-summation
-radical
-partialdiff
-micro
-perthousand
+estimated
+onethird
+twothirds
+leftArrow
 upArrow
-northEastArrow
 rightArrow
-southEastArrow
 downArrow
-southWestArrow
-leftArrow
-northWestArrow
 leftRightArrow
 upDownArrow
-blackCircle
-whiteCircle
-whiteBullet
-blackDiamond
-whiteDiamond
-lozenge
+northWestArrow
+northEastArrow
+southEastArrow
+southWestArrow
+partialdiff
+emptyset
+increment
+product
+summation
+radical
+infinity
+integral
+approxequal
+notequal
+lessequal
+greaterequal
 blackSquare
+whiteSquare
 blackSmallSquare
 whiteSmallSquare
 upBlackTriangle
-rightBlackTriangle
-downBlackTriangle
-leftBlackTriangle
 upWhiteTriangle
-rightWhiteTriangle
-downWhiteTriangle
-leftWhiteTriangle
 upBlackSmallTriangle
-rightBlackSmallTriangle
-downBlackSmallTriangle
-leftBlackSmallTriangle
 upWhiteSmallTriangle
+rightBlackTriangle
+rightWhiteTriangle
+rightBlackSmallTriangle
 rightWhiteSmallTriangle
+downBlackTriangle
+downWhiteTriangle
+downBlackSmallTriangle
 downWhiteSmallTriangle
-leftWhiteSmallTriangle
+leftBlackTriangle
+leftWhiteTriangle
+leftBlackSmallTriangle
+leftWhiteSmallTriangle
+blackDiamond
+whiteDiamond
+lozenge
+whiteCircle
+blackCircle
+whiteBullet
+leftanglebracket-math
+rightanglebracket-math
+zero.zero
+zero.tf
+one.tf
+two.tf
+three.tf
+four.tf
+five.tf
+six.tf
+seven.tf
+eight.tf
+nine.tf
+zero.dnom
+one.dnom
+two.dnom
+three.dnom
+four.dnom
+five.dnom
+six.dnom
+seven.dnom
+eight.dnom
+nine.dnom
+zero.numr
+one.numr
+two.numr
+three.numr
+four.numr
+five.numr
+six.numr
+seven.numr
+eight.numr
+nine.numr
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_Core.txt`

 * *Files 6% similar despite different names*

```diff
@@ -206,16 +206,14 @@
 gbreve
 Gdotaccent
 gdotaccent
 uni0122
 uni0123
 Hbar
 hbar
-Itilde
-itilde
 Imacron
 imacron
 Iogonek
 iogonek
 Idotaccent
 dotlessi
 uni0136
@@ -246,16 +244,14 @@
 sacute
 Scedilla
 scedilla
 Scaron
 scaron
 Tcaron
 tcaron
-Utilde
-utilde
 Umacron
 umacron
 Uring
 uring
 Uhungarumlaut
 uhungarumlaut
 Uogonek
@@ -272,15 +268,14 @@
 Zcaron
 zcaron
 uni0218
 uni0219
 uni021A
 uni021B
 uni0237
-uni02BC
 circumflex
 caron
 breve
 dotaccent
 ring
 ogonek
 tilde
@@ -302,20 +297,16 @@
 Wgrave
 wgrave
 Wacute
 wacute
 Wdieresis
 wdieresis
 uni1E9E
-uni1EBC
-uni1EBD
 Ygrave
 ygrave
-uni1EF8
-uni1EF9
 endash
 emdash
 quoteleft
 quoteright
 quotesinglbase
 quotedblleft
 quotedblright
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Latin_Plus.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,140 +1,141 @@
-uni2116
-uni20B4
-uni20B8
-uni20AE
-uni25A1
+# This file is auto-generated; do not edit. See /README.md for instructions.
+brokenbar
+logicalnot
+plusminus
+uni00B2
+uni00B3
+uni00B5
+uni00B9
+onequarter
+onehalf
+threequarters
 pi
+uni0E3F
 uni2016
-uni20AD
-zero.zero
-zero.tf
-one.tf
-two.tf
-three.tf
-four.tf
-five.tf
-six.tf
-seven.tf
-eight.tf
-nine.tf
-zero.dnom
-one.dnom
-two.dnom
-three.dnom
-four.dnom
-five.dnom
-six.dnom
-seven.dnom
-eight.dnom
-nine.dnom
-zero.numr
-one.numr
-two.numr
-three.numr
-four.numr
-five.numr
-six.numr
-seven.numr
-eight.numr
-nine.numr
+dagger
+daggerdbl
+perthousand
+minute
+second
 fraction
-onehalf
-uni2153
-uni2154
-onequarter
-threequarters
+uni2074
+uni2075
+uni2076
+uni2077
+uni2078
+uni2079
 uni2081
 uni2082
 uni2083
 uni2084
 uni2085
 uni2086
 uni2087
 uni2088
 uni2089
-uni00B9
-uni00B2
-uni00B3
-uni2074
-uni2075
-uni2076
-uni2077
-uni2078
-uni2079
-uni27E8
-uni27E9
-uni0E3F
-minute
-second
-brokenbar
-dagger
-uni2113
-daggerdbl
-estimated
-uni20BF
-uni20B5
 colonmonetary
+uni20A6
+uni20A8
+uni20A9
+uni20AA
 dong
+uni20AD
+uni20AE
+uni20B1
 uni20B2
-uni20BE
+uni20B4
+uni20B5
+uni20B8
+uni20B9
 uni20BA
 uni20BC
-uni20A6
-uni20B1
 uni20BD
-uni20A8
-uni20B9
-uni20AA
-uni20A9
-notequal
-greaterequal
-lessequal
-plusminus
-approxequal
-logicalnot
-emptyset
-infinity
-integral
+uni20BE
+uni20BF
+uni2113
+uni2116
 uni2126
-uni2206
-product
-summation
-radical
-partialdiff
-uni00B5
-perthousand
+estimated
+uni2153
+uni2154
+arrowleft
 arrowup
-uni2197
 arrowright
-uni2198
 arrowdown
-uni2199
-arrowleft
-uni2196
 arrowboth
 arrowupdn
-uni25CF
-circle
-openbullet
-uni25C6
-uni25C7
-lozenge
+uni2196
+uni2197
+uni2198
+uni2199
+partialdiff
+emptyset
+uni2206
+product
+summation
+radical
+infinity
+integral
+approxequal
+notequal
+lessequal
+greaterequal
 filledbox
+uni25A1
 uni25AA
 uni25AB
 triagup
-uni25B6
-triagdn
-uni25C0
 uni25B3
-uni25B7
-uni25BD
-uni25C1
 uni25B4
-uni25B8
-uni25BE
-uni25C2
 uni25B5
+uni25B6
+uni25B7
+uni25B8
 uni25B9
+triagdn
+uni25BD
+uni25BE
 uni25BF
-uni25C3
+uni25C0
+uni25C1
+uni25C2
+uni25C3
+uni25C6
+uni25C7
+lozenge
+circle
+uni25CF
+openbullet
+uni27E8
+uni27E9
+zero.zero
+zero.tf
+one.tf
+two.tf
+three.tf
+four.tf
+five.tf
+six.tf
+seven.tf
+eight.tf
+nine.tf
+zero.dnom
+one.dnom
+two.dnom
+three.dnom
+four.dnom
+five.dnom
+six.dnom
+seven.dnom
+eight.dnom
+nine.dnom
+zero.numr
+one.numr
+two.numr
+three.numr
+four.numr
+five.numr
+six.numr
+seven.numr
+eight.numr
+nine.numr
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs` & `glyphsets-1.0.0/data/definitions/per_glyphset/GF_Greek_Pro.stub.glyphs`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,28 @@
 {
-.appVersion = "3135";
+.appVersion = "3151";
 .formatVersion = 3;
-date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Phonetics APA";
-featurePrefixes = (
-{
-automatic = 1;
-code = "languagesystem DFLT dflt;
-
-languagesystem latn dflt;
-languagesystem latn AZE;
-languagesystem latn CRT;
-languagesystem latn KAZ;
-languagesystem latn TAT;
-languagesystem latn TRK;
-languagesystem latn ROM;
-languagesystem latn MOL;
-languagesystem latn CAT;
-";
-name = Languagesystems;
-}
-);
-features = (
+axes = (
 {
-automatic = 1;
-code = "feature locl;
-feature ordn;
-feature case;
-";
-tag = aalt;
-},
-{
-automatic = 1;
-code = "lookup ccmp_Other_1 {
-	@CombiningTopAccents = [acutecomb brevecomb caroncomb circumflexcomb commaturnedabovecomb dieresiscomb dotaccentcomb gravecomb hungarumlautcomb macroncomb ringcomb tildecomb];
-	@CombiningNonTopAccents = [cedillacomb ogonekcomb];
-	sub [i j]' @CombiningTopAccents by [idotless jdotless];
-	sub [i j]' @CombiningNonTopAccents @CombiningTopAccents by [idotless jdotless];
-} ccmp_Other_1;
-";
-tag = ccmp;
-},
-{
-automatic = 1;
-code = "lookup locl_latn_0 {
-	script latn;
-	language AZE;
-	sub i by idotaccent;
-	language CRT;
-	sub i by idotaccent;
-	language KAZ;
-	sub i by idotaccent;
-	language TAT;
-	sub i by idotaccent;
-	language TRK;
-	sub i by idotaccent;
-} locl_latn_0;
-
-lookup locl_latn_1 {
-	script latn;
-	language ROM;
-	sub Scedilla by Scommaaccent;
-	sub scedilla by scommaaccent;
-	language MOL;
-	sub Scedilla by Scommaaccent;
-	sub scedilla by scommaaccent;
-} locl_latn_1;
-
-lookup locl_latn_2 {
-	script latn;
-	language CAT;
-	sub l periodcentered' l by periodcentered.loclCAT;
-	sub L periodcentered' L by periodcentered.loclCAT.case;
-} locl_latn_2;
-";
-tag = locl;
-},
-{
-automatic = 1;
-code = "sub [zero one two three four five six seven eight nine] [A a]' by ordfeminine;
-sub [zero one two three four five six seven eight nine] [O o]' by ordmasculine;
-";
-tag = ordn;
-},
-{
-automatic = 1;
-code = "sub periodcentered.loclCAT by periodcentered.loclCAT.case;
-";
-tag = case;
+name = Weight;
+tag = wght;
+},
+{
+name = Width;
+tag = wdth;
 }
 );
+date = "2023-12-13 14:28:10 +0000";
+familyName = "Neue Schrift";
 fontMaster = (
 {
+axesValues = (
+100,
+100
+);
 id = m01;
 metricValues = (
 {
 over = 16;
 pos = 800;
 },
 {
@@ -118,245 +45,346 @@
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-glyphname = Cstroke;
-layers = (
+glyphname = plussuperior;
+unicode = 8314;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 571;
+glyphname = minussuperior;
+unicode = 8315;
 },
 {
-glyphname = Dsmall;
-layers = (
+glyphname = equalsuperior;
+unicode = 8316;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 7429;
+glyphname = plusinferior;
+unicode = 8330;
 },
 {
-glyphname = Ismallstroke;
-layers = (
+glyphname = minusinferior;
+unicode = 8331;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 7547;
+glyphname = equalinferior;
+unicode = 8332;
 },
 {
-glyphname = Usmallstroke;
-lastChange = "2022-09-14 12:52:34 +0000";
-layers = (
+glyphname = alephsymbol;
+unicode = 8501;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 7550;
+glyphname = betsymbol;
+unicode = 8502;
 },
 {
-glyphname = cstroke;
-layers = (
+glyphname = multiply.circled;
+unicode = 8855;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 572;
+glyphname = ellipsisvertical;
+unicode = 8942;
 },
 {
-glyphname = ezhcaron;
-layers = (
+glyphname = metricalbreve;
+unicode = 9169;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 495;
+glyphname = metricallongovershort;
+unicode = 9170;
 },
 {
-glyphname = jcaron;
-layers = (
+glyphname = metricalshortoverlong;
+unicode = 9171;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 496;
+glyphname = metricallongovertwoshorts;
+unicode = 9172;
 },
 {
-glyphname = lacute;
-layers = (
+glyphname = metricaltwoshortsoverlong;
+unicode = 9173;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 314;
+glyphname = metricaltwoshortsjoined;
+unicode = 9174;
 },
 {
-glyphname = lambdastroke;
-layers = (
+glyphname = metricaltriseme;
+unicode = 9175;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 411;
+glyphname = metricaltetraseme;
+unicode = 9176;
 },
 {
-glyphname = lbar;
-layers = (
+glyphname = metricalpentaseme;
+unicode = 9177;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 410;
+glyphname = doubleSolidusOperator;
+unicode = 11005;
 },
 {
-glyphname = odotaccent;
-layers = (
+glyphname = dblverticalbar;
+unicode = 8214;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 559;
+glyphname = referencemark;
+unicode = 8251;
 },
 {
-glyphname = rdotbelow;
-layers = (
+glyphname = undertie;
+unicode = 8255;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 7771;
+glyphname = asterism;
+unicode = 8258;
 },
 {
-glyphname = tcircumflexbelow;
-layers = (
+glyphname = threedotpunctuation;
+unicode = 8278;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 7793;
+glyphname = fourdotpunctuation;
+unicode = 8280;
 },
 {
-glyphname = wdotbelow;
-layers = (
+glyphname = fivedotpunctuation;
+unicode = 8281;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 7817;
+glyphname = twodotpunctuation;
+unicode = 8282;
 },
 {
-glyphname = xdotaccent;
-layers = (
+glyphname = fourdotmark;
+unicode = 8283;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 7819;
+glyphname = dottedcross;
+unicode = 8284;
 },
 {
-glyphname = ymod;
-layers = (
+glyphname = tricolon;
+unicode = 8285;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 696;
+glyphname = verticalfourdots;
+unicode = 8286;
 },
 {
-glyphname = lambda;
-layers = (
+glyphname = rightanglesubstitutionmarker;
+unicode = 11776;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 955;
+glyphname = rightangledottedsubstitutionmarker;
+unicode = 11777;
 },
 {
-glyphname = phi;
-layers = (
+glyphname = leftsubstitutionbracket;
+unicode = 11778;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 966;
+glyphname = rightsubstitutionbracket;
+unicode = 11779;
 },
 {
-glyphname = gmod;
-layers = (
+glyphname = leftdottedsubstitutionbracket;
+unicode = 11780;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 7501;
+glyphname = rightdottedsubstitutionbracket;
+unicode = 11781;
 },
 {
-glyphname = thetamod;
-layers = (
+glyphname = raisedinterpolationmarker;
+unicode = 11782;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 7615;
+glyphname = raiseddottedinterpolationmarker;
+unicode = 11783;
 },
 {
-glyphname = colonmod;
-layers = (
+glyphname = dottedtranspositionmarker;
+unicode = 11784;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 42889;
+glyphname = lefttranspositionbracket;
+unicode = 11785;
 },
 {
-glyphname = commaabovecomb;
-layers = (
+glyphname = righttranspositionbracket;
+unicode = 11786;
+},
 {
-layerId = m01;
-width = 600;
-}
-);
-unicode = 787;
+glyphname = raisedsquare;
+unicode = 11787;
+},
+{
+glyphname = leftraisedomissionbracket;
+unicode = 11788;
 },
 {
-glyphname = ogonekcomb;
-layers = (
+glyphname = rightraisedomissionbracket;
+unicode = 11789;
+},
+{
+glyphname = editorialcoronis;
+unicode = 11790;
+},
+{
+glyphname = paragraphos;
+unicode = 11791;
+},
+{
+glyphname = forkedparagraphos;
+unicode = 11792;
+},
+{
+glyphname = reversedforkedparagraphos;
+unicode = 11793;
+},
+{
+glyphname = hypodiastole;
+unicode = 11794;
+},
+{
+glyphname = dottedobelos;
+unicode = 11795;
+},
+{
+glyphname = downancora;
+unicode = 11796;
+},
+{
+glyphname = upancora;
+unicode = 11797;
+},
+{
+glyphname = dottedrightpointingangle;
+unicode = 11798;
+},
+{
+glyphname = doubleobliquehyphen;
+unicode = 11799;
+},
+{
+glyphname = anglebracketleft;
+unicode = 12296;
+},
+{
+glyphname = anglebracketright;
+unicode = 12297;
+},
+{
+glyphname = dblanglebracketleft;
+unicode = 12298;
+},
+{
+glyphname = dblanglebracketright;
+unicode = 12299;
+},
+{
+glyphname = cornerbracketleft;
+unicode = 12300;
+},
+{
+glyphname = cornerbracketright;
+unicode = 12301;
+},
+{
+glyphname = whitesquarebracketleft;
+unicode = 12314;
+},
+{
+glyphname = whitesquarebracketright;
+unicode = 12315;
+},
 {
-layerId = m01;
-width = 600;
+glyphname = dotaccent;
+unicode = 729;
+},
+{
+glyphname = overlinecomb;
+unicode = 773;
+},
+{
+glyphname = dotbelowcomb;
+unicode = 803;
+},
+{
+glyphname = asteriskbelowcomb;
+unicode = 857;
+},
+{
+glyphname = doublebrevebelowcomb;
+unicode = 860;
+},
+{
+glyphname = Stigma;
+unicode = 986;
+},
+{
+glyphname = stigma;
+unicode = 987;
+},
+{
+glyphname = Digamma;
+unicode = 988;
+},
+{
+glyphname = digamma;
+unicode = 989;
+},
+{
+glyphname = Koppa;
+unicode = 990;
+},
+{
+glyphname = koppa;
+unicode = 991;
+},
+{
+glyphname = Sampi;
+unicode = 992;
+},
+{
+glyphname = sampi;
+unicode = 993;
+},
+{
+glyphname = "litalic-math";
+unicode = 119897;
+},
+{
+glyphname = "M-fraktur";
+unicode = 120080;
+},
+{
+glyphname = "P-fraktur";
+unicode = 120083;
+},
+{
+glyphname = "S-fraktur";
+unicode = 120086;
+},
+{
+glyphname = "p-fraktur";
+unicode = 120109;
 }
 );
-unicode = 808;
-}
+instances = (
 );
+kerningLTR = {
+};
 metrics = (
 {
 type = ascender;
 },
 {
 type = "cap height";
 },
@@ -369,11 +397,13 @@
 {
 type = descender;
 },
 {
 type = "italic angle";
 }
 );
+stems = (
+);
 unitsPerEm = 1000;
 versionMajor = 1;
 versionMinor = 0;
 }
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Phonetics_APA.nam`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x013A LATIN SMALL LETTER L WITH ACUTE
 0x019A LATIN SMALL LETTER L WITH BAR
 0x019B LATIN SMALL LETTER LAMBDA WITH STROKE
 0x01EF LATIN SMALL LETTER EZH WITH CARON
 0x01F0 LATIN SMALL LETTER J WITH CARON
 0x022F LATIN SMALL LETTER O WITH DOT ABOVE
 0x023B LATIN CAPITAL LETTER C WITH STROKE
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Phonetics_DisorderedSpeech.nam`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x0021 EXCLAMATION MARK
 0x002A ASTERISK
 0x00A1 INVERTED EXCLAMATION MARK
 0x02A9 LATIN SMALL LETTER FENG DIGRAPH
 0x02AA LATIN SMALL LETTER LS DIGRAPH
 0x02AB LATIN SMALL LETTER LZ DIGRAPH
 0x02AC LATIN LETTER BILABIAL PERCUSSIVE
@@ -17,40 +18,22 @@
 0x034B COMBINING HOMOTHETIC ABOVE
 0x034C COMBINING ALMOST EQUAL TO ABOVE
 0x034D COMBINING LEFT RIGHT ARROW BELOW
 0x034E COMBINING UPWARDS ARROW BELOW
 0x0354 COMBINING LEFT ARROWHEAD BELOW
 0x0355 COMBINING RIGHT ARROWHEAD BELOW
 0x0362 COMBINING DOUBLE RIGHTWARDS ARROW BELOW
-0x10790 MODIFIER LETTER SMALL FENG DIGRAPH
-0x10799 MODIFIER LETTER SMALL LS DIGRAPH
-0x1079A MODIFIER LETTER SMALL LZ DIGRAPH
-0x1079C MODIFIER LETTER SMALL CAPITAL L WITH BELT
-0x1079D MODIFIER LETTER SMALL L WITH RETROFLEX HOOK AND BELT
-0x1079F MODIFIER LETTER SMALL LEZH WITH RETROFLEX HOOK
-0x107A1 MODIFIER LETTER SMALL TURNED Y WITH BELT
-0x107AA MODIFIER LETTER SMALL CAPITAL R
 0x1ABB COMBINING PARENTHESES ABOVE
 0x1ABD COMBINING PARENTHESES BELOW
 0x1AC1 COMBINING LEFT PARENTHESIS ABOVE LEFT
 0x1AC2 COMBINING RIGHT PARENTHESIS ABOVE RIGHT
 0x1AC3 COMBINING LEFT PARENTHESIS BELOW LEFT
 0x1AC4 COMBINING RIGHT PARENTHESIS BELOW RIGHT
 0x1D3A MODIFIER LETTER CAPITAL N
-0x1D453 MATHEMATICAL ITALIC SMALL F
-0x1D45D MATHEMATICAL ITALIC SMALL P
 0x1D4A MODIFIER LETTER SMALL SCHWA
-0x1DF00 LATIN SMALL LETTER FENG DIGRAPH WITH TRILL
-0x1DF01 LATIN SMALL LETTER REVERSED SCRIPT G
-0x1DF02 LATIN LETTER SMALL CAPITAL TURNED G
-0x1DF03 LATIN SMALL LETTER REVERSED K
-0x1DF04 LATIN LETTER SMALL CAPITAL L WITH BELT
-0x1DF05 LATIN SMALL LETTER LEZH WITH RETROFLEX HOOK
-0x1DF06 LATIN SMALL LETTER TURNED Y WITH BELT
-0x1DF07 LATIN SMALL LETTER REVERSED ENG
 0x208D SUBSCRIPT LEFT PARENTHESIS
 0x208E SUBSCRIPT RIGHT PARENTHESIS
 0x24B8 CIRCLED LATIN CAPITAL LETTER C
 0x24BB CIRCLED LATIN CAPITAL LETTER F
 0x24BC CIRCLED LATIN CAPITAL LETTER G
 0x24C1 CIRCLED LATIN CAPITAL LETTER L
 0x24C3 CIRCLED LATIN CAPITAL LETTER N
@@ -58,8 +41,26 @@
 0x24C7 CIRCLED LATIN CAPITAL LETTER R
 0x24C8 CIRCLED LATIN CAPITAL LETTER S
 0x24C9 CIRCLED LATIN CAPITAL LETTER T
 0x24CB CIRCLED LATIN CAPITAL LETTER V
 0x25EF LARGE CIRCLE
 0xA78E LATIN SMALL LETTER L WITH RETROFLEX HOOK AND BELT
 0xA7AF LATIN LETTER SMALL CAPITAL Q
-0xA7B0 LATIN CAPITAL LETTER TURNED K
+0xA7B0 LATIN CAPITAL LETTER TURNED K
+0x10790 MODIFIER LETTER SMALL FENG DIGRAPH
+0x10799 MODIFIER LETTER SMALL LS DIGRAPH
+0x1079A MODIFIER LETTER SMALL LZ DIGRAPH
+0x1079C MODIFIER LETTER SMALL CAPITAL L WITH BELT
+0x1079D MODIFIER LETTER SMALL L WITH RETROFLEX HOOK AND BELT
+0x1079F MODIFIER LETTER SMALL LEZH WITH RETROFLEX HOOK
+0x107A1 MODIFIER LETTER SMALL TURNED Y WITH BELT
+0x107AA MODIFIER LETTER SMALL CAPITAL R
+0x1D453 MATHEMATICAL ITALIC SMALL F
+0x1D45D MATHEMATICAL ITALIC SMALL P
+0x1DF00 LATIN SMALL LETTER FENG DIGRAPH WITH TRILL
+0x1DF01 LATIN SMALL LETTER REVERSED SCRIPT G
+0x1DF02 LATIN LETTER SMALL CAPITAL TURNED G
+0x1DF03 LATIN SMALL LETTER REVERSED K
+0x1DF04 LATIN LETTER SMALL CAPITAL L WITH BELT
+0x1DF05 LATIN SMALL LETTER LEZH WITH RETROFLEX HOOK
+0x1DF06 LATIN SMALL LETTER TURNED Y WITH BELT
+0x1DF07 LATIN SMALL LETTER REVERSED ENG
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Phonetics_IPAStandard.nam`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x0021 EXCLAMATION MARK
 0x002E FULL STOP
 0x007C VERTICAL LINE
 0x00E6 LATIN SMALL LETTER AE
 0x00E7 LATIN SMALL LETTER C WITH CEDILLA
 0x00F0 LATIN SMALL LETTER ETH
 0x00F8 LATIN SMALL LETTER O WITH STROKE
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,20 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 exclam
 asterisk
 exclamdown
-Kturned
-Kturned.circled
-bidentalpercussive
-bilabialpercussive
 fengdigraph
-lretroflexhookandbelt
 lsdigraph
 lzdigraph
+bilabialpercussive
+bidentalpercussive
 rturnedmod
 smod
-fitalic-math
-pitalic-math
-fitalic-math.subs
-pitalic-math.subs
-fitalic-math.sups
-pitalic-math.sups
-Nmod
-schwamod
-parenleftinferior
-parenrightinferior
-unaspiratedmod
 voicingmod
-C.circled
-F.circled
-G.circled
-L.circled
-N.circled
-P.circled
-R.circled
-S.circled
-T.circled
-V.circled
-largeCircle
+unaspiratedmod
 gbridgeabovecomb
 equalbelowcomb
 leftanglebelowcomb
 nottildeabovecomb
 homotheticabovecomb
 almostequaltoabovecomb
 arrowleftrightbelowcomb
@@ -47,24 +24,48 @@
 arrowdoublerightbelowcomb
 parentabovecomb
 parentbelowcomb
 uni1AC1
 uni1AC2
 uni1AC3
 uni1AC4
+Nmod
+schwamod
+parenleftinferior
+parenrightinferior
+C.circled
+F.circled
+G.circled
+L.circled
+N.circled
+P.circled
+R.circled
+S.circled
+T.circled
+V.circled
+largeCircle
+lretroflexhookandbelt
 uniA7AF
-u10790
-u10799
-u1079A
-u1079C
-u1079D
-u1079F
-u107A1
-u107AA
-u1DF00
-u1DF01
-u1DF02
-u1DF03
-u1DF04
-u1DF05
-u1DF06
-u1DF07
+Kturned
+uni10790
+uni10799
+uni1079A
+uni1079C
+uni1079D
+uni1079F
+uni107A1
+uni107AA
+fitalic-math
+pitalic-math
+uni1DF00
+uni1DF01
+uni1DF02
+uni1DF03
+uni1DF04
+uni1DF05
+uni1DF06
+uni1DF07
+Kturned.circled
+fitalic-math.subs
+pitalic-math.subs
+fitalic-math.sups
+pitalic-math.sups
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_Phonetics_IPAStandard.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,168 +1,169 @@
-period
+# This file is auto-generated; do not edit. See /README.md for instructions.
 exclam
+period
 bar
-dieresiscomb
-gravecomb
-acutecomb
-hungarumlautcomb
-macroncomb
-apostrophemod
-beta
-theta
-chi
-dblverticalbar
-undertie
-overlinecomb
-doublebrevebelowcomb
-Ismall
+ae
+ccedilla
+eth
+oslash
+hbar
+eng
+oe
+clickdental
+clicklateral
+clickalveolar
+clickretroflex
+edblgrave
+aturned
 alpha-latin
-beta-latin
+alphaturned-latin
 bhook
-bilabialclick
-chi-latin
-dhook
+oopen
+ccurl
 dtail
-edblgrave
-eopen
-esh
+dhook
+ereversed
 schwa
-ezh
-gamma-latin
+schwahook
+eopen
+eopenreversed
+eopenreversedhook
+eopenreversedclosed
+jdotlessstroke
 ghook
-glottalstop
-glottalstopreversed
-hhook
+gsingle
+Gsmall
+gamma-latin
+ramshorn
 hturned
+hhook
+henghook
 istroke
-jcrossedtail
-lbelt
+Ismall
 lmiddletilde
+lbelt
+lhookretroflex
+lezh
 mturned
+mlonglegturned
+mhook
 nhookleft
+nhookretroflex
+Nsmall
 obarred
-oopen
+OEsmall
+phi-latin
+rturned
+rlonglegturned
+rhookturned
+rhook
 rfishhook
-rtail
+Rsmall
+Rsmallinverted
+shook
+esh
+jdotlessstrokehook
 tretroflexhook
 ubar
 upsilon-latin
 vhook
 vturned
-hmod
-nmod
-wmod
-clickalveolar
-clickdental
-clicklateral
-clickretroflex
-dblgravecomb
-ringbelowcomb
-verticallinebelowcomb
-breveinvertedbelowcomb
-tildebelowcomb
-lowlinecomb
-tildeoverlaycomb
-acutemacroncomb
-gravemacroncomb
-macronacutecomb
-macrongravecomb
-verticallinemod
-ae
-ccedilla
-eth
-hbar
-eng
-oslash
-oe
-circumflexcomb
-caroncomb
-brevecomb
-ringcomb
-tildecomb
+wturned
+yturned
+Ysmall
+zretroflexhook
+zcurl
+ezh
+glottalstop
+glottalstopreversed
+bilabialclick
 Bsmall
-Gsmall
 Gsmallhook
 Hsmall
+jcrossedtail
 Lsmall
-Nsmall
-OEsmall
-Rsmall
-Rsmallinverted
-Ysmall
-alphaturned-latin
-aturned
-bmiddletilde
-ccurl
-dmiddletilde
-eopenreversed
-eopenreversedclosed
-eopenreversedhook
-ereversed
-schwahook
-fmiddletilde
 glottalstopstroke
 glottalstopstrokereversed
-gsingle
-henghook
-jdotlessstroke
-jdotlessstrokehook
-lezh
-lhookretroflex
-mhook
-mlonglegturned
-mmiddletilde
-nhookretroflex
-nmiddletilde
-phi-latin
-pmiddletilde
-ramshorn
-rfishhookmiddletilde
-rhookturned
-rlonglegturned
-rmiddletilde
-rturned
-shook
-smiddletilde
-tmiddletilde
-wturned
-yturned
-zcurl
-zmiddletilde
-zretroflexhook
+hmod
 jmod
-lmod
-raiseddownarrowmod
-raiseduparrowmod
+wmod
+apostrophemod
+glottalstopreversedmod
+verticallinemod
+verticallinelowmod
+colontriangularmod
+colontriangularhalfmod
+rhotichookmod
 gammamod-latin
-lowringmod
+lmod
 tonebarextrahighmod
-tonebarextralowmod
 tonebarhighmod
-tonebarlowmod
 tonebarmidmod
-rhotichookmod
-dottedCircle
+tonebarlowmod
+tonebarextralowmod
+lowringmod
+gravecomb
+acutecomb
+circumflexcomb
+tildecomb
+macroncomb
+overlinecomb
+brevecomb
+dieresiscomb
+ringcomb
+hungarumlautcomb
+caroncomb
+dblgravecomb
 lefttackbelowcomb
 righttackbelowcomb
 leftangleabovecomb
 ringhalfleftbelowcomb
 uptackbelowcomb
 downtackbelowcomb
 plusbelowcomb
 minusbelowcomb
 dieresisbelowcomb
+ringbelowcomb
+verticallinebelowcomb
 bridgebelowcomb
 caronbelowcomb
+breveinvertedbelowcomb
+tildebelowcomb
+lowlinecomb
+tildeoverlaycomb
 ringhalfrightbelowcomb
 bridgeinvertedbelowcomb
 squarebelowcomb
 seagullbelowcomb
 xabovecomb
 doubleverticallinebelowcomb
+doublebrevebelowcomb
 breveinverteddoublecomb
-acutegraveacutecomb
+beta
+theta
+chi
+bmiddletilde
+dmiddletilde
+fmiddletilde
+mmiddletilde
+nmiddletilde
+pmiddletilde
+rmiddletilde
+rfishhookmiddletilde
+smiddletilde
+tmiddletilde
+zmiddletilde
+macronacutecomb
+gravemacroncomb
+macrongravecomb
+acutemacroncomb
 graveacutegravecomb
-colontriangularhalfmod
-colontriangularmod
-glottalstopreversedmod
-verticallinelowmod
+acutegraveacutecomb
+dblverticalbar
+undertie
+nmod
+dottedCircle
+raiseduparrowmod
+raiseddownarrowmod
+beta-latin
+chi-latin
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,20 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 exclam
 asterisk
 exclamdown
-uniA7B0
-uniA7B0.circled
-uni02AD
-uni02AC
 uni02A9
-uniA78E
 uni02AA
 uni02AB
+uni02AC
+uni02AD
 uni02B4
 uni02E2
-u1D453
-u1D45D
-u1D453.subs
-u1D45D.subs
-u1D453.sups
-u1D45D.sups
-uni1D3A
-uni1D4A
-uni208D
-uni208E
-uni02ED
 uni02EC
-uni24B8
-uni24BB
-uni24BC
-uni24C1
-uni24C3
-uni24C5
-uni24C7
-uni24C8
-uni24C9
-uni24CB
-uni25EF
+uni02ED
 uni0346
 uni0347
 uni0349
 uni034A
 uni034B
 uni034C
 uni034D
@@ -47,24 +24,48 @@
 uni0362
 uni1ABB
 uni1ABD
 uni1AC1
 uni1AC2
 uni1AC3
 uni1AC4
+uni1D3A
+uni1D4A
+uni208D
+uni208E
+uni24B8
+uni24BB
+uni24BC
+uni24C1
+uni24C3
+uni24C5
+uni24C7
+uni24C8
+uni24C9
+uni24CB
+uni25EF
+uniA78E
 uniA7AF
-u10790
-u10799
-u1079A
-u1079C
-u1079D
-u1079F
-u107A1
-u107AA
-u1DF00
-u1DF01
-u1DF02
-u1DF03
-u1DF04
-u1DF05
-u1DF06
-u1DF07
+uniA7B0
+uni10790
+uni10799
+uni1079A
+uni1079C
+uni1079D
+uni1079F
+uni107A1
+uni107AA
+u1D453
+u1D45D
+uni1DF00
+uni1DF01
+uni1DF02
+uni1DF03
+uni1DF04
+uni1DF05
+uni1DF06
+uni1DF07
+uniA7B0.circled
+u1D453.subs
+u1D45D.subs
+u1D453.sups
+u1D45D.sups
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_Phonetics_IPAStandard.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,168 +1,169 @@
-period
+# This file is auto-generated; do not edit. See /README.md for instructions.
 exclam
+period
 bar
-uni0308
-gravecomb
-acutecomb
-uni030B
-uni0304
-uni02BC
-beta
-theta
-chi
-uni2016
-uni203F
-uni0305
-uni035C
-uni026A
+ae
+ccedilla
+eth
+oslash
+hbar
+eng
+oe
+uni01C0
+uni01C1
+uni01C2
+uni01C3
+uni0205
+uni0250
 uni0251
-uniA7B5
+uni0252
 uni0253
-uni0298
-uniAB53
-uni0257
+uni0254
+uni0255
 uni0256
-uni0205
-uni025B
-uni0283
+uni0257
+uni0258
 uni0259
-uni0292
-uni0263
+uni025A
+uni025B
+uni025C
+uni025D
+uni025E
+uni025F
 uni0260
-uni0294
-uni0295
-uni0266
+uni0261
+uni0262
+uni0263
+uni0264
 uni0265
+uni0266
+uni0267
 uni0268
-uni029D
-uni026C
+uni026A
 uni026B
+uni026C
+uni026D
+uni026E
 uni026F
+uni0270
+uni0271
 uni0272
+uni0273
+uni0274
 uni0275
-uni0254
+uni0276
+uni0278
+uni0279
+uni027A
+uni027B
+uni027D
 uni027E
-rtail
+uni0280
+uni0281
+uni0282
+uni0283
+uni0284
 uni0288
 uni0289
 uni028A
 uni028B
 uni028C
-uni02B0
-uni207F
-uni02B7
-uni01C2
-uni01C0
-uni01C1
-uni01C3
-uni030F
-uni0325
-uni0329
-uni032F
-uni0330
-uni0332
-uni0334
-uni1DC7
-uni1DC5
-uni1DC4
-uni1DC6
-uni02C8
-ae
-ccedilla
-eth
-hbar
-eng
-oslash
-oe
-uni0302
-uni030C
-uni0306
-uni030A
-tildecomb
+uni028D
+uni028E
+uni028F
+uni0290
+uni0291
+uni0292
+uni0294
+uni0295
+uni0298
 uni0299
-uni0262
 uni029B
 uni029C
+uni029D
 uni029F
-uni0274
-uni0276
-uni0280
-uni0281
-uni028F
-uni0252
-uni0250
-uni1D6C
-uni0255
-uni1D6D
-uni025C
-uni025E
-uni025D
-uni0258
-uni025A
-uni1D6E
 uni02A1
 uni02A2
-uni0261
-uni0267
-uni025F
-uni0284
-uni026E
-uni026D
-uni0271
-uni0270
-uni1D6F
-uni0273
-uni1D70
-uni0278
-uni1D71
-uni0264
-uni1D73
-uni027B
-uni027A
-uni1D72
-uni0279
-uni0282
-uni1D74
-uni1D75
-uni028D
-uni028E
-uni0291
-uni1D76
-uni0290
+uni02B0
 uni02B2
-uni02E1
-uniA71C
-uniA71B
+uni02B7
+uni02BC
+uni02C1
+uni02C8
+uni02CC
+uni02D0
+uni02D1
+uni02DE
 uni02E0
-uni02F3
+uni02E1
 uni02E5
-uni02E9
 uni02E6
-uni02E8
 uni02E7
-uni02DE
-uni25CC
+uni02E8
+uni02E9
+uni02F3
+gravecomb
+acutecomb
+uni0302
+tildecomb
+uni0304
+uni0305
+uni0306
+uni0308
+uni030A
+uni030B
+uni030C
+uni030F
 uni0318
 uni0319
 uni031A
 uni031C
 uni031D
 uni031E
 uni031F
 uni0320
 uni0324
+uni0325
+uni0329
 uni032A
 uni032C
+uni032F
+uni0330
+uni0332
+uni0334
 uni0339
 uni033A
 uni033B
 uni033C
 uni033D
 uni0348
+uni035C
 uni0361
-uni1DC9
+beta
+theta
+chi
+uni1D6C
+uni1D6D
+uni1D6E
+uni1D6F
+uni1D70
+uni1D71
+uni1D72
+uni1D73
+uni1D74
+uni1D75
+uni1D76
+uni1DC4
+uni1DC5
+uni1DC6
+uni1DC7
 uni1DC8
-uni02D1
-uni02D0
-uni02C1
-uni02CC
+uni1DC9
+uni2016
+uni203F
+uni207F
+uni25CC
+uniA71B
+uniA71C
+uniA7B5
+uniAB53
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs` & `glyphsets-1.0.0/data/definitions/per_glyphset/GF_Latin_Core.stub.glyphs`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 {
-.appVersion = "3124";
+.appVersion = "3246";
 .formatVersion = 3;
+axes = (
+{
+name = Weight;
+tag = wght;
+},
+{
+name = Width;
+tag = wdth;
+}
+);
 date = "2021-10-28 12:22:31 +0000";
-familyName = "GF TransLatin Pinyin";
+familyName = "GF Latin Core";
 featurePrefixes = (
 {
 automatic = 1;
 code = "languagesystem DFLT dflt;
 
 languagesystem latn dflt;
 languagesystem latn AZE;
@@ -88,14 +98,18 @@
 code = "sub periodcentered.loclCAT by periodcentered.loclCAT.case;
 ";
 tag = case;
 }
 );
 fontMaster = (
 {
+axesValues = (
+100,
+100
+);
 id = m01;
 metricValues = (
 {
 over = 16;
 pos = 800;
 },
 {
@@ -110,1126 +124,1029 @@
 over = -16;
 },
 {
 over = -16;
 pos = -200;
 },
 {
-over = -16;
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-color = 3;
-glyphname = Aacute;
-lastChange = "2022-04-29 09:57:47 +0000";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 193;
-},
-{
-color = 3;
-glyphname = Abreve;
-lastChange = "2022-04-29 09:57:47 +0000";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 258;
-},
-{
-glyphname = Acaron;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 461;
-},
-{
-color = 3;
-glyphname = Acircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 194;
-},
-{
-color = 3;
-glyphname = Acircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 194;
-},
-{
-color = 3;
-glyphname = Agrave;
-lastChange = "2022-04-29 09:57:47 +0000";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 192;
-},
-{
-glyphname = Amacron;
+glyphname = idotaccent;
+lastChange = "2022-03-04 12:31:03 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 256;
 },
 {
-color = 3;
-glyphname = Eacute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = jdotless;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 201;
+unicode = 567;
 },
 {
-color = 3;
-glyphname = Ebreve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = ordfeminine;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 276;
+unicode = 170;
 },
 {
-glyphname = Ecaron;
+glyphname = ordmasculine;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 282;
+unicode = 186;
 },
 {
-color = 3;
-glyphname = Ecircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = zero;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 202;
+unicode = 48;
 },
 {
-color = 3;
-glyphname = Egrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = one;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 200;
+unicode = 49;
 },
 {
-color = 3;
-glyphname = Emacron;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = two;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 274;
+unicode = 50;
 },
 {
-color = 3;
-glyphname = Iacute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = three;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 205;
+unicode = 51;
 },
 {
-color = 3;
-glyphname = Ibreve;
-lastChange = "2022-04-29 09:45:08 +0000";
+glyphname = four;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 300;
+unicode = 52;
 },
 {
-glyphname = Icaron;
+glyphname = five;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 463;
+unicode = 53;
 },
 {
-color = 3;
-glyphname = Icircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = six;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 206;
+unicode = 54;
 },
 {
-color = 3;
-glyphname = Idieresis;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = seven;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 207;
+unicode = 55;
 },
 {
-color = 3;
-glyphname = Igrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = eight;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 204;
+unicode = 56;
 },
 {
-glyphname = Imacron;
+glyphname = nine;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 298;
+unicode = 57;
 },
 {
-color = 3;
-glyphname = Macute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = space;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7742;
+unicode = 32;
 },
 {
-color = 3;
-glyphname = Nacute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = nbspace;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 323;
+unicode = 160;
 },
 {
-color = 3;
-glyphname = Ngrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+color = 10;
+glyphname = .notdef;
+lastChange = "2022-03-04 12:31:22 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 504;
 },
 {
-color = 3;
-glyphname = Oacute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = period;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 211;
+unicode = 46;
 },
 {
-color = 3;
-glyphname = Obreve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = comma;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 334;
+unicode = 44;
 },
 {
-glyphname = Ocaron;
+glyphname = colon;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 465;
+unicode = 58;
 },
 {
-color = 3;
-glyphname = Ocircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = semicolon;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 212;
+unicode = 59;
 },
 {
-color = 3;
-glyphname = Ograve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = ellipsis;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 210;
+unicode = 8230;
 },
 {
-color = 3;
-glyphname = Omacron;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = exclam;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 332;
+unicode = 33;
 },
 {
-color = 3;
-glyphname = Uacute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = exclamdown;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 218;
+unicode = 161;
 },
 {
-color = 3;
-glyphname = Ubreve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = question;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 364;
+unicode = 63;
 },
 {
-glyphname = Ucaron;
+glyphname = questiondown;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 467;
+unicode = 191;
 },
 {
-color = 3;
-glyphname = Ucircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = periodcentered;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 219;
+unicode = 183;
 },
 {
-glyphname = Udieresis;
+glyphname = bullet;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 220;
+unicode = 8226;
 },
 {
-glyphname = Udieresisacute;
+glyphname = asterisk;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 471;
+unicode = 42;
 },
 {
-glyphname = Udieresiscaron;
+glyphname = numbersign;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 473;
+unicode = 35;
 },
 {
-glyphname = Udieresisgrave;
+glyphname = slash;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 475;
+unicode = 47;
 },
 {
-glyphname = Udieresismacron;
+glyphname = backslash;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 469;
+unicode = 92;
 },
 {
-color = 3;
-glyphname = Ugrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = hyphen;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 217;
+unicode = 45;
 },
 {
-glyphname = Umacron;
+glyphname = endash;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 362;
+unicode = 8211;
 },
 {
-color = 3;
-glyphname = aacute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = emdash;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 225;
+unicode = 8212;
 },
 {
-color = 3;
-glyphname = abreve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = underscore;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 259;
+unicode = 95;
 },
 {
-glyphname = acaron;
+glyphname = parenleft;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 462;
+unicode = 40;
 },
 {
-color = 3;
-glyphname = acircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = parenright;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 226;
+unicode = 41;
 },
 {
-color = 3;
-glyphname = agrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = braceleft;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 224;
+unicode = 123;
 },
 {
-color = 3;
-glyphname = agrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = braceright;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 224;
+unicode = 125;
 },
 {
-glyphname = amacron;
+glyphname = bracketleft;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 257;
+unicode = 91;
 },
 {
-glyphname = eacute;
+glyphname = bracketright;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 233;
+unicode = 93;
 },
 {
-color = 3;
-glyphname = ebreve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = quotesinglbase;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 277;
+unicode = 8218;
 },
 {
-glyphname = ecaron;
+glyphname = quotedblbase;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 283;
+unicode = 8222;
 },
 {
-color = 3;
-glyphname = ecircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = quotedblleft;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 234;
+unicode = 8220;
 },
 {
-color = 3;
-glyphname = egrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = quotedblright;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 232;
+unicode = 8221;
 },
 {
-color = 3;
-glyphname = emacron;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = quoteleft;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 275;
+unicode = 8216;
 },
 {
-glyphname = iacute;
+glyphname = quoteright;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 237;
+unicode = 8217;
 },
 {
-color = 3;
-glyphname = ibreve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = guillemetleft;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 301;
+unicode = 171;
 },
 {
-glyphname = icaron;
+glyphname = guillemetright;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 464;
+unicode = 187;
 },
 {
-color = 3;
-glyphname = icircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = guilsinglleft;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 238;
+unicode = 8249;
 },
 {
-color = 3;
-glyphname = igrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = guilsinglright;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 236;
+unicode = 8250;
 },
 {
-color = 3;
-glyphname = igrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = quotedbl;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 236;
+unicode = 34;
 },
 {
-color = 3;
-glyphname = imacron;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = quotesingle;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 299;
+unicode = 39;
 },
 {
-color = 3;
-glyphname = macute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = at;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7743;
+unicode = 64;
 },
 {
-color = 3;
-glyphname = ngrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = ampersand;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 505;
+unicode = 38;
 },
 {
-color = 3;
-glyphname = ntilde;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = paragraph;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 241;
+unicode = 182;
 },
 {
-color = 3;
-glyphname = oacute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = section;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 243;
+unicode = 167;
 },
 {
-color = 3;
-glyphname = obreve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = copyright;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 335;
+unicode = 169;
 },
 {
-glyphname = ocaron;
+glyphname = registered;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 466;
+unicode = 174;
 },
 {
-color = 3;
-glyphname = ocircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = trademark;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 244;
+unicode = 8482;
 },
 {
-color = 3;
-glyphname = ograve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = degree;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 242;
+unicode = 176;
 },
 {
-color = 3;
-glyphname = omacron;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = bar;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 333;
+unicode = 124;
 },
 {
-color = 3;
-glyphname = uacute;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = cent;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 250;
+unicode = 162;
 },
 {
-color = 3;
-glyphname = ubreve;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = dollar;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 365;
+unicode = 36;
 },
 {
-glyphname = ucaron;
+glyphname = euro;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 468;
+unicode = 8364;
 },
 {
-color = 3;
-glyphname = ucircumflex;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = sterling;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 251;
+unicode = 163;
 },
 {
-glyphname = udieresis;
+glyphname = yen;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 252;
+unicode = 165;
 },
 {
-glyphname = udieresisacute;
+glyphname = plus;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 472;
+unicode = 43;
 },
 {
-glyphname = udieresiscaron;
+glyphname = minus;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 474;
+unicode = 8722;
 },
 {
-glyphname = udieresisgrave;
+glyphname = multiply;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 476;
+unicode = 215;
 },
 {
-glyphname = udieresismacron;
+glyphname = divide;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 470;
+unicode = 247;
 },
 {
-color = 3;
-glyphname = ugrave;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = equal;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 249;
+unicode = 61;
 },
 {
-color = 3;
-glyphname = umacron;
-lastChange = "2022-04-29 09:57:47 +0000";
+glyphname = greater;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 363;
+unicode = 62;
 },
 {
-color = 3;
-glyphname = nmod;
-lastChange = "2022-04-29 09:49:06 +0000";
+glyphname = less;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8319;
+unicode = 60;
 },
 {
-color = 3;
-glyphname = Nmod;
-lastChange = "2022-04-29 09:47:49 +0000";
+glyphname = asciitilde;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 7482;
+unicode = 126;
 },
 {
-glyphname = dieresiscomb;
+glyphname = asciicircum;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 776;
+unicode = 94;
 },
 {
-glyphname = gravecomb;
+glyphname = percent;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 768;
+unicode = 37;
 },
 {
-color = 3;
-glyphname = gravecomb_dotaboverightcomb;
-lastChange = "2022-04-29 09:38:36 +0000";
+glyphname = caroncomb.alt;
+lastChange = "2022-03-04 12:31:03 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
 },
 {
-glyphname = acutecomb;
+glyphname = dieresis;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 769;
+unicode = 168;
 },
 {
-color = 3;
-glyphname = acutecomb_dotaboverightcomb;
-lastChange = "2022-04-29 09:38:36 +0000";
+glyphname = dotaccent;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
+unicode = 729;
 },
 {
-glyphname = circumflexcomb;
+glyphname = grave;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 770;
+unicode = 96;
 },
 {
-color = 3;
-glyphname = circumflexcomb_dotaboverightcomb;
-lastChange = "2022-04-29 09:38:36 +0000";
+glyphname = acute;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
+unicode = 180;
 },
 {
-glyphname = caroncomb;
+glyphname = hungarumlaut;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 780;
+unicode = 733;
 },
 {
-color = 3;
-glyphname = brevecomb;
-lastChange = "2022-04-29 09:54:41 +0000";
+glyphname = circumflex;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 774;
+unicode = 710;
 },
 {
-color = 3;
-glyphname = brevecomb_dotaboverightcomb;
-lastChange = "2022-04-29 09:39:46 +0000";
+glyphname = caron;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
+unicode = 711;
 },
 {
-glyphname = macroncomb;
+glyphname = breve;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 772;
+unicode = 728;
 },
 {
-color = 3;
-glyphname = macroncomb_dotaboverightcomb;
-lastChange = "2022-04-29 09:38:54 +0000";
+glyphname = ring;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
+unicode = 730;
 },
 {
-color = 3;
-glyphname = verticallineabovecomb;
-lastChange = "2022-04-29 09:35:43 +0000";
+glyphname = tilde;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 781;
+unicode = 732;
 },
 {
-color = 3;
-glyphname = verticallineabovecomb_dotaboverightcomb;
-lastChange = "2022-04-29 09:39:27 +0000";
+glyphname = macron;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
+unicode = 175;
 },
 {
-color = 3;
-glyphname = dotaboverightcomb;
-lastChange = "2022-04-29 09:38:36 +0000";
+glyphname = cedilla;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 856;
+unicode = 184;
 },
 {
-color = 3;
-glyphname = apostrophemod;
-lastChange = "2022-04-29 09:38:36 +0000";
+glyphname = ogonek;
+lastChange = "2024-03-21 09:41:23 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 700;
+unicode = 731;
 }
 );
 metrics = (
 {
 type = ascender;
 },
 {
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_TransLatin_Arabic.nam`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x01E6 LATIN CAPITAL LETTER G WITH CARON
 0x01E7 LATIN SMALL LETTER G WITH CARON
 0x0232 LATIN CAPITAL LETTER Y WITH MACRON
 0x0233 LATIN SMALL LETTER Y WITH MACRON
 0x02BC MODIFIER LETTER APOSTROPHE
 0x02BD MODIFIER LETTER REVERSED COMMA
 0x02BE MODIFIER LETTER RIGHT HALF RING
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_TransLatin_Pinyin.nam`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x00C0 LATIN CAPITAL LETTER A WITH GRAVE
 0x00C1 LATIN CAPITAL LETTER A WITH ACUTE
 0x00C2 LATIN CAPITAL LETTER A WITH CIRCUMFLEX
 0x00C8 LATIN CAPITAL LETTER E WITH GRAVE
 0x00C9 LATIN CAPITAL LETTER E WITH ACUTE
 0x00CA LATIN CAPITAL LETTER E WITH CIRCUMFLEX
 0x00CC LATIN CAPITAL LETTER I WITH GRAVE
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt` & `glyphsets-1.0.0/Lib/glyphsets/results/txt/nice-names/GF_TransLatin_Pinyin.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,96 @@
-dieresiscomb
-gravecomb
-acutecomb
-macroncomb
-apostrophemod
-Acaron
-Icaron
-Macute
-Ngrave
-Ocaron
-Ucaron
-Udieresisacute
-Udieresiscaron
-Udieresisgrave
-Udieresismacron
-acaron
-icaron
-macute
-ngrave
-ocaron
-ucaron
-udieresisacute
-udieresiscaron
-udieresisgrave
-udieresismacron
-nmod
-verticallineabovecomb
-dotaboverightcomb
+# This file is auto-generated; do not edit. See /README.md for instructions.
+Agrave
 Aacute
-Abreve
 Acircumflex
-Agrave
-Amacron
+Egrave
 Eacute
-Ecaron
 Ecircumflex
-Egrave
-Emacron
+Igrave
 Iacute
 Icircumflex
 Idieresis
-Igrave
-Imacron
-Nacute
+Ograve
 Oacute
 Ocircumflex
-Ograve
-Omacron
+Ugrave
 Uacute
-Ubreve
 Ucircumflex
 Udieresis
-Ugrave
-Umacron
+agrave
 aacute
-abreve
 acircumflex
-agrave
-amacron
+egrave
 eacute
-ecaron
 ecircumflex
-egrave
-emacron
+igrave
 iacute
 icircumflex
-igrave
-imacron
 ntilde
+ograve
 oacute
 ocircumflex
-ograve
-omacron
+ugrave
 uacute
-ubreve
 ucircumflex
 udieresis
-ugrave
-umacron
-circumflexcomb
-caroncomb
-brevecomb
-Nmod
+Amacron
+amacron
+Abreve
+abreve
+Emacron
+emacron
 Ebreve
-Ibreve
-Obreve
 ebreve
+Ecaron
+ecaron
+Imacron
+imacron
+Ibreve
 ibreve
+Nacute
+Omacron
+omacron
+Obreve
 obreve
+Umacron
+umacron
+Ubreve
+ubreve
+Acaron
+acaron
+Icaron
+icaron
+Ocaron
+ocaron
+Ucaron
+ucaron
+Udieresismacron
+udieresismacron
+Udieresisacute
+udieresisacute
+Udieresiscaron
+udieresiscaron
+Udieresisgrave
+udieresisgrave
+Ngrave
+ngrave
+apostrophemod
+gravecomb
+acutecomb
+circumflexcomb
+macroncomb
+brevecomb
+dieresiscomb
+caroncomb
+verticallineabovecomb
+dotaboverightcomb
+Nmod
+Macute
+macute
+nmod
 gravecomb_dotaboverightcomb
 acutecomb_dotaboverightcomb
 circumflexcomb_dotaboverightcomb
 brevecomb_dotaboverightcomb
 macroncomb_dotaboverightcomb
 verticallineabovecomb_dotaboverightcomb
```

### Comparing `glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt` & `glyphsets-1.0.0/data/results/txt/prod-names/GF_TransLatin_Pinyin.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,96 @@
-uni0308
-gravecomb
-acutecomb
-uni0304
-uni02BC
-uni01CD
-uni01CF
-uni1E3E
-uni01F8
-uni01D1
-uni01D3
-uni01D7
-uni01D9
-uni01DB
-uni01D5
-uni01CE
-uni01D0
-uni1E3F
-uni01F9
-uni01D2
-uni01D4
-uni01D8
-uni01DA
-uni01DC
-uni01D6
-uni207F
-uni030D
-uni0358
+# This file is auto-generated; do not edit. See /README.md for instructions.
+Agrave
 Aacute
-Abreve
 Acircumflex
-Agrave
-Amacron
+Egrave
 Eacute
-Ecaron
 Ecircumflex
-Egrave
-Emacron
+Igrave
 Iacute
 Icircumflex
 Idieresis
-Igrave
-Imacron
-Nacute
+Ograve
 Oacute
 Ocircumflex
-Ograve
-Omacron
+Ugrave
 Uacute
-Ubreve
 Ucircumflex
 Udieresis
-Ugrave
-Umacron
+agrave
 aacute
-abreve
 acircumflex
-agrave
-amacron
+egrave
 eacute
-ecaron
 ecircumflex
-egrave
-emacron
+igrave
 iacute
 icircumflex
-igrave
-imacron
 ntilde
+ograve
 oacute
 ocircumflex
-ograve
-omacron
+ugrave
 uacute
-ubreve
 ucircumflex
 udieresis
-ugrave
-umacron
-uni0302
-uni030C
-uni0306
-uni1D3A
+Amacron
+amacron
+Abreve
+abreve
+Emacron
+emacron
 Ebreve
-Ibreve
-Obreve
 ebreve
+Ecaron
+ecaron
+Imacron
+imacron
+Ibreve
 ibreve
+Nacute
+Omacron
+omacron
+Obreve
 obreve
+Umacron
+umacron
+Ubreve
+ubreve
+uni01CD
+uni01CE
+uni01CF
+uni01D0
+uni01D1
+uni01D2
+uni01D3
+uni01D4
+uni01D5
+uni01D6
+uni01D7
+uni01D8
+uni01D9
+uni01DA
+uni01DB
+uni01DC
+uni01F8
+uni01F9
+uni02BC
+gravecomb
+acutecomb
+uni0302
+uni0304
+uni0306
+uni0308
+uni030C
+uni030D
+uni0358
+uni1D3A
+uni1E3E
+uni1E3F
+uni207F
 uni03000358
 uni03010358
 uni03020358
 uni03060358
 uni03040358
 uni030D0358
```

### Comparing `glyphsets-0.6.9/LICENSE` & `glyphsets-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Lib/glyphsets/__init__.py` & `glyphsets-1.0.0/scripts/assemble_charactersets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,272 +1,283 @@
 """
-GF Glyph Database
+Assemble .nam files from .nam stub files and language definitions.
 """
-import plistlib
-import json
-import os
-from re import L
-from glyphsLib import GSFont, GSGlyph
-from defcon import Font
-import logging
-import unicodedata2 as uni
-from glyphsLib.glyphdata import get_glyph
-from copy import deepcopy as copy
-
-try:
-    from ._version import version as __version__  # type: ignore
-except ImportError:
-    __version__ = "0.0.0+unknown"
-
-
-DATA_FP = os.path.join(os.path.dirname(__file__), "data.json")
-TEST_STRINGS_DATA = os.path.join(os.path.dirname(__file__), "test_strings.json")
-log = logging.getLogger(__file__)
-
-
-class _GFGlyphData:
-    def __init__(self, data=json.load(open(DATA_FP, encoding="utf8"))):
-        self._data = copy(data)
-        self._in_use = set(g["nice_name"] for g in self._data["glyphs"])
-
-    def save(self, fp=DATA_FP):
-        with open(fp, "w") as db:
-            json.dump(self._data, db, indent=2)
-
-    @classmethod
-    def from_json(cls, fp):
-        with open(fp) as db:
-            data = json.load(db)
-            return cls(data)
-
-    def __getitem__(self, k):
-        return self._data[k]
-
-    def glyphsets_in_font(self, ttFont):
-        glyphs_in_font = set(ttFont.getGlyphOrder())
-        unicodes_in_font = set(ttFont.getBestCmap().keys())
-        res = {}
-        for g in self["glyphs"]:
-            for glyphset in g["glyphsets"]:
-                if glyphset not in res:
-                    res[glyphset] = {"has": [], "missing": []}
-                if any(
-                    [
-                        g["nice_name"] in glyphs_in_font,
-                        g["production_name"] in glyphs_in_font,
-                        g["unicode"] in unicodes_in_font,
-                    ]
-                ):
-                    res[glyphset]["has"].append(g)
-                else:
-                    res[glyphset]["missing"].append(g)
-        return res
 
-    def glyphsets_fulfilled(self, ttFont):
-        res = self.glyphsets_in_font(ttFont)
-        return {
-            k: len(v["has"]) / (len(v["has"]) + len(v["missing"]))
-            for k, v in res.items()
-        }
-
-    def missing_glyphsets_in_font(self, ttFont, threshold=0.8):
-        res = self.glyphsets_in_font(ttFont)
-        fulfilled = {
-            k: len(v["has"]) / (len(v["has"]) + len(v["missing"]))
-            for k, v in res.items()
-        }
-        missing = {}
-        for k, v in fulfilled.items():
-            if v == 1.0 or v < threshold:
-                continue
-            missing[k] = res[k]["missing"]
-        return missing
-
-    def glyphs_in_glyphsets(self, glyphsets):
-        res = []
-        seen = set()
-        for g in self["glyphs"]:
-            for glyphset in g["glyphsets"]:
-                if glyphset not in glyphsets or g["nice_name"] in seen:
-                    continue
-                res.append(g)
-                seen.add(g["nice_name"])
-        return res
-
-    def update_db_from_sources(self, sources):
-        """Update the database by using the glyphsets from source files.
-
-        Please note that you may need to edit some data by hand"""
-        for src in sources:
-            if isinstance(src, GSFont):
-                glyphset = os.path.basename(src.filepath).split(".")[0]
-                for g in src.glyphs:
-                    if not g.export:
-                        continue
-                    self.add_glyph(glyphset, g.name, unicodes=g.unicode)
-            elif isinstance(src, Font):
-                glyphset = os.path.basename(src.path).split(".")[0]
-                for g in src:
-                    self.add_glyph(glyphset, g.name, unicodes=g.unicode)
-            else:
-                raise NotImplementedError(f"{src} not supported yet!")
+import sys
+import os
+import shutil
+import gflanguages
+import unicodedata
+import glyphsLib
+import functools
+import plistlib
+from glyphsLib.glyphdata import get_glyph, _lookup_attributes_by_unicode
+from fontTools.unicodedata.Scripts import NAMES as SCRIPT_NAMES
 
-    def add_glyph(self, glyphset, nice_name=None, unicodes=None):
-        if nice_name in self._in_use:
-            entry = next(
-                (g for g in self._data["glyphs"] if g["nice_name"] == nice_name), None
-            )
-            if glyphset in entry["glyphsets"]:
-                log.warning(f"Skipping {glyphset}.{nice_name}. Already exists!")
-                return
-            entry["glyphsets"].append(glyphset)
-        else:
-            # glyphsapp use hex strings for the unicode val. Convert these to ints
-            if unicodes:
-                uni_char = unicodes if isinstance(unicodes, int) else int(unicodes, 16)
-                character = chr(uni_char)
-            else:
-                uni_char = None
-                character = None
-            glyphslib_data = get_glyph(nice_name)
-            glyphslib_unicode = (
-                None if not glyphslib_data.unicode else int(glyphslib_data.unicode, 16)
-            )
-            self._data["glyphs"].append(
-                {
-                    "nice_name": nice_name,
-                    "production_name": glyphslib_data.production_name,
-                    "character": character,
-                    "unicode": uni_char or glyphslib_unicode,
-                    "glyphsets": [glyphset],
-                }
-            )
-            self._in_use.add(nice_name)
-
-    def get_glyph(self, nice_name=None, production_name=None, character=None, uni=None):
-        if nice_name:
-            return next(
-                (g for g in self._data["glyphs"] if g["nice_name"] == nice_name), None
-            )
-        elif production_name:
-            return next(
-                (
-                    g
-                    for g in self._data["glyphs"]
-                    if g["production_name"] == production_name
-                ),
-                None,
-            )
-        elif character:
-            return next(
-                (g for g in self._data["glyphs"] if g["character"] == character), None
-            )
-        elif uni:
-            return next((g for g in self._data["glyphs"] if g["unicode"] == uni), None)
-        return None
-
-    def build_glyphsapp_filter_list(
-        self, glyphsets, use_production_names=False, out=None
-    ):
-        """Build filter lists"""
-        glyphs = self.glyphs_in_glyphsets(glyphsets)
-        if out and out.endswith("plist"):
-            # glyphsapp need a prefix for the out file of "CustomFilter"
-            if not os.path.basename(out).startswith("CustomFilter"):
-                print(
-                    "Prefixing 'CustomFilter' to out path since file is intended for Glyphsapp"
+# Insert local module path at beginning of sys.path
+# so that up-to-date version of glyphsets package is used
+sys.path.insert(0, os.path.join(os.path.dirname(__file__), "..", "Lib"))
+from glyphsets import (
+    get_script,
+    defined_glyphsets,
+    get_glyphset_definition,
+    unicodes_per_glyphset,
+    languages_per_glyphset,
+    read_nam_file,
+)  # noqa: E402
+
+
+def sort_unicodes(a, b):
+    if a.unicode and b.unicode:
+        return int(a.unicode, 16) - int(b.unicode, 16)
+    elif a.unicode:
+        return -1
+    elif b.unicode:
+        return 1
+    else:
+        return 0
+
+
+def sort_by_category(a, b):
+    info_a = get_glyph(a.name)
+    info_b = get_glyph(b.name)
+
+    if info_a.category is None:
+        return -1
+    elif info_b.category is None:
+        return 1
+
+    value = sorted([info_a.category, info_b.category]).index(info_a.category)
+    if value == 0:
+        value = -1
+    value *= -1
+
+    return value
+
+
+def assemble_characterset(root_folder, glyphset_name):
+
+    script = get_script(glyphset_name)
+    glyphset_definition = get_glyphset_definition(glyphset_name)
+    language_codes = languages_per_glyphset(glyphset_name)
+    use_aux = glyphset_definition.get("use_auxiliary", False)
+
+    nam_stub_path = os.path.join(
+        root_folder, "definitions", "per_glyphset", f"{glyphset_name}.stub.nam"
+    )
+    nam_path = os.path.join(root_folder, "results", "nam", f"{glyphset_name}.nam")
+    nam_in_package_path = os.path.abspath(
+        os.path.join(
+            root_folder,
+            "..",
+            "Lib",
+            "glyphsets",
+            "results",
+            "nam",
+            f"{glyphset_name}.nam",
+        )
+    )
+    txt_in_package_path = os.path.abspath(
+        os.path.join(
+            root_folder,
+            "..",
+            "Lib",
+            "glyphsets",
+            "results",
+            "txt",
+            "nice-names",
+            f"{glyphset_name}.txt",
+        )
+    )
+    glyphs_stub_path = os.path.join(
+        root_folder, "definitions", "per_glyphset", f"{glyphset_name}.stub.glyphs"
+    )
+    glyphs_path = os.path.join(
+        root_folder, "results", "glyphs", f"{glyphset_name}.glyphs"
+    )
+    glyphs_empty_path = os.path.join(root_folder, f"empty_font.glyphs")
+    txt_nicenames_path = os.path.join(
+        root_folder, "results", "txt", "nice-names", f"{glyphset_name}.txt"
+    )
+    txt_prodnames_path = os.path.join(
+        root_folder, "results", "txt", "prod-names", f"{glyphset_name}.txt"
+    )
+    plist_path = os.path.join(
+        root_folder, "results", "plist", f"CustomFilter_GF_{script}.plist"
+    )
+
+    character_set = set()
+
+    # Assemble character sets from gflanguages
+    languages = gflanguages.LoadLanguages()
+    for language_code in language_codes:
+        chars = languages[language_code].exemplar_chars
+        # chars.base.upper() is important because many Latin languages don't
+        # contain a complete set of uppercase letters in "index"
+        character_set.update(
+            {
+                ord(c)
+                for c in list(
+                    set(chars.base)
+                    | set(chars.base.upper())
+                    | set(chars.index)
+                    | set(chars.marks)
+                    | set(chars.numerals)
+                    | set(chars.punctuation)
+                    | (set(chars.auxiliary) if use_aux else set())
                 )
-                out = os.path.join(
-                    os.path.dirname(out), "CustomFilter" + os.path.basename(out)
-                )
-            res = {k: [] for k in glyphsets}
-            for glyphset in glyphsets:
-                for glyph in glyphs:
-                    if glyphset in glyph["glyphsets"]:
-                        if use_production_names:
-                            res[glyphset].append(glyph["production_name"])
-                        else:
-                            res[glyphset].append(glyph["nice_name"])
-
-            res = [{"name": k, "list": v} for k, v in res.items()]
-            res = [plistlib.dumps(res).decode("utf-8")]
-        else:
-            if use_production_names:
-                res = [g["production_name"] for g in glyphs]
-            else:
-                res = [g["nice_name"] for g in glyphs]
+                if c not in (" ", "{", "}", "◌")
+            }
+        )
+
+    # Call get_glyph once so that GLYPHDATA gets filled in glyphsLib
+    get_glyph("A")
+    # If I import GLYPHDATA at the top of the file, it doesn't get filled
+    from glyphsLib.glyphdata import GLYPHDATA
+
+    assert type(GLYPHDATA) is glyphsLib.glyphdata.GlyphData
+
+    def _font_has_unicode(font, unicode):
+        for glyph in font.glyphs:
+            if glyph.unicode:
+                if int(glyph.unicode, 16) == unicode:
+                    return True
+
+    # Create or open glyphs file and add characters
+    if os.path.exists(glyphs_stub_path):
+        font = glyphsLib.load(glyphs_stub_path)
+        for glyph in font.glyphs:
+            if glyph.unicodes:
+                for unicode in glyph.unicodes:
+                    character_set.update({int(unicode, 16)})
+    else:
+        font = glyphsLib.load(glyphs_empty_path)
+
+    font.familyName = glyphset_name
+
+    # Add language-specific glyphs
+    for language_code in language_codes:
+        per_language_glyphs_stub_path = os.path.join(
+            root_folder, "definitions", "per_language", f"{language_code}.stub.glyphs"
+        )
+        if os.path.exists(per_language_glyphs_stub_path):
+            per_language_font = glyphsLib.load(per_language_glyphs_stub_path)
+
+            for glyph in per_language_font.glyphs:
+
+                # Add encoded characters to character_set
+                if glyph.unicodes:
+                    for unicode in glyph.unicodes:
+                        character_set.update({int(unicode, 16)})
+
+                # Add unencoded glyphs to .glyphs file
+                else:
+                    new_glyph = glyphsLib.GSGlyph(glyph.name)
+                    font.glyphs.append(new_glyph)
 
-        if out:
-            with open(out, "w") as doc:
-                doc.write("\n".join(res))
-        return res
-
-    def build_nam_file(self, glyphsets, out=None):
-        "Build GF nam files from glyphsets"
-        glyphs = [g for g in self.glyphs_in_glyphsets(glyphsets) if g["unicode"]]
-        res = []
-        for glyph in glyphs:
-            code = (
-                "0x" + hex(ord(glyph["character"])).replace("0x", "").zfill(4).upper()
-            )
-            res.append(f"{code} {uni.name(glyph['character'])}")
-        res.sort()
-        if out:
-            with open(out, "w") as doc:
-                doc.write("\n".join(res))
-        return res
-
-    def update_source_glyphset(self, src, glyphsets):
-        """Add glyphs to a source file"""
-        glyphs = self.glyphs_in_glyphsets(glyphsets)
-        if isinstance(src, Font):
-            glyphs_in_font = set(g.name for g in src)
-            for glyph in glyphs:
-                if glyph["nice_name"] in glyphs_in_font:
-                    continue
-                new_glyph = src.newGlyph(glyph["nice_name"])
-                new_glyph.color = "Red"
-                glyphs_in_font.add(glyph["nice_name"])
-        elif isinstance(src, GSFont):
-            glyphs_in_font = set(g.name for g in src.glyphs)
-            for glyph in glyphs:
-                if glyph["nice_name"] in glyphs_in_font:
-                    continue
-                new_glyph = GSGlyph(glyph["nice_name"])
-                new_glyph.color = 1
-                src.glyphs.append(new_glyph)
-                glyphs_in_font.add(glyph["nice_name"])
-        else:
-            raise NotImplementedError(f"Cannot add glyphs font source not supported!")
-
-    def build_fea(self, glyphset):
-        """Generate a .fea file based on a glyphset"""
-        # TODO this is 2022 Q3/4 goal
-        raise NotImplementedError()
-
-
-GFGlyphData = _GFGlyphData()
-
-
-class _TestDocData:
-    def __init__(
-        self,
-        data=json.load(open(TEST_STRINGS_DATA, encoding="utf8")),
-        glyphsets=GFGlyphData,
-    ):
-        self._data = data
-        self._glyphsets = glyphsets
-
-    def test_strings_in_font(self, ttFont, threshold=0.95):
-        res = {}
-        glyphsets_in_font = self._glyphsets.glyphsets_fulfilled(ttFont)
-        for glyphset, coverage in glyphsets_in_font.items():
-            if coverage < threshold:
-                continue
-            test_strings = self._data.get(glyphset)
-            if not test_strings:
-                continue
-            res[glyphset] = test_strings
-        return res
+    # Add encoded characters to .glyphs file
+    for _i, unicode in enumerate(sorted(list(character_set))):
+        if not _font_has_unicode(font, unicode):
+            unicode = f"{unicode:#0{6}X}".replace("0X", "")
+            glyph_info = _lookup_attributes_by_unicode(unicode, GLYPHDATA)
+            if "name" in glyph_info:
+                new_glyph = glyphsLib.GSGlyph(glyph_info["name"])
+            else:
+                new_glyph = glyphsLib.GSGlyph(f"uni{unicode}")
+            new_glyph.unicode = unicode
+            font.glyphs.append(new_glyph)
+
+    # Sort
+    font.glyphs = sorted(font.glyphs, key=functools.cmp_to_key(sort_by_category))
+    unicode_sorted_glyphs = sorted(font.glyphs, key=functools.cmp_to_key(sort_unicodes))
+    glyph_names = [glyph.name for glyph in unicode_sorted_glyphs]
+    production_glyph_names = [
+        get_glyph(glyph.name).production_name for glyph in unicode_sorted_glyphs
+    ]
+
+    # Save glyphs file
+    os.makedirs(os.path.dirname(glyphs_path), exist_ok=True)
+    font.save(glyphs_path)
+
+    # Output sorted character set to .nam file
+    os.makedirs(os.path.dirname(nam_path), exist_ok=True)
+    os.makedirs(os.path.dirname(nam_in_package_path), exist_ok=True)
+    with open(nam_path, "w") as f:
+        f.write(
+            "# This file is auto-generated; do not edit. See /README.md for instructions.\n"
+        )
+        for i, unicode in enumerate(sorted(list(character_set))):
+            unicode_string = f"{unicode:#0{6}X}".replace("0X", "0x")
+            try:
+                unicode_name = unicodedata.name(chr(unicode))
+            except ValueError:
+                unicode_name = ""
+            f.write(f"{unicode_string} {unicode_name}")
+            if i < len(character_set) - 1:
+                f.write("\n")
+    shutil.copyfile(nam_path, nam_in_package_path)
+
+    # Output txt files
+    os.makedirs(os.path.dirname(txt_nicenames_path), exist_ok=True)
+    with open(txt_nicenames_path, "w") as f:
+        f.write(
+            "# This file is auto-generated; do not edit. See /README.md for instructions.\n"
+        )
+        f.write("\n".join(glyph_names))
+    os.makedirs(os.path.dirname(txt_prodnames_path), exist_ok=True)
+    with open(txt_prodnames_path, "w") as f:
+        f.write(
+            "# This file is auto-generated; do not edit. See /README.md for instructions.\n"
+        )
+        f.write("\n".join(production_glyph_names))
+    os.makedirs(os.path.dirname(txt_in_package_path), exist_ok=True)
+    shutil.copyfile(txt_nicenames_path, txt_in_package_path)
+
+    # Adjust .plist
+    os.makedirs(os.path.dirname(plist_path), exist_ok=True)
+    if os.path.exists(plist_path):
+        with open(plist_path, "rb") as f:
+            plist = plistlib.load(f)
+    else:
+        plist = []
+    found_list = False
+    for plist_glyphset in plist:
+        if "name" in plist_glyphset and plist_glyphset["name"] == glyphset_name:
+            plist_glyphset["list"] = glyph_names
+            found_list = True
+    if not found_list:
+        plist.append({"name": glyphset_name, "list": glyph_names})
+    with open(plist_path, "wb") as f:
+        plistlib.dump(plist, f)
+
+
+if __name__ == "__main__":
+    # Check for gflanguages version
+    installed = None
+    latest = None
+    for line in os.popen("pip index versions gflanguages").read().split("\n"):
+        if "INSTALLED" in line:
+            installed = line.split(" ")[-1].strip()
+        if "LATEST" in line:
+            latest = line.split(" ")[-1].strip()
+    print(
+        f"""
+*************************************************************
+*
+*   WARNING:
+*   Make sure you're using the correct version of gflanguages,
+*   otherwise the glyphsets will be incorrect.
+*
+*   You have: {installed}
+*   Location: {gflanguages.__file__}
+*
+*************************************************************
+"""
+    )
 
+    root_folder = os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "data"))
 
-GFTestData = _TestDocData()
+    for glyphset_name in defined_glyphsets():
+        print(f"Assembling '{glyphset_name}'...")
+        assemble_characterset(root_folder, glyphset_name)
+        # Proof of work:
+        # assert unicodes_per_glyphset(glyphset_name) != []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Arabic_Core.nam` & `glyphsets-1.0.0/data/results/nam/GF_Arabic_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Arabic_Plus.nam` & `glyphsets-1.0.0/data/results/nam/GF_Arabic_Plus.nam`

 * *Files 18% similar despite different names*

```diff
@@ -79,31 +79,49 @@
 0x0667 ARABIC-INDIC DIGIT SEVEN
 0x0668 ARABIC-INDIC DIGIT EIGHT
 0x0669 ARABIC-INDIC DIGIT NINE
 0x066A ARABIC PERCENT SIGN
 0x066B ARABIC DECIMAL SEPARATOR
 0x066C ARABIC THOUSANDS SEPARATOR
 0x0670 ARABIC LETTER SUPERSCRIPT ALEF
+0x067A ARABIC LETTER TTEHEH
+0x067B ARABIC LETTER BEEH
 0x067C ARABIC LETTER TEH WITH RING
+0x067D ARABIC LETTER TEH WITH THREE DOTS ABOVE DOWNWARDS
 0x067E ARABIC LETTER PEH
+0x067F ARABIC LETTER TEHEH
+0x0680 ARABIC LETTER BEHEH
 0x0681 ARABIC LETTER HAH WITH HAMZA ABOVE
+0x0683 ARABIC LETTER NYEH
+0x0684 ARABIC LETTER DYEH
 0x0685 ARABIC LETTER HAH WITH THREE DOTS ABOVE
 0x0686 ARABIC LETTER TCHEH
+0x0687 ARABIC LETTER TCHEHEH
 0x0689 ARABIC LETTER DAL WITH RING
+0x068A ARABIC LETTER DAL WITH DOT BELOW
+0x068C ARABIC LETTER DAHAL
+0x068D ARABIC LETTER DDAHAL
+0x068F ARABIC LETTER DAL WITH THREE DOTS ABOVE DOWNWARDS
 0x0693 ARABIC LETTER REH WITH RING
 0x0695 ARABIC LETTER REH WITH SMALL V BELOW
 0x0696 ARABIC LETTER REH WITH DOT BELOW AND DOT ABOVE
 0x0698 ARABIC LETTER JEH
+0x0699 ARABIC LETTER REH WITH FOUR DOTS ABOVE
 0x069A ARABIC LETTER SEEN WITH DOT BELOW AND DOT ABOVE
 0x06A4 ARABIC LETTER VEH
+0x06A6 ARABIC LETTER PEHEH
 0x06A9 ARABIC LETTER KEHEH
+0x06AA ARABIC LETTER SWASH KAF
 0x06AB ARABIC LETTER KAF WITH RING
 0x06AD ARABIC LETTER NG
 0x06AF ARABIC LETTER GAF
+0x06B1 ARABIC LETTER NGOEH
+0x06B3 ARABIC LETTER GUEH
 0x06B5 ARABIC LETTER LAM WITH SMALL V
+0x06BB ARABIC LETTER RNOON
 0x06BC ARABIC LETTER NOON WITH RING
 0x06BE ARABIC LETTER HEH DOACHASHMEE
 0x06C6 ARABIC LETTER OE
 0x06C7 ARABIC LETTER U
 0x06C8 ARABIC LETTER YU
 0x06CB ARABIC LETTER VE
 0x06CC ARABIC LETTER FARSI YEH
@@ -123,8 +141,10 @@
 0x06F8 EXTENDED ARABIC-INDIC DIGIT EIGHT
 0x06F9 EXTENDED ARABIC-INDIC DIGIT NINE
 0x06FD ARABIC SIGN SINDHI AMPERSAND
 0x06FE ARABIC SIGN SINDHI POSTPOSITION MEN
 0x200E LEFT-TO-RIGHT MARK
 0x200F RIGHT-TO-LEFT MARK
 0x2018 LEFT SINGLE QUOTATION MARK
-0x2212 MINUS SIGN
+0x204F REVERSED SEMICOLON
+0x2212 MINUS SIGN
+0x2E41 REVERSED COMMA
```

### Comparing `glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Latin_Core.nam` & `glyphsets-1.0.0/data/results/nam/GF_Latin_Core.nam`

 * *Files 2% similar despite different names*

```diff
@@ -206,16 +206,14 @@
 0x011F LATIN SMALL LETTER G WITH BREVE
 0x0120 LATIN CAPITAL LETTER G WITH DOT ABOVE
 0x0121 LATIN SMALL LETTER G WITH DOT ABOVE
 0x0122 LATIN CAPITAL LETTER G WITH CEDILLA
 0x0123 LATIN SMALL LETTER G WITH CEDILLA
 0x0126 LATIN CAPITAL LETTER H WITH STROKE
 0x0127 LATIN SMALL LETTER H WITH STROKE
-0x0128 LATIN CAPITAL LETTER I WITH TILDE
-0x0129 LATIN SMALL LETTER I WITH TILDE
 0x012A LATIN CAPITAL LETTER I WITH MACRON
 0x012B LATIN SMALL LETTER I WITH MACRON
 0x012E LATIN CAPITAL LETTER I WITH OGONEK
 0x012F LATIN SMALL LETTER I WITH OGONEK
 0x0130 LATIN CAPITAL LETTER I WITH DOT ABOVE
 0x0131 LATIN SMALL LETTER DOTLESS I
 0x0136 LATIN CAPITAL LETTER K WITH CEDILLA
@@ -246,16 +244,14 @@
 0x015B LATIN SMALL LETTER S WITH ACUTE
 0x015E LATIN CAPITAL LETTER S WITH CEDILLA
 0x015F LATIN SMALL LETTER S WITH CEDILLA
 0x0160 LATIN CAPITAL LETTER S WITH CARON
 0x0161 LATIN SMALL LETTER S WITH CARON
 0x0164 LATIN CAPITAL LETTER T WITH CARON
 0x0165 LATIN SMALL LETTER T WITH CARON
-0x0168 LATIN CAPITAL LETTER U WITH TILDE
-0x0169 LATIN SMALL LETTER U WITH TILDE
 0x016A LATIN CAPITAL LETTER U WITH MACRON
 0x016B LATIN SMALL LETTER U WITH MACRON
 0x016E LATIN CAPITAL LETTER U WITH RING ABOVE
 0x016F LATIN SMALL LETTER U WITH RING ABOVE
 0x0170 LATIN CAPITAL LETTER U WITH DOUBLE ACUTE
 0x0171 LATIN SMALL LETTER U WITH DOUBLE ACUTE
 0x0172 LATIN CAPITAL LETTER U WITH OGONEK
@@ -272,15 +268,14 @@
 0x017D LATIN CAPITAL LETTER Z WITH CARON
 0x017E LATIN SMALL LETTER Z WITH CARON
 0x0218 LATIN CAPITAL LETTER S WITH COMMA BELOW
 0x0219 LATIN SMALL LETTER S WITH COMMA BELOW
 0x021A LATIN CAPITAL LETTER T WITH COMMA BELOW
 0x021B LATIN SMALL LETTER T WITH COMMA BELOW
 0x0237 LATIN SMALL LETTER DOTLESS J
-0x02BC MODIFIER LETTER APOSTROPHE
 0x02C6 MODIFIER LETTER CIRCUMFLEX ACCENT
 0x02C7 CARON
 0x02D8 BREVE
 0x02D9 DOT ABOVE
 0x02DA RING ABOVE
 0x02DB OGONEK
 0x02DC SMALL TILDE
@@ -302,20 +297,16 @@
 0x1E80 LATIN CAPITAL LETTER W WITH GRAVE
 0x1E81 LATIN SMALL LETTER W WITH GRAVE
 0x1E82 LATIN CAPITAL LETTER W WITH ACUTE
 0x1E83 LATIN SMALL LETTER W WITH ACUTE
 0x1E84 LATIN CAPITAL LETTER W WITH DIAERESIS
 0x1E85 LATIN SMALL LETTER W WITH DIAERESIS
 0x1E9E LATIN CAPITAL LETTER SHARP S
-0x1EBC LATIN CAPITAL LETTER E WITH TILDE
-0x1EBD LATIN SMALL LETTER E WITH TILDE
 0x1EF2 LATIN CAPITAL LETTER Y WITH GRAVE
 0x1EF3 LATIN SMALL LETTER Y WITH GRAVE
-0x1EF8 LATIN CAPITAL LETTER Y WITH TILDE
-0x1EF9 LATIN SMALL LETTER Y WITH TILDE
 0x2013 EN DASH
 0x2014 EM DASH
 0x2018 LEFT SINGLE QUOTATION MARK
 0x2019 RIGHT SINGLE QUOTATION MARK
 0x201A SINGLE LOW-9 QUOTATION MARK
 0x201C LEFT DOUBLE QUOTATION MARK
 0x201D RIGHT DOUBLE QUOTATION MARK
```

### Comparing `glyphsets-0.6.9/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam` & `glyphsets-1.0.0/Lib/glyphsets/results/nam/GF_Latin_PriAfrican.nam`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,178 @@
-0x0102  Ă LATIN CAPITAL LETTER A WITH BREVE
-0x0103  ă LATIN SMALL LETTER A WITH BREVE
-0x0110  Đ LATIN CAPITAL LETTER D WITH STROKE
-0x0111  đ LATIN SMALL LETTER D WITH STROKE
-0x01A0  Ơ LATIN CAPITAL LETTER O WITH HORN
-0x01A1  ơ LATIN SMALL LETTER O WITH HORN
-0x01AF  Ư LATIN CAPITAL LETTER U WITH HORN
-0x0128  Ĩ LATIN CAPITAL LETTER I WITH TILDE
-0x0129  ĩ LATIN SMALL LETTER I WITH TILDE
-0x0168  Ũ LATIN CAPITAL LETTER U WITH TILDE
-0x0169  ũ LATIN SMALL LETTER U WITH TILDE
-0x01B0  ư LATIN SMALL LETTER U WITH HORN
-0x0300    COMBINING GRAVE ACCENT
-0x0301    COMBINING ACUTE ACCENT
-0x0303    COMBINING TILDE
-0x0304    COMBINING MACRON
-0x0308    COMBINING DIAERESIS
-0x0309    COMBINING HOOK ABOVE
-0x0323    COMBINING DOT BELOW
-0x0329    COMBINING VERTICAL LINE BELOW
-0x1EA0  Ạ LATIN CAPITAL LETTER A WITH DOT BELOW
-0x1EA1  ạ LATIN SMALL LETTER A WITH DOT BELOW
-0x1EA2  Ả LATIN CAPITAL LETTER A WITH HOOK ABOVE
-0x1EA3  ả LATIN SMALL LETTER A WITH HOOK ABOVE
-0x1EA4  Ấ LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND ACUTE
-0x1EA5  ấ LATIN SMALL LETTER A WITH CIRCUMFLEX AND ACUTE
-0x1EA6  Ầ LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND GRAVE
-0x1EA7  ầ LATIN SMALL LETTER A WITH CIRCUMFLEX AND GRAVE
-0x1EA8  Ẩ LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND HOOK ABOVE
-0x1EA9  ẩ LATIN SMALL LETTER A WITH CIRCUMFLEX AND HOOK ABOVE
-0x1EAA  Ẫ LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND TILDE
-0x1EAB  ẫ LATIN SMALL LETTER A WITH CIRCUMFLEX AND TILDE
-0x1EAC  Ậ LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND DOT BELOW
-0x1EAD  ậ LATIN SMALL LETTER A WITH CIRCUMFLEX AND DOT BELOW
-0x1EAE  Ắ LATIN CAPITAL LETTER A WITH BREVE AND ACUTE
-0x1EAF  ắ LATIN SMALL LETTER A WITH BREVE AND ACUTE
-0x1EB0  Ằ LATIN CAPITAL LETTER A WITH BREVE AND GRAVE
-0x1EB1  ằ LATIN SMALL LETTER A WITH BREVE AND GRAVE
-0x1EB2  Ẳ LATIN CAPITAL LETTER A WITH BREVE AND HOOK ABOVE
-0x1EB3  ẳ LATIN SMALL LETTER A WITH BREVE AND HOOK ABOVE
-0x1EB4  Ẵ LATIN CAPITAL LETTER A WITH BREVE AND TILDE
-0x1EB5  ẵ LATIN SMALL LETTER A WITH BREVE AND TILDE
-0x1EB6  Ặ LATIN CAPITAL LETTER A WITH BREVE AND DOT BELOW
-0x1EB7  ặ LATIN SMALL LETTER A WITH BREVE AND DOT BELOW
-0x1EB8  Ẹ LATIN CAPITAL LETTER E WITH DOT BELOW
-0x1EB9  ẹ LATIN SMALL LETTER E WITH DOT BELOW
-0x1EBA  Ẻ LATIN CAPITAL LETTER E WITH HOOK ABOVE
-0x1EBB  ẻ LATIN SMALL LETTER E WITH HOOK ABOVE
-0x1EBC  Ẽ LATIN CAPITAL LETTER E WITH TILDE
-0x1EBD  ẽ LATIN SMALL LETTER E WITH TILDE
-0x1EBE  Ế LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND ACUTE
-0x1EBF  ế LATIN SMALL LETTER E WITH CIRCUMFLEX AND ACUTE
-0x1EC0  Ề LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND GRAVE
-0x1EC1  ề LATIN SMALL LETTER E WITH CIRCUMFLEX AND GRAVE
-0x1EC2  Ể LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND HOOK ABOVE
-0x1EC3  ể LATIN SMALL LETTER E WITH CIRCUMFLEX AND HOOK ABOVE
-0x1EC4  Ễ LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND TILDE
-0x1EC5  ễ LATIN SMALL LETTER E WITH CIRCUMFLEX AND TILDE
-0x1EC6  Ệ LATIN CAPITAL LETTER E WITH CIRCUMFLEX AND DOT BELOW
-0x1EC7  ệ LATIN SMALL LETTER E WITH CIRCUMFLEX AND DOT BELOW
-0x1EC8  Ỉ LATIN CAPITAL LETTER I WITH HOOK ABOVE
-0x1EC9  ỉ LATIN SMALL LETTER I WITH HOOK ABOVE
-0x1ECA  Ị LATIN CAPITAL LETTER I WITH DOT BELOW
-0x1ECB  ị LATIN SMALL LETTER I WITH DOT BELOW
-0x1ECC  Ọ LATIN CAPITAL LETTER O WITH DOT BELOW
-0x1ECD  ọ LATIN SMALL LETTER O WITH DOT BELOW
-0x1ECE  Ỏ LATIN CAPITAL LETTER O WITH HOOK ABOVE
-0x1ECF  ỏ LATIN SMALL LETTER O WITH HOOK ABOVE
-0x1ED0  Ố LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND ACUTE
-0x1ED1  ố LATIN SMALL LETTER O WITH CIRCUMFLEX AND ACUTE
-0x1ED2  Ồ LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND GRAVE
-0x1ED3  ồ LATIN SMALL LETTER O WITH CIRCUMFLEX AND GRAVE
-0x1ED4  Ổ LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND HOOK ABOVE
-0x1ED5  ổ LATIN SMALL LETTER O WITH CIRCUMFLEX AND HOOK ABOVE
-0x1ED6  Ỗ LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND TILDE
-0x1ED7  ỗ LATIN SMALL LETTER O WITH CIRCUMFLEX AND TILDE
-0x1ED8  Ộ LATIN CAPITAL LETTER O WITH CIRCUMFLEX AND DOT BELOW
-0x1ED9  ộ LATIN SMALL LETTER O WITH CIRCUMFLEX AND DOT BELOW
-0x1EDA  Ớ LATIN CAPITAL LETTER O WITH HORN AND ACUTE
-0x1EDB  ớ LATIN SMALL LETTER O WITH HORN AND ACUTE
-0x1EDC  Ờ LATIN CAPITAL LETTER O WITH HORN AND GRAVE
-0x1EDD  ờ LATIN SMALL LETTER O WITH HORN AND GRAVE
-0x1EDE  Ở LATIN CAPITAL LETTER O WITH HORN AND HOOK ABOVE
-0x1EDF  ở LATIN SMALL LETTER O WITH HORN AND HOOK ABOVE
-0x1EE0  Ỡ LATIN CAPITAL LETTER O WITH HORN AND TILDE
-0x1EE1  ỡ LATIN SMALL LETTER O WITH HORN AND TILDE
-0x1EE2  Ợ LATIN CAPITAL LETTER O WITH HORN AND DOT BELOW
-0x1EE3  ợ LATIN SMALL LETTER O WITH HORN AND DOT BELOW
-0x1EE4  Ụ LATIN CAPITAL LETTER U WITH DOT BELOW
-0x1EE5  ụ LATIN SMALL LETTER U WITH DOT BELOW
-0x1EE6  Ủ LATIN CAPITAL LETTER U WITH HOOK ABOVE
-0x1EE7  ủ LATIN SMALL LETTER U WITH HOOK ABOVE
-0x1EE8  Ứ LATIN CAPITAL LETTER U WITH HORN AND ACUTE
-0x1EE9  ứ LATIN SMALL LETTER U WITH HORN AND ACUTE
-0x1EEA  Ừ LATIN CAPITAL LETTER U WITH HORN AND GRAVE
-0x1EEB  ừ LATIN SMALL LETTER U WITH HORN AND GRAVE
-0x1EEC  Ử LATIN CAPITAL LETTER U WITH HORN AND HOOK ABOVE
-0x1EED  ử LATIN SMALL LETTER U WITH HORN AND HOOK ABOVE
-0x1EEE  Ữ LATIN CAPITAL LETTER U WITH HORN AND TILDE
-0x1EEF  ữ LATIN SMALL LETTER U WITH HORN AND TILDE
-0x1EF0  Ự LATIN CAPITAL LETTER U WITH HORN AND DOT BELOW
-0x1EF1  ự LATIN SMALL LETTER U WITH HORN AND DOT BELOW
-0x1EF2  Ỳ LATIN CAPITAL LETTER Y WITH GRAVE
-0x1EF3  ỳ LATIN SMALL LETTER Y WITH GRAVE
-0x1EF4  Ỵ LATIN CAPITAL LETTER Y WITH DOT BELOW
-0x1EF5  ỵ LATIN SMALL LETTER Y WITH DOT BELOW
-0x1EF6  Ỷ LATIN CAPITAL LETTER Y WITH HOOK ABOVE
-0x1EF7  ỷ LATIN SMALL LETTER Y WITH HOOK ABOVE
-0x1EF8  Ỹ LATIN CAPITAL LETTER Y WITH TILDE
-0x1EF9  ỹ LATIN SMALL LETTER Y WITH TILDE
-0x20AB  ₫ DONG SIGN
+# This file is auto-generated; do not edit. See /README.md for instructions.
+0x0021 EXCLAMATION MARK
+0x0022 QUOTATION MARK
+0x0023 NUMBER SIGN
+0x0025 PERCENT SIGN
+0x0026 AMPERSAND
+0x0027 APOSTROPHE
+0x0028 LEFT PARENTHESIS
+0x0029 RIGHT PARENTHESIS
+0x002A ASTERISK
+0x002B PLUS SIGN
+0x002C COMMA
+0x002D HYPHEN-MINUS
+0x002E FULL STOP
+0x002F SOLIDUS
+0x0030 DIGIT ZERO
+0x0031 DIGIT ONE
+0x0032 DIGIT TWO
+0x0033 DIGIT THREE
+0x0034 DIGIT FOUR
+0x0035 DIGIT FIVE
+0x0036 DIGIT SIX
+0x0037 DIGIT SEVEN
+0x0038 DIGIT EIGHT
+0x0039 DIGIT NINE
+0x003A COLON
+0x003B SEMICOLON
+0x003F QUESTION MARK
+0x0040 COMMERCIAL AT
+0x0041 LATIN CAPITAL LETTER A
+0x0042 LATIN CAPITAL LETTER B
+0x0043 LATIN CAPITAL LETTER C
+0x0044 LATIN CAPITAL LETTER D
+0x0045 LATIN CAPITAL LETTER E
+0x0046 LATIN CAPITAL LETTER F
+0x0047 LATIN CAPITAL LETTER G
+0x0048 LATIN CAPITAL LETTER H
+0x0049 LATIN CAPITAL LETTER I
+0x004A LATIN CAPITAL LETTER J
+0x004B LATIN CAPITAL LETTER K
+0x004C LATIN CAPITAL LETTER L
+0x004D LATIN CAPITAL LETTER M
+0x004E LATIN CAPITAL LETTER N
+0x004F LATIN CAPITAL LETTER O
+0x0050 LATIN CAPITAL LETTER P
+0x0051 LATIN CAPITAL LETTER Q
+0x0052 LATIN CAPITAL LETTER R
+0x0053 LATIN CAPITAL LETTER S
+0x0054 LATIN CAPITAL LETTER T
+0x0055 LATIN CAPITAL LETTER U
+0x0056 LATIN CAPITAL LETTER V
+0x0057 LATIN CAPITAL LETTER W
+0x0058 LATIN CAPITAL LETTER X
+0x0059 LATIN CAPITAL LETTER Y
+0x005A LATIN CAPITAL LETTER Z
+0x005B LEFT SQUARE BRACKET
+0x005D RIGHT SQUARE BRACKET
+0x0061 LATIN SMALL LETTER A
+0x0062 LATIN SMALL LETTER B
+0x0063 LATIN SMALL LETTER C
+0x0064 LATIN SMALL LETTER D
+0x0065 LATIN SMALL LETTER E
+0x0066 LATIN SMALL LETTER F
+0x0067 LATIN SMALL LETTER G
+0x0068 LATIN SMALL LETTER H
+0x0069 LATIN SMALL LETTER I
+0x006A LATIN SMALL LETTER J
+0x006B LATIN SMALL LETTER K
+0x006C LATIN SMALL LETTER L
+0x006D LATIN SMALL LETTER M
+0x006E LATIN SMALL LETTER N
+0x006F LATIN SMALL LETTER O
+0x0070 LATIN SMALL LETTER P
+0x0071 LATIN SMALL LETTER Q
+0x0072 LATIN SMALL LETTER R
+0x0073 LATIN SMALL LETTER S
+0x0074 LATIN SMALL LETTER T
+0x0075 LATIN SMALL LETTER U
+0x0076 LATIN SMALL LETTER V
+0x0077 LATIN SMALL LETTER W
+0x0078 LATIN SMALL LETTER X
+0x0079 LATIN SMALL LETTER Y
+0x007A LATIN SMALL LETTER Z
+0x00C0 LATIN CAPITAL LETTER A WITH GRAVE
+0x00C1 LATIN CAPITAL LETTER A WITH ACUTE
+0x00C4 LATIN CAPITAL LETTER A WITH DIAERESIS
+0x00C8 LATIN CAPITAL LETTER E WITH GRAVE
+0x00C9 LATIN CAPITAL LETTER E WITH ACUTE
+0x00CA LATIN CAPITAL LETTER E WITH CIRCUMFLEX
+0x00CB LATIN CAPITAL LETTER E WITH DIAERESIS
+0x00CC LATIN CAPITAL LETTER I WITH GRAVE
+0x00CD LATIN CAPITAL LETTER I WITH ACUTE
+0x00CE LATIN CAPITAL LETTER I WITH CIRCUMFLEX
+0x00CF LATIN CAPITAL LETTER I WITH DIAERESIS
+0x00D1 LATIN CAPITAL LETTER N WITH TILDE
+0x00D2 LATIN CAPITAL LETTER O WITH GRAVE
+0x00D3 LATIN CAPITAL LETTER O WITH ACUTE
+0x00D4 LATIN CAPITAL LETTER O WITH CIRCUMFLEX
+0x00D6 LATIN CAPITAL LETTER O WITH DIAERESIS
+0x00D9 LATIN CAPITAL LETTER U WITH GRAVE
+0x00DA LATIN CAPITAL LETTER U WITH ACUTE
+0x00DB LATIN CAPITAL LETTER U WITH CIRCUMFLEX
+0x00DC LATIN CAPITAL LETTER U WITH DIAERESIS
+0x00DD LATIN CAPITAL LETTER Y WITH ACUTE
+0x00E0 LATIN SMALL LETTER A WITH GRAVE
+0x00E1 LATIN SMALL LETTER A WITH ACUTE
+0x00E4 LATIN SMALL LETTER A WITH DIAERESIS
+0x00E8 LATIN SMALL LETTER E WITH GRAVE
+0x00E9 LATIN SMALL LETTER E WITH ACUTE
+0x00EA LATIN SMALL LETTER E WITH CIRCUMFLEX
+0x00EB LATIN SMALL LETTER E WITH DIAERESIS
+0x00EC LATIN SMALL LETTER I WITH GRAVE
+0x00ED LATIN SMALL LETTER I WITH ACUTE
+0x00EE LATIN SMALL LETTER I WITH CIRCUMFLEX
+0x00EF LATIN SMALL LETTER I WITH DIAERESIS
+0x00F1 LATIN SMALL LETTER N WITH TILDE
+0x00F2 LATIN SMALL LETTER O WITH GRAVE
+0x00F3 LATIN SMALL LETTER O WITH ACUTE
+0x00F4 LATIN SMALL LETTER O WITH CIRCUMFLEX
+0x00F6 LATIN SMALL LETTER O WITH DIAERESIS
+0x00F9 LATIN SMALL LETTER U WITH GRAVE
+0x00FA LATIN SMALL LETTER U WITH ACUTE
+0x00FB LATIN SMALL LETTER U WITH CIRCUMFLEX
+0x00FC LATIN SMALL LETTER U WITH DIAERESIS
+0x00FD LATIN SMALL LETTER Y WITH ACUTE
+0x0143 LATIN CAPITAL LETTER N WITH ACUTE
+0x0144 LATIN SMALL LETTER N WITH ACUTE
+0x014A LATIN CAPITAL LETTER ENG
+0x014B LATIN SMALL LETTER ENG
+0x0181 LATIN CAPITAL LETTER B WITH HOOK
+0x0186 LATIN CAPITAL LETTER OPEN O
+0x018A LATIN CAPITAL LETTER D WITH HOOK
+0x0190 LATIN CAPITAL LETTER OPEN E
+0x0198 LATIN CAPITAL LETTER K WITH HOOK
+0x0199 LATIN SMALL LETTER K WITH HOOK
+0x019D LATIN CAPITAL LETTER N WITH LEFT HOOK
+0x01B3 LATIN CAPITAL LETTER Y WITH HOOK
+0x01B4 LATIN SMALL LETTER Y WITH HOOK
+0x01F8 LATIN CAPITAL LETTER N WITH GRAVE
+0x01F9 LATIN SMALL LETTER N WITH GRAVE
+0x0253 LATIN SMALL LETTER B WITH HOOK
+0x0254 LATIN SMALL LETTER OPEN O
+0x0257 LATIN SMALL LETTER D WITH HOOK
+0x025B LATIN SMALL LETTER OPEN E
+0x0272 LATIN SMALL LETTER N WITH LEFT HOOK
+0x02BC MODIFIER LETTER APOSTROPHE
+0x0300 COMBINING GRAVE ACCENT
+0x0301 COMBINING ACUTE ACCENT
+0x0302 COMBINING CIRCUMFLEX ACCENT
+0x0303 COMBINING TILDE
+0x0304 COMBINING MACRON
+0x0306 COMBINING BREVE
+0x0307 COMBINING DOT ABOVE
+0x0308 COMBINING DIAERESIS
+0x030A COMBINING RING ABOVE
+0x0323 COMBINING DOT BELOW
+0x0327 COMBINING CEDILLA
+0x1E3E LATIN CAPITAL LETTER M WITH ACUTE
+0x1E3F LATIN SMALL LETTER M WITH ACUTE
+0x1E44 LATIN CAPITAL LETTER N WITH DOT ABOVE
+0x1E45 LATIN SMALL LETTER N WITH DOT ABOVE
+0x1E62 LATIN CAPITAL LETTER S WITH DOT BELOW
+0x1E63 LATIN SMALL LETTER S WITH DOT BELOW
+0x1EB8 LATIN CAPITAL LETTER E WITH DOT BELOW
+0x1EB9 LATIN SMALL LETTER E WITH DOT BELOW
+0x1ECA LATIN CAPITAL LETTER I WITH DOT BELOW
+0x1ECB LATIN SMALL LETTER I WITH DOT BELOW
+0x1ECC LATIN CAPITAL LETTER O WITH DOT BELOW
+0x1ECD LATIN SMALL LETTER O WITH DOT BELOW
+0x1EE4 LATIN CAPITAL LETTER U WITH DOT BELOW
+0x1EE5 LATIN SMALL LETTER U WITH DOT BELOW
+0x2013 EN DASH
+0x2014 EM DASH
+0x2018 LEFT SINGLE QUOTATION MARK
+0x2019 RIGHT SINGLE QUOTATION MARK
+0x201C LEFT DOUBLE QUOTATION MARK
+0x201D RIGHT DOUBLE QUOTATION MARK
+0x2026 HORIZONTAL ELLIPSIS
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `glyphsets-0.6.9/scripts/assemble_languages.py` & `glyphsets-1.0.0/scripts/assemble_languages.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 """
 Read all languages and regions from gflanguages and print out the languages that are supported
 in Europe or Americas and have more than 5 million speakers.
 """
 
 import argparse
 import gflanguages
+import logging
 
 SPEAKERS = 5000000
 
 
 def main(args):
     arg_parser = argparse.ArgumentParser(
         description="Generates a list of language ids based on given requirements."
     )
     arg_parser.add_argument(
-        "--regions", nargs="+", help="Region or region groups where languages are used."
+        "--regions",
+        nargs="+",
+        help="Region or region groups where languages are used.",
+        default=[],
     )
     arg_parser.add_argument(
         "--population", help="Minimum speakers’ population.", default=SPEAKERS
     )
-    arg_parser.add_argument("--script", help="Script of the languages.")
+    arg_parser.add_argument(
+        "--script",
+        nargs="+",
+        required=True,
+        help="Script of the languages.",
+    )
     arg_parser.add_argument(
         "--include-languages",
         nargs="+",
         default=[],
         help="Languages that should be included even if they don’t match the other requirements.",
     )
+    arg_parser.add_argument(
+        "--exclude-languages",
+        nargs="+",
+        default=[],
+        help="Languages that should be excluded even if they match the other requirements.",
+    )
     options = arg_parser.parse_args(args)
     options.population = int(options.population)
 
     regions = gflanguages.LoadRegions()
+    if not options.regions:
+        options.regions = [country_code for country_code in regions]
     languages = gflanguages.LoadLanguages()
 
     country_codes = set()
 
     # Go through countries and add them to the set if their region_group is in options.regions or they are in options.regions
     for country_code in regions:
         if set(regions[country_code].region_group).intersection(
@@ -41,26 +58,27 @@
         ) or (country_code in options.regions):
             country_codes.add(country_code)
 
     # Go through languages and add them to the set if their regions are in country_codes
     language_codes = set()
 
     # Print languages if they are supported through the logic
+    print("language_codes:")
     for language_code in sorted(languages.keys()):
         if (
             (
                 language_code in options.include_languages
                 or set(languages[language_code].region).intersection(country_codes)
-            )
+            ) and language_code not in options.exclude_languages
             and languages[language_code].population >= options.population
-            and languages[language_code].script == options.script
+            and languages[language_code].script in options.script
         ):
             if not languages[language_code].exemplar_chars:
-                print(
-                    f"WARNING, {languages[language_code].name} has no character defintions."
+                logging.warning(
+                    f"{languages[language_code].name} has no character definitions."
                 )
             language_codes.add(language_code)
             print(f"  - {language_code}  # {languages[language_code].name}")
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `glyphsets-0.6.9/scripts/find_language_for_character.py` & `glyphsets-1.0.0/scripts/find_language_for_character.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.9/setup.py` & `glyphsets-1.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,53 +16,64 @@
 # limitations under the License.
 #
 # See AUTHORS.txt for the list of Authors and LICENSE.txt for the License.
 import os
 from setuptools import setup
 
 # Read the contents of the README file
-with open('README.md', encoding="utf-8") as f:
+with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="glyphsets",
     use_scm_version={"write_to": "Lib/glyphsets/_version.py"},
-    url='https://github.com/googlefonts/glyphsets/',
-    description='A python API for evaluating coverage of glyph sets in font projects.',
+    url="https://github.com/googlefonts/glyphsets/",
+    description="A python API for evaluating coverage of glyph sets in font projects.",
     long_description=long_description,
-    long_description_content_type='text/markdown',  # This is important!
-    author=('Dave Crossland, '
-            'Eli Heuer, '
-            'Felipe Sanches, '
-            'Lasse Fister, '
-            'Marc Foley, '
-            'Yanone, '
-            'Roderick Sheeter'),
-    author_email='dave@lab6.com',
-    package_dir={'': 'Lib'},
-    packages=['glyphsets', 'glyphsets.definitions'],
-    package_data={'glyphsets': [
-                      "encodings/*.nam",
-                      "encodings/GF Glyph Sets/*.nam",
-                      "definitions/nam/*.nam",
-                      "*.json",
-                  ]
-                 },
+    long_description_content_type="text/markdown",  # This is important!
+    author=(
+        "Dave Crossland, "
+        "Eli Heuer, "
+        "Felipe Sanches, "
+        "Lasse Fister, "
+        "Marc Foley, "
+        "Yanone, "
+        "Roderick Sheeter"
+    ),
+    author_email="dave@lab6.com",
+    package_dir={"": "Lib"},
+    packages=["glyphsets"],
+    package_data={
+        "glyphsets": [
+            "*.json",
+            "definitions/*.yaml",
+            "results/nam/*.nam",
+            "results/txt/nice-names/*.txt",
+        ]
+    },
     entry_points={"console_scripts": ["glyphsets = glyphsets.__main__:main"]},
     zip_safe=False,
     classifiers=[
-        'Intended Audience :: Developers',
-        'Topic :: Text Processing :: Fonts',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3'
+        "Intended Audience :: Developers",
+        "Topic :: Text Processing :: Fonts",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
     ],
-    python_requires=">=3.7",
-    setup_requires=['setuptools_scm>=4,<6.1'],
+    python_requires=">=3.8",
+    setup_requires=["setuptools_scm>=8.0.4,<8.1"],
     install_requires=[
-        'setuptools',
-        'FontTools[ufo]',
-        'glyphsLib',
-        'defcon',
-        'unicodedata2',
-    ]
+        "requests",
+        "setuptools",
+        "FontTools[ufo]",
+        "glyphsLib>=6.7.1",
+        "defcon",
+        "unicodedata2",
+        "gflanguages>=0.6.0",
+        "pyyaml",
+    ],
+    extras_require={
+        "dev": [  # For the tests to run
+            "gfsubsets",
+        ]
+    },
 )
```

### Comparing `glyphsets-0.6.9/tests/data/MavenPro[wght].ttf` & `glyphsets-1.0.0/tests/data/MavenPro[wght].ttf`

 * *Files identical despite different names*

