# Comparing `tmp/perturb_tools-0.3.2.tar.gz` & `tmp/perturb_tools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perturb_tools-0.3.2.tar", last modified: Sat Apr 13 21:08:19 2024, max compression
+gzip compressed data, was "perturb_tools-0.3.3.tar", last modified: Fri May  3 19:57:22 2024, max compression
```

## Comparing `perturb_tools-0.3.2.tar` & `perturb_tools-0.3.3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.142079 perturb_tools-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-13 21:08:19.142079 perturb_tools-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.126079 perturb_tools-0.3.2/perturb_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.130079 perturb_tools-0.3.2/perturb_tools/_arithmetic/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_arithmetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.130079 perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.130079 perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/_LogFoldChange/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_LogFoldChange_Module.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/_LogFoldChange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_calculate_log_fold_change.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/_SequenceManipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/_log_fold_change.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.130079 perturb_tools-0.3.2/perturb_tools/_experimental_design/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.130079 perturb_tools-0.3.2/perturb_tools/_experimental_design/_coding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.130079 perturb_tools-0.3.2/perturb_tools/_experimental_design/_coding/_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_coding/_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_coding/_funcs/_plot_CDS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.130079 perturb_tools-0.3.2/perturb_tools/_experimental_design/_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_funcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.134079 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_GTF_Module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_TargetModule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_add_region_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_add_sgRNA_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_annotate_guide_biochemistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_annotate_protospacer.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_get_chromosome_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_get_screen_target_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_identify_overlapping_fragments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_make_guide_library_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_query_region_for_PAM.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_scan_for_BsmbI.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_widen_regions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.134079 perturb_tools-0.3.2/perturb_tools/_external_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_external_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.134079 perturb_tools-0.3.2/perturb_tools/_framework/
--rw-r--r--   0 runner    (1001) docker     (127)    15293 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_ScreenModule.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.134079 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.134079 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_GuideAnnotationModule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.134079 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_context_sequence_to_gene_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_guide_target_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_annotate_guide_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_annotate_protospacer.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_create_gene_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_print_screen_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_read_write_poolQ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.134079 perturb_tools-0.3.2/perturb_tools/_normalization/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_normalization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.134079 perturb_tools-0.3.2/perturb_tools/_normalization/_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_normalization/_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_normalization/_funcs/_read_count_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.134079 perturb_tools-0.3.2/perturb_tools/_plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.138079 perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_get_default_matplotlib_figure_width_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_correlation_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_gene_exon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_guide_enrichment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_rep_consistency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_set_matplotlib_rc_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.138079 perturb_tools-0.3.2/perturb_tools/_qc/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_qc/qc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.138079 perturb_tools-0.3.2/perturb_tools/_readwrite/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_readwrite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.138079 perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_check_fix_file_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_read_screen_from_PoolQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_read_screen_from_csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_write_experiment_report_to_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_write_screen_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_write_screen_to_excel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.138079 perturb_tools-0.3.2/perturb_tools/_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.138079 perturb_tools-0.3.2/perturb_tools/_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.142079 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_SequenceManipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_fetch_chromosome_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_flexible_mkdir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_get_chromosome_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_get_gene_exons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_glob_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_scan_sequence_for_motif.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_update_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.142079 perturb_tools-0.3.2/perturb_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-13 21:08:19.000000 perturb_tools-0.3.2/perturb_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-13 21:08:19.000000 perturb_tools-0.3.2/perturb_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:08:19.000000 perturb_tools-0.3.2/perturb_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-13 21:08:19.000000 perturb_tools-0.3.2/perturb_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 21:08:19.000000 perturb_tools-0.3.2/perturb_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 21:08:19.142079 perturb_tools-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:08:19.142079 perturb_tools-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-13 21:08:07.000000 perturb_tools-0.3.2/tests/test_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.541277 perturb_tools-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-03 19:57:22.541277 perturb_tools-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.525277 perturb_tools-0.3.3/perturb_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.525277 perturb_tools-0.3.3/perturb_tools/_arithmetic/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_arithmetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.525277 perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.529277 perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/_LogFoldChange/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_LogFoldChange_Module.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/_LogFoldChange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_calculate_log_fold_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/_SequenceManipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/_log_fold_change.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.529277 perturb_tools-0.3.3/perturb_tools/_experimental_design/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.529277 perturb_tools-0.3.3/perturb_tools/_experimental_design/_coding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.529277 perturb_tools-0.3.3/perturb_tools/_experimental_design/_coding/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_coding/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_coding/_funcs/_plot_CDS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.529277 perturb_tools-0.3.3/perturb_tools/_experimental_design/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_funcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.529277 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_GTF_Module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_TargetModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_add_region_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_add_sgRNA_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_annotate_guide_biochemistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_annotate_protospacer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_get_chromosome_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_get_screen_target_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_identify_overlapping_fragments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_make_guide_library_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_query_region_for_PAM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_scan_for_BsmbI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_widen_regions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.529277 perturb_tools-0.3.3/perturb_tools/_external_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_external_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.533277 perturb_tools-0.3.3/perturb_tools/_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)    15293 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_ScreenModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.533277 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.533277 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_GuideAnnotationModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.533277 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_context_sequence_to_gene_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_guide_target_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_annotate_guide_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_annotate_protospacer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_create_gene_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_print_screen_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_read_write_poolQ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.533277 perturb_tools-0.3.3/perturb_tools/_normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_normalization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.533277 perturb_tools-0.3.3/perturb_tools/_normalization/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_normalization/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_normalization/_funcs/_read_count_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.533277 perturb_tools-0.3.3/perturb_tools/_plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.537277 perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_get_default_matplotlib_figure_width_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_correlation_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_gene_exon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_guide_enrichment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_rep_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_set_matplotlib_rc_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.537277 perturb_tools-0.3.3/perturb_tools/_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_qc/qc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.537277 perturb_tools-0.3.3/perturb_tools/_readwrite/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_readwrite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.537277 perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_check_fix_file_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_read_screen_from_PoolQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_read_screen_from_csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_write_experiment_report_to_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_write_screen_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_write_screen_to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.537277 perturb_tools-0.3.3/perturb_tools/_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.537277 perturb_tools-0.3.3/perturb_tools/_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.537277 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_SequenceManipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_fetch_chromosome_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_flexible_mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_get_chromosome_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_get_gene_exons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_glob_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_scan_sequence_for_motif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_update_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.541277 perturb_tools-0.3.3/perturb_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-03 19:57:22.000000 perturb_tools-0.3.3/perturb_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-03 19:57:22.000000 perturb_tools-0.3.3/perturb_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:57:22.000000 perturb_tools-0.3.3/perturb_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 19:57:22.000000 perturb_tools-0.3.3/perturb_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 19:57:22.000000 perturb_tools-0.3.3/perturb_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:57:22.541277 perturb_tools-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:57:22.541277 perturb_tools-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-03 19:57:14.000000 perturb_tools-0.3.3/tests/test_screen.py
```

### Comparing `perturb_tools-0.3.2/LICENSE` & `perturb_tools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/PKG-INFO` & `perturb_tools-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perturb-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: perturb-tools - Analysis Framework for Pooled CRISPR Genome Editing Screens.
 Home-page: https://github.com/pinellolab/perturb-tools
 Author: ['Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard', 'Jayoung K. Ryu - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard']
 Author-email: mvinyard@broadinstitute.org, jayoung_ryu@g.harvard.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `perturb_tools-0.3.2/README.md` & `perturb_tools-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_LogFoldChange_Module.py` & `perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_LogFoldChange_Module.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_calculate_log_fold_change.py` & `perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_calculate_log_fold_change.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_arithmetic/_funcs/_SequenceManipulation.py` & `perturb_tools-0.3.3/perturb_tools/_arithmetic/_funcs/_SequenceManipulation.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_coding/_funcs/_plot_CDS.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_coding/_funcs/_plot_CDS.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_TargetModule.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_TargetModule.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_add_sgRNA_context.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_add_sgRNA_context.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_annotate_guide_biochemistry.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_annotate_guide_biochemistry.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_annotate_protospacer.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_annotate_protospacer.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_get_chromosome_sequence.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_get_chromosome_sequence.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_get_screen_target_features.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_get_screen_target_features.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_identify_overlapping_fragments.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_identify_overlapping_fragments.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_make_guide_library_df.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_make_guide_library_df.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_query_region_for_PAM.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_query_region_for_PAM.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_experimental_design/_general/_scan_for_BsmbI.py` & `perturb_tools-0.3.3/perturb_tools/_experimental_design/_general/_scan_for_BsmbI.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_framework/_ScreenModule.py` & `perturb_tools-0.3.3/perturb_tools/_framework/_ScreenModule.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_GuideAnnotationModule.py` & `perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_GuideAnnotationModule.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_context_sequence_to_gene_dict.py` & `perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_context_sequence_to_gene_dict.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_guide_target_metadata.py` & `perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_guide_target_metadata.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_annotate_guide_position.py` & `perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_annotate_guide_position.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_print_screen_object.py` & `perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_print_screen_object.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_framework/_supporting_functions/_read_write_poolQ.py` & `perturb_tools-0.3.3/perturb_tools/_framework/_supporting_functions/_read_write_poolQ.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_normalization/_funcs/_read_count_norm.py` & `perturb_tools-0.3.3/perturb_tools/_normalization/_funcs/_read_count_norm.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_get_default_matplotlib_figure_width_height.py` & `perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_get_default_matplotlib_figure_width_height.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_correlation_heatmap.py` & `perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_correlation_heatmap.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_gene_exon.py` & `perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_gene_exon.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_guide_enrichment.py` & `perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_guide_enrichment.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_rep_consistency.py` & `perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_rep_consistency.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_plotting/_funcs/_plot_stats.py` & `perturb_tools-0.3.3/perturb_tools/_plotting/_funcs/_plot_stats.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_qc/qc.py` & `perturb_tools-0.3.3/perturb_tools/_qc/qc.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_check_fix_file_extension.py` & `perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_check_fix_file_extension.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_read_screen_from_PoolQ.py` & `perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_read_screen_from_PoolQ.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_read_screen_from_csvs.py` & `perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_read_screen_from_csvs.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,21 @@
             for key, df_path in layers_filenames_dict.items():
                 try:
                     check_indices(layer_df, guides_df.index, samples_df.index)
                 except ValueError as e:
                     raise ValueError("Error raised for layer_df") from e
                 layers_dict[key] = layer_df
     else:
-        if guides_df:
+        if guides_df is not None:
             X_df = X_df.loc[guides_df.index, :]
             if layers_filenames_dict:
                 for key, df_path in layers_filenames_dict.items():
                     layer_df = layer_df.loc[guides_df.index, :]
                     layers_dict[key] = layer_df
-        if samples_df:
+        if samples_df is not None:
             X_df = X_df.loc[:, samples_df.index]
             if layers_filenames_dict:
                 for key, df_path in layers_filenames_dict.items():
                     layer_df = layer_df.loc[:, samples_df.index]
                     layers_dict[key] = layer_df
     if layers_dict:
         for key, df in layers_dict.items():
```

### Comparing `perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_write_experiment_report_to_excel.py` & `perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_write_experiment_report_to_excel.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_write_screen_to_csv.py` & `perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_write_screen_to_csv.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_readwrite/_funcs/_write_screen_to_excel.py` & `perturb_tools-0.3.3/perturb_tools/_readwrite/_funcs/_write_screen_to_excel.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_FileHandler.py` & `perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_FileHandler.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_SequenceManipulation.py` & `perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_SequenceManipulation.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_fetch_chromosome_sequence.py` & `perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_fetch_chromosome_sequence.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_flexible_mkdir.py` & `perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_flexible_mkdir.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_get_chromosome_sequence.py` & `perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_get_chromosome_sequence.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_get_gene_exons.py` & `perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_get_gene_exons.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools/_utilities/_funcs/_glob_dict.py` & `perturb_tools-0.3.3/perturb_tools/_utilities/_funcs/_glob_dict.py`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/perturb_tools.egg-info/PKG-INFO` & `perturb_tools-0.3.3/perturb_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perturb-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: perturb-tools - Analysis Framework for Pooled CRISPR Genome Editing Screens.
 Home-page: https://github.com/pinellolab/perturb-tools
 Author: ['Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard', 'Jayoung K. Ryu - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard']
 Author-email: mvinyard@broadinstitute.org, jayoung_ryu@g.harvard.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `perturb_tools-0.3.2/perturb_tools.egg-info/SOURCES.txt` & `perturb_tools-0.3.3/perturb_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perturb_tools-0.3.2/setup.py` & `perturb_tools-0.3.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import os
 import sys
 
 
 setup(
     name="perturb-tools",
-    version="0.3.2",
+    version="0.3.3",
     python_requires=">3.7.0",
     author=[
         "Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
         "Jayoung K. Ryu - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
     ],
     author_email="mvinyard@broadinstitute.org, jayoung_ryu@g.harvard.edu",
     url="https://github.com/pinellolab/perturb-tools",
```

### Comparing `perturb_tools-0.3.2/tests/test_screen.py` & `perturb_tools-0.3.3/tests/test_screen.py`

 * *Files identical despite different names*

