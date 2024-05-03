# Comparing `tmp/orjson-3.9.8.tar.gz` & `tmp/orjson-3.9.9.tar.gz`

## Comparing `orjson-3.9.8.tar` & `orjson-3.9.9.tar`

### file list

```diff
@@ -1,2019 +1,2023 @@
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 orjson-3.9.8/Cargo.toml
--rw-r--r--   0     1001      127    18948 2023-10-10 14:53:05.000000 orjson-3.9.8/CHANGELOG.md
--rw-r--r--   0     1001      127    10847 2023-10-10 14:53:05.000000 orjson-3.9.8/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:53:05.000000 orjson-3.9.8/LICENSE-MIT
--rw-r--r--   0     1001      127    47773 2023-10-10 14:53:05.000000 orjson-3.9.8/README.md
--rw-r--r--   0     1001      127     8780 2023-10-10 14:53:05.000000 orjson-3.9.8/data/blns.txt.xz
--rw-r--r--   0     1001      127   376512 2023-10-10 14:53:05.000000 orjson-3.9.8/data/canada.json.xz
--rw-r--r--   0     1001      127    12336 2023-10-10 14:53:05.000000 orjson-3.9.8/data/citm_catalog.json.xz
--rw-r--r--   0     1001      127     8264 2023-10-10 14:53:05.000000 orjson-3.9.8/data/github.json.xz
--rw-r--r--   0     1001      127      592 2023-10-10 14:53:05.000000 orjson-3.9.8/data/issue331_1.json.xz
--rw-r--r--   0     1001      127      592 2023-10-10 14:53:05.000000 orjson-3.9.8/data/issue331_2.json.xz
--rw-r--r--   0     1001      127       60 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail01.json
--rw-r--r--   0     1001      127       17 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail02.json
--rw-r--r--   0     1001      127       37 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail03.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail04.json
--rw-r--r--   0     1001      127       24 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail05.json
--rw-r--r--   0     1001      127       26 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail06.json
--rw-r--r--   0     1001      127       26 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail07.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail08.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail09.json
--rw-r--r--   0     1001      127       58 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail10.json
--rw-r--r--   0     1001      127       29 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail11.json
--rw-r--r--   0     1001      127       31 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail12.json
--rw-r--r--   0     1001      127       43 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail13.json
--rw-r--r--   0     1001      127       31 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail14.json
--rw-r--r--   0     1001      127       34 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail15.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail16.json
--rw-r--r--   0     1001      127       34 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail17.json
--rw-r--r--   0     1001      127       50 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail18.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail19.json
--rw-r--r--   0     1001      127       23 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail20.json
--rw-r--r--   0     1001      127       32 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail21.json
--rw-r--r--   0     1001      127       33 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail22.json
--rw-r--r--   0     1001      127       20 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail23.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail24.json
--rw-r--r--   0     1001      127       29 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail25.json
--rw-r--r--   0     1001      127       38 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail26.json
--rw-r--r--   0     1001      127       14 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail27.json
--rw-r--r--   0     1001      127       15 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail28.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail29.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail30.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail31.json
--rw-r--r--   0     1001      127       40 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail32.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/fail33.json
--rw-r--r--   0     1001      127     1441 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/pass01.json
--rw-r--r--   0     1001      127       52 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/pass02.json
--rw-r--r--   0     1001      127      148 2023-10-10 14:53:05.000000 orjson-3.9.8/data/jsonchecker/pass03.json
--rw-r--r--   0     1001      127       14 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_double_huge_neg_exp.json
--rw-r--r--   0     1001      127      137 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_huge_exp.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_neg_int_huge_exp.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_pos_double_huge_exp.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_real_neg_overflow.json
--rw-r--r--   0     1001      127       15 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_real_pos_overflow.json
--rw-r--r--   0     1001      127       15 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_real_underflow.json
--rw-r--r--   0     1001      127       33 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_too_big_neg_int.json
--rw-r--r--   0     1001      127       23 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_too_big_pos_int.json
--rw-r--r--   0     1001      127       51 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_number_very_big_negative_int.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_object_key_lone_2nd_surrogate.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_1st_surrogate_but_2nd_missing.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_1st_valid_surrogate_2nd_invalid.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_UTF-16LE_with_BOM.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_UTF-8_invalid_sequence.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_UTF8_surrogate_U+D800.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_incomplete_surrogate_and_escape_valid.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_incomplete_surrogate_pair.json
--rw-r--r--   0     1001      127       18 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_incomplete_surrogates_escape_valid.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_invalid_lonely_surrogate.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_invalid_surrogate.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_invalid_utf-8.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_inverted_surrogates_U+1D11E.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_iso_latin_1.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_lone_second_surrogate.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_lone_utf8_continuation_byte.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_not_in_unicode_range.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_overlong_sequence_2_bytes.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_overlong_sequence_6_bytes.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_overlong_sequence_6_bytes_null.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_truncated-utf-8.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_utf16BE_no_BOM.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_string_utf16LE_no_BOM.json
--rw-r--r--   0     1001      127       80 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_structure_500_nested_arrays.json.xz
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/i_structure_UTF-8_BOM_empty_object.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_1_true_without_comma.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_a_invalid_utf8.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_colon_instead_of_comma.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_comma_after_close.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_comma_and_number.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_double_comma.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_double_extra_comma.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_extra_close.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_extra_comma.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_incomplete.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_incomplete_invalid_value.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_inner_array_no_comma.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_invalid_utf8.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_items_separated_by_semicolon.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_just_comma.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_just_minus.json
--rw-r--r--   0     1001      127        9 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_missing_value.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_newlines_unclosed.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_number_and_comma.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_number_and_several_commas.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_spaces_vertical_tab_formfeed.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_star_inside.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_unclosed.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_unclosed_trailing_comma.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_unclosed_with_new_lines.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_array_unclosed_with_object_inside.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_incomplete_false.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_incomplete_null.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_incomplete_true.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_multidigit_number_then_00.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_++.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_+1.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_+Inf.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_-01.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_-1.0..json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_-2..json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_-NaN.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_.-1.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_.2e-3.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_0.1.2.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_0.3e+.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_0.3e.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_0.e1.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_0_capital_E+.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_0_capital_E.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_0e+.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_0e.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_1.0e+.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_1.0e-.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_1.0e.json
--rw-r--r--   0     1001      127        9 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_1_000.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_1eE2.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_2.e+3.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_2.e-3.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_2.e3.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_9.e+.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_Inf.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_NaN.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_U+FF11_fullwidth_digit_one.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_expression.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_hex_1_digit.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_hex_2_digits.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_infinity.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_invalid+-.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_invalid-negative-real.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_invalid-utf-8-in-bigger-int.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_invalid-utf-8-in-exponent.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_invalid-utf-8-in-int.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_minus_infinity.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_minus_sign_with_trailing_garbage.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_minus_space_1.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_neg_int_starting_with_zero.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_neg_real_without_int_part.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_neg_with_garbage_at_end.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_real_garbage_after_e.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_real_with_invalid_utf8_after_e.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_real_without_fractional_part.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_starting_with_dot.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_with_alpha.json
--rw-r--r--   0     1001      127       25 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_with_alpha_char.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_number_with_leading_zero.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_bad_value.json
--rw-r--r--   0     1001      127        9 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_bracket_key.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_comma_instead_of_colon.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_double_colon.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_emoji.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_garbage_at_end.json
--rw-r--r--   0     1001      127       14 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_key_with_single_quotes.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_lone_continuation_byte_in_key_and_trailing_comma.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_missing_colon.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_missing_key.json
--rw-r--r--   0     1001      127        9 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_missing_semicolon.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_missing_value.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_no-colon.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_non_string_key.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_non_string_key_but_huge_number_instead.json
--rw-r--r--   0     1001      127       21 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_repeated_null_null.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_several_trailing_commas.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_single_quote.json
--rw-r--r--   0     1001      127        9 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_trailing_comma.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_trailing_comment.json
--rw-r--r--   0     1001      127       14 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_trailing_comment_open.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_trailing_comment_slash_open.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_trailing_comment_slash_open_incomplete.json
--rw-r--r--   0     1001      127       18 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_two_commas_in_a_row.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_unquoted_key.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_unterminated-value.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_with_single_string.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_object_with_trailing_garbage.json
--rw-r--r--   0     1001      127        1 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_single_space.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_1_surrogate_then_escape.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_1_surrogate_then_escape_u.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_1_surrogate_then_escape_u1.json
--rw-r--r--   0     1001      127       14 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_1_surrogate_then_escape_u1x.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_accentuated_char_no_quotes.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_backslash_00.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_escape_x.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_escaped_backslash_bad.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_escaped_ctrl_char_tab.json
--rw-r--r--   0     1001      127        9 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_escaped_emoji.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_incomplete_escape.json
--rw-r--r--   0     1001      127        9 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_incomplete_escaped_character.json
--rw-r--r--   0     1001      127       14 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_incomplete_surrogate.json
--rw-r--r--   0     1001      127       18 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_incomplete_surrogate_escape_invalid.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_invalid-utf-8-in-escape.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_invalid_backslash_esc.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_invalid_unicode_escape.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_invalid_utf8_after_escape.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_leading_uescaped_thinspace.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_no_quotes_with_bad_escape.json
--rw-r--r--   0     1001      127        1 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_single_doublequote.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_single_quote.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_single_string_no_double_quotes.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_start_escape_unclosed.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_unescaped_crtl_char.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_unescaped_newline.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_unescaped_tab.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_unicode_CapitalU.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_string_with_trailing_garbage.json
--rw-r--r--   0     1001      127      148 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_100000_opening_arrays.json.xz
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_U+2060_word_joined.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_UTF8_BOM_no_data.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_angle_bracket_..json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_angle_bracket_null.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_array_trailing_garbage.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_array_with_extra_array_close.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_array_with_unclosed_string.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_ascii-unicode-identifier.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_capitalized_True.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_close_unopened_array.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_comma_instead_of_closing_brace.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_double_array.json
--rw-r--r--   0     1001      127        1 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_end_array.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_incomplete_UTF8_BOM.json
--rw-r--r--   0     1001      127        1 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_lone-invalid-utf-8.json
--rw-r--r--   0     1001      127        1 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_lone-open-bracket.json
--rw-r--r--   0     1001      127        0 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_no_data.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_null-byte-outside-string.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_number_with_trailing_garbage.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_object_followed_by_closing_object.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_object_unclosed_no_value.json
--rw-r--r--   0     1001      127       20 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_object_with_comment.json
--rw-r--r--   0     1001      127       15 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_object_with_trailing_garbage.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_array_apostrophe.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_array_comma.json
--rw-r--r--   0     1001      127      176 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_array_object.json.xz
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_array_open_object.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_array_open_string.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_array_string.json
--rw-r--r--   0     1001      127        1 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_object.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_object_close_array.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_object_comma.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_object_open_array.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_object_open_string.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_object_string_with_apostrophes.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_open_open.json
--rw-r--r--   0     1001      127        1 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_single_eacute.json
--rw-r--r--   0     1001      127        1 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_single_star.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_trailing_#.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_uescaped_LF_before_string.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_unclosed_array.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_unclosed_array_partial_null.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_unclosed_array_unfinished_false.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_unclosed_array_unfinished_true.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_unclosed_object.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_unicode-identifier.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_whitespace_U+2060_word_joiner.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/n_structure_whitespace_formfeed.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_arraysWithSpaces.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_empty-string.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_empty.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_ending_with_newline.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_false.json
--rw-r--r--   0     1001      127       18 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_heterogeneous.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_null.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_with_1_and_newline.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_with_leading_space.json
--rw-r--r--   0     1001      127       20 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_with_several_null.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_array_with_trailing_space.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_0e+1.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_0e1.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_after_space.json
--rw-r--r--   0     1001      127       84 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_double_close_to_zero.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_int_with_exp.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_minus_zero.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_negative_int.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_negative_one.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_negative_zero.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_real_capital_e.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_real_capital_e_neg_exp.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_real_capital_e_pos_exp.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_real_exponent.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_real_fraction_exponent.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_real_neg_exp.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_real_pos_exponent.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_simple_int.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_number_simple_real.json
--rw-r--r--   0     1001      127       26 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_basic.json
--rw-r--r--   0     1001      127       17 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_duplicated_key.json
--rw-r--r--   0     1001      127       17 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_duplicated_key_and_value.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_empty.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_empty_key.json
--rw-r--r--   0     1001      127       20 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_escaped_null_in_key.json
--rw-r--r--   0     1001      127       35 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_extreme_numbers.json
--rw-r--r--   0     1001      127      108 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_long_strings.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_simple.json
--rw-r--r--   0     1001      127      110 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_string_unicode.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_object_with_newlines.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_1_2_3_bytes_UTF-8_sequences.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_accepted_surrogate_pair.json
--rw-r--r--   0     1001      127       28 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_accepted_surrogate_pairs.json
--rw-r--r--   0     1001      127       20 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_allowed_escapes.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_backslash_and_u_escaped_zero.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_backslash_doublequotes.json
--rw-r--r--   0     1001      127       17 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_comments.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_double_escape_a.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_double_escape_n.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_escaped_control_character.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_escaped_noncharacter.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_in_array.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_in_array_with_leading_space.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_last_surrogates_1_and_2.json
--rw-r--r--   0     1001      127       17 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_nbsp_uescaped.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_nonCharacterInUTF-8_U+10FFFF.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_nonCharacterInUTF-8_U+FFFF.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_null_escape.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_one-byte-utf-8.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_pi.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_reservedCharacterInUTF-8_U+1BFFF.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_simple_ascii.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_space.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_surrogates_U+1D11E_MUSICAL_SYMBOL_G_CLEF.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_three-byte-utf-8.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_two-byte-utf-8.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_u+2028_line_sep.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_u+2029_par_sep.json
--rw-r--r--   0     1001      127       28 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_uEscape.json
--rw-r--r--   0     1001      127       17 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_uescaped_newline.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unescaped_char_delete.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicode.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicodeEscapedBackslash.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicode_2.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicode_U+10FFFE_nonchar.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicode_U+1FFFE_nonchar.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicode_U+200B_ZERO_WIDTH_SPACE.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicode_U+2064_invisible_plus.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicode_U+FDD0_nonchar.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicode_U+FFFE_nonchar.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_unicode_escaped_double_quote.json
--rw-r--r--   0     1001      127       11 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_utf8.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_string_with_del_character.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_lonely_false.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_lonely_int.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_lonely_negative_real.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_lonely_null.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_lonely_string.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_lonely_true.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_string_empty.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_trailing_newline.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_true_in_array.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/parsing/y_structure_whitespace_array.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip01.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip02.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip03.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip04.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip05.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip06.json
--rw-r--r--   0     1001      127        2 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip07.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip08.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip09.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip10.json
--rw-r--r--   0     1001      127        4 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip11.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip12.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip13.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip14.json
--rw-r--r--   0     1001      127        3 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip15.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip16.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip17.json
--rw-r--r--   0     1001      127       21 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip18.json
--rw-r--r--   0     1001      127       21 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip19.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip20.json
--rw-r--r--   0     1001      127        6 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip21.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip22.json
--rw-r--r--   0     1001      127        9 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip23.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip24.json
--rw-r--r--   0     1001      127       24 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip25.json
--rw-r--r--   0     1001      127       25 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip26.json
--rw-r--r--   0     1001      127       24 2023-10-10 14:53:05.000000 orjson-3.9.8/data/roundtrip/roundtrip27.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/number_1.0.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/number_1.000000000000000005.json
--rw-r--r--   0     1001      127       19 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/number_1000000000000000.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/number_10000000000000000999.json
--rw-r--r--   0     1001      127        8 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/number_1e-999.json
--rw-r--r--   0     1001      127        5 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/number_1e6.json
--rw-r--r--   0     1001      127       24 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/object_key_nfc_nfd.json
--rw-r--r--   0     1001      127       24 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/object_key_nfd_nfc.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/object_same_key_different_values.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/object_same_key_same_value.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/object_same_key_unclear_values.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/string_1_escaped_invalid_codepoint.json
--rw-r--r--   0     1001      127        7 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/string_1_invalid_codepoint.json
--rw-r--r--   0     1001      127       16 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/string_2_escaped_invalid_codepoints.json
--rw-r--r--   0     1001      127       10 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/string_2_invalid_codepoints.json
--rw-r--r--   0     1001      127       22 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/string_3_escaped_invalid_codepoints.json
--rw-r--r--   0     1001      127       13 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/string_3_invalid_codepoints.json
--rw-r--r--   0     1001      127       12 2023-10-10 14:53:05.000000 orjson-3.9.8/data/transform/string_with_escaped_NULL.json
--rw-r--r--   0     1001      127    34780 2023-10-10 14:53:05.000000 orjson-3.9.8/data/twitter.json.xz
--rw-r--r--   0     1001      127   346765 2023-10-10 14:53:05.000000 orjson-3.9.8/include/yyjson/yyjson.c
--rw-r--r--   0     1001      127   303585 2023-10-10 14:53:05.000000 orjson-3.9.8/include/yyjson/yyjson.h
--rw-r--r--   0     1001      127     1374 2023-10-10 14:53:05.000000 orjson-3.9.8/src/deserialize/cache.rs
--rw-r--r--   0     1001      127     1034 2023-10-10 14:53:05.000000 orjson-3.9.8/src/deserialize/deserializer.rs
--rw-r--r--   0     1001      127     3096 2023-10-10 14:53:05.000000 orjson-3.9.8/src/deserialize/error.rs
--rw-r--r--   0     1001      127     4041 2023-10-10 14:53:05.000000 orjson-3.9.8/src/deserialize/json.rs
--rw-r--r--   0     1001      127      312 2023-10-10 14:53:05.000000 orjson-3.9.8/src/deserialize/mod.rs
--rw-r--r--   0     1001      127     1994 2023-10-10 14:53:05.000000 orjson-3.9.8/src/deserialize/pyobject.rs
--rw-r--r--   0     1001      127     3192 2023-10-10 14:53:05.000000 orjson-3.9.8/src/deserialize/utf8.rs
--rw-r--r--   0     1001      127     5992 2023-10-10 14:53:05.000000 orjson-3.9.8/src/deserialize/yyjson.rs
--rw-r--r--   0     1001      127      727 2023-10-10 14:53:05.000000 orjson-3.9.8/src/ffi/buffer.rs
--rw-r--r--   0     1001      127      469 2023-10-10 14:53:05.000000 orjson-3.9.8/src/ffi/bytes.rs
--rw-r--r--   0     1001      127     4076 2023-10-10 14:53:05.000000 orjson-3.9.8/src/ffi/fragment.rs
--rw-r--r--   0     1001      127     1004 2023-10-10 14:53:05.000000 orjson-3.9.8/src/ffi/immortal.rs
--rw-r--r--   0     1001      127     1016 2023-10-10 14:53:05.000000 orjson-3.9.8/src/ffi/list.rs
--rw-r--r--   0     1001      127     1056 2023-10-10 14:53:05.000000 orjson-3.9.8/src/ffi/long.rs
--rw-r--r--   0     1001      127      400 2023-10-10 14:53:05.000000 orjson-3.9.8/src/ffi/mod.rs
--rw-r--r--   0     1001      127     1884 2023-10-10 14:53:05.000000 orjson-3.9.8/src/ffi/yyjson.rs
--rw-r--r--   0     1001      127    11690 2023-10-10 14:53:05.000000 orjson-3.9.8/src/lib.rs
--rw-r--r--   0     1001      127     1133 2023-10-10 14:53:05.000000 orjson-3.9.8/src/opt.rs
--rw-r--r--   0     1001      127     2591 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/error.rs
--rw-r--r--   0     1001      127    34700 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/json.rs
--rw-r--r--   0     1001      127      144 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/mod.rs
--rw-r--r--   0     1001      127     7518 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/dataclass.rs
--rw-r--r--   0     1001      127     7955 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/datetime.rs
--rw-r--r--   0     1001      127     6099 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/datetimelike.rs
--rw-r--r--   0     1001      127     2549 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/default.rs
--rw-r--r--   0     1001      127    13553 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/dict.rs
--rw-r--r--   0     1001      127      544 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/float.rs
--rw-r--r--   0     1001      127     1570 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/fragment.rs
--rw-r--r--   0     1001      127     2233 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/int.rs
--rw-r--r--   0     1001      127     1728 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/list.rs
--rw-r--r--   0     1001      127      848 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/mod.rs
--rw-r--r--   0     1001      127      405 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/none.rs
--rw-r--r--   0     1001      127    36974 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/numpy.rs
--rw-r--r--   0     1001      127      544 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/pybool.rs
--rw-r--r--   0     1001      127     1323 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/pyenum.rs
--rw-r--r--   0     1001      127     1606 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/tuple.rs
--rw-r--r--   0     1001      127     1299 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/unicode.rs
--rw-r--r--   0     1001      127     2012 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/per_type/uuid.rs
--rw-r--r--   0     1001      127     7647 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/serializer.rs
--rw-r--r--   0     1001      127     5480 2023-10-10 14:53:05.000000 orjson-3.9.8/src/serialize/writer.rs
--rw-r--r--   0     1001      127     1053 2023-10-10 14:53:05.000000 orjson-3.9.8/src/str/check.rs
--rw-r--r--   0     1001      127     2839 2023-10-10 14:53:05.000000 orjson-3.9.8/src/str/create.rs
--rw-r--r--   0     1001      127     1928 2023-10-10 14:53:05.000000 orjson-3.9.8/src/str/ffi.rs
--rw-r--r--   0     1001      127      135 2023-10-10 14:53:05.000000 orjson-3.9.8/src/str/mod.rs
--rw-r--r--   0     1001      127    13435 2023-10-10 14:53:05.000000 orjson-3.9.8/src/typeref.rs
--rw-r--r--   0     1001      127     4948 2023-10-10 14:53:05.000000 orjson-3.9.8/src/util.rs
--rw-r--r--   0     1001      127        0 2023-10-10 14:53:05.000000 orjson-3.9.8/test/__init__.py
--rw-r--r--   0     1001      127      501 2023-10-10 14:53:05.000000 orjson-3.9.8/test/requirements.txt
--rw-r--r--   0     1001      127     6205 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_api.py
--rw-r--r--   0     1001      127     1319 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_append_newline.py
--rw-r--r--   0     1001      127      680 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_canonical.py
--rw-r--r--   0     1001      127     2097 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_circular.py
--rw-r--r--   0     1001      127     7288 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_dataclass.py
--rw-r--r--   0     1001      127    22713 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_datetime.py
--rw-r--r--   0     1001      127     9050 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_default.py
--rw-r--r--   0     1001      127     1926 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_dict.py
--rw-r--r--   0     1001      127     2630 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_enum.py
--rw-r--r--   0     1001      127     5444 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_error.py
--rw-r--r--   0     1001      127     1117 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_fake.py
--rw-r--r--   0     1001      127     1492 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_fixture.py
--rw-r--r--   0     1001      127    40451 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_fragment.py
--rw-r--r--   0     1001      127     2496 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_indent.py
--rw-r--r--   0     1001      127      274 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_issue221.py
--rw-r--r--   0     1001      127    11816 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_issue331.py
--rw-r--r--   0     1001      127     6187 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_jsonchecker.py
--rw-r--r--   0     1001      127     8356 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_memory.py
--rw-r--r--   0     1001      127     9175 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_non_str_keys.py
--rw-r--r--   0     1001      127    26642 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_numpy.py
--rw-r--r--   0     1001      127    56984 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_parsing.py
--rw-r--r--   0     1001      127      210 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_reentrant.py
--rw-r--r--   0     1001      127     3994 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_roundtrip.py
--rw-r--r--   0     1001      127     1656 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_sort_keys.py
--rw-r--r--   0     1001      127     3126 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_subclass.py
--rw-r--r--   0     1001      127     3725 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_transform.py
--rw-r--r--   0     1001      127    16489 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_type.py
--rw-r--r--   0     1001      127      453 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_typeddict.py
--rw-r--r--   0     1001      127    10773 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_ujson.py
--rw-r--r--   0     1001      127     3445 2023-10-10 14:53:05.000000 orjson-3.9.8/test/test_uuid.py
--rw-r--r--   0     1001      127      948 2023-10-10 14:53:05.000000 orjson-3.9.8/test/util.py
--rw-r--r--   0     1001      127     8352 2023-10-10 14:53:05.000000 orjson-3.9.8/Cargo.lock
--rw-r--r--   0     1001      127     1568 2023-10-10 14:53:05.000000 orjson-3.9.8/pyproject.toml
--rw-r--r--   0     1001      127        0 2023-10-10 14:53:05.000000 orjson-3.9.8/pysrc/orjson/py.typed
--rw-r--r--   0     1001      127      589 2023-10-10 14:53:05.000000 orjson-3.9.8/pysrc/orjson/__init__.py
--rw-r--r--   0     1001      127      761 2023-10-10 14:53:05.000000 orjson-3.9.8/pysrc/orjson/__init__.pyi
--rw-r--r--   0     1001      127      108 2023-10-10 14:57:07.000000 orjson-3.9.8/.cargo/config.toml
--rw-r--r--   0     1001      127     2061 2023-10-10 14:53:05.000000 orjson-3.9.8/build.rs
--rw-r--r--   0     1001      127     1772 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/.cargo-checksum.json
--rw-r--r--   0     1001      127     2849 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/Cargo.toml
--rw-r--r--   0     1001      127     9236 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/FAQ.md
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/LICENSE-APACHE
--rw-r--r--   0     1001      127     1057 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/LICENSE-MIT
--rw-r--r--   0     1001      127     5683 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/README.md
--rw-r--r--   0     1001      127      823 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/build.rs
--rw-r--r--   0     1001      127       16 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/rustfmt.toml
--rw-r--r--   0     1001      127    13200 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/aes_hash.rs
--rw-r--r--   0     1001      127     4503 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/convert.rs
--rw-r--r--   0     1001      127    12167 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/fallback_hash.rs
--rw-r--r--   0     1001      127    14078 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/hash_map.rs
--rw-r--r--   0     1001      127    16962 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/hash_quality_test.rs
--rw-r--r--   0     1001      127     9372 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/hash_set.rs
--rw-r--r--   0     1001      127    12338 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/lib.rs
--rw-r--r--   0     1001      127    12446 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/operations.rs
--rw-r--r--   0     1001      127    18456 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/random_state.rs
--rw-r--r--   0     1001      127     7158 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/src/specialize.rs
--rw-r--r--   0     1001      127     5968 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/tests/bench.rs
--rw-r--r--   0     1001      127    11469 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/tests/map_tests.rs
--rw-r--r--   0     1001      127     2107 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ahash-0.8.3/tests/nopanic.rs
--rw-r--r--   0     1001      127     1431 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/.cargo-checksum.json
--rw-r--r--   0     1001      127     9959 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/CHANGELOG.md
--rw-r--r--   0     1001      127     1644 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/LICENSE-APACHE
--rw-r--r--   0     1001      127     1071 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/LICENSE-MIT
--rw-r--r--   0     1001      127      958 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/README.md
--rw-r--r--   0     1001      127     1963 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/benches/arraystring.rs
--rw-r--r--   0     1001      127     1739 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/benches/extend.rs
--rw-r--r--   0     1001      127    19612 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/array_string.rs
--rw-r--r--   0     1001      127    38497 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/arrayvec.rs
--rw-r--r--   0     1001      127     2339 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/arrayvec_impl.rs
--rw-r--r--   0     1001      127     3315 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/char.rs
--rw-r--r--   0     1001      127     1193 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/errors.rs
--rw-r--r--   0     1001      127     1640 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/lib.rs
--rw-r--r--   0     1001      127      325 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/utils.rs
--rw-r--r--   0     1001      127     1809 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/tests/serde.rs
--rw-r--r--   0     1001      127    19485 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/arrayvec-0.7.4/tests/tests.rs
--rw-r--r--   0     1001      127      839 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/.cargo-checksum.json
--rw-r--r--   0     1001      127     1196 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/Cargo.toml
--rw-r--r--   0     1001      127     1896 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/README.md
--rw-r--r--   0     1001      127     1310 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/capacity.rs
--rw-r--r--   0     1001      127     5655 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/entry.rs
--rw-r--r--   0     1001      127     6633 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/indices.rs
--rw-r--r--   0     1001      127     3853 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/iter.rs
--rwxr-xr-x   0     1001      127    34057 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/lib.rs
--rw-r--r--   0     1001      127     8018 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/replacement/lru.rs
--rw-r--r--   0     1001      127     2592 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/replacement.rs
--rw-r--r--   0     1001      127     1263 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/.cargo-checksum.json
--rw-r--r--   0     1001      127      151 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/Cargo.lock
--rw-r--r--   0     1001      127      861 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1054 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/LICENSE-MIT
--rw-r--r--   0     1001      127     2946 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/README.md
--rw-r--r--   0     1001      127      235 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/examples/integers.rs
--rw-r--r--   0     1001      127      672 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/examples/paths.rs
--rw-r--r--   0     1001      127      826 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/examples/traits.rs
--rw-r--r--   0     1001      127      223 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/examples/versions.rs
--rw-r--r--   0     1001      127     1414 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/src/error.rs
--rw-r--r--   0     1001      127    14815 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/src/lib.rs
--rw-r--r--   0     1001      127     5038 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/src/tests.rs
--rw-r--r--   0     1001      127     2092 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/src/version.rs
--rw-r--r--   0     1001      127     1184 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/autocfg-1.1.0/tests/rustflags.rs
--rw-r--r--   0     1001      127     1069 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/.cargo-checksum.json
--rw-r--r--   0     1001      127     1237 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/Cargo.toml
--rw-r--r--   0     1001      127    10856 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/LICENSE-APACHE
--rw-r--r--   0     1001      127     1100 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/LICENSE-MIT
--rw-r--r--   0     1001      127     4394 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/README.md
--rw-r--r--   0     1001      127     4552 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/benches/bench.rs
--rwxr-xr-x   0     1001      127      363 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/ci/miri.sh
--rw-r--r--   0     1001      127    13270 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/src/generic.rs
--rw-r--r--   0     1001      127     1670 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/src/lean.rs
--rw-r--r--   0     1001      127     7781 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/src/lib.rs
--rw-r--r--   0     1001      127     3434 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/src/serde.rs
--rw-r--r--   0     1001      127     5532 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/src/traits.rs
--rw-r--r--   0     1001      127     1027 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/beef-0.5.2/src/wide.rs
--rw-r--r--   0     1001      127     1357 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/.cargo-checksum.json
--rw-r--r--   0     1001      127     1412 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/Cargo.toml
--rw-r--r--   0     1001      127    11357 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/LICENSE.Apache2
--rw-r--r--   0     1001      127     1068 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/LICENSE.MIT
--rw-r--r--   0     1001      127     2866 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/README.md
--rw-r--r--   0     1001      127     3054 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/benches/bench.rs
--rw-r--r--   0     1001      127      369 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/ci/miri.sh
--rw-r--r--   0     1001      127     3619 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/src/integer_simd.rs
--rw-r--r--   0     1001      127     4785 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/src/lib.rs
--rw-r--r--   0     1001      127     1351 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/src/naive.rs
--rw-r--r--   0     1001      127     4757 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/aarch64.rs
--rw-r--r--   0     1001      127     4512 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/generic.rs
--rw-r--r--   0     1001      127      657 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/mod.rs
--rw-r--r--   0     1001      127     4597 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/x86_avx2.rs
--rw-r--r--   0     1001      127     4607 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/x86_sse2.rs
--rw-r--r--   0     1001      127     2415 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/bytecount-0.6.4/tests/check.rs
--rw-r--r--   0     1001      127      661 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/castaway-0.2.2/.cargo-checksum.json
--rw-r--r--   0     1001      127     1028 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/castaway-0.2.2/Cargo.toml
--rw-r--r--   0     1001      127     1075 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/castaway-0.2.2/LICENSE
--rw-r--r--   0     1001      127     3446 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/castaway-0.2.2/README.md
--rw-r--r--   0     1001      127     7141 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/castaway-0.2.2/src/internal.rs
--rw-r--r--   0     1001      127    17016 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/castaway-0.2.2/src/lib.rs
--rw-r--r--   0     1001      127     3494 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/castaway-0.2.2/src/lifetime_free.rs
--rw-r--r--   0     1001      127     3782 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/castaway-0.2.2/src/utils.rs
--rw-r--r--   0     1001      127     1963 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/.cargo-checksum.json
--rw-r--r--   0     1001      127     2886 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/Cargo.lock
--rw-r--r--   0     1001      127     1283 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/LICENSE-APACHE
--rw-r--r--   0     1001      127     1057 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/LICENSE-MIT
--rw-r--r--   0     1001      127     8224 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/README.md
--rw-r--r--   0     1001      127     1921 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/bin/gcc-shim.rs
--rw-r--r--   0     1001      127     3917 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/com.rs
--rw-r--r--   0     1001      127   153381 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/lib.rs
--rw-r--r--   0     1001      127     3087 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/os_pipe/unix.rs
--rw-r--r--   0     1001      127      783 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/os_pipe/windows.rs
--rw-r--r--   0     1001      127      971 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/os_pipe.rs
--rw-r--r--   0     1001      127     6402 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/registry.rs
--rw-r--r--   0     1001      127     8886 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/setup_config.rs
--rw-r--r--   0     1001      127     6483 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/vs_instances.rs
--rw-r--r--   0     1001      127     4539 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/winapi.rs
--rw-r--r--   0     1001      127    34449 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/windows_registry.rs
--rw-r--r--   0     1001      127     5154 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/src/windows_sys.rs
--rw-r--r--   0     1001      127     2739 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/tests/cc_env.rs
--rw-r--r--   0     1001      127      415 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/tests/cflags.rs
--rw-r--r--   0     1001      127      431 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/tests/cxxflags.rs
--rw-r--r--   0     1001      127     5205 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/tests/support/mod.rs
--rw-r--r--   0     1001      127    10318 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cc-1.0.83/tests/test.rs
--rw-r--r--   0     1001      127      577 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cfg-if-1.0.0/.cargo-checksum.json
--rw-r--r--   0     1001      127     1308 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cfg-if-1.0.0/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cfg-if-1.0.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1057 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cfg-if-1.0.0/LICENSE-MIT
--rw-r--r--   0     1001      127     1123 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cfg-if-1.0.0/README.md
--rw-r--r--   0     1001      127     4893 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cfg-if-1.0.0/src/lib.rs
--rw-r--r--   0     1001      127      245 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/cfg-if-1.0.0/tests/xcrate.rs
--rw-r--r--   0     1001      127     4953 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/.cargo-checksum.json
--rw-r--r--   0     1001      127    23977 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/CHANGELOG.md
--rw-r--r--   0     1001      127      768 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/CITATION.cff
--rw-r--r--   0     1001      127     2874 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/Cargo.toml
--rw-r--r--   0     1001      127    12307 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/LICENSE.txt
--rw-r--r--   0     1001      127     3846 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/README.md
--rw-r--r--   0     1001      127      203 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/appveyor.yml
--rw-r--r--   0     1001      127      354 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/deny.toml
--rw-r--r--   0     1001      127       29 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/rustfmt.toml
--rw-r--r--   0     1001      127    22157 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/date.rs
--rw-r--r--   0     1001      127    58971 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/datetime/mod.rs
--rw-r--r--   0     1001      127     3826 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/datetime/rustc_serialize.rs
--rw-r--r--   0     1001      127    40754 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/datetime/serde.rs
--rw-r--r--   0     1001      127    56886 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/datetime/tests.rs
--rw-r--r--   0     1001      127    29113 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/duration.rs
--rw-r--r--   0     1001      127    40713 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/formatting.rs
--rw-r--r--   0     1001      127     2994 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/locales.rs
--rw-r--r--   0     1001      127    20158 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/mod.rs
--rw-r--r--   0     1001      127    96229 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/parse.rs
--rw-r--r--   0     1001      127    58073 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/parsed.rs
--rw-r--r--   0     1001      127    14584 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/scan.rs
--rw-r--r--   0     1001      127    45514 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/strftime.rs
--rw-r--r--   0     1001      127    29231 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/lib.rs
--rw-r--r--   0     1001      127    12973 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/month.rs
--rw-r--r--   0     1001      127   122213 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/date.rs
--rw-r--r--   0     1001      127    80792 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/datetime/mod.rs
--rw-r--r--   0     1001      127     1940 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/datetime/rustc_serialize.rs
--rw-r--r--   0     1001      127    38392 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/datetime/serde.rs
--rw-r--r--   0     1001      127    18291 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/datetime/tests.rs
--rw-r--r--   0     1001      127    36370 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/internals.rs
--rw-r--r--   0     1001      127     7118 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/isoweek.rs
--rw-r--r--   0     1001      127     1324 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/mod.rs
--rw-r--r--   0     1001      127    61287 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/time/mod.rs
--rw-r--r--   0     1001      127      780 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/time/rustc_serialize.rs
--rw-r--r--   0     1001      127     1854 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/time/serde.rs
--rw-r--r--   0     1001      127    13167 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/time/tests.rs
--rw-r--r--   0     1001      127     9661 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/fixed.rs
--rw-r--r--   0     1001      127     8606 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/mod.rs
--rw-r--r--   0     1001      127     3499 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/tz_info/mod.rs
--rw-r--r--   0     1001      127    11352 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/tz_info/parser.rs
--rw-r--r--   0     1001      127    39593 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/tz_info/rule.rs
--rw-r--r--   0     1001      127    36987 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/tz_info/timezone.rs
--rw-r--r--   0     1001      127     6416 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/unix.rs
--rw-r--r--   0     1001      127     1741 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/win_bindings.rs
--rw-r--r--   0     1001      127      244 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/win_bindings.txt
--rw-r--r--   0     1001      127     5229 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/windows.rs
--rw-r--r--   0     1001      127    24070 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/mod.rs
--rw-r--r--   0     1001      127     4314 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/utc.rs
--rw-r--r--   0     1001      127    26668 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/round.rs
--rw-r--r--   0     1001      127    15140 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/traits.rs
--rw-r--r--   0     1001      127    12970 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/src/weekday.rs
--rw-r--r--   0     1001      127       83 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/taplo.toml
--rw-r--r--   0     1001      127     6102 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/tests/dateutils.rs
--rw-r--r--   0     1001      127     2795 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/tests/wasm.rs
--rw-r--r--   0     1001      127      746 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/chrono-0.4.31/tests/win_bindings.rs
--rw-r--r--   0     1001      127     2357 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/.cargo-checksum.json
--rw-r--r--   0     1001      127     2567 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/Cargo.toml
--rw-r--r--   0     1001      127     1073 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/LICENSE
--rw-r--r--   0     1001      127    11977 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/README.md
--rw-r--r--   0     1001      127     1445 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/arbitrary.rs
--rw-r--r--   0     1001      127     4030 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/bytes.rs
--rw-r--r--   0     1001      127      884 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/markup.rs
--rw-r--r--   0     1001      127      425 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/mod.rs
--rw-r--r--   0     1001      127     1512 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/proptest.rs
--rw-r--r--   0     1001      127     1491 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/quickcheck.rs
--rw-r--r--   0     1001      127     3769 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/rkyv.rs
--rw-r--r--   0     1001      127     5217 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/serde.rs
--rw-r--r--   0     1001      127     2702 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/smallvec.rs
--rw-r--r--   0     1001      127    61364 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/lib.rs
--rw-r--r--   0     1001      127     1550 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/macros.rs
--rw-r--r--   0     1001      127     6353 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/bytes.rs
--rw-r--r--   0     1001      127     6390 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/capacity.rs
--rw-r--r--   0     1001      127    19999 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/heap.rs
--rw-r--r--   0     1001      127     6616 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/inline.rs
--rw-r--r--   0     1001      127     6797 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/iter.rs
--rw-r--r--   0     1001      127    35548 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/mod.rs
--rw-r--r--   0     1001      127     4433 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/nonmax.rs
--rw-r--r--   0     1001      127    16237 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/num.rs
--rw-r--r--   0     1001      127     1334 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/smallvec.rs
--rw-r--r--   0     1001      127     3958 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/traits.rs
--rw-r--r--   0     1001      127    44008 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/tests.rs
--rw-r--r--   0     1001      127    14163 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/compact_str-0.7.1/src/traits.rs
--rw-r--r--   0     1001      127     8900 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/.cargo-checksum.json
--rw-r--r--   0     1001      127     1956 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/CONTRIBUTING.md
--rw-r--r--   0     1001      127      713 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/COPYRIGHT
--rw-r--r--   0     1001      127     1915 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/Cargo.toml
--rw-r--r--   0     1001      127     4979 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/Ideas.md
--rw-r--r--   0     1001      127    11358 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/LICENSE-APACHE
--rw-r--r--   0     1001      127     1053 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/LICENSE-MIT
--rw-r--r--   0     1001      127     1501 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/LICENSE-WHATWG
--rw-r--r--   0     1001      127    31179 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/README.md
--rw-r--r--   0     1001      127      502 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/ci/miri.sh
--rw-r--r--   0     1001      127      869 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/Big5.txt
--rw-r--r--   0     1001      127      650 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/EUC-JP.txt
--rw-r--r--   0     1001      127      631 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/EUC-KR.txt
--rw-r--r--   0     1001      127      967 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/GBK.txt
--rw-r--r--   0     1001      127      412 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/IBM866.txt
--rw-r--r--   0     1001      127      557 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-2022-JP.txt
--rw-r--r--   0     1001      127      400 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-10.txt
--rw-r--r--   0     1001      127      427 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-13.txt
--rw-r--r--   0     1001      127      400 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-14.txt
--rw-r--r--   0     1001      127      359 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-15.txt
--rw-r--r--   0     1001      127      417 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-16.txt
--rw-r--r--   0     1001      127      345 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-2.txt
--rw-r--r--   0     1001      127      343 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-3.txt
--rw-r--r--   0     1001      127      343 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-4.txt
--rw-r--r--   0     1001      127      297 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-5.txt
--rw-r--r--   0     1001      127      381 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-6.txt
--rw-r--r--   0     1001      127      695 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-7.txt
--rw-r--r--   0     1001      127      513 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-8-I.txt
--rw-r--r--   0     1001      127      512 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-8.txt
--rw-r--r--   0     1001      127      312 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/KOI8-R.txt
--rw-r--r--   0     1001      127      281 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/KOI8-U.txt
--rw-r--r--   0     1001      127      475 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/Shift_JIS.txt
--rw-r--r--   0     1001      127      400 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/UTF-16BE.txt
--rw-r--r--   0     1001      127      403 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/UTF-16LE.txt
--rw-r--r--   0     1001      127      261 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/UTF-8.txt
--rw-r--r--   0     1001      127      524 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/gb18030.txt
--rw-r--r--   0     1001      127      380 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/macintosh.txt
--rw-r--r--   0     1001      127      499 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/replacement.txt
--rw-r--r--   0     1001      127      288 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1250.txt
--rw-r--r--   0     1001      127      280 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1251.txt
--rw-r--r--   0     1001      127      344 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1252.txt
--rw-r--r--   0     1001      127      450 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1253.txt
--rw-r--r--   0     1001      127      344 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1254.txt
--rw-r--r--   0     1001      127      437 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1255.txt
--rw-r--r--   0     1001      127      278 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1256.txt
--rw-r--r--   0     1001      127      364 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1257.txt
--rw-r--r--   0     1001      127      666 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1258.txt
--rw-r--r--   0     1001      127      404 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-874.txt
--rw-r--r--   0     1001      127      297 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/x-mac-cyrillic.txt
--rw-r--r--   0     1001      127      332 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/x-user-defined.txt
--rw-r--r--   0     1001      127    61842 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/generate-encoding-data.py
--rw-r--r--   0     1001      127       31 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/rustfmt.toml
--rw-r--r--   0     1001      127    69771 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/ascii.rs
--rw-r--r--   0     1001      127    15340 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/big5.rs
--rw-r--r--   0     1001      127  2574354 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/data.rs
--rw-r--r--   0     1001      127    17647 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/euc_jp.rs
--rw-r--r--   0     1001      127    17433 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/euc_kr.rs
--rw-r--r--   0     1001      127    29634 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/gb18030.rs
--rw-r--r--   0     1001      127    67096 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/handles.rs
--rw-r--r--   0     1001      127    45706 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/iso_2022_jp.rs
--rw-r--r--   0     1001      127   247846 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/lib.rs
--rw-r--r--   0     1001      127    74150 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/macros.rs
--rw-r--r--   0     1001      127   130328 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/mem.rs
--rw-r--r--   0     1001      127     3175 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/replacement.rs
--rw-r--r--   0     1001      127    17079 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/shift_jis.rs
--rw-r--r--   0     1001      127    13578 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/simd_funcs.rs
--rw-r--r--   0     1001      127    32312 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/single_byte.rs
--rw-r--r--   0     1001      127    59587 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/big5_in.txt
--rw-r--r--   0     1001      127    81302 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/big5_in_ref.txt
--rw-r--r--   0     1001      127    58777 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/big5_out.txt
--rw-r--r--   0     1001      127    44029 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/big5_out_ref.txt
--rw-r--r--   0     1001      127    72061 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_in.txt
--rw-r--r--   0     1001      127   100162 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_in_ref.txt
--rw-r--r--   0     1001      127    68262 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_out.txt
--rw-r--r--   0     1001      127    51385 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_out_ref.txt
--rw-r--r--   0     1001      127    72061 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_in.txt
--rw-r--r--   0     1001      127    95843 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_in_ref.txt
--rw-r--r--   0     1001      127    95839 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_out.txt
--rw-r--r--   0     1001      127    72058 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_out_ref.txt
--rw-r--r--   0     1001      127    79765 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_in.txt
--rw-r--r--   0     1001      127    35463 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_in_ref.txt
--rw-r--r--   0     1001      127    29715 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_out.txt
--rw-r--r--   0     1001      127    66832 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_out_ref.txt
--rw-r--r--   0     1001      127    26749 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_in.txt
--rw-r--r--   0     1001      127    35463 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_in_ref.txt
--rw-r--r--   0     1001      127    29463 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_out.txt
--rw-r--r--   0     1001      127    22249 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_out_ref.txt
--rw-r--r--   0     1001      127    35585 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0212_in.txt
--rw-r--r--   0     1001      127    35322 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0212_in_ref.txt
--rw-r--r--   0     1001      127    34081 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_in.txt
--rw-r--r--   0     1001      127    45731 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_in_ref.txt
--rw-r--r--   0     1001      127    29519 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_out.txt
--rw-r--r--   0     1001      127    22291 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_out_ref.txt
--rw-r--r--   0     1001      127    15992 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_labels_names.rs
--rw-r--r--   0     1001      127     8321 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/testing.rs
--rw-r--r--   0     1001      127    18725 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/utf_16.rs
--rw-r--r--   0     1001      127    63069 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/utf_8.rs
--rw-r--r--   0     1001      127    17213 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/variant.rs
--rw-r--r--   0     1001      127     7516 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/x_user_defined.rs
--rw-r--r--   0     1001      127      745 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoa-1.0.9/.cargo-checksum.json
--rw-r--r--   0     1001      127     1155 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoa-1.0.9/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoa-1.0.9/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoa-1.0.9/LICENSE-MIT
--rw-r--r--   0     1001      127     2025 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoa-1.0.9/README.md
--rw-r--r--   0     1001      127     1344 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoa-1.0.9/benches/bench.rs
--rw-r--r--   0     1001      127    10597 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoa-1.0.9/src/lib.rs
--rw-r--r--   0     1001      127     1480 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoa-1.0.9/src/udiv128.rs
--rw-r--r--   0     1001      127      842 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoa-1.0.9/tests/test.rs
--rw-r--r--   0     1001      127      981 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/.cargo-checksum.json
--rw-r--r--   0     1001      127     1226 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/Cargo.toml
--rw-r--r--   0     1001      127     1122 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/LICENSE
--rw-r--r--   0     1001      127     2616 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/README.md
--rw-r--r--   0     1001      127    77666 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/bench.png
--rw-r--r--   0     1001      127     2710 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/benches/bench.rs
--rw-r--r--   0     1001      127      245 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/codecov.yml
--rw-r--r--   0     1001      127      128 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/rustfmt.toml
--rw-r--r--   0     1001      127     7375 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/src/common.rs
--rw-r--r--   0     1001      127     1619 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/src/fallback.rs
--rw-r--r--   0     1001      127    12645 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/src/lib.rs
--rw-r--r--   0     1001      127     4385 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/itoap-1.0.1/src/sse2.rs
--rw-r--r--   0     1001      127    25249 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/.cargo-checksum.json
--rw-r--r--   0     1001      127     4446 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/CONTRIBUTING.md
--rw-r--r--   0     1001      127     4788 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/LICENSE-APACHE
--rw-r--r--   0     1001      127     1076 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/LICENSE-MIT
--rw-r--r--   0     1001      127     4134 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/README.md
--rw-r--r--   0     1001      127     8994 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/build.rs
--rw-r--r--   0     1001      127       30 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/rustfmt.toml
--rw-r--r--   0     1001      127     4884 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/fixed_width_ints.rs
--rw-r--r--   0     1001      127     1952 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/aarch64.rs
--rw-r--r--   0     1001      127     5480 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/align.rs
--rw-r--r--   0     1001      127   151602 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/mod.rs
--rw-r--r--   0     1001      127     5036 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/no_align.rs
--rw-r--r--   0     1001      127     1169 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/riscv64.rs
--rw-r--r--   0     1001      127     4550 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/x86_64.rs
--rw-r--r--   0     1001      127       46 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/hermit/aarch64.rs
--rw-r--r--   0     1001      127     1480 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/hermit/mod.rs
--rw-r--r--   0     1001      127       46 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/hermit/x86_64.rs
--rw-r--r--   0     1001      127     4751 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/lib.rs
--rw-r--r--   0     1001      127    10703 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/macros.rs
--rw-r--r--   0     1001      127   126764 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/psp.rs
--rw-r--r--   0     1001      127     1217 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/sgx.rs
--rw-r--r--   0     1001      127       93 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/solid/aarch64.rs
--rw-r--r--   0     1001      127       93 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/solid/arm.rs
--rw-r--r--   0     1001      127    33199 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/solid/mod.rs
--rw-r--r--   0     1001      127     1266 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/switch.rs
--rw-r--r--   0     1001      127    30167 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/teeos/mod.rs
--rw-r--r--   0     1001      127   118783 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/aix/mod.rs
--rw-r--r--   0     1001      127    22868 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/aix/powerpc64.rs
--rw-r--r--   0     1001      127       92 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/align.rs
--rw-r--r--   0     1001      127      149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b32/align.rs
--rw-r--r--   0     1001      127     3327 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b32/mod.rs
--rw-r--r--   0     1001      127     1478 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/aarch64/align.rs
--rw-r--r--   0     1001      127      255 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/aarch64/mod.rs
--rw-r--r--   0     1001      127      149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/align.rs
--rw-r--r--   0     1001      127     3434 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/mod.rs
--rw-r--r--   0     1001      127      149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/x86_64/align.rs
--rw-r--r--   0     1001      127     5717 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/x86_64/mod.rs
--rw-r--r--   0     1001      127      151 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/long_array.rs
--rw-r--r--   0     1001      127   228985 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/mod.rs
--rw-r--r--   0     1001      127      377 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/dragonfly/errno.rs
--rw-r--r--   0     1001      127    59079 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/dragonfly/mod.rs
--rw-r--r--   0     1001      127     4973 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/aarch64.rs
--rw-r--r--   0     1001      127     1420 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/arm.rs
--rw-r--r--   0     1001      127      811 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd11/b64.rs
--rw-r--r--   0     1001      127    17516 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd11/mod.rs
--rw-r--r--   0     1001      127      860 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/b64.rs
--rw-r--r--   0     1001      127    17656 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/mod.rs
--rw-r--r--   0     1001      127      287 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/x86_64.rs
--rw-r--r--   0     1001      127      860 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/b64.rs
--rw-r--r--   0     1001      127    18823 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/mod.rs
--rw-r--r--   0     1001      127      287 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/x86_64.rs
--rw-r--r--   0     1001      127      860 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/b64.rs
--rw-r--r--   0     1001      127    18823 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/mod.rs
--rw-r--r--   0     1001      127      666 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/x86_64.rs
--rw-r--r--   0     1001      127   196144 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/mod.rs
--rw-r--r--   0     1001      127     1272 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/powerpc.rs
--rw-r--r--   0     1001      127     1273 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/powerpc64.rs
--rw-r--r--   0     1001      127     5469 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/riscv64.rs
--rw-r--r--   0     1001      127     7585 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86.rs
--rw-r--r--   0     1001      127     7805 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86_64/align.rs
--rw-r--r--   0     1001      127    10953 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86_64/mod.rs
--rw-r--r--   0     1001      127    63043 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/mod.rs
--rw-r--r--   0     1001      127    29933 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/mod.rs
--rw-r--r--   0     1001      127    25504 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/mod.rs
--rw-r--r--   0     1001      127     2950 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/aarch64.rs
--rw-r--r--   0     1001      127      628 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/arm.rs
--rw-r--r--   0     1001      127   106675 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/mod.rs
--rw-r--r--   0     1001      127      569 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/powerpc.rs
--rw-r--r--   0     1001      127      221 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/sparc64.rs
--rw-r--r--   0     1001      127      401 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/x86.rs
--rw-r--r--   0     1001      127     1076 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/x86_64.rs
--rw-r--r--   0     1001      127      722 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/aarch64.rs
--rw-r--r--   0     1001      127      397 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/arm.rs
--rw-r--r--   0     1001      127      157 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/mips64.rs
--rw-r--r--   0     1001      127    67743 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/mod.rs
--rw-r--r--   0     1001      127      397 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/powerpc.rs
--rw-r--r--   0     1001      127      395 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/powerpc64.rs
--rw-r--r--   0     1001      127      395 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/riscv64.rs
--rw-r--r--   0     1001      127      159 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/sparc64.rs
--rw-r--r--   0     1001      127      394 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/x86.rs
--rw-r--r--   0     1001      127     4403 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/x86_64.rs
--rw-r--r--   0     1001      127      495 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/haiku/b32.rs
--rw-r--r--   0     1001      127      498 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/haiku/b64.rs
--rw-r--r--   0     1001      127    69317 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/haiku/mod.rs
--rw-r--r--   0     1001      127    50141 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/haiku/native.rs
--rw-r--r--   0     1001      127     9816 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/haiku/x86_64.rs
--rw-r--r--   0     1001      127       20 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/hurd/align.rs
--rw-r--r--   0     1001      127     2557 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/hurd/b32.rs
--rw-r--r--   0     1001      127     2582 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/hurd/b64.rs
--rw-r--r--   0     1001      127   106355 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/hurd/mod.rs
--rw-r--r--   0     1001      127       20 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/hurd/no_align.rs
--rw-r--r--   0     1001      127    22019 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/arm.rs
--rw-r--r--   0     1001      127     6584 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/mod.rs
--rw-r--r--   0     1001      127      148 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/x86/align.rs
--rw-r--r--   0     1001      127    24209 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/x86/mod.rs
--rw-r--r--   0     1001      127      756 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/align.rs
--rw-r--r--   0     1001      127      142 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/int128.rs
--rw-r--r--   0     1001      127    16376 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/mod.rs
--rw-r--r--   0     1001      127    10479 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/mod.rs
--rw-r--r--   0     1001      127      149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/riscv64/align.rs
--rw-r--r--   0     1001      127    13474 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/riscv64/mod.rs
--rw-r--r--   0     1001      127      149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/x86_64/align.rs
--rw-r--r--   0     1001      127    28839 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/x86_64/mod.rs
--rw-r--r--   0     1001      127   131658 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/mod.rs
--rw-r--r--   0     1001      127     2376 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/align.rs
--rw-r--r--   0     1001      127     5193 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/lfs64.rs
--rw-r--r--   0     1001      127    59263 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/mod.rs
--rw-r--r--   0     1001      127     2066 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/no_align.rs
--rw-r--r--   0     1001      127     8872 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/align.rs
--rw-r--r--   0     1001      127    11583 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/generic/mod.rs
--rw-r--r--   0     1001      127    11454 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/mips/mod.rs
--rw-r--r--   0     1001      127      567 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/mod.rs
--rw-r--r--   0     1001      127    10012 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/powerpc/mod.rs
--rw-r--r--   0     1001      127     9375 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/sparc/mod.rs
--rw-r--r--   0     1001      127      378 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/align.rs
--rw-r--r--   0     1001      127     1805 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/arm/align.rs
--rw-r--r--   0     1001      127    31048 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/arm/mod.rs
--rw-r--r--   0     1001      127      148 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/csky/align.rs
--rw-r--r--   0     1001      127    26449 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/csky/mod.rs
--rw-r--r--   0     1001      127      148 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/m68k/align.rs
--rw-r--r--   0     1001      127    31243 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/m68k/mod.rs
--rw-r--r--   0     1001      127      148 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mips/align.rs
--rw-r--r--   0     1001      127    31942 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mips/mod.rs
--rw-r--r--   0     1001      127    11752 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mod.rs
--rw-r--r--   0     1001      127    29822 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/powerpc.rs
--rw-r--r--   0     1001      127     1213 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/riscv32/align.rs
--rw-r--r--   0     1001      127    28172 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/riscv32/mod.rs
--rw-r--r--   0     1001      127      148 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/sparc/align.rs
--rw-r--r--   0     1001      127    30083 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/sparc/mod.rs
--rw-r--r--   0     1001      127      149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/x86/align.rs
--rw-r--r--   0     1001      127    38841 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/x86/mod.rs
--rw-r--r--   0     1001      127     1516 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/align.rs
--rw-r--r--   0     1001      127      163 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/fallback.rs
--rw-r--r--   0     1001      127     2294 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/ilp32.rs
--rw-r--r--   0     1001      127      142 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/int128.rs
--rw-r--r--   0     1001      127     2798 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/lp64.rs
--rw-r--r--   0     1001      127    32357 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/mod.rs
--rw-r--r--   0     1001      127     1037 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/loongarch64/align.rs
--rw-r--r--   0     1001      127    31949 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/loongarch64/mod.rs
--rw-r--r--   0     1001      127      149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mips64/align.rs
--rw-r--r--   0     1001      127    35131 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mips64/mod.rs
--rw-r--r--   0     1001      127     3772 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mod.rs
--rw-r--r--   0     1001      127      149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/powerpc64/align.rs
--rw-r--r--   0     1001      127    34180 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/powerpc64/mod.rs
--rw-r--r--   0     1001      127     1213 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/riscv64/align.rs
--rw-r--r--   0     1001      127    29650 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/riscv64/mod.rs
--rw-r--r--   0     1001      127    33048 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/s390x.rs
--rw-r--r--   0     1001      127      149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/sparc64/align.rs
--rw-r--r--   0     1001      127    32202 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/sparc64/mod.rs
--rw-r--r--   0     1001      127      615 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/align.rs
--rw-r--r--   0     1001      127    26263 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/mod.rs
--rw-r--r--   0     1001      127    17621 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/not_x32.rs
--rw-r--r--   0     1001      127    22804 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/x32.rs
--rw-r--r--   0     1001      127    49833 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/mod.rs
--rw-r--r--   0     1001      127      258 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/no_align.rs
--rw-r--r--   0     1001      127   169363 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/mod.rs
--rw-r--r--   0     1001      127      150 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/arm/align.rs
--rw-r--r--   0     1001      127    30616 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/arm/mod.rs
--rw-r--r--   0     1001      127    24091 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/hexagon.rs
--rw-r--r--   0     1001      127      148 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mips/align.rs
--rw-r--r--   0     1001      127    31187 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mips/mod.rs
--rw-r--r--   0     1001      127     1627 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mod.rs
--rw-r--r--   0     1001      127    29188 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/powerpc.rs
--rw-r--r--   0     1001      127      150 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/riscv32/align.rs
--rw-r--r--   0     1001      127    28063 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/riscv32/mod.rs
--rw-r--r--   0     1001      127      148 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/x86/align.rs
--rw-r--r--   0     1001      127    31972 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/x86/mod.rs
--rw-r--r--   0     1001      127     1080 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/align.rs
--rw-r--r--   0     1001      127      142 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/int128.rs
--rw-r--r--   0     1001      127    24219 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/mod.rs
--rw-r--r--   0     1001      127    27809 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/mips64.rs
--rw-r--r--   0     1001      127     4425 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/mod.rs
--rw-r--r--   0     1001      127    26015 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/powerpc64.rs
--rw-r--r--   0     1001      127     1213 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/riscv64/align.rs
--rw-r--r--   0     1001      127    25593 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/riscv64/mod.rs
--rw-r--r--   0     1001      127    26240 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/s390x.rs
--rw-r--r--   0     1001      127      616 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/x86_64/align.rs
--rw-r--r--   0     1001      127    32792 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/x86_64/mod.rs
--rw-r--r--   0     1001      127     5732 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/lfs64.rs
--rw-r--r--   0     1001      127    26755 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/mod.rs
--rw-r--r--   0     1001      127     6370 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/no_align.rs
--rw-r--r--   0     1001      127      169 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/non_exhaustive.rs
--rw-r--r--   0     1001      127     1074 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/align.rs
--rw-r--r--   0     1001      127      378 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/arm/align.rs
--rw-r--r--   0     1001      127    32707 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/arm/mod.rs
--rw-r--r--   0     1001      127      258 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/arm/no_align.rs
--rw-r--r--   0     1001      127      378 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips32/align.rs
--rw-r--r--   0     1001      127    26773 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips32/mod.rs
--rw-r--r--   0     1001      127      258 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips32/no_align.rs
--rw-r--r--   0     1001      127      258 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips64/align.rs
--rw-r--r--   0     1001      127     5470 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips64/mod.rs
--rw-r--r--   0     1001      127      138 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips64/no_align.rs
--rw-r--r--   0     1001      127    10293 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mod.rs
--rw-r--r--   0     1001      127    12819 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mod.rs
--rw-r--r--   0     1001      127     2037 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/no_align.rs
--rw-r--r--   0     1001      127     1857 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/l4re.rs
--rw-r--r--   0     1001      127    10398 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/mod.rs
--rw-r--r--   0     1001      127      172 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/other.rs
--rw-r--r--   0     1001      127    67338 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/mod.rs
--rw-r--r--   0     1001      127    61430 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/mod.rs
--rw-r--r--   0     1001      127     1346 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/aarch64/mod.rs
--rw-r--r--   0     1001      127     2572 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/align.rs
--rw-r--r--   0     1001      127     1380 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/arm/mod.rs
--rw-r--r--   0     1001      127     3066 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/espidf/mod.rs
--rw-r--r--   0     1001      127      830 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/generic.rs
--rw-r--r--   0     1001      127     7356 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/horizon/mod.rs
--rw-r--r--   0     1001      127    25647 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/mod.rs
--rw-r--r--   0     1001      127     2082 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/no_align.rs
--rw-r--r--   0     1001      127      353 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/powerpc/mod.rs
--rw-r--r--   0     1001      127     6573 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/vita/mod.rs
--rw-r--r--   0     1001      127       97 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/no_align.rs
--rw-r--r--   0     1001      127      730 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/nto/aarch64.rs
--rw-r--r--   0     1001      127   117100 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/nto/mod.rs
--rw-r--r--   0     1001      127    42200 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/nto/neutrino.rs
--rw-r--r--   0     1001      127     3479 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/nto/x86_64.rs
--rw-r--r--   0     1001      127    46971 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/redox/mod.rs
--rw-r--r--   0     1001      127     6492 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/compat.rs
--rw-r--r--   0     1001      127     2814 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/illumos.rs
--rw-r--r--   0     1001      127   113204 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/mod.rs
--rw-r--r--   0     1001      127     3000 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/solaris.rs
--rw-r--r--   0     1001      127      859 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/x86.rs
--rw-r--r--   0     1001      127     6023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/x86_64.rs
--rw-r--r--   0     1001      127     2717 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/x86_common.rs
--rw-r--r--   0     1001      127       93 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/vxworks/aarch64.rs
--rw-r--r--   0     1001      127       93 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/vxworks/arm.rs
--rw-r--r--   0     1001      127    62286 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/vxworks/mod.rs
--rw-r--r--   0     1001      127       93 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/vxworks/powerpc.rs
--rw-r--r--   0     1001      127       93 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/vxworks/powerpc64.rs
--rw-r--r--   0     1001      127       93 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/vxworks/x86.rs
--rw-r--r--   0     1001      127       93 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/vxworks/x86_64.rs
--rw-r--r--   0     1001      127    31119 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/wasi.rs
--rw-r--r--   0     1001      127      525 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/windows/gnu/align.rs
--rw-r--r--   0     1001      127      749 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/windows/gnu/mod.rs
--rw-r--r--   0     1001      127    22035 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/windows/mod.rs
--rw-r--r--   0     1001      127      639 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/windows/msvc/mod.rs
--rw-r--r--   0     1001      127     1264 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/src/xous.rs
--rw-r--r--   0     1001      127      220 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libc-0.2.149/tests/const_fn.rs
--rw-r--r--   0     1001      127    11291 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/.cargo-checksum.json
--rw-r--r--   0     1001      127     1609 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/CHANGELOG.md
--rw-r--r--   0     1001      127     3428 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/CONTRIBUTING.md
--rw-r--r--   0     1001      127     1073 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/LICENSE-APACHE
--rw-r--r--   0     1001      127     1058 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/LICENSE-MIT
--rw-r--r--   0     1001      127     1467 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/README.md
--rw-r--r--   0     1001      127    15767 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/build.rs
--rw-r--r--   0     1001      127     1461 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/lib.rs
--rw-r--r--   0     1001      127     8395 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/libm_helper.rs
--rw-r--r--   0     1001      127     3810 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/acos.rs
--rw-r--r--   0     1001      127     2218 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/acosf.rs
--rw-r--r--   0     1001      127      867 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/acosh.rs
--rw-r--r--   0     1001      127      823 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/acoshf.rs
--rw-r--r--   0     1001      127     4288 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/asin.rs
--rw-r--r--   0     1001      127     2054 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/asinf.rs
--rw-r--r--   0     1001      127     1162 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/asinh.rs
--rw-r--r--   0     1001      127     1133 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/asinhf.rs
--rw-r--r--   0     1001      127     5774 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atan.rs
--rw-r--r--   0     1001      127     4355 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atan2.rs
--rw-r--r--   0     1001      127     2894 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atan2f.rs
--rw-r--r--   0     1001      127     3149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atanf.rs
--rw-r--r--   0     1001      127      970 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atanh.rs
--rw-r--r--   0     1001      127      968 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atanhf.rs
--rw-r--r--   0     1001      127     4343 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cbrt.rs
--rw-r--r--   0     1001      127     2149 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cbrtf.rs
--rw-r--r--   0     1001      127     2333 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ceil.rs
--rw-r--r--   0     1001      127     1750 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ceilf.rs
--rw-r--r--   0     1001      127      403 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/copysign.rs
--rw-r--r--   0     1001      127      406 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/copysignf.rs
--rw-r--r--   0     1001      127     2255 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cos.rs
--rw-r--r--   0     1001      127     2438 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cosf.rs
--rw-r--r--   0     1001      127      993 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cosh.rs
--rw-r--r--   0     1001      127      910 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/coshf.rs
--rw-r--r--   0     1001      127    12647 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/erf.rs
--rw-r--r--   0     1001      127     7600 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/erff.rs
--rw-r--r--   0     1001      127     5099 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp.rs
--rw-r--r--   0     1001      127      754 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp10.rs
--rw-r--r--   0     1001      127      735 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp10f.rs
--rw-r--r--   0     1001      127    16436 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp2.rs
--rw-r--r--   0     1001      127     4725 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp2f.rs
--rw-r--r--   0     1001      127     3032 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/expf.rs
--rw-r--r--   0     1001      127     4321 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/expm1.rs
--rw-r--r--   0     1001      127     3951 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/expm1f.rs
--rw-r--r--   0     1001      127      568 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/expo2.rs
--rw-r--r--   0     1001      127     1189 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fabs.rs
--rw-r--r--   0     1001      127     1302 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fabsf.rs
--rw-r--r--   0     1001      127      470 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fdim.rs
--rw-r--r--   0     1001      127      471 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fdimf.rs
--rw-r--r--   0     1001      127      478 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fenv.rs
--rw-r--r--   0     1001      127     2333 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/floor.rs
--rw-r--r--   0     1001      127     1783 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/floorf.rs
--rw-r--r--   0     1001      127     6706 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fma.rs
--rw-r--r--   0     1001      127     4135 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmaf.rs
--rw-r--r--   0     1001      127      771 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmax.rs
--rw-r--r--   0     1001      127      772 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmaxf.rs
--rw-r--r--   0     1001      127      771 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmin.rs
--rw-r--r--   0     1001      127      772 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fminf.rs
--rw-r--r--   0     1001      127     1637 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmod.rs
--rw-r--r--   0     1001      127     1649 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmodf.rs
--rw-r--r--   0     1001      127      492 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/frexp.rs
--rw-r--r--   0     1001      127      485 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/frexpf.rs
--rw-r--r--   0     1001      127     1780 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/hypot.rs
--rw-r--r--   0     1001      127     1000 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/hypotf.rs
--rw-r--r--   0     1001      127      726 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ilogb.rs
--rw-r--r--   0     1001      127      716 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ilogbf.rs
--rw-r--r--   0     1001      127    15469 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/j0.rs
--rw-r--r--   0     1001      127    10448 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/j0f.rs
--rw-r--r--   0     1001      127    14881 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/j1.rs
--rw-r--r--   0     1001      127    10641 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/j1f.rs
--rw-r--r--   0     1001      127    10179 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/jn.rs
--rw-r--r--   0     1001      127     6930 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/jnf.rs
--rw-r--r--   0     1001      127     2985 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_cos.rs
--rw-r--r--   0     1001      127     1132 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_cosf.rs
--rw-r--r--   0     1001      127      566 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_expo2.rs
--rw-r--r--   0     1001      127      542 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_expo2f.rs
--rw-r--r--   0     1001      127     2470 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_sin.rs
--rw-r--r--   0     1001      127     1137 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_sinf.rs
--rw-r--r--   0     1001      127     4236 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_tan.rs
--rw-r--r--   0     1001      127     1924 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_tanf.rs
--rw-r--r--   0     1001      127      124 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ldexp.rs
--rw-r--r--   0     1001      127      126 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ldexpf.rs
--rw-r--r--   0     1001      127      133 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/lgamma.rs
--rw-r--r--   0     1001      127    12707 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/lgamma_r.rs
--rw-r--r--   0     1001      127      136 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/lgammaf.rs
--rw-r--r--   0     1001      127     8573 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/lgammaf_r.rs
--rw-r--r--   0     1001      127     4552 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log.rs
--rw-r--r--   0     1001      127     3767 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log10.rs
--rw-r--r--   0     1001      127     2561 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log10f.rs
--rw-r--r--   0     1001      127     4769 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log1p.rs
--rw-r--r--   0     1001      127     2836 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log1pf.rs
--rw-r--r--   0     1001      127     3225 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log2.rs
--rw-r--r--   0     1001      127     2378 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log2f.rs
--rw-r--r--   0     1001      127     2076 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/logf.rs
--rw-r--r--   0     1001      127     8036 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/mod.rs
--rw-r--r--   0     1001      127      730 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/modf.rs
--rw-r--r--   0     1001      127      739 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/modff.rs
--rw-r--r--   0     1001      127      886 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/nextafter.rs
--rw-r--r--   0     1001      127      920 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/nextafterf.rs
--rw-r--r--   0     1001      127    21546 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/pow.rs
--rw-r--r--   0     1001      127    10039 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/powf.rs
--rw-r--r--   0     1001      127     7501 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rem_pio2.rs
--rw-r--r--   0     1001      127    20354 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rem_pio2_large.rs
--rw-r--r--   0     1001      127     2323 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rem_pio2f.rs
--rw-r--r--   0     1001      127      158 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/remainder.rs
--rw-r--r--   0     1001      127      160 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/remainderf.rs
--rw-r--r--   0     1001      127     2462 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/remquo.rs
--rw-r--r--   0     1001      127     2159 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/remquof.rs
--rw-r--r--   0     1001      127     1776 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rint.rs
--rw-r--r--   0     1001      127     1783 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rintf.rs
--rw-r--r--   0     1001      127      635 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/round.rs
--rw-r--r--   0     1001      127      775 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/roundf.rs
--rw-r--r--   0     1001      127      964 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/scalbn.rs
--rw-r--r--   0     1001      127      807 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/scalbnf.rs
--rw-r--r--   0     1001      127     2803 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sin.rs
--rw-r--r--   0     1001      127     3569 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sincos.rs
--rw-r--r--   0     1001      127     5286 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sincosf.rs
--rw-r--r--   0     1001      127     2647 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sinf.rs
--rw-r--r--   0     1001      127     1261 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sinh.rs
--rw-r--r--   0     1001      127      693 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sinhf.rs
--rw-r--r--   0     1001      127     9295 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sqrt.rs
--rw-r--r--   0     1001      127     4842 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sqrtf.rs
--rw-r--r--   0     1001      127     2248 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tan.rs
--rw-r--r--   0     1001      127     2411 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tanf.rs
--rw-r--r--   0     1001      127     1360 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tanh.rs
--rw-r--r--   0     1001      127      902 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tanhf.rs
--rw-r--r--   0     1001      127     5518 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tgamma.rs
--rw-r--r--   0     1001      127      142 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tgammaf.rs
--rw-r--r--   0     1001      127      962 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/trunc.rs
--rw-r--r--   0     1001      127     1078 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/libm-0.2.8/src/math/truncf.rs
--rw-r--r--   0     1001      127     1037 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/.cargo-checksum.json
--rw-r--r--   0     1001      127     1348 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/LICENSE-MIT
--rw-r--r--   0     1001      127     4233 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/README.md
--rw-r--r--   0     1001      127     9498 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/src/lib.rs
--rw-r--r--   0     1001      127     2339 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/tests/compiletest/mod.rs
--rw-r--r--   0     1001      127     4891 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/tests/test.rs
--rw-r--r--   0     1001      127      100 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/tests/ui/async-fn.rs
--rw-r--r--   0     1001      127      254 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/tests/ui/async-fn.stderr
--rw-r--r--   0     1001      127      121 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/tests/ui/trait-fn.rs
--rw-r--r--   0     1001      127       96 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/no-panic-0.1.26/tests/ui/trait-fn.stderr
--rw-r--r--   0     1001      127     2261 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/.cargo-checksum.json
--rw-r--r--   0     1001      127     1294 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/LICENSE-APACHE
--rw-r--r--   0     1001      127     1071 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/LICENSE-MIT
--rw-r--r--   0     1001      127     1796 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/README.md
--rw-r--r--   0     1001      127    11754 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/RELEASES.md
--rw-r--r--   0     1001      127      799 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/build.rs
--rw-r--r--   0     1001      127     3870 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/bounds.rs
--rw-r--r--   0     1001      127    26072 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/cast.rs
--rw-r--r--   0     1001      127    64284 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/float.rs
--rw-r--r--   0     1001      127     4595 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/identities.rs
--rw-r--r--   0     1001      127    15915 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/int.rs
--rw-r--r--   0     1001      127    21755 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/lib.rs
--rw-r--r--   0     1001      127     1397 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/macros.rs
--rw-r--r--   0     1001      127    11368 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/bytes.rs
--rw-r--r--   0     1001      127    10040 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/checked.rs
--rw-r--r--   0     1001      127    10278 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/euclid.rs
--rw-r--r--   0     1001      127      931 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/inv.rs
--rw-r--r--   0     1001      127      137 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/mod.rs
--rw-r--r--   0     1001      127     3983 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/mul_add.rs
--rw-r--r--   0     1001      127     4283 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/overflowing.rs
--rw-r--r--   0     1001      127     5103 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/saturating.rs
--rw-r--r--   0     1001      127    11260 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/wrapping.rs
--rw-r--r--   0     1001      127     6574 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/pow.rs
--rw-r--r--   0     1001      127    22158 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/real.rs
--rw-r--r--   0     1001      127     5877 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/src/sign.rs
--rw-r--r--   0     1001      127    12080 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/num-traits-0.2.17/tests/cast.rs
--rw-r--r--   0     1001      127     2279 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/.cargo-checksum.json
--rw-r--r--   0     1001      127     6036 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/CHANGELOG.md
--rw-r--r--   0     1001      127     4884 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/Cargo.lock
--rw-r--r--   0     1001      127     2012 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/LICENSE-MIT
--rw-r--r--   0     1001      127     2186 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/README.md
--rw-r--r--   0     1001      127       50 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/bors.toml
--rw-r--r--   0     1001      127      831 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/bench.rs
--rw-r--r--   0     1001      127     1344 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/bench_acquire.rs
--rw-r--r--   0     1001      127     1036 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/lazy_static.rs
--rw-r--r--   0     1001      127      351 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/reentrant_init_deadlocks.rs
--rw-r--r--   0     1001      127     1663 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/regex.rs
--rw-r--r--   0     1001      127     1225 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/test_synchronization.rs
--rw-r--r--   0     1001      127     2485 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/src/imp_cs.rs
--rw-r--r--   0     1001      127     5803 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/src/imp_pl.rs
--rw-r--r--   0     1001      127    12743 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/src/imp_std.rs
--rw-r--r--   0     1001      127    46956 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/src/lib.rs
--rw-r--r--   0     1001      127    13279 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/src/race.rs
--rw-r--r--   0     1001      127      297 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/main.rs
--rw-r--r--   0     1001      127     3055 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/race.rs
--rw-r--r--   0     1001      127     3389 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/race_once_box.rs
--rw-r--r--   0     1001      127     3685 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/sync_lazy.rs
--rw-r--r--   0     1001      127     7663 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/sync_once_cell.rs
--rw-r--r--   0     1001      127     2765 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/unsync_lazy.rs
--rw-r--r--   0     1001      127     3853 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/unsync_once_cell.rs
--rw-r--r--   0     1001      127    20422 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/.cargo-checksum.json
--rw-r--r--   0     1001      127     1903 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/LICENSE-APACHE
--rw-r--r--   0     1001      127     1071 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/LICENSE-MIT
--rw-r--r--   0     1001      127     6869 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/README.md
--rw-r--r--   0     1001      127       56 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/bors.toml
--rw-r--r--   0     1001      127      195 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/build.rs
--rwxr-xr-x   0     1001      127      848 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/all.sh
--rw-r--r--   0     1001      127      735 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/android-install-ndk.sh
--rw-r--r--   0     1001      127     1664 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/android-install-sdk.sh
--rw-r--r--   0     1001      127     1664 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/android-sysimage.sh
--rwxr-xr-x   0     1001      127      821 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/benchmark.sh
--rw-r--r--   0     1001      127     5815 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/deploy_and_run_on_ios_simulator.rs
--rw-r--r--   0     1001      127     1230 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/aarch64-linux-android/Dockerfile
--rw-r--r--   0     1001      127      415 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/aarch64-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127      463 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/arm-unknown-linux-gnueabi/Dockerfile
--rw-r--r--   0     1001      127      422 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/arm-unknown-linux-gnueabihf/Dockerfile
--rw-r--r--   0     1001      127     1222 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/armv7-linux-androideabi/Dockerfile
--rw-r--r--   0     1001      127      426 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/armv7-unknown-linux-gnueabihf/Dockerfile
--rw-r--r--   0     1001      127      152 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/i586-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127      152 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/i686-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127      448 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/mips-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127      456 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/mips64-unknown-linux-gnuabi64/Dockerfile
--rw-r--r--   0     1001      127      464 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/mips64el-unknown-linux-gnuabi64/Dockerfile
--rw-r--r--   0     1001      127      849 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/mipsel-unknown-linux-musl/Dockerfile
--rw-r--r--   0     1001      127      489 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/powerpc-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127      499 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/powerpc64-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127      491 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/powerpc64le-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127      554 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/s390x-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127      603 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/sparc64-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127     1238 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/thumbv7neon-linux-androideabi/Dockerfile
--rw-r--r--   0     1001      127      438 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/thumbv7neon-unknown-linux-gnueabihf/Dockerfile
--rw-r--r--   0     1001      127     1345 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/wasm32-unknown-unknown/Dockerfile
--rw-r--r--   0     1001      127      892 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/x86_64-linux-android/Dockerfile
--rw-r--r--   0     1001      127      180 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/x86_64-unknown-linux-gnu/Dockerfile
--rw-r--r--   0     1001      127      451 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/x86_64-unknown-linux-gnu-emulated/Dockerfile
--rwxr-xr-x   0     1001      127      663 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/dox.sh
--rw-r--r--   0     1001      127      515 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/linux-s390x.sh
--rw-r--r--   0     1001      127      433 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/linux-sparc64.sh
--rw-r--r--   0     1001      127      282 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/lld-shim.rs
--rwxr-xr-x   0     1001      127      281 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/max_line_width.sh
--rwxr-xr-x   0     1001      127      976 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/run-docker.sh
--rwxr-xr-x   0     1001      127     3275 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/run.sh
--rw-r--r--   0     1001      127     1881 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/run_examples.sh
--rw-r--r--   0     1001      127     1365 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/runtest-android.rs
--rwxr-xr-x   0     1001      127      180 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/setup_benchmarks.sh
--rwxr-xr-x   0     1001      127      454 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/test-runner-linux
--rw-r--r--   0     1001      127     2956 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/contributing.md
--rw-r--r--   0     1001      127      296 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/book.toml
--rw-r--r--   0     1001      127      794 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/SUMMARY.md
--rw-r--r--   0     1001      127      134 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/ascii.css
--rw-r--r--   0     1001      127      911 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/bound_checks.md
--rw-r--r--   0     1001      127      265 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/float-math/approx.md
--rw-r--r--   0     1001      127      186 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/float-math/fma.md
--rw-r--r--   0     1001      127      108 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/float-math/fp.md
--rw-r--r--   0     1001      127      165 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/float-math/svml.md
--rw-r--r--   0     1001      127      638 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/introduction.md
--rw-r--r--   0     1001      127     3476 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/linux.md
--rw-r--r--   0     1001      127     3629 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/mca.md
--rw-r--r--   0     1001      127      738 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/profiling.md
--rw-r--r--   0     1001      127       91 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/attribute.md
--rw-r--r--   0     1001      127      745 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/features.md
--rw-r--r--   0     1001      127       97 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/inlining.md
--rw-r--r--   0     1001      127     1486 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/practice.md
--rw-r--r--   0     1001      127       82 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/runtime.md
--rw-r--r--   0     1001      127     2625 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/rustflags.md
--rw-r--r--   0     1001      127     2719 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/vert-hor-ops.md
--rw-r--r--   0     1001      127        8 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/rust-toolchain
--rw-r--r--   0     1001      127      112 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/rustfmt.toml
--rw-r--r--   0     1001      127     5477 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/bit_manip.rs
--rw-r--r--   0     1001      127     3075 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/bitmask.rs
--rw-r--r--   0     1001      127     2435 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/macros.rs
--rw-r--r--   0     1001      127     4101 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v128.rs
--rw-r--r--   0     1001      127      870 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v16.rs
--rw-r--r--   0     1001      127     4066 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v256.rs
--rw-r--r--   0     1001      127     1629 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v32.rs
--rw-r--r--   0     1001      127     3202 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v512.rs
--rw-r--r--   0     1001      127     2531 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v64.rs
--rw-r--r--   0     1001      127     3070 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast.rs
--rw-r--r--   0     1001      127      811 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/eq.rs
--rw-r--r--   0     1001      127     1365 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/ord.rs
--rw-r--r--   0     1001      127     2195 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/partial_eq.rs
--rw-r--r--   0     1001      127    11164 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/partial_ord.rs
--rw-r--r--   0     1001      127     4094 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/vertical.rs
--rw-r--r--   0     1001      127      176 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp.rs
--rw-r--r--   0     1001      127      997 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/default.rs
--rw-r--r--   0     1001      127     2258 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/binary.rs
--rw-r--r--   0     1001      127     2418 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/debug.rs
--rw-r--r--   0     1001      127     2270 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/lower_hex.rs
--rw-r--r--   0     1001      127     2258 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/octal.rs
--rw-r--r--   0     1001      127     2274 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/upper_hex.rs
--rw-r--r--   0     1001      127      161 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt.rs
--rw-r--r--   0     1001      127     4759 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/from/from_array.rs
--rw-r--r--   0     1001      127     2153 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/from/from_vector.rs
--rw-r--r--   0     1001      127      113 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/from.rs
--rw-r--r--   0     1001      127     1857 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/hash.rs
--rw-r--r--   0     1001      127     7989 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/arch_specific.rs
--rw-r--r--   0     1001      127     2761 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/macros.rs
--rw-r--r--   0     1001      127     3049 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v128.rs
--rw-r--r--   0     1001      127      312 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v16.rs
--rw-r--r--   0     1001      127     3087 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v256.rs
--rw-r--r--   0     1001      127      520 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v32.rs
--rw-r--r--   0     1001      127     3138 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v512.rs
--rw-r--r--   0     1001      127      972 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v64.rs
--rw-r--r--   0     1001      127     1223 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits.rs
--rw-r--r--   0     1001      127      981 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/abs.rs
--rw-r--r--   0     1001      127     2687 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/consts.rs
--rw-r--r--   0     1001      127     1569 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/cos.rs
--rw-r--r--   0     1001      127     1183 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/exp.rs
--rw-r--r--   0     1001      127     1157 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/ln.rs
--rw-r--r--   0     1001      127     1700 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/mul_add.rs
--rw-r--r--   0     1001      127     2016 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/mul_adde.rs
--rw-r--r--   0     1001      127     1312 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/powf.rs
--rw-r--r--   0     1001      127     1292 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/recpre.rs
--rw-r--r--   0     1001      127     1496 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/rsqrte.rs
--rw-r--r--   0     1001      127     1759 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/sin.rs
--rw-r--r--   0     1001      127     1179 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/sqrt.rs
--rw-r--r--   0     1001      127     1593 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/sqrte.rs
--rw-r--r--   0     1001      127      871 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/tanh.rs
--rw-r--r--   0     1001      127      957 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float.rs
--rw-r--r--   0     1001      127       65 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math.rs
--rw-r--r--   0     1001      127     6798 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/minimal/iuf.rs
--rw-r--r--   0     1001      127     6833 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/minimal/mask.rs
--rw-r--r--   0     1001      127    58636 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/minimal/ptr.rs
--rw-r--r--   0     1001      127       67 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/minimal.rs
--rw-r--r--   0     1001      127     7094 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_arithmetic.rs
--rw-r--r--   0     1001      127     5612 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_bitwise.rs
--rw-r--r--   0     1001      127     4673 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_mask_bitwise.rs
--rw-r--r--   0     1001      127     4166 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_shifts.rs
--rw-r--r--   0     1001      127     5010 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_arithmetic.rs
--rw-r--r--   0     1001      127     4285 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_bitwise.rs
--rw-r--r--   0     1001      127     2920 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_float_min_max.rs
--rw-r--r--   0     1001      127     2037 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_int_min_max.rs
--rw-r--r--   0     1001      127     3832 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_mask_bitwise.rs
--rw-r--r--   0     1001      127     1569 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_neg.rs
--rw-r--r--   0     1001      127     4106 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_rotates.rs
--rw-r--r--   0     1001      127     4052 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_shifts.rs
--rw-r--r--   0     1001      127      462 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops.rs
--rw-r--r--   0     1001      127     8262 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ptr/gather_scatter.rs
--rw-r--r--   0     1001      127       57 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ptr.rs
--rw-r--r--   0     1001      127     6109 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/bitwise.rs
--rw-r--r--   0     1001      127    13834 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/float_arithmetic.rs
--rw-r--r--   0     1001      127     8030 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/integer_arithmetic.rs
--rw-r--r--   0     1001      127     3573 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/mask.rs
--rw-r--r--   0     1001      127    17484 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/min_max.rs
--rw-r--r--   0     1001      127      163 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions.rs
--rw-r--r--   0     1001      127     2516 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/select.rs
--rw-r--r--   0     1001      127     6595 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/shuffle.rs
--rw-r--r--   0     1001      127     6570 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/shuffle1_dyn.rs
--rw-r--r--   0     1001      127     9045 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/slice/from_slice.rs
--rw-r--r--   0     1001      127     9000 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/slice/write_to_slice.rs
--rw-r--r--   0     1001      127       90 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/slice.rs
--rw-r--r--   0     1001      127     7085 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/swap_bytes.rs
--rw-r--r--   0     1001      127    13620 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api.rs
--rw-r--r--   0     1001      127    13558 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/bit_manip.rs
--rw-r--r--   0     1001      127     3842 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/llvm.rs
--rw-r--r--   0     1001      127     3752 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/abs.rs
--rw-r--r--   0     1001      127     3749 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/cos.rs
--rw-r--r--   0     1001      127     2827 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/cos_pi.rs
--rw-r--r--   0     1001      127     4276 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/exp.rs
--rw-r--r--   0     1001      127     4237 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/ln.rs
--rw-r--r--   0     1001      127    18033 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/macros.rs
--rw-r--r--   0     1001      127     4150 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/mul_add.rs
--rw-r--r--   0     1001      127     2093 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/mul_adde.rs
--rw-r--r--   0     1001      127     4471 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/powf.rs
--rw-r--r--   0     1001      127     3750 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin.rs
--rw-r--r--   0     1001      127     6535 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin_cos_pi.rs
--rw-r--r--   0     1001      127     2830 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin_pi.rs
--rw-r--r--   0     1001      127     3756 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sqrt.rs
--rw-r--r--   0     1001      127     2603 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sqrte.rs
--rw-r--r--   0     1001      127     4289 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/tanh.rs
--rw-r--r--   0     1001      127      425 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float.rs
--rw-r--r--   0     1001      127       52 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math.rs
--rw-r--r--   0     1001      127      908 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/pointer_sized_int.rs
--rw-r--r--   0     1001      127     2309 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/aarch64.rs
--rw-r--r--   0     1001      127     1845 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/arm.rs
--rw-r--r--   0     1001      127      182 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/fallback.rs
--rw-r--r--   0     1001      127     6614 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/fallback_impl.rs
--rw-r--r--   0     1001      127     3692 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/avx.rs
--rw-r--r--   0     1001      127     1351 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/avx2.rs
--rw-r--r--   0     1001      127     1322 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/sse.rs
--rw-r--r--   0     1001      127     2581 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/sse2.rs
--rw-r--r--   0     1001      127     5387 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86.rs
--rw-r--r--   0     1001      127     1745 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask.rs
--rw-r--r--   0     1001      127       21 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions.rs
--rw-r--r--   0     1001      127     5876 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/shuffle.rs
--rw-r--r--   0     1001      127    15039 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/shuffle1_dyn.rs
--rw-r--r--   0     1001      127     5365 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/swap_bytes.rs
--rw-r--r--   0     1001      127     1251 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v128.rs
--rw-r--r--   0     1001      127      187 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v16.rs
--rw-r--r--   0     1001      127     1871 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v256.rs
--rw-r--r--   0     1001      127      350 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v32.rs
--rw-r--r--   0     1001      127     3082 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v512.rs
--rw-r--r--   0     1001      127      778 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v64.rs
--rw-r--r--   0     1001      127     1231 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/vPtr.rs
--rw-r--r--   0     1001      127      823 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/vSize.rs
--rw-r--r--   0     1001      127     1475 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen.rs
--rw-r--r--   0     1001      127    11525 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/lib.rs
--rw-r--r--   0     1001      127     3436 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/masks.rs
--rw-r--r--   0     1001      127     1147 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/sealed.rs
--rw-r--r--   0     1001      127     1916 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/testing/macros.rs
--rw-r--r--   0     1001      127     4512 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/testing/utils.rs
--rw-r--r--   0     1001      127      115 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/testing.rs
--rw-r--r--   0     1001      127     3079 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v128.rs
--rw-r--r--   0     1001      127      447 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v16.rs
--rw-r--r--   0     1001      127     3462 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v256.rs
--rw-r--r--   0     1001      127      895 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v32.rs
--rw-r--r--   0     1001      127     4555 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v512.rs
--rw-r--r--   0     1001      127     2379 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v64.rs
--rw-r--r--   0     1001      127      966 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/vPtr.rs
--rw-r--r--   0     1001      127     1484 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/vSize.rs
--rw-r--r--   0     1001      127     7391 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/packed_simd-0.3.9/tests/endianness.rs
--rw-r--r--   0     1001      127     1845 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/.cargo-checksum.json
--rw-r--r--   0     1001      127     1675 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/LICENSE-MIT
--rw-r--r--   0     1001      127     3866 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/README.md
--rw-r--r--   0     1001      127     4230 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/build.rs
--rw-r--r--   0     1001      127       38 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/rust-toolchain.toml
--rw-r--r--   0     1001      127     2703 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/detection.rs
--rw-r--r--   0     1001      127     2565 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/extra.rs
--rw-r--r--   0     1001      127    29816 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/fallback.rs
--rw-r--r--   0     1001      127    43477 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/lib.rs
--rw-r--r--   0     1001      127      872 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/location.rs
--rw-r--r--   0     1001      127      499 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/marker.rs
--rw-r--r--   0     1001      127    28375 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/parse.rs
--rw-r--r--   0     1001      127     2901 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/rcvec.rs
--rw-r--r--   0     1001      127    26672 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/wrapper.rs
--rw-r--r--   0     1001      127     3425 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/comments.rs
--rw-r--r--   0     1001      127      152 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/features.rs
--rw-r--r--   0     1001      127     2705 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/marker.rs
--rw-r--r--   0     1001      127    22341 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/test.rs
--rw-r--r--   0     1001      127     1312 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/test_fmt.rs
--rw-r--r--   0     1001      127     1365 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/test_size.rs
--rw-r--r--   0     1001      127      655 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/.cargo-checksum.json
--rw-r--r--   0     1001      127     1452 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/Cargo.toml
--rw-r--r--   0     1001      127    10781 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/LICENSE
--rw-r--r--   0     1001      127     2498 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/build.rs
--rw-r--r--   0     1001      127     3898 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/src/errors.rs
--rw-r--r--   0     1001      127    91298 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/src/impl_.rs
--rw-r--r--   0     1001      127     2032 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/src/import_lib.rs
--rw-r--r--   0     1001      127     9853 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/src/lib.rs
--rw-r--r--   0     1001      127     7657 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/.cargo-checksum.json
--rw-r--r--   0     1001      127     1586 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/Cargo.toml
--rw-r--r--   0     1001      127    30464 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/LICENSE
--rw-r--r--   0     1001      127     6375 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/README.md
--rw-r--r--   0     1001      127     4027 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/build.rs
--rw-r--r--   0     1001      127    15383 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/abstract_.rs
--rw-r--r--   0     1001      127      233 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/bltinmodule.rs
--rw-r--r--   0     1001      127     1282 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/boolobject.rs
--rw-r--r--   0     1001      127     1857 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/bytearrayobject.rs
--rw-r--r--   0     1001      127     2333 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/bytesobject.rs
--rw-r--r--   0     1001      127     4431 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/ceval.rs
--rw-r--r--   0     1001      127       53 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/code.rs
--rw-r--r--   0     1001      127     2632 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/codecs.rs
--rw-r--r--   0     1001      127      257 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/compile.rs
--rw-r--r--   0     1001      127     2110 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/complexobject.rs
--rw-r--r--   0     1001      127     1592 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/context.rs
--rw-r--r--   0     1001      127     9978 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/abstract_.rs
--rw-r--r--   0     1001      127      556 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/bytesobject.rs
--rw-r--r--   0     1001      127      507 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/ceval.rs
--rw-r--r--   0     1001      127     8871 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/code.rs
--rw-r--r--   0     1001      127     3206 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/compile.rs
--rw-r--r--   0     1001      127     1790 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/descrobject.rs
--rw-r--r--   0     1001      127     2163 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/dictobject.rs
--rw-r--r--   0     1001      127      572 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/floatobject.rs
--rw-r--r--   0     1001      127     2508 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/frameobject.rs
--rw-r--r--   0     1001      127     3437 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/funcobject.rs
--rw-r--r--   0     1001      127     2579 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/genobject.rs
--rw-r--r--   0     1001      127     1927 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/import.rs
--rw-r--r--   0     1001      127     6136 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/initconfig.rs
--rw-r--r--   0     1001      127      968 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/listobject.rs
--rw-r--r--   0     1001      127     1724 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/methodobject.rs
--rw-r--r--   0     1001      127     1743 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/mod.rs
--rw-r--r--   0     1001      127    13705 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/object.rs
--rw-r--r--   0     1001      127     1679 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pydebug.rs
--rw-r--r--   0     1001      127     4597 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pyerrors.rs
--rw-r--r--   0     1001      127     1345 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pylifecycle.rs
--rw-r--r--   0     1001      127     1645 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pymem.rs
--rw-r--r--   0     1001      127     3225 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pystate.rs
--rw-r--r--   0     1001      127     7235 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pythonrun.rs
--rw-r--r--   0     1001      127      875 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/tupleobject.rs
--rw-r--r--   0     1001      127    22551 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/unicodeobject.rs
--rw-r--r--   0     1001      127      465 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/weakrefobject.rs
--rw-r--r--   0     1001      127    20094 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/datetime.rs
--rw-r--r--   0     1001      127     2512 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/descrobject.rs
--rw-r--r--   0     1001      127     4500 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/dictobject.rs
--rw-r--r--   0     1001      127      191 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/enumobject.rs
--rw-r--r--   0     1001      127     1274 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/fileobject.rs
--rw-r--r--   0     1001      127      274 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/fileutils.rs
--rw-r--r--   0     1001      127     1528 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/floatobject.rs
--rw-r--r--   0     1001      127     3192 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/import.rs
--rw-r--r--   0     1001      127      642 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/intrcheck.rs
--rw-r--r--   0     1001      127      773 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/iterobject.rs
--rw-r--r--   0     1001      127    13771 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/lib.rs
--rw-r--r--   0     1001      127     2644 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/listobject.rs
--rw-r--r--   0     1001      127     5361 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/longobject.rs
--rw-r--r--   0     1001      127      755 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/marshal.rs
--rw-r--r--   0     1001      127     1347 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/memoryobject.rs
--rw-r--r--   0     1001      127     7563 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/methodobject.rs
--rw-r--r--   0     1001      127     5558 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/modsupport.rs
--rw-r--r--   0     1001      127     3175 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/moduleobject.rs
--rw-r--r--   0     1001      127    23709 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/object.rs
--rw-r--r--   0     1001      127     4025 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/objimpl.rs
--rw-r--r--   0     1001      127      107 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/osmodule.rs
--rw-r--r--   0     1001      127       25 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pyarena.rs
--rw-r--r--   0     1001      127     4630 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pybuffer.rs
--rw-r--r--   0     1001      127     2154 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pycapsule.rs
--rw-r--r--   0     1001      127    17662 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pyerrors.rs
--rw-r--r--   0     1001      127      427 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pyframe.rs
--rw-r--r--   0     1001      127     1298 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pyhash.rs
--rw-r--r--   0     1001      127     1754 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pylifecycle.rs
--rw-r--r--   0     1001      127      510 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pymem.rs
--rw-r--r--   0     1001      127      726 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pyport.rs
--rw-r--r--   0     1001      127     3096 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pystate.rs
--rw-r--r--   0     1001      127     1164 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pystrtod.rs
--rw-r--r--   0     1001      127     1992 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pythonrun.rs
--rw-r--r--   0     1001      127      447 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/rangeobject.rs
--rw-r--r--   0     1001      127     4431 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/setobject.rs
--rw-r--r--   0     1001      127     2337 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/sliceobject.rs
--rw-r--r--   0     1001      127     2084 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/structmember.rs
--rw-r--r--   0     1001      127     1892 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/structseq.rs
--rw-r--r--   0     1001      127     1369 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/sysmodule.rs
--rw-r--r--   0     1001      127      773 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/traceback.rs
--rw-r--r--   0     1001      127     1468 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/tupleobject.rs
--rw-r--r--   0     1001      127     3057 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/typeslots.rs
--rw-r--r--   0     1001      127    13559 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/unicodeobject.rs
--rw-r--r--   0     1001      127      959 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/warnings.rs
--rw-r--r--   0     1001      127     1982 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/weakrefobject.rs
--rw-r--r--   0     1001      127     2744 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/.cargo-checksum.json
--rw-r--r--   0     1001      127     1322 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/LICENSE-MIT
--rw-r--r--   0     1001      127     9302 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/README.md
--rw-r--r--   0     1001      127       38 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/rust-toolchain.toml
--rw-r--r--   0     1001      127     2739 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/src/ext.rs
--rw-r--r--   0     1001      127     4796 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/src/format.rs
--rw-r--r--   0     1001      127     2309 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/src/ident_fragment.rs
--rw-r--r--   0     1001      127    44977 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/src/lib.rs
--rw-r--r--   0     1001      127    16224 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/src/runtime.rs
--rw-r--r--   0     1001      127     1112 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/src/spanned.rs
--rw-r--r--   0     1001      127     5454 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/src/to_tokens.rs
--rw-r--r--   0     1001      127      166 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/compiletest.rs
--rw-r--r--   0     1001      127    12980 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/test.rs
--rw-r--r--   0     1001      127      209 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated-dup.rs
--rw-r--r--   0     1001      127      559 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated-dup.stderr
--rw-r--r--   0     1001      127      201 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated.rs
--rw-r--r--   0     1001      127      539 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated.stderr
--rw-r--r--   0     1001      127       55 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-separated.rs
--rw-r--r--   0     1001      127      444 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-separated.stderr
--rw-r--r--   0     1001      127       54 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter.rs
--rw-r--r--   0     1001      127      432 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter.stderr
--rw-r--r--   0     1001      127      119 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/not-quotable.rs
--rw-r--r--   0     1001      127      659 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/not-quotable.stderr
--rw-r--r--   0     1001      127      106 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/not-repeatable.rs
--rw-r--r--   0     1001      127     1464 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/not-repeatable.stderr
--rw-r--r--   0     1001      127      109 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/wrong-type-span.rs
--rw-r--r--   0     1001      127      346 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/wrong-type-span.stderr
--rw-r--r--   0     1001      127     2936 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/.cargo-checksum.json
--rw-r--r--   0     1001      127     1157 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/LICENSE-MIT
--rw-r--r--   0     1001      127     4317 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/README.md
--rw-r--r--   0     1001      127     2340 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/build/build.rs
--rw-r--r--   0     1001      127     3661 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/build/rustc.rs
--rw-r--r--   0     1001      127      886 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/attr.rs
--rw-r--r--   0     1001      127     1982 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/bound.rs
--rw-r--r--   0     1001      127     1827 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/constfn.rs
--rw-r--r--   0     1001      127     1406 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/date.rs
--rw-r--r--   0     1001      127     1714 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/error.rs
--rw-r--r--   0     1001      127     2746 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/expand.rs
--rw-r--r--   0     1001      127     5189 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/expr.rs
--rw-r--r--   0     1001      127     1061 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/iter.rs
--rw-r--r--   0     1001      127     7698 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/lib.rs
--rw-r--r--   0     1001      127      929 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/release.rs
--rw-r--r--   0     1001      127     1408 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/time.rs
--rw-r--r--   0     1001      127     2442 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/token.rs
--rw-r--r--   0     1001      127      289 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/src/version.rs
--rw-r--r--   0     1001      127      166 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/compiletest.rs
--rw-r--r--   0     1001      127      800 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/test_const.rs
--rw-r--r--   0     1001      127      307 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/test_eval.rs
--rw-r--r--   0     1001      127     2522 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/test_parse.rs
--rw-r--r--   0     1001      127      100 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/bad-bound.rs
--rw-r--r--   0     1001      127      374 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/bad-bound.stderr
--rw-r--r--   0     1001      127      104 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/bad-date.rs
--rw-r--r--   0     1001      127      312 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/bad-date.stderr
--rw-r--r--   0     1001      127       90 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/bad-not.rs
--rw-r--r--   0     1001      127      239 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/bad-not.stderr
--rw-r--r--   0     1001      127      104 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/bad-version.rs
--rw-r--r--   0     1001      127      322 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/bad-version.stderr
--rw-r--r--   0     1001      127       63 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/const-not-fn.rs
--rw-r--r--   0     1001      127      148 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/ui/const-not-fn.stderr
--rw-r--r--   0     1001      127     2765 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/.cargo-checksum.json
--rw-r--r--   0     1001      127     3777 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/Cargo.lock
--rw-r--r--   0     1001      127     1311 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/LICENSE-APACHE
--rw-r--r--   0     1001      127     1338 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/LICENSE-BOOST
--rw-r--r--   0     1001      127     3702 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/README.md
--rw-r--r--   0     1001      127     1532 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/benches/bench.rs
--rw-r--r--   0     1001      127     2189 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/examples/upstream_benchmark.rs
--rw-r--r--   0     1001      127     5138 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/buffer/mod.rs
--rw-r--r--   0     1001      127     3237 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/common.rs
--rw-r--r--   0     1001      127    11284 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/d2s.rs
--rw-r--r--   0     1001      127    32886 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/d2s_full_table.rs
--rw-r--r--   0     1001      127     2567 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/d2s_intrinsics.rs
--rw-r--r--   0     1001      127     5370 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/d2s_small_table.rs
--rw-r--r--   0     1001      127     1203 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/digit_table.rs
--rw-r--r--   0     1001      127     6959 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/f2s.rs
--rw-r--r--   0     1001      127     3700 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/f2s_intrinsics.rs
--rw-r--r--   0     1001      127     4039 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/lib.rs
--rw-r--r--   0     1001      127      479 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/parse.rs
--rw-r--r--   0     1001      127     1242 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/pretty/exponent.rs
--rw-r--r--   0     1001      127     2391 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/pretty/mantissa.rs
--rw-r--r--   0     1001      127     8015 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/pretty/mod.rs
--rw-r--r--   0     1001      127     7756 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/s2d.rs
--rw-r--r--   0     1001      127     8315 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/src/s2f.rs
--rw-r--r--   0     1001      127     2497 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/tests/common_test.rs
--rw-r--r--   0     1001      127     1698 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/tests/d2s_table_test.rs
--rw-r--r--   0     1001      127     9617 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/tests/d2s_test.rs
--rw-r--r--   0     1001      127     1613 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/tests/exhaustive.rs
--rw-r--r--   0     1001      127     4572 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/tests/f2s_test.rs
--rw-r--r--   0     1001      127      183 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/tests/macros/mod.rs
--rw-r--r--   0     1001      127     5059 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/tests/s2d_test.rs
--rw-r--r--   0     1001      127     3152 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/ryu-1.0.15/tests/s2f_test.rs
--rw-r--r--   0     1001      127     2207 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/.cargo-checksum.json
--rw-r--r--   0     1001      127     1565 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/LICENSE-MIT
--rw-r--r--   0     1001      127     4366 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/README.md
--rw-r--r--   0     1001      127     3138 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/build.rs
--rw-r--r--   0     1001      127     2538 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/crates-io.md
--rw-r--r--   0     1001      127      726 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/de/format.rs
--rw-r--r--   0     1001      127     6154 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/de/ignored_any.rs
--rw-r--r--   0     1001      127    91490 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/de/impls.rs
--rw-r--r--   0     1001      127    80313 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/de/mod.rs
--rw-r--r--   0     1001      127      563 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/de/seed.rs
--rw-r--r--   0     1001      127      644 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/de/size_hint.rs
--rw-r--r--   0     1001      127    44831 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/de/value.rs
--rw-r--r--   0     1001      127      243 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/integer128.rs
--rw-r--r--   0     1001      127    13294 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/lib.rs
--rw-r--r--   0     1001      127     8264 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/macros.rs
--rw-r--r--   0     1001      127    86931 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/private/de.rs
--rw-r--r--   0     1001      127     4888 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/private/doc.rs
--rw-r--r--   0     1001      127     1567 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/private/mod.rs
--rw-r--r--   0     1001      127    40321 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/private/ser.rs
--rw-r--r--   0     1001      127     4169 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/ser/fmt.rs
--rw-r--r--   0     1001      127    28630 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/ser/impls.rs
--rw-r--r--   0     1001      127     5287 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/ser/impossible.rs
--rw-r--r--   0     1001      127    62995 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/ser/mod.rs
--rw-r--r--   0     1001      127     1347 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde-1.0.188/src/std_error.rs
--rw-r--r--   0     1001      127     1973 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/.cargo-checksum.json
--rw-r--r--   0     1001      127     1412 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/LICENSE-MIT
--rw-r--r--   0     1001      127     4366 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/README.md
--rw-r--r--   0     1001      127     2538 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/crates-io.md
--rw-r--r--   0     1001      127    14709 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/bound.rs
--rw-r--r--   0     1001      127   109306 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/de.rs
--rw-r--r--   0     1001      127      611 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/dummy.rs
--rw-r--r--   0     1001      127     2116 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/fragment.rs
--rw-r--r--   0     1001      127     6601 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/ast.rs
--rw-r--r--   0     1001      127    68804 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/attr.rs
--rw-r--r--   0     1001      127     7121 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/case.rs
--rw-r--r--   0     1001      127    16638 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/check.rs
--rw-r--r--   0     1001      127     2021 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/ctxt.rs
--rw-r--r--   0     1001      127      381 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/mod.rs
--rw-r--r--   0     1001      127    10519 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/receiver.rs
--rw-r--r--   0     1001      127      451 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/respan.rs
--rw-r--r--   0     1001      127     2523 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/symbol.rs
--rw-r--r--   0     1001      127     3000 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/lib.rs
--rw-r--r--   0     1001      127     5718 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/pretend.rs
--rw-r--r--   0     1001      127    45209 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/ser.rs
--rw-r--r--   0     1001      127     1007 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/this.rs
--rw-r--r--   0     1001      127     7848 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/.cargo-checksum.json
--rw-r--r--   0     1001      127     1733 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/CONTRIBUTING.md
--rw-r--r--   0     1001      127     2170 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/LICENSE-MIT
--rw-r--r--   0     1001      127    14217 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/README.md
--rw-r--r--   0     1001      127      521 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/build.rs
--rw-r--r--   0     1001      127    85485 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/de.rs
--rw-r--r--   0     1001      127    16571 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/error.rs
--rw-r--r--   0     1001      127       80 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/features_check/error.rs
--rw-r--r--   0     1001      127      269 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/features_check/mod.rs
--rw-r--r--   0     1001      127     1739 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/io/core.rs
--rw-r--r--   0     1001      127      684 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/io/mod.rs
--rw-r--r--   0     1001      127     1848 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/iter.rs
--rw-r--r--   0     1001      127     6154 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/algorithm.rs
--rw-r--r--   0     1001      127     7039 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/bhcomp.rs
--rw-r--r--   0     1001      127      654 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/bignum.rs
--rw-r--r--   0     1001      127     2156 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/cached.rs
--rw-r--r--   0     1001      127     5782 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/cached_float80.rs
--rw-r--r--   0     1001      127      444 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/digit.rs
--rw-r--r--   0     1001      127     5082 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/errors.rs
--rw-r--r--   0     1001      127     1578 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/exponent.rs
--rw-r--r--   0     1001      127     5482 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/float.rs
--rw-r--r--   0     1001      127      232 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/large_powers.rs
--rw-r--r--   0     1001      127    15360 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/large_powers32.rs
--rw-r--r--   0     1001      127    15877 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/large_powers64.rs
--rw-r--r--   0     1001      127    26259 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/math.rs
--rw-r--r--   0     1001      127     1041 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/mod.rs
--rw-r--r--   0     1001      127    11811 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/num.rs
--rw-r--r--   0     1001      127     2241 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/parse.rs
--rw-r--r--   0     1001      127     7396 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/rounding.rs
--rw-r--r--   0     1001      127     1235 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/shift.rs
--rw-r--r--   0     1001      127     1318 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/small_powers.rs
--rw-r--r--   0     1001      127    13642 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lib.rs
--rw-r--r--   0     1001      127    10129 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/macros.rs
--rw-r--r--   0     1001      127    24860 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/map.rs
--rw-r--r--   0     1001      127    24054 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/number.rs
--rw-r--r--   0     1001      127    21194 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/raw.rs
--rw-r--r--   0     1001      127    31338 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/read.rs
--rw-r--r--   0     1001      127    62121 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/ser.rs
--rw-r--r--   0     1001      127    38943 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/de.rs
--rw-r--r--   0     1001      127     5962 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/from.rs
--rw-r--r--   0     1001      127     8789 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/index.rs
--rw-r--r--   0     1001      127    29737 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/mod.rs
--rw-r--r--   0     1001      127     2371 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/partial_eq.rs
--rw-r--r--   0     1001      127    27587 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/ser.rs
--rw-r--r--   0     1001      127      166 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/compiletest.rs
--rw-r--r--   0     1001      127     1995 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/debug.rs
--rw-r--r--   0     1001      127     3867 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/algorithm.rs
--rw-r--r--   0     1001      127     1548 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/exponent.rs
--rw-r--r--   0     1001      127    14186 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/float.rs
--rw-r--r--   0     1001      127     5418 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/math.rs
--rw-r--r--   0     1001      127     1642 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/num.rs
--rw-r--r--   0     1001      127    17154 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/parse.rs
--rw-r--r--   0     1001      127     9038 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/rounding.rs
--rw-r--r--   0     1001      127     1080 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical.rs
--rw-r--r--   0     1001      127     1511 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/macros/mod.rs
--rw-r--r--   0     1001      127     1268 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/map.rs
--rw-r--r--   0     1001      127      362 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/regression/issue1004.rs
--rw-r--r--   0     1001      127      401 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/regression/issue520.rs
--rw-r--r--   0     1001      127     1605 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/regression/issue795.rs
--rw-r--r--   0     1001      127     1895 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/regression/issue845.rs
--rw-r--r--   0     1001      127      236 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/regression/issue953.rs
--rw-r--r--   0     1001      127       58 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/regression.rs
--rw-r--r--   0     1001      127     5130 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/stream.rs
--rw-r--r--   0     1001      127    74363 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/test.rs
--rw-r--r--   0     1001      127       57 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/missing_colon.rs
--rw-r--r--   0     1001      127      448 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/missing_colon.stderr
--rw-r--r--   0     1001      127       69 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/missing_comma.rs
--rw-r--r--   0     1001      127      377 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/missing_comma.stderr
--rw-r--r--   0     1001      127       59 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/missing_value.rs
--rw-r--r--   0     1001      127      452 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/missing_value.stderr
--rw-r--r--   0     1001      127       61 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/not_found.rs
--rw-r--r--   0     1001      127      162 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/not_found.stderr
--rw-r--r--   0     1001      127       61 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/parse_expr.rs
--rw-r--r--   0     1001      127      305 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/parse_expr.stderr
--rw-r--r--   0     1001      127       65 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/parse_key.rs
--rw-r--r--   0     1001      127      139 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/parse_key.stderr
--rw-r--r--   0     1001      127       61 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/unexpected_after_array_element.rs
--rw-r--r--   0     1001      127      241 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/unexpected_after_array_element.stderr
--rw-r--r--   0     1001      127       66 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/unexpected_after_map_entry.rs
--rw-r--r--   0     1001      127      247 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/unexpected_after_map_entry.stderr
--rw-r--r--   0     1001      127       60 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/unexpected_colon.rs
--rw-r--r--   0     1001      127      219 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/unexpected_colon.stderr
--rw-r--r--   0     1001      127       69 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/unexpected_comma.rs
--rw-r--r--   0     1001      127      232 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/ui/unexpected_comma.stderr
--rw-r--r--   0     1001      127     2259 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/.cargo-checksum.json
--rw-r--r--   0     1001      127     2729 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/CHANGELOG.md
--rw-r--r--   0     1001      127      152 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/Cargo.lock
--rw-r--r--   0     1001      127     1464 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/Cargo.toml
--rw-r--r--   0     1001      127    10173 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/LICENSE-Apache
--rw-r--r--   0     1001      127     1035 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/LICENSE-MIT
--rw-r--r--   0     1001      127     9360 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/README.md
--rw-r--r--   0     1001      127     1063 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/examples/streaming.rs
--rw-r--r--   0     1001      127      952 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/release.toml
--rw-r--r--   0     1001      127       14 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/rustfmt.toml
--rw-r--r--   0     1001      127    10608 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/basic.rs
--rw-r--r--   0     1001      127     4838 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/compat.rs
--rw-r--r--   0     1001      127     1479 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/aarch64/mod.rs
--rw-r--r--   0     1001      127     6044 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/aarch64/neon.rs
--rw-r--r--   0     1001      127    23187 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/algorithm.rs
--rw-r--r--   0     1001      127     3620 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/helpers.rs
--rw-r--r--   0     1001      127     2537 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/mod.rs
--rw-r--r--   0     1001      127     1304 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/wasm32/mod.rs
--rw-r--r--   0     1001      127     6185 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/wasm32/simd128.rs
--rw-r--r--   0     1001      127     7088 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/x86/avx2.rs
--rw-r--r--   0     1001      127     5494 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/x86/mod.rs
--rw-r--r--   0     1001      127     6525 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/x86/sse42.rs
--rw-r--r--   0     1001      127     5414 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/lib.rs
--rw-r--r--   0     1001      127    16410 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/tests/tests.rs
--rw-r--r--   0     1001      127     1475 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/simdutf8-0.1.4/wasm32-development.md
--rw-r--r--   0     1001      127     1302 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/.cargo-checksum.json
--rw-r--r--   0     1001      127     1684 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/LICENSE-APACHE
--rw-r--r--   0     1001      127     1072 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/LICENSE-MIT
--rw-r--r--   0     1001      127      649 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/README.md
--rw-r--r--   0     1001      127     8567 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/benches/bench.rs
--rw-r--r--   0     1001      127     5231 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/debug_metadata/README.md
--rw-r--r--   0     1001      127     1561 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/debug_metadata/smallvec.natvis
--rw-r--r--   0     1001      127      730 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/scripts/run_miri.sh
--rw-r--r--   0     1001      127      570 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/src/arbitrary.rs
--rw-r--r--   0     1001      127    78554 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/src/lib.rs
--rw-r--r--   0     1001      127      611 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/src/specialization.rs
--rw-r--r--   0     1001      127    25779 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/src/tests.rs
--rw-r--r--   0     1001      127     1888 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/tests/debugger_visualizer.rs
--rw-r--r--   0     1001      127      542 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/smallvec-1.11.1/tests/macro.rs
--rw-r--r--   0     1001      127     1380 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/.cargo-checksum.json
--rw-r--r--   0     1001      127     6229 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/CHANGELOG.md
--rw-r--r--   0     1001      127     1411 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/Cargo.toml
--rw-r--r--   0     1001      127    11358 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1072 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/LICENSE-MIT
--rw-r--r--   0     1001      127     7437 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/README.md
--rw-r--r--   0     1001      127     1734 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_cfg.rs
--rw-r--r--   0     1001      127     1405 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_eq_align.rs
--rw-r--r--   0     1001      127     3450 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_eq_size.rs
--rw-r--r--   0     1001      127     1865 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_fields.rs
--rw-r--r--   0     1001      127    12894 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_impl.rs
--rw-r--r--   0     1001      127     2381 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_obj_safe.rs
--rw-r--r--   0     1001      127     3106 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_trait.rs
--rw-r--r--   0     1001      127     2854 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_type.rs
--rw-r--r--   0     1001      127     2994 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/const_assert.rs
--rw-r--r--   0     1001      127     3450 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/lib.rs
--rw-r--r--   0     1001      127     8306 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/.cargo-checksum.json
--rw-r--r--   0     1001      127     2678 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/LICENSE-MIT
--rw-r--r--   0     1001      127    10396 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/README.md
--rw-r--r--   0     1001      127     1331 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/benches/file.rs
--rw-r--r--   0     1001      127     4956 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/benches/rust.rs
--rw-r--r--   0     1001      127    26351 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/attr.rs
--rw-r--r--   0     1001      127     1610 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/bigint.rs
--rw-r--r--   0     1001      127    15994 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/buffer.rs
--rw-r--r--   0     1001      127     7826 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/custom_keyword.rs
--rw-r--r--   0     1001      127     9061 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/custom_punctuation.rs
--rw-r--r--   0     1001      127     9777 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/data.rs
--rw-r--r--   0     1001      127     8263 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/derive.rs
--rw-r--r--   0     1001      127     9053 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/discouraged.rs
--rw-r--r--   0     1001      127     1430 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/drops.rs
--rw-r--r--   0     1001      127    14065 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/error.rs
--rw-r--r--   0     1001      127     1584 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/export.rs
--rw-r--r--   0     1001      127   112265 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/expr.rs
--rw-r--r--   0     1001      127     3886 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/ext.rs
--rw-r--r--   0     1001      127     3749 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/file.rs
--rw-r--r--   0     1001      127    69617 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/clone.rs
--rw-r--r--   0     1001      127   126176 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/debug.rs
--rw-r--r--   0     1001      127    84324 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/eq.rs
--rw-r--r--   0     1001      127   102480 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/fold.rs
--rw-r--r--   0     1001      127    72585 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/hash.rs
--rw-r--r--   0     1001      127    97057 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/visit.rs
--rw-r--r--   0     1001      127   101467 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/visit_mut.rs
--rw-r--r--   0     1001      127      840 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/gen_helper.rs
--rw-r--r--   0     1001      127    41419 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/generics.rs
--rw-r--r--   0     1001      127     7922 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/group.rs
--rw-r--r--   0     1001      127     3122 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/ident.rs
--rw-r--r--   0     1001      127   117455 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/item.rs
--rw-r--r--   0     1001      127    31818 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/lib.rs
--rw-r--r--   0     1001      127     3825 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/lifetime.rs
--rw-r--r--   0     1001      127    49150 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/lit.rs
--rw-r--r--   0     1001      127     5345 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/lookahead.rs
--rw-r--r--   0     1001      127     7463 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/mac.rs
--rw-r--r--   0     1001      127     4653 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/macros.rs
--rw-r--r--   0     1001      127    14112 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/meta.rs
--rw-r--r--   0     1001      127     8429 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/op.rs
--rw-r--r--   0     1001      127    44840 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/parse.rs
--rw-r--r--   0     1001      127     3497 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/parse_macro_input.rs
--rw-r--r--   0     1001      127     5373 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/parse_quote.rs
--rw-r--r--   0     1001      127    29968 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/pat.rs
--rw-r--r--   0     1001      127    30668 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/path.rs
--rw-r--r--   0     1001      127      390 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/print.rs
--rw-r--r--   0     1001      127    29942 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/punctuated.rs
--rw-r--r--   0     1001      127     5815 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/restriction.rs
--rw-r--r--   0     1001      127       87 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/sealed.rs
--rw-r--r--   0     1001      127     1197 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/span.rs
--rw-r--r--   0     1001      127     3763 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/spanned.rs
--rw-r--r--   0     1001      127    15355 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/stmt.rs
--rw-r--r--   0     1001      127     1904 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/thread.rs
--rw-r--r--   0     1001      127    37419 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/token.rs
--rw-r--r--   0     1001      127     3727 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/tt.rs
--rw-r--r--   0     1001      127    41263 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/ty.rs
--rw-r--r--   0     1001      127     1216 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/verbatim.rs
--rw-r--r--   0     1001      127     2103 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/src/whitespace.rs
--rw-r--r--   0     1001      127    30636 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/common/eq.rs
--rw-r--r--   0     1001      127      760 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/common/mod.rs
--rw-r--r--   0     1001      127     1399 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/common/parse.rs
--rw-r--r--   0     1001      127   188757 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/debug/gen.rs
--rw-r--r--   0     1001      127     3199 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/debug/mod.rs
--rw-r--r--   0     1001      127     2275 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/macros/mod.rs
--rw-r--r--   0     1001      127       97 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/regression/issue1108.rs
--rw-r--r--   0     1001      127      932 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/regression/issue1235.rs
--rw-r--r--   0     1001      127      132 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/regression.rs
--rw-r--r--   0     1001      127    15054 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/repo/mod.rs
--rw-r--r--   0     1001      127      844 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/repo/progress.rs
--rw-r--r--   0     1001      127      728 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_asyncness.rs
--rw-r--r--   0     1001      127     4429 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_attribute.rs
--rw-r--r--   0     1001      127    21384 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_derive_input.rs
--rw-r--r--   0     1001      127     8562 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_expr.rs
--rw-r--r--   0     1001      127     8906 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_generics.rs
--rw-r--r--   0     1001      127     1518 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_grouping.rs
--rw-r--r--   0     1001      127     1288 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_ident.rs
--rw-r--r--   0     1001      127     7974 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_item.rs
--rw-r--r--   0     1001      127     1774 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_iterators.rs
--rw-r--r--   0     1001      127     8512 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_lit.rs
--rw-r--r--   0     1001      127     3128 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_meta.rs
--rw-r--r--   0     1001      127     2686 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_parse_buffer.rs
--rw-r--r--   0     1001      127      311 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_parse_stream.rs
--rw-r--r--   0     1001      127     3244 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_pat.rs
--rw-r--r--   0     1001      127     3700 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_path.rs
--rw-r--r--   0     1001      127    16304 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_precedence.rs
--rw-r--r--   0     1001      127     8290 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_receiver.rs
--rw-r--r--   0     1001      127     8115 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_round_trip.rs
--rw-r--r--   0     1001      127     1655 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_shebang.rs
--rw-r--r--   0     1001      127      915 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_should_parse.rs
--rw-r--r--   0     1001      127      780 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_size.rs
--rw-r--r--   0     1001      127     6398 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_stmt.rs
--rw-r--r--   0     1001      127      675 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_token_trees.rs
--rw-r--r--   0     1001      127    10949 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_ty.rs
--rw-r--r--   0     1001      127     3704 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_visibility.rs
--rw-r--r--   0     1001      127     1098 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/syn-2.0.38/tests/zzz_stable.rs
--rw-r--r--   0     1001      127     1250 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/.cargo-checksum.json
--rw-r--r--   0     1001      127     1012 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/Cargo.lock
--rw-r--r--   0     1001      127     1172 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/Cargo.toml
--rw-r--r--   0     1001      127    12243 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/LICENSE
--rw-r--r--   0     1001      127      957 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/README.md
--rw-r--r--   0     1001      127     5117 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/build.rs
--rw-r--r--   0     1001      127      208 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/examples/host.rs
--rw-r--r--   0     1001      127      405 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/examples/misc.rs
--rwxr-xr-x   0     1001      127      212 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/scripts/rust-targets.sh
--rw-r--r--   0     1001      127     3160 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/data_model.rs
--rw-r--r--   0     1001      127     1557 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/host.rs
--rw-r--r--   0     1001      127     3098 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/lib.rs
--rw-r--r--   0     1001      127     1208 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/parse_error.rs
--rw-r--r--   0     1001      127    54160 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/targets.rs
--rw-r--r--   0     1001      127    18653 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/triple.rs
--rw-r--r--   0     1001      127     1641 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/.cargo-checksum.json
--rw-r--r--   0     1001      127     1594 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/Cargo.toml
--rw-r--r--   0     1001      127     9723 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/LICENSE-MIT
--rw-r--r--   0     1001      127     2315 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/LICENSE-UNICODE
--rw-r--r--   0     1001      127    12498 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/README.md
--rw-r--r--   0     1001      127     4020 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/benches/xid.rs
--rw-r--r--   0     1001      127    12596 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/src/lib.rs
--rw-r--r--   0     1001      127    62702 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/src/tables.rs
--rw-r--r--   0     1001      127     1790 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/compare.rs
--rw-r--r--   0     1001      127      385 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/fst/mod.rs
--rw-r--r--   0     1001      127    73249 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/fst/xid_continue.fst
--rw-r--r--   0     1001      127    65487 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/fst/xid_start.fst
--rw-r--r--   0     1001      127      502 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/roaring/mod.rs
--rw-r--r--   0     1001      127     2456 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/static_size.rs
--rw-r--r--   0     1001      127      144 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/tables/mod.rs
--rw-r--r--   0     1001      127    23400 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/tables/tables.rs
--rw-r--r--   0     1001      127      179 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/trie/mod.rs
--rw-r--r--   0     1001      127    30278 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/trie/trie.rs
--rw-r--r--   0     1001      127      741 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/version_check-0.9.4/.cargo-checksum.json
--rw-r--r--   0     1001      127      890 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/version_check-0.9.4/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/version_check-0.9.4/LICENSE-APACHE
--rw-r--r--   0     1001      127     1085 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/version_check-0.9.4/LICENSE-MIT
--rw-r--r--   0     1001      127     2669 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/version_check-0.9.4/README.md
--rw-r--r--   0     1001      127     5425 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/version_check-0.9.4/src/channel.rs
--rw-r--r--   0     1001      127     6198 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/version_check-0.9.4/src/date.rs
--rw-r--r--   0     1001      127    19153 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/version_check-0.9.4/src/lib.rs
--rw-r--r--   0     1001      127    10435 2023-10-10 14:57:08.000000 orjson-3.9.8/include/cargo/version_check-0.9.4/src/version.rs
--rw-r--r--   0        0        0    49225 1970-01-01 00:00:00.000000 orjson-3.9.8/PKG-INFO
+-rw-r--r--   0        0        0     2776 1970-01-01 00:00:00.000000 orjson-3.9.9/Cargo.toml
+-rw-r--r--   0     1001      127    19063 2023-10-12 22:57:33.000000 orjson-3.9.9/CHANGELOG.md
+-rw-r--r--   0     1001      127    10847 2023-10-12 22:57:33.000000 orjson-3.9.9/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 22:57:33.000000 orjson-3.9.9/LICENSE-MIT
+-rw-r--r--   0     1001      127    47805 2023-10-12 22:57:33.000000 orjson-3.9.9/README.md
+-rw-r--r--   0     1001      127     8780 2023-10-12 22:57:33.000000 orjson-3.9.9/data/blns.txt.xz
+-rw-r--r--   0     1001      127   376512 2023-10-12 22:57:33.000000 orjson-3.9.9/data/canada.json.xz
+-rw-r--r--   0     1001      127    12336 2023-10-12 22:57:33.000000 orjson-3.9.9/data/citm_catalog.json.xz
+-rw-r--r--   0     1001      127     8264 2023-10-12 22:57:33.000000 orjson-3.9.9/data/github.json.xz
+-rw-r--r--   0     1001      127      592 2023-10-12 22:57:33.000000 orjson-3.9.9/data/issue331_1.json.xz
+-rw-r--r--   0     1001      127      592 2023-10-12 22:57:33.000000 orjson-3.9.9/data/issue331_2.json.xz
+-rw-r--r--   0     1001      127       60 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail01.json
+-rw-r--r--   0     1001      127       17 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail02.json
+-rw-r--r--   0     1001      127       37 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail03.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail04.json
+-rw-r--r--   0     1001      127       24 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail05.json
+-rw-r--r--   0     1001      127       26 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail06.json
+-rw-r--r--   0     1001      127       26 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail07.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail08.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail09.json
+-rw-r--r--   0     1001      127       58 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail10.json
+-rw-r--r--   0     1001      127       29 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail11.json
+-rw-r--r--   0     1001      127       31 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail12.json
+-rw-r--r--   0     1001      127       43 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail13.json
+-rw-r--r--   0     1001      127       31 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail14.json
+-rw-r--r--   0     1001      127       34 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail15.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail16.json
+-rw-r--r--   0     1001      127       34 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail17.json
+-rw-r--r--   0     1001      127       50 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail18.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail19.json
+-rw-r--r--   0     1001      127       23 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail20.json
+-rw-r--r--   0     1001      127       32 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail21.json
+-rw-r--r--   0     1001      127       33 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail22.json
+-rw-r--r--   0     1001      127       20 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail23.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail24.json
+-rw-r--r--   0     1001      127       29 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail25.json
+-rw-r--r--   0     1001      127       38 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail26.json
+-rw-r--r--   0     1001      127       14 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail27.json
+-rw-r--r--   0     1001      127       15 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail28.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail29.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail30.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail31.json
+-rw-r--r--   0     1001      127       40 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail32.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/fail33.json
+-rw-r--r--   0     1001      127     1441 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/pass01.json
+-rw-r--r--   0     1001      127       52 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/pass02.json
+-rw-r--r--   0     1001      127      148 2023-10-12 22:57:33.000000 orjson-3.9.9/data/jsonchecker/pass03.json
+-rw-r--r--   0     1001      127       14 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_double_huge_neg_exp.json
+-rw-r--r--   0     1001      127      137 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_huge_exp.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_neg_int_huge_exp.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_pos_double_huge_exp.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_real_neg_overflow.json
+-rw-r--r--   0     1001      127       15 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_real_pos_overflow.json
+-rw-r--r--   0     1001      127       15 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_real_underflow.json
+-rw-r--r--   0     1001      127       33 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_too_big_neg_int.json
+-rw-r--r--   0     1001      127       23 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_too_big_pos_int.json
+-rw-r--r--   0     1001      127       51 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_number_very_big_negative_int.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_object_key_lone_2nd_surrogate.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_1st_surrogate_but_2nd_missing.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_1st_valid_surrogate_2nd_invalid.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_UTF-16LE_with_BOM.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_UTF-8_invalid_sequence.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_UTF8_surrogate_U+D800.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_incomplete_surrogate_and_escape_valid.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_incomplete_surrogate_pair.json
+-rw-r--r--   0     1001      127       18 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_incomplete_surrogates_escape_valid.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_invalid_lonely_surrogate.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_invalid_surrogate.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_invalid_utf-8.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_inverted_surrogates_U+1D11E.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_iso_latin_1.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_lone_second_surrogate.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_lone_utf8_continuation_byte.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_not_in_unicode_range.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_overlong_sequence_2_bytes.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_overlong_sequence_6_bytes.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_overlong_sequence_6_bytes_null.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_truncated-utf-8.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_utf16BE_no_BOM.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_string_utf16LE_no_BOM.json
+-rw-r--r--   0     1001      127       80 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_structure_500_nested_arrays.json.xz
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/i_structure_UTF-8_BOM_empty_object.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_1_true_without_comma.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_a_invalid_utf8.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_colon_instead_of_comma.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_comma_after_close.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_comma_and_number.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_double_comma.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_double_extra_comma.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_extra_close.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_extra_comma.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_incomplete.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_incomplete_invalid_value.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_inner_array_no_comma.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_invalid_utf8.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_items_separated_by_semicolon.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_just_comma.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_just_minus.json
+-rw-r--r--   0     1001      127        9 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_missing_value.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_newlines_unclosed.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_number_and_comma.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_number_and_several_commas.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_spaces_vertical_tab_formfeed.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_star_inside.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_unclosed.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_unclosed_trailing_comma.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_unclosed_with_new_lines.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_array_unclosed_with_object_inside.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_incomplete_false.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_incomplete_null.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_incomplete_true.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_multidigit_number_then_00.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_++.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_+1.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_+Inf.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_-01.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_-1.0..json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_-2..json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_-NaN.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_.-1.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_.2e-3.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_0.1.2.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_0.3e+.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_0.3e.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_0.e1.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_0_capital_E+.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_0_capital_E.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_0e+.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_0e.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_1.0e+.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_1.0e-.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_1.0e.json
+-rw-r--r--   0     1001      127        9 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_1_000.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_1eE2.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_2.e+3.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_2.e-3.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_2.e3.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_9.e+.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_Inf.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_NaN.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_U+FF11_fullwidth_digit_one.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_expression.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_hex_1_digit.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_hex_2_digits.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_infinity.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_invalid+-.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_invalid-negative-real.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_invalid-utf-8-in-bigger-int.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_invalid-utf-8-in-exponent.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_invalid-utf-8-in-int.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_minus_infinity.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_minus_sign_with_trailing_garbage.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_minus_space_1.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_neg_int_starting_with_zero.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_neg_real_without_int_part.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_neg_with_garbage_at_end.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_real_garbage_after_e.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_real_with_invalid_utf8_after_e.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_real_without_fractional_part.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_starting_with_dot.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_with_alpha.json
+-rw-r--r--   0     1001      127       25 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_with_alpha_char.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_number_with_leading_zero.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_bad_value.json
+-rw-r--r--   0     1001      127        9 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_bracket_key.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_comma_instead_of_colon.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_double_colon.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_emoji.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_garbage_at_end.json
+-rw-r--r--   0     1001      127       14 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_key_with_single_quotes.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_lone_continuation_byte_in_key_and_trailing_comma.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_missing_colon.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_missing_key.json
+-rw-r--r--   0     1001      127        9 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_missing_semicolon.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_missing_value.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_no-colon.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_non_string_key.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_non_string_key_but_huge_number_instead.json
+-rw-r--r--   0     1001      127       21 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_repeated_null_null.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_several_trailing_commas.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_single_quote.json
+-rw-r--r--   0     1001      127        9 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_trailing_comma.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_trailing_comment.json
+-rw-r--r--   0     1001      127       14 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_trailing_comment_open.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_trailing_comment_slash_open.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_trailing_comment_slash_open_incomplete.json
+-rw-r--r--   0     1001      127       18 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_two_commas_in_a_row.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_unquoted_key.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_unterminated-value.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_with_single_string.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_object_with_trailing_garbage.json
+-rw-r--r--   0     1001      127        1 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_single_space.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_1_surrogate_then_escape.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_1_surrogate_then_escape_u.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_1_surrogate_then_escape_u1.json
+-rw-r--r--   0     1001      127       14 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_1_surrogate_then_escape_u1x.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_accentuated_char_no_quotes.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_backslash_00.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_escape_x.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_escaped_backslash_bad.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_escaped_ctrl_char_tab.json
+-rw-r--r--   0     1001      127        9 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_escaped_emoji.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_incomplete_escape.json
+-rw-r--r--   0     1001      127        9 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_incomplete_escaped_character.json
+-rw-r--r--   0     1001      127       14 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_incomplete_surrogate.json
+-rw-r--r--   0     1001      127       18 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_incomplete_surrogate_escape_invalid.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_invalid-utf-8-in-escape.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_invalid_backslash_esc.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_invalid_unicode_escape.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_invalid_utf8_after_escape.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_leading_uescaped_thinspace.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_no_quotes_with_bad_escape.json
+-rw-r--r--   0     1001      127        1 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_single_doublequote.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_single_quote.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_single_string_no_double_quotes.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_start_escape_unclosed.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_unescaped_crtl_char.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_unescaped_newline.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_unescaped_tab.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_unicode_CapitalU.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_string_with_trailing_garbage.json
+-rw-r--r--   0     1001      127      148 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_100000_opening_arrays.json.xz
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_U+2060_word_joined.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_UTF8_BOM_no_data.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_angle_bracket_..json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_angle_bracket_null.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_array_trailing_garbage.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_array_with_extra_array_close.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_array_with_unclosed_string.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_ascii-unicode-identifier.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_capitalized_True.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_close_unopened_array.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_comma_instead_of_closing_brace.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_double_array.json
+-rw-r--r--   0     1001      127        1 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_end_array.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_incomplete_UTF8_BOM.json
+-rw-r--r--   0     1001      127        1 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_lone-invalid-utf-8.json
+-rw-r--r--   0     1001      127        1 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_lone-open-bracket.json
+-rw-r--r--   0     1001      127        0 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_no_data.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_null-byte-outside-string.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_number_with_trailing_garbage.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_object_followed_by_closing_object.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_object_unclosed_no_value.json
+-rw-r--r--   0     1001      127       20 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_object_with_comment.json
+-rw-r--r--   0     1001      127       15 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_object_with_trailing_garbage.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_array_apostrophe.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_array_comma.json
+-rw-r--r--   0     1001      127      176 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_array_object.json.xz
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_array_open_object.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_array_open_string.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_array_string.json
+-rw-r--r--   0     1001      127        1 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_object.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_object_close_array.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_object_comma.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_object_open_array.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_object_open_string.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_object_string_with_apostrophes.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_open_open.json
+-rw-r--r--   0     1001      127        1 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_single_eacute.json
+-rw-r--r--   0     1001      127        1 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_single_star.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_trailing_#.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_uescaped_LF_before_string.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_unclosed_array.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_unclosed_array_partial_null.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_unclosed_array_unfinished_false.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_unclosed_array_unfinished_true.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_unclosed_object.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_unicode-identifier.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_whitespace_U+2060_word_joiner.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/n_structure_whitespace_formfeed.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_arraysWithSpaces.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_empty-string.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_empty.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_ending_with_newline.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_false.json
+-rw-r--r--   0     1001      127       18 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_heterogeneous.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_null.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_with_1_and_newline.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_with_leading_space.json
+-rw-r--r--   0     1001      127       20 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_with_several_null.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_array_with_trailing_space.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_0e+1.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_0e1.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_after_space.json
+-rw-r--r--   0     1001      127       84 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_double_close_to_zero.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_int_with_exp.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_minus_zero.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_negative_int.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_negative_one.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_negative_zero.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_real_capital_e.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_real_capital_e_neg_exp.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_real_capital_e_pos_exp.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_real_exponent.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_real_fraction_exponent.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_real_neg_exp.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_real_pos_exponent.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_simple_int.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_number_simple_real.json
+-rw-r--r--   0     1001      127       26 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_basic.json
+-rw-r--r--   0     1001      127       17 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_duplicated_key.json
+-rw-r--r--   0     1001      127       17 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_duplicated_key_and_value.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_empty.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_empty_key.json
+-rw-r--r--   0     1001      127       20 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_escaped_null_in_key.json
+-rw-r--r--   0     1001      127       35 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_extreme_numbers.json
+-rw-r--r--   0     1001      127      108 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_long_strings.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_simple.json
+-rw-r--r--   0     1001      127      110 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_string_unicode.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_object_with_newlines.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_1_2_3_bytes_UTF-8_sequences.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_accepted_surrogate_pair.json
+-rw-r--r--   0     1001      127       28 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_accepted_surrogate_pairs.json
+-rw-r--r--   0     1001      127       20 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_allowed_escapes.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_backslash_and_u_escaped_zero.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_backslash_doublequotes.json
+-rw-r--r--   0     1001      127       17 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_comments.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_double_escape_a.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_double_escape_n.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_escaped_control_character.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_escaped_noncharacter.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_in_array.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_in_array_with_leading_space.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_last_surrogates_1_and_2.json
+-rw-r--r--   0     1001      127       17 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_nbsp_uescaped.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_nonCharacterInUTF-8_U+10FFFF.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_nonCharacterInUTF-8_U+FFFF.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_null_escape.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_one-byte-utf-8.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_pi.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_reservedCharacterInUTF-8_U+1BFFF.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_simple_ascii.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_space.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_surrogates_U+1D11E_MUSICAL_SYMBOL_G_CLEF.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_three-byte-utf-8.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_two-byte-utf-8.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_u+2028_line_sep.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_u+2029_par_sep.json
+-rw-r--r--   0     1001      127       28 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_uEscape.json
+-rw-r--r--   0     1001      127       17 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_uescaped_newline.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unescaped_char_delete.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicode.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicodeEscapedBackslash.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicode_2.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicode_U+10FFFE_nonchar.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicode_U+1FFFE_nonchar.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicode_U+200B_ZERO_WIDTH_SPACE.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicode_U+2064_invisible_plus.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicode_U+FDD0_nonchar.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicode_U+FFFE_nonchar.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_unicode_escaped_double_quote.json
+-rw-r--r--   0     1001      127       11 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_utf8.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_string_with_del_character.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_lonely_false.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_lonely_int.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_lonely_negative_real.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_lonely_null.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_lonely_string.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_lonely_true.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_string_empty.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_trailing_newline.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_true_in_array.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/parsing/y_structure_whitespace_array.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip01.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip02.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip03.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip04.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip05.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip06.json
+-rw-r--r--   0     1001      127        2 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip07.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip08.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip09.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip10.json
+-rw-r--r--   0     1001      127        4 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip11.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip12.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip13.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip14.json
+-rw-r--r--   0     1001      127        3 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip15.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip16.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip17.json
+-rw-r--r--   0     1001      127       21 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip18.json
+-rw-r--r--   0     1001      127       21 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip19.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip20.json
+-rw-r--r--   0     1001      127        6 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip21.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip22.json
+-rw-r--r--   0     1001      127        9 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip23.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip24.json
+-rw-r--r--   0     1001      127       24 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip25.json
+-rw-r--r--   0     1001      127       25 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip26.json
+-rw-r--r--   0     1001      127       24 2023-10-12 22:57:33.000000 orjson-3.9.9/data/roundtrip/roundtrip27.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/number_1.0.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/number_1.000000000000000005.json
+-rw-r--r--   0     1001      127       19 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/number_1000000000000000.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/number_10000000000000000999.json
+-rw-r--r--   0     1001      127        8 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/number_1e-999.json
+-rw-r--r--   0     1001      127        5 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/number_1e6.json
+-rw-r--r--   0     1001      127       24 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/object_key_nfc_nfd.json
+-rw-r--r--   0     1001      127       24 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/object_key_nfd_nfc.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/object_same_key_different_values.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/object_same_key_same_value.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/object_same_key_unclear_values.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/string_1_escaped_invalid_codepoint.json
+-rw-r--r--   0     1001      127        7 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/string_1_invalid_codepoint.json
+-rw-r--r--   0     1001      127       16 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/string_2_escaped_invalid_codepoints.json
+-rw-r--r--   0     1001      127       10 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/string_2_invalid_codepoints.json
+-rw-r--r--   0     1001      127       22 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/string_3_escaped_invalid_codepoints.json
+-rw-r--r--   0     1001      127       13 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/string_3_invalid_codepoints.json
+-rw-r--r--   0     1001      127       12 2023-10-12 22:57:33.000000 orjson-3.9.9/data/transform/string_with_escaped_NULL.json
+-rw-r--r--   0     1001      127    34780 2023-10-12 22:57:33.000000 orjson-3.9.9/data/twitter.json.xz
+-rw-r--r--   0     1001      127   346765 2023-10-12 22:57:33.000000 orjson-3.9.9/include/yyjson/yyjson.c
+-rw-r--r--   0     1001      127   303585 2023-10-12 22:57:33.000000 orjson-3.9.9/include/yyjson/yyjson.h
+-rw-r--r--   0     1001      127     1374 2023-10-12 22:57:33.000000 orjson-3.9.9/src/deserialize/cache.rs
+-rw-r--r--   0     1001      127     1034 2023-10-12 22:57:33.000000 orjson-3.9.9/src/deserialize/deserializer.rs
+-rw-r--r--   0     1001      127     3096 2023-10-12 22:57:33.000000 orjson-3.9.9/src/deserialize/error.rs
+-rw-r--r--   0     1001      127     4041 2023-10-12 22:57:33.000000 orjson-3.9.9/src/deserialize/json.rs
+-rw-r--r--   0     1001      127      312 2023-10-12 22:57:33.000000 orjson-3.9.9/src/deserialize/mod.rs
+-rw-r--r--   0     1001      127     1994 2023-10-12 22:57:33.000000 orjson-3.9.9/src/deserialize/pyobject.rs
+-rw-r--r--   0     1001      127     3192 2023-10-12 22:57:33.000000 orjson-3.9.9/src/deserialize/utf8.rs
+-rw-r--r--   0     1001      127     5992 2023-10-12 22:57:33.000000 orjson-3.9.9/src/deserialize/yyjson.rs
+-rw-r--r--   0     1001      127      727 2023-10-12 22:57:33.000000 orjson-3.9.9/src/ffi/buffer.rs
+-rw-r--r--   0     1001      127      469 2023-10-12 22:57:33.000000 orjson-3.9.9/src/ffi/bytes.rs
+-rw-r--r--   0     1001      127     4076 2023-10-12 22:57:33.000000 orjson-3.9.9/src/ffi/fragment.rs
+-rw-r--r--   0     1001      127     1016 2023-10-12 22:57:33.000000 orjson-3.9.9/src/ffi/list.rs
+-rw-r--r--   0     1001      127     1056 2023-10-12 22:57:33.000000 orjson-3.9.9/src/ffi/long.rs
+-rw-r--r--   0     1001      127      320 2023-10-12 22:57:33.000000 orjson-3.9.9/src/ffi/mod.rs
+-rw-r--r--   0     1001      127     1884 2023-10-12 22:57:33.000000 orjson-3.9.9/src/ffi/yyjson.rs
+-rw-r--r--   0     1001      127    11983 2023-10-12 22:57:33.000000 orjson-3.9.9/src/lib.rs
+-rw-r--r--   0     1001      127     1133 2023-10-12 22:57:33.000000 orjson-3.9.9/src/opt.rs
+-rw-r--r--   0     1001      127     2591 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/error.rs
+-rw-r--r--   0     1001      127    34700 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/json.rs
+-rw-r--r--   0     1001      127      144 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/mod.rs
+-rw-r--r--   0     1001      127     7518 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/dataclass.rs
+-rw-r--r--   0     1001      127     7955 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/datetime.rs
+-rw-r--r--   0     1001      127     6099 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/datetimelike.rs
+-rw-r--r--   0     1001      127     2549 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/default.rs
+-rw-r--r--   0     1001      127    13553 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/dict.rs
+-rw-r--r--   0     1001      127      544 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/float.rs
+-rw-r--r--   0     1001      127     1570 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/fragment.rs
+-rw-r--r--   0     1001      127     2233 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/int.rs
+-rw-r--r--   0     1001      127     1728 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/list.rs
+-rw-r--r--   0     1001      127      848 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/mod.rs
+-rw-r--r--   0     1001      127      405 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/none.rs
+-rw-r--r--   0     1001      127    36974 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/numpy.rs
+-rw-r--r--   0     1001      127      544 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/pybool.rs
+-rw-r--r--   0     1001      127     1323 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/pyenum.rs
+-rw-r--r--   0     1001      127     1606 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/tuple.rs
+-rw-r--r--   0     1001      127     1299 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/unicode.rs
+-rw-r--r--   0     1001      127     2012 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/per_type/uuid.rs
+-rw-r--r--   0     1001      127     7647 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/serializer.rs
+-rw-r--r--   0     1001      127     5480 2023-10-12 22:57:33.000000 orjson-3.9.9/src/serialize/writer.rs
+-rw-r--r--   0     1001      127     1053 2023-10-12 22:57:33.000000 orjson-3.9.9/src/str/check.rs
+-rw-r--r--   0     1001      127     2839 2023-10-12 22:57:33.000000 orjson-3.9.9/src/str/create.rs
+-rw-r--r--   0     1001      127     1928 2023-10-12 22:57:33.000000 orjson-3.9.9/src/str/ffi.rs
+-rw-r--r--   0     1001      127      135 2023-10-12 22:57:33.000000 orjson-3.9.9/src/str/mod.rs
+-rw-r--r--   0     1001      127    13435 2023-10-12 22:57:33.000000 orjson-3.9.9/src/typeref.rs
+-rw-r--r--   0     1001      127     4946 2023-10-12 22:57:33.000000 orjson-3.9.9/src/util.rs
+-rw-r--r--   0     1001      127        0 2023-10-12 22:57:33.000000 orjson-3.9.9/test/__init__.py
+-rw-r--r--   0     1001      127      501 2023-10-12 22:57:33.000000 orjson-3.9.9/test/requirements.txt
+-rw-r--r--   0     1001      127     6205 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_api.py
+-rw-r--r--   0     1001      127     1319 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_append_newline.py
+-rw-r--r--   0     1001      127      680 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_canonical.py
+-rw-r--r--   0     1001      127     2097 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_circular.py
+-rw-r--r--   0     1001      127     7288 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_dataclass.py
+-rw-r--r--   0     1001      127    22713 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_datetime.py
+-rw-r--r--   0     1001      127     9050 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_default.py
+-rw-r--r--   0     1001      127     1926 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_dict.py
+-rw-r--r--   0     1001      127     2630 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_enum.py
+-rw-r--r--   0     1001      127     5444 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_error.py
+-rw-r--r--   0     1001      127     1117 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_fake.py
+-rw-r--r--   0     1001      127     1492 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_fixture.py
+-rw-r--r--   0     1001      127    40451 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_fragment.py
+-rw-r--r--   0     1001      127     2496 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_indent.py
+-rw-r--r--   0     1001      127      274 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_issue221.py
+-rw-r--r--   0     1001      127    11816 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_issue331.py
+-rw-r--r--   0     1001      127     6187 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_jsonchecker.py
+-rw-r--r--   0     1001      127     8356 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_memory.py
+-rw-r--r--   0     1001      127     9175 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_non_str_keys.py
+-rw-r--r--   0     1001      127    26642 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_numpy.py
+-rw-r--r--   0     1001      127    56984 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_parsing.py
+-rw-r--r--   0     1001      127      210 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_reentrant.py
+-rw-r--r--   0     1001      127     3994 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_roundtrip.py
+-rw-r--r--   0     1001      127     1656 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_sort_keys.py
+-rw-r--r--   0     1001      127     3126 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_subclass.py
+-rw-r--r--   0     1001      127     3725 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_transform.py
+-rw-r--r--   0     1001      127    16489 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_type.py
+-rw-r--r--   0     1001      127      453 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_typeddict.py
+-rw-r--r--   0     1001      127    10773 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_ujson.py
+-rw-r--r--   0     1001      127     3445 2023-10-12 22:57:33.000000 orjson-3.9.9/test/test_uuid.py
+-rw-r--r--   0     1001      127      948 2023-10-12 22:57:33.000000 orjson-3.9.9/test/util.py
+-rw-r--r--   0     1001      127     8352 2023-10-12 22:57:33.000000 orjson-3.9.9/Cargo.lock
+-rw-r--r--   0     1001      127     1568 2023-10-12 22:57:33.000000 orjson-3.9.9/pyproject.toml
+-rw-r--r--   0     1001      127        0 2023-10-12 22:57:33.000000 orjson-3.9.9/pysrc/orjson/py.typed
+-rw-r--r--   0     1001      127      589 2023-10-12 22:57:33.000000 orjson-3.9.9/pysrc/orjson/__init__.py
+-rw-r--r--   0     1001      127      761 2023-10-12 22:57:33.000000 orjson-3.9.9/pysrc/orjson/__init__.pyi
+-rw-r--r--   0     1001      127      108 2023-10-12 23:01:36.000000 orjson-3.9.9/.cargo/config.toml
+-rw-r--r--   0     1001      127     2061 2023-10-12 22:57:33.000000 orjson-3.9.9/build.rs
+-rw-r--r--   0     1001      127     1772 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/.cargo-checksum.json
+-rw-r--r--   0     1001      127     2849 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/Cargo.toml
+-rw-r--r--   0     1001      127     9236 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/FAQ.md
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1057 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/LICENSE-MIT
+-rw-r--r--   0     1001      127     5683 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/README.md
+-rw-r--r--   0     1001      127      823 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/build.rs
+-rw-r--r--   0     1001      127       16 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/rustfmt.toml
+-rw-r--r--   0     1001      127    13200 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/aes_hash.rs
+-rw-r--r--   0     1001      127     4503 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/convert.rs
+-rw-r--r--   0     1001      127    12167 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/fallback_hash.rs
+-rw-r--r--   0     1001      127    14078 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/hash_map.rs
+-rw-r--r--   0     1001      127    16962 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/hash_quality_test.rs
+-rw-r--r--   0     1001      127     9372 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/hash_set.rs
+-rw-r--r--   0     1001      127    12338 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/lib.rs
+-rw-r--r--   0     1001      127    12446 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/operations.rs
+-rw-r--r--   0     1001      127    18456 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/random_state.rs
+-rw-r--r--   0     1001      127     7158 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/src/specialize.rs
+-rw-r--r--   0     1001      127     5968 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/tests/bench.rs
+-rw-r--r--   0     1001      127    11469 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/tests/map_tests.rs
+-rw-r--r--   0     1001      127     2107 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ahash-0.8.3/tests/nopanic.rs
+-rw-r--r--   0     1001      127     1431 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/.cargo-checksum.json
+-rw-r--r--   0     1001      127     9959 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/CHANGELOG.md
+-rw-r--r--   0     1001      127     1644 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1071 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/LICENSE-MIT
+-rw-r--r--   0     1001      127      958 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/README.md
+-rw-r--r--   0     1001      127     1963 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/benches/arraystring.rs
+-rw-r--r--   0     1001      127     1739 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/benches/extend.rs
+-rw-r--r--   0     1001      127    19612 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/array_string.rs
+-rw-r--r--   0     1001      127    38497 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/arrayvec.rs
+-rw-r--r--   0     1001      127     2339 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/arrayvec_impl.rs
+-rw-r--r--   0     1001      127     3315 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/char.rs
+-rw-r--r--   0     1001      127     1193 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/errors.rs
+-rw-r--r--   0     1001      127     1640 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/lib.rs
+-rw-r--r--   0     1001      127      325 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/utils.rs
+-rw-r--r--   0     1001      127     1809 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/tests/serde.rs
+-rw-r--r--   0     1001      127    19485 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/arrayvec-0.7.4/tests/tests.rs
+-rw-r--r--   0     1001      127      839 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1196 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/Cargo.toml
+-rw-r--r--   0     1001      127     1896 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/README.md
+-rw-r--r--   0     1001      127     1310 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/capacity.rs
+-rw-r--r--   0     1001      127     5655 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/entry.rs
+-rw-r--r--   0     1001      127     6633 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/indices.rs
+-rw-r--r--   0     1001      127     3853 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/iter.rs
+-rwxr-xr-x   0     1001      127    34057 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/lib.rs
+-rw-r--r--   0     1001      127     8018 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/replacement/lru.rs
+-rw-r--r--   0     1001      127     2592 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/replacement.rs
+-rw-r--r--   0     1001      127     1263 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/.cargo-checksum.json
+-rw-r--r--   0     1001      127      151 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/Cargo.lock
+-rw-r--r--   0     1001      127      861 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1054 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/LICENSE-MIT
+-rw-r--r--   0     1001      127     2946 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/README.md
+-rw-r--r--   0     1001      127      235 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/examples/integers.rs
+-rw-r--r--   0     1001      127      672 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/examples/paths.rs
+-rw-r--r--   0     1001      127      826 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/examples/traits.rs
+-rw-r--r--   0     1001      127      223 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/examples/versions.rs
+-rw-r--r--   0     1001      127     1414 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/src/error.rs
+-rw-r--r--   0     1001      127    14815 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/src/lib.rs
+-rw-r--r--   0     1001      127     5038 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/src/tests.rs
+-rw-r--r--   0     1001      127     2092 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/src/version.rs
+-rw-r--r--   0     1001      127     1184 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/autocfg-1.1.0/tests/rustflags.rs
+-rw-r--r--   0     1001      127     1069 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1237 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/Cargo.toml
+-rw-r--r--   0     1001      127    10856 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1100 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/LICENSE-MIT
+-rw-r--r--   0     1001      127     4394 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/README.md
+-rw-r--r--   0     1001      127     4552 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/benches/bench.rs
+-rwxr-xr-x   0     1001      127      363 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/ci/miri.sh
+-rw-r--r--   0     1001      127    13270 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/src/generic.rs
+-rw-r--r--   0     1001      127     1670 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/src/lean.rs
+-rw-r--r--   0     1001      127     7781 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/src/lib.rs
+-rw-r--r--   0     1001      127     3434 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/src/serde.rs
+-rw-r--r--   0     1001      127     5532 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/src/traits.rs
+-rw-r--r--   0     1001      127     1027 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/beef-0.5.2/src/wide.rs
+-rw-r--r--   0     1001      127     1357 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1412 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/Cargo.toml
+-rw-r--r--   0     1001      127    11357 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/LICENSE.Apache2
+-rw-r--r--   0     1001      127     1068 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/LICENSE.MIT
+-rw-r--r--   0     1001      127     2866 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/README.md
+-rw-r--r--   0     1001      127     3054 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/benches/bench.rs
+-rw-r--r--   0     1001      127      369 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/ci/miri.sh
+-rw-r--r--   0     1001      127     3619 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/src/integer_simd.rs
+-rw-r--r--   0     1001      127     4785 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/src/lib.rs
+-rw-r--r--   0     1001      127     1351 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/src/naive.rs
+-rw-r--r--   0     1001      127     4757 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/aarch64.rs
+-rw-r--r--   0     1001      127     4512 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/generic.rs
+-rw-r--r--   0     1001      127      657 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/mod.rs
+-rw-r--r--   0     1001      127     4597 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/x86_avx2.rs
+-rw-r--r--   0     1001      127     4607 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/x86_sse2.rs
+-rw-r--r--   0     1001      127     2415 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/bytecount-0.6.4/tests/check.rs
+-rw-r--r--   0     1001      127      661 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/castaway-0.2.2/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1028 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/castaway-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      127     1075 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/castaway-0.2.2/LICENSE
+-rw-r--r--   0     1001      127     3446 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/castaway-0.2.2/README.md
+-rw-r--r--   0     1001      127     7141 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/castaway-0.2.2/src/internal.rs
+-rw-r--r--   0     1001      127    17016 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/castaway-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      127     3494 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/castaway-0.2.2/src/lifetime_free.rs
+-rw-r--r--   0     1001      127     3782 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/castaway-0.2.2/src/utils.rs
+-rw-r--r--   0     1001      127     1963 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/.cargo-checksum.json
+-rw-r--r--   0     1001      127     2886 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/Cargo.lock
+-rw-r--r--   0     1001      127     1283 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1057 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/LICENSE-MIT
+-rw-r--r--   0     1001      127     8224 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/README.md
+-rw-r--r--   0     1001      127     1921 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/bin/gcc-shim.rs
+-rw-r--r--   0     1001      127     3917 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/com.rs
+-rw-r--r--   0     1001      127   153381 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/lib.rs
+-rw-r--r--   0     1001      127     3087 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/os_pipe/unix.rs
+-rw-r--r--   0     1001      127      783 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/os_pipe/windows.rs
+-rw-r--r--   0     1001      127      971 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/os_pipe.rs
+-rw-r--r--   0     1001      127     6402 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/registry.rs
+-rw-r--r--   0     1001      127     8886 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/setup_config.rs
+-rw-r--r--   0     1001      127     6483 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/vs_instances.rs
+-rw-r--r--   0     1001      127     4539 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/winapi.rs
+-rw-r--r--   0     1001      127    34449 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/windows_registry.rs
+-rw-r--r--   0     1001      127     5154 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/src/windows_sys.rs
+-rw-r--r--   0     1001      127     2739 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/tests/cc_env.rs
+-rw-r--r--   0     1001      127      415 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/tests/cflags.rs
+-rw-r--r--   0     1001      127      431 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/tests/cxxflags.rs
+-rw-r--r--   0     1001      127     5205 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/tests/support/mod.rs
+-rw-r--r--   0     1001      127    10318 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cc-1.0.83/tests/test.rs
+-rw-r--r--   0     1001      127      577 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cfg-if-1.0.0/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1308 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cfg-if-1.0.0/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cfg-if-1.0.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1057 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cfg-if-1.0.0/LICENSE-MIT
+-rw-r--r--   0     1001      127     1123 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cfg-if-1.0.0/README.md
+-rw-r--r--   0     1001      127     4893 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cfg-if-1.0.0/src/lib.rs
+-rw-r--r--   0     1001      127      245 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/cfg-if-1.0.0/tests/xcrate.rs
+-rw-r--r--   0     1001      127     4953 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/.cargo-checksum.json
+-rw-r--r--   0     1001      127    23977 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/CHANGELOG.md
+-rw-r--r--   0     1001      127      768 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/CITATION.cff
+-rw-r--r--   0     1001      127     2874 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/Cargo.toml
+-rw-r--r--   0     1001      127    12307 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/LICENSE.txt
+-rw-r--r--   0     1001      127     3846 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/README.md
+-rw-r--r--   0     1001      127      203 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/appveyor.yml
+-rw-r--r--   0     1001      127      354 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/deny.toml
+-rw-r--r--   0     1001      127       29 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/rustfmt.toml
+-rw-r--r--   0     1001      127    22157 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/date.rs
+-rw-r--r--   0     1001      127    58971 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/datetime/mod.rs
+-rw-r--r--   0     1001      127     3826 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/datetime/rustc_serialize.rs
+-rw-r--r--   0     1001      127    40754 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/datetime/serde.rs
+-rw-r--r--   0     1001      127    56886 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/datetime/tests.rs
+-rw-r--r--   0     1001      127    29113 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/duration.rs
+-rw-r--r--   0     1001      127    40713 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/formatting.rs
+-rw-r--r--   0     1001      127     2994 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/locales.rs
+-rw-r--r--   0     1001      127    20158 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/mod.rs
+-rw-r--r--   0     1001      127    96229 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/parse.rs
+-rw-r--r--   0     1001      127    58073 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/parsed.rs
+-rw-r--r--   0     1001      127    14584 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/scan.rs
+-rw-r--r--   0     1001      127    45514 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/strftime.rs
+-rw-r--r--   0     1001      127    29231 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/lib.rs
+-rw-r--r--   0     1001      127    12973 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/month.rs
+-rw-r--r--   0     1001      127   122213 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/date.rs
+-rw-r--r--   0     1001      127    80792 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/datetime/mod.rs
+-rw-r--r--   0     1001      127     1940 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/datetime/rustc_serialize.rs
+-rw-r--r--   0     1001      127    38392 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/datetime/serde.rs
+-rw-r--r--   0     1001      127    18291 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/datetime/tests.rs
+-rw-r--r--   0     1001      127    36370 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/internals.rs
+-rw-r--r--   0     1001      127     7118 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/isoweek.rs
+-rw-r--r--   0     1001      127     1324 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/mod.rs
+-rw-r--r--   0     1001      127    61287 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/time/mod.rs
+-rw-r--r--   0     1001      127      780 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/time/rustc_serialize.rs
+-rw-r--r--   0     1001      127     1854 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/time/serde.rs
+-rw-r--r--   0     1001      127    13167 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/time/tests.rs
+-rw-r--r--   0     1001      127     9661 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/fixed.rs
+-rw-r--r--   0     1001      127     8606 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/mod.rs
+-rw-r--r--   0     1001      127     3499 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/tz_info/mod.rs
+-rw-r--r--   0     1001      127    11352 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/tz_info/parser.rs
+-rw-r--r--   0     1001      127    39593 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/tz_info/rule.rs
+-rw-r--r--   0     1001      127    36987 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/tz_info/timezone.rs
+-rw-r--r--   0     1001      127     6416 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/unix.rs
+-rw-r--r--   0     1001      127     1741 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/win_bindings.rs
+-rw-r--r--   0     1001      127      244 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/win_bindings.txt
+-rw-r--r--   0     1001      127     5229 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/windows.rs
+-rw-r--r--   0     1001      127    24070 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/mod.rs
+-rw-r--r--   0     1001      127     4314 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/utc.rs
+-rw-r--r--   0     1001      127    26668 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/round.rs
+-rw-r--r--   0     1001      127    15140 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/traits.rs
+-rw-r--r--   0     1001      127    12970 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/src/weekday.rs
+-rw-r--r--   0     1001      127       83 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/taplo.toml
+-rw-r--r--   0     1001      127     6102 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/tests/dateutils.rs
+-rw-r--r--   0     1001      127     2795 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/tests/wasm.rs
+-rw-r--r--   0     1001      127      746 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/chrono-0.4.31/tests/win_bindings.rs
+-rw-r--r--   0     1001      127     2357 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/.cargo-checksum.json
+-rw-r--r--   0     1001      127     2567 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/Cargo.toml
+-rw-r--r--   0     1001      127     1073 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/LICENSE
+-rw-r--r--   0     1001      127    11977 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/README.md
+-rw-r--r--   0     1001      127     1445 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/arbitrary.rs
+-rw-r--r--   0     1001      127     4030 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/bytes.rs
+-rw-r--r--   0     1001      127      884 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/markup.rs
+-rw-r--r--   0     1001      127      425 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/mod.rs
+-rw-r--r--   0     1001      127     1512 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/proptest.rs
+-rw-r--r--   0     1001      127     1491 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/quickcheck.rs
+-rw-r--r--   0     1001      127     3769 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/rkyv.rs
+-rw-r--r--   0     1001      127     5217 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/serde.rs
+-rw-r--r--   0     1001      127     2702 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/smallvec.rs
+-rw-r--r--   0     1001      127    61364 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/lib.rs
+-rw-r--r--   0     1001      127     1550 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/macros.rs
+-rw-r--r--   0     1001      127     6353 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/bytes.rs
+-rw-r--r--   0     1001      127     6390 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/capacity.rs
+-rw-r--r--   0     1001      127    19999 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/heap.rs
+-rw-r--r--   0     1001      127     6616 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/inline.rs
+-rw-r--r--   0     1001      127     6797 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/iter.rs
+-rw-r--r--   0     1001      127    35548 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/mod.rs
+-rw-r--r--   0     1001      127     4433 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/nonmax.rs
+-rw-r--r--   0     1001      127    16237 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/num.rs
+-rw-r--r--   0     1001      127     1334 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/smallvec.rs
+-rw-r--r--   0     1001      127     3958 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/traits.rs
+-rw-r--r--   0     1001      127    44008 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/tests.rs
+-rw-r--r--   0     1001      127    14163 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/compact_str-0.7.1/src/traits.rs
+-rw-r--r--   0     1001      127     8900 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1956 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/CONTRIBUTING.md
+-rw-r--r--   0     1001      127      713 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/COPYRIGHT
+-rw-r--r--   0     1001      127     1915 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/Cargo.toml
+-rw-r--r--   0     1001      127     4979 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/Ideas.md
+-rw-r--r--   0     1001      127    11358 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1053 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/LICENSE-MIT
+-rw-r--r--   0     1001      127     1501 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/LICENSE-WHATWG
+-rw-r--r--   0     1001      127    31179 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/README.md
+-rw-r--r--   0     1001      127      502 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/ci/miri.sh
+-rw-r--r--   0     1001      127      869 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/Big5.txt
+-rw-r--r--   0     1001      127      650 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/EUC-JP.txt
+-rw-r--r--   0     1001      127      631 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/EUC-KR.txt
+-rw-r--r--   0     1001      127      967 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/GBK.txt
+-rw-r--r--   0     1001      127      412 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/IBM866.txt
+-rw-r--r--   0     1001      127      557 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-2022-JP.txt
+-rw-r--r--   0     1001      127      400 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-10.txt
+-rw-r--r--   0     1001      127      427 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-13.txt
+-rw-r--r--   0     1001      127      400 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-14.txt
+-rw-r--r--   0     1001      127      359 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-15.txt
+-rw-r--r--   0     1001      127      417 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-16.txt
+-rw-r--r--   0     1001      127      345 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-2.txt
+-rw-r--r--   0     1001      127      343 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-3.txt
+-rw-r--r--   0     1001      127      343 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-4.txt
+-rw-r--r--   0     1001      127      297 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-5.txt
+-rw-r--r--   0     1001      127      381 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-6.txt
+-rw-r--r--   0     1001      127      695 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-7.txt
+-rw-r--r--   0     1001      127      513 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-8-I.txt
+-rw-r--r--   0     1001      127      512 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-8.txt
+-rw-r--r--   0     1001      127      312 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/KOI8-R.txt
+-rw-r--r--   0     1001      127      281 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/KOI8-U.txt
+-rw-r--r--   0     1001      127      475 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/Shift_JIS.txt
+-rw-r--r--   0     1001      127      400 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/UTF-16BE.txt
+-rw-r--r--   0     1001      127      403 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/UTF-16LE.txt
+-rw-r--r--   0     1001      127      261 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/UTF-8.txt
+-rw-r--r--   0     1001      127      524 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/gb18030.txt
+-rw-r--r--   0     1001      127      380 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/macintosh.txt
+-rw-r--r--   0     1001      127      499 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/replacement.txt
+-rw-r--r--   0     1001      127      288 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1250.txt
+-rw-r--r--   0     1001      127      280 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1251.txt
+-rw-r--r--   0     1001      127      344 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1252.txt
+-rw-r--r--   0     1001      127      450 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1253.txt
+-rw-r--r--   0     1001      127      344 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1254.txt
+-rw-r--r--   0     1001      127      437 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1255.txt
+-rw-r--r--   0     1001      127      278 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1256.txt
+-rw-r--r--   0     1001      127      364 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1257.txt
+-rw-r--r--   0     1001      127      666 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1258.txt
+-rw-r--r--   0     1001      127      404 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-874.txt
+-rw-r--r--   0     1001      127      297 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/x-mac-cyrillic.txt
+-rw-r--r--   0     1001      127      332 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/x-user-defined.txt
+-rw-r--r--   0     1001      127    61842 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/generate-encoding-data.py
+-rw-r--r--   0     1001      127       31 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/rustfmt.toml
+-rw-r--r--   0     1001      127    69771 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/ascii.rs
+-rw-r--r--   0     1001      127    15340 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/big5.rs
+-rw-r--r--   0     1001      127  2574354 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/data.rs
+-rw-r--r--   0     1001      127    17647 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/euc_jp.rs
+-rw-r--r--   0     1001      127    17433 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/euc_kr.rs
+-rw-r--r--   0     1001      127    29634 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/gb18030.rs
+-rw-r--r--   0     1001      127    67096 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/handles.rs
+-rw-r--r--   0     1001      127    45706 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/iso_2022_jp.rs
+-rw-r--r--   0     1001      127   247846 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/lib.rs
+-rw-r--r--   0     1001      127    74150 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/macros.rs
+-rw-r--r--   0     1001      127   130328 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/mem.rs
+-rw-r--r--   0     1001      127     3175 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/replacement.rs
+-rw-r--r--   0     1001      127    17079 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/shift_jis.rs
+-rw-r--r--   0     1001      127    13578 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/simd_funcs.rs
+-rw-r--r--   0     1001      127    32312 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/single_byte.rs
+-rw-r--r--   0     1001      127    59587 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/big5_in.txt
+-rw-r--r--   0     1001      127    81302 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/big5_in_ref.txt
+-rw-r--r--   0     1001      127    58777 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/big5_out.txt
+-rw-r--r--   0     1001      127    44029 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/big5_out_ref.txt
+-rw-r--r--   0     1001      127    72061 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_in.txt
+-rw-r--r--   0     1001      127   100162 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_in_ref.txt
+-rw-r--r--   0     1001      127    68262 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_out.txt
+-rw-r--r--   0     1001      127    51385 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_out_ref.txt
+-rw-r--r--   0     1001      127    72061 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_in.txt
+-rw-r--r--   0     1001      127    95843 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_in_ref.txt
+-rw-r--r--   0     1001      127    95839 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_out.txt
+-rw-r--r--   0     1001      127    72058 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_out_ref.txt
+-rw-r--r--   0     1001      127    79765 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_in.txt
+-rw-r--r--   0     1001      127    35463 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_in_ref.txt
+-rw-r--r--   0     1001      127    29715 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_out.txt
+-rw-r--r--   0     1001      127    66832 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_out_ref.txt
+-rw-r--r--   0     1001      127    26749 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_in.txt
+-rw-r--r--   0     1001      127    35463 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_in_ref.txt
+-rw-r--r--   0     1001      127    29463 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_out.txt
+-rw-r--r--   0     1001      127    22249 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_out_ref.txt
+-rw-r--r--   0     1001      127    35585 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0212_in.txt
+-rw-r--r--   0     1001      127    35322 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0212_in_ref.txt
+-rw-r--r--   0     1001      127    34081 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_in.txt
+-rw-r--r--   0     1001      127    45731 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_in_ref.txt
+-rw-r--r--   0     1001      127    29519 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_out.txt
+-rw-r--r--   0     1001      127    22291 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_out_ref.txt
+-rw-r--r--   0     1001      127    15992 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_labels_names.rs
+-rw-r--r--   0     1001      127     8321 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/testing.rs
+-rw-r--r--   0     1001      127    18725 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/utf_16.rs
+-rw-r--r--   0     1001      127    63069 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/utf_8.rs
+-rw-r--r--   0     1001      127    17213 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/variant.rs
+-rw-r--r--   0     1001      127     7516 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/x_user_defined.rs
+-rw-r--r--   0     1001      127      745 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoa-1.0.9/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1155 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoa-1.0.9/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoa-1.0.9/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoa-1.0.9/LICENSE-MIT
+-rw-r--r--   0     1001      127     2025 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoa-1.0.9/README.md
+-rw-r--r--   0     1001      127     1344 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoa-1.0.9/benches/bench.rs
+-rw-r--r--   0     1001      127    10597 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoa-1.0.9/src/lib.rs
+-rw-r--r--   0     1001      127     1480 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoa-1.0.9/src/udiv128.rs
+-rw-r--r--   0     1001      127      842 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoa-1.0.9/tests/test.rs
+-rw-r--r--   0     1001      127      981 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1226 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/Cargo.toml
+-rw-r--r--   0     1001      127     1122 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/LICENSE
+-rw-r--r--   0     1001      127     2616 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/README.md
+-rw-r--r--   0     1001      127    77666 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/bench.png
+-rw-r--r--   0     1001      127     2710 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/benches/bench.rs
+-rw-r--r--   0     1001      127      245 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/codecov.yml
+-rw-r--r--   0     1001      127      128 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/rustfmt.toml
+-rw-r--r--   0     1001      127     7375 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/src/common.rs
+-rw-r--r--   0     1001      127     1619 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/src/fallback.rs
+-rw-r--r--   0     1001      127    12645 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/src/lib.rs
+-rw-r--r--   0     1001      127     4385 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/itoap-1.0.1/src/sse2.rs
+-rw-r--r--   0     1001      127    25249 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/.cargo-checksum.json
+-rw-r--r--   0     1001      127     4446 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/CONTRIBUTING.md
+-rw-r--r--   0     1001      127     4788 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1076 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/LICENSE-MIT
+-rw-r--r--   0     1001      127     4134 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/README.md
+-rw-r--r--   0     1001      127     8994 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/build.rs
+-rw-r--r--   0     1001      127       30 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/rustfmt.toml
+-rw-r--r--   0     1001      127     4884 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/fixed_width_ints.rs
+-rw-r--r--   0     1001      127     1952 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/aarch64.rs
+-rw-r--r--   0     1001      127     5480 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/align.rs
+-rw-r--r--   0     1001      127   151602 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/mod.rs
+-rw-r--r--   0     1001      127     5036 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/no_align.rs
+-rw-r--r--   0     1001      127     1169 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/riscv64.rs
+-rw-r--r--   0     1001      127     4550 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/x86_64.rs
+-rw-r--r--   0     1001      127       46 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/hermit/aarch64.rs
+-rw-r--r--   0     1001      127     1480 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/hermit/mod.rs
+-rw-r--r--   0     1001      127       46 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/hermit/x86_64.rs
+-rw-r--r--   0     1001      127     4751 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/lib.rs
+-rw-r--r--   0     1001      127    10703 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/macros.rs
+-rw-r--r--   0     1001      127   126764 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/psp.rs
+-rw-r--r--   0     1001      127     1217 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/sgx.rs
+-rw-r--r--   0     1001      127       93 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/solid/aarch64.rs
+-rw-r--r--   0     1001      127       93 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/solid/arm.rs
+-rw-r--r--   0     1001      127    33199 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/solid/mod.rs
+-rw-r--r--   0     1001      127     1266 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/switch.rs
+-rw-r--r--   0     1001      127    30167 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/teeos/mod.rs
+-rw-r--r--   0     1001      127   118783 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/aix/mod.rs
+-rw-r--r--   0     1001      127    22868 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/aix/powerpc64.rs
+-rw-r--r--   0     1001      127       92 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/align.rs
+-rw-r--r--   0     1001      127      149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b32/align.rs
+-rw-r--r--   0     1001      127     3327 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b32/mod.rs
+-rw-r--r--   0     1001      127     1478 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/aarch64/align.rs
+-rw-r--r--   0     1001      127      255 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/aarch64/mod.rs
+-rw-r--r--   0     1001      127      149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/align.rs
+-rw-r--r--   0     1001      127     3434 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/mod.rs
+-rw-r--r--   0     1001      127      149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/x86_64/align.rs
+-rw-r--r--   0     1001      127     5717 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/x86_64/mod.rs
+-rw-r--r--   0     1001      127      151 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/long_array.rs
+-rw-r--r--   0     1001      127   228985 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/mod.rs
+-rw-r--r--   0     1001      127      377 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/dragonfly/errno.rs
+-rw-r--r--   0     1001      127    59079 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/dragonfly/mod.rs
+-rw-r--r--   0     1001      127     4973 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/aarch64.rs
+-rw-r--r--   0     1001      127     1420 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/arm.rs
+-rw-r--r--   0     1001      127      811 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd11/b64.rs
+-rw-r--r--   0     1001      127    17516 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd11/mod.rs
+-rw-r--r--   0     1001      127      860 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/b64.rs
+-rw-r--r--   0     1001      127    17656 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/mod.rs
+-rw-r--r--   0     1001      127      287 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/x86_64.rs
+-rw-r--r--   0     1001      127      860 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/b64.rs
+-rw-r--r--   0     1001      127    18823 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/mod.rs
+-rw-r--r--   0     1001      127      287 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/x86_64.rs
+-rw-r--r--   0     1001      127      860 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/b64.rs
+-rw-r--r--   0     1001      127    18823 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/mod.rs
+-rw-r--r--   0     1001      127      666 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/x86_64.rs
+-rw-r--r--   0     1001      127   196144 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/mod.rs
+-rw-r--r--   0     1001      127     1272 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/powerpc.rs
+-rw-r--r--   0     1001      127     1273 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/powerpc64.rs
+-rw-r--r--   0     1001      127     5469 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/riscv64.rs
+-rw-r--r--   0     1001      127     7585 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86.rs
+-rw-r--r--   0     1001      127     7805 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86_64/align.rs
+-rw-r--r--   0     1001      127    10953 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86_64/mod.rs
+-rw-r--r--   0     1001      127    63043 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/mod.rs
+-rw-r--r--   0     1001      127    29933 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/mod.rs
+-rw-r--r--   0     1001      127    25504 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/mod.rs
+-rw-r--r--   0     1001      127     2950 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/aarch64.rs
+-rw-r--r--   0     1001      127      628 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/arm.rs
+-rw-r--r--   0     1001      127   106675 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/mod.rs
+-rw-r--r--   0     1001      127      569 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/powerpc.rs
+-rw-r--r--   0     1001      127      221 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/sparc64.rs
+-rw-r--r--   0     1001      127      401 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/x86.rs
+-rw-r--r--   0     1001      127     1076 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/x86_64.rs
+-rw-r--r--   0     1001      127      722 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/aarch64.rs
+-rw-r--r--   0     1001      127      397 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/arm.rs
+-rw-r--r--   0     1001      127      157 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/mips64.rs
+-rw-r--r--   0     1001      127    67743 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/mod.rs
+-rw-r--r--   0     1001      127      397 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/powerpc.rs
+-rw-r--r--   0     1001      127      395 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/powerpc64.rs
+-rw-r--r--   0     1001      127      395 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/riscv64.rs
+-rw-r--r--   0     1001      127      159 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/sparc64.rs
+-rw-r--r--   0     1001      127      394 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/x86.rs
+-rw-r--r--   0     1001      127     4403 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/x86_64.rs
+-rw-r--r--   0     1001      127      495 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/haiku/b32.rs
+-rw-r--r--   0     1001      127      498 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/haiku/b64.rs
+-rw-r--r--   0     1001      127    69317 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/haiku/mod.rs
+-rw-r--r--   0     1001      127    50141 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/haiku/native.rs
+-rw-r--r--   0     1001      127     9816 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/haiku/x86_64.rs
+-rw-r--r--   0     1001      127       20 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/hurd/align.rs
+-rw-r--r--   0     1001      127     2557 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/hurd/b32.rs
+-rw-r--r--   0     1001      127     2582 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/hurd/b64.rs
+-rw-r--r--   0     1001      127   106355 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/hurd/mod.rs
+-rw-r--r--   0     1001      127       20 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/hurd/no_align.rs
+-rw-r--r--   0     1001      127    22019 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/arm.rs
+-rw-r--r--   0     1001      127     6584 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/mod.rs
+-rw-r--r--   0     1001      127      148 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/x86/align.rs
+-rw-r--r--   0     1001      127    24209 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/x86/mod.rs
+-rw-r--r--   0     1001      127      756 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/align.rs
+-rw-r--r--   0     1001      127      142 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/int128.rs
+-rw-r--r--   0     1001      127    16376 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/mod.rs
+-rw-r--r--   0     1001      127    10479 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/mod.rs
+-rw-r--r--   0     1001      127      149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/riscv64/align.rs
+-rw-r--r--   0     1001      127    13474 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/riscv64/mod.rs
+-rw-r--r--   0     1001      127      149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/x86_64/align.rs
+-rw-r--r--   0     1001      127    28839 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/x86_64/mod.rs
+-rw-r--r--   0     1001      127   131658 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/mod.rs
+-rw-r--r--   0     1001      127     2376 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/align.rs
+-rw-r--r--   0     1001      127     5193 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/lfs64.rs
+-rw-r--r--   0     1001      127    59263 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/mod.rs
+-rw-r--r--   0     1001      127     2066 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/no_align.rs
+-rw-r--r--   0     1001      127     8872 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/align.rs
+-rw-r--r--   0     1001      127    11583 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/generic/mod.rs
+-rw-r--r--   0     1001      127    11454 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/mips/mod.rs
+-rw-r--r--   0     1001      127      567 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/mod.rs
+-rw-r--r--   0     1001      127    10012 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/powerpc/mod.rs
+-rw-r--r--   0     1001      127     9375 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/sparc/mod.rs
+-rw-r--r--   0     1001      127      378 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/align.rs
+-rw-r--r--   0     1001      127     1805 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/arm/align.rs
+-rw-r--r--   0     1001      127    31048 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/arm/mod.rs
+-rw-r--r--   0     1001      127      148 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/csky/align.rs
+-rw-r--r--   0     1001      127    26449 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/csky/mod.rs
+-rw-r--r--   0     1001      127      148 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/m68k/align.rs
+-rw-r--r--   0     1001      127    31243 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/m68k/mod.rs
+-rw-r--r--   0     1001      127      148 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mips/align.rs
+-rw-r--r--   0     1001      127    31942 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mips/mod.rs
+-rw-r--r--   0     1001      127    11752 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mod.rs
+-rw-r--r--   0     1001      127    29822 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/powerpc.rs
+-rw-r--r--   0     1001      127     1213 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/riscv32/align.rs
+-rw-r--r--   0     1001      127    28172 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/riscv32/mod.rs
+-rw-r--r--   0     1001      127      148 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/sparc/align.rs
+-rw-r--r--   0     1001      127    30083 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/sparc/mod.rs
+-rw-r--r--   0     1001      127      149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/x86/align.rs
+-rw-r--r--   0     1001      127    38841 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/x86/mod.rs
+-rw-r--r--   0     1001      127     1516 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/align.rs
+-rw-r--r--   0     1001      127      163 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/fallback.rs
+-rw-r--r--   0     1001      127     2294 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/ilp32.rs
+-rw-r--r--   0     1001      127      142 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/int128.rs
+-rw-r--r--   0     1001      127     2798 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/lp64.rs
+-rw-r--r--   0     1001      127    32357 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/mod.rs
+-rw-r--r--   0     1001      127     1037 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/loongarch64/align.rs
+-rw-r--r--   0     1001      127    31949 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/loongarch64/mod.rs
+-rw-r--r--   0     1001      127      149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mips64/align.rs
+-rw-r--r--   0     1001      127    35131 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mips64/mod.rs
+-rw-r--r--   0     1001      127     3772 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mod.rs
+-rw-r--r--   0     1001      127      149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/powerpc64/align.rs
+-rw-r--r--   0     1001      127    34180 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/powerpc64/mod.rs
+-rw-r--r--   0     1001      127     1213 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/riscv64/align.rs
+-rw-r--r--   0     1001      127    29650 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/riscv64/mod.rs
+-rw-r--r--   0     1001      127    33048 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/s390x.rs
+-rw-r--r--   0     1001      127      149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/sparc64/align.rs
+-rw-r--r--   0     1001      127    32202 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/sparc64/mod.rs
+-rw-r--r--   0     1001      127      615 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/align.rs
+-rw-r--r--   0     1001      127    26263 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/mod.rs
+-rw-r--r--   0     1001      127    17621 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/not_x32.rs
+-rw-r--r--   0     1001      127    22804 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/x32.rs
+-rw-r--r--   0     1001      127    49833 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/mod.rs
+-rw-r--r--   0     1001      127      258 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/no_align.rs
+-rw-r--r--   0     1001      127   169363 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/mod.rs
+-rw-r--r--   0     1001      127      150 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/arm/align.rs
+-rw-r--r--   0     1001      127    30616 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/arm/mod.rs
+-rw-r--r--   0     1001      127    24091 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/hexagon.rs
+-rw-r--r--   0     1001      127      148 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mips/align.rs
+-rw-r--r--   0     1001      127    31187 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mips/mod.rs
+-rw-r--r--   0     1001      127     1627 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mod.rs
+-rw-r--r--   0     1001      127    29188 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/powerpc.rs
+-rw-r--r--   0     1001      127      150 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/riscv32/align.rs
+-rw-r--r--   0     1001      127    28063 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/riscv32/mod.rs
+-rw-r--r--   0     1001      127      148 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/x86/align.rs
+-rw-r--r--   0     1001      127    31972 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/x86/mod.rs
+-rw-r--r--   0     1001      127     1080 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/align.rs
+-rw-r--r--   0     1001      127      142 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/int128.rs
+-rw-r--r--   0     1001      127    24219 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/mod.rs
+-rw-r--r--   0     1001      127    27809 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/mips64.rs
+-rw-r--r--   0     1001      127     4425 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/mod.rs
+-rw-r--r--   0     1001      127    26015 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/powerpc64.rs
+-rw-r--r--   0     1001      127     1213 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/riscv64/align.rs
+-rw-r--r--   0     1001      127    25593 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/riscv64/mod.rs
+-rw-r--r--   0     1001      127    26240 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/s390x.rs
+-rw-r--r--   0     1001      127      616 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/x86_64/align.rs
+-rw-r--r--   0     1001      127    32792 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/x86_64/mod.rs
+-rw-r--r--   0     1001      127     5732 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/lfs64.rs
+-rw-r--r--   0     1001      127    26755 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/mod.rs
+-rw-r--r--   0     1001      127     6370 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/no_align.rs
+-rw-r--r--   0     1001      127      169 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/non_exhaustive.rs
+-rw-r--r--   0     1001      127     1074 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/align.rs
+-rw-r--r--   0     1001      127      378 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/arm/align.rs
+-rw-r--r--   0     1001      127    32707 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/arm/mod.rs
+-rw-r--r--   0     1001      127      258 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/arm/no_align.rs
+-rw-r--r--   0     1001      127      378 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips32/align.rs
+-rw-r--r--   0     1001      127    26773 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips32/mod.rs
+-rw-r--r--   0     1001      127      258 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips32/no_align.rs
+-rw-r--r--   0     1001      127      258 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips64/align.rs
+-rw-r--r--   0     1001      127     5470 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips64/mod.rs
+-rw-r--r--   0     1001      127      138 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips64/no_align.rs
+-rw-r--r--   0     1001      127    10293 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mod.rs
+-rw-r--r--   0     1001      127    12819 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mod.rs
+-rw-r--r--   0     1001      127     2037 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/no_align.rs
+-rw-r--r--   0     1001      127     1857 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/l4re.rs
+-rw-r--r--   0     1001      127    10398 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/mod.rs
+-rw-r--r--   0     1001      127      172 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/other.rs
+-rw-r--r--   0     1001      127    67338 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/mod.rs
+-rw-r--r--   0     1001      127    61430 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/mod.rs
+-rw-r--r--   0     1001      127     1346 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/aarch64/mod.rs
+-rw-r--r--   0     1001      127     2572 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/align.rs
+-rw-r--r--   0     1001      127     1380 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/arm/mod.rs
+-rw-r--r--   0     1001      127     3066 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/espidf/mod.rs
+-rw-r--r--   0     1001      127      830 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/generic.rs
+-rw-r--r--   0     1001      127     7356 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/horizon/mod.rs
+-rw-r--r--   0     1001      127    25647 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/mod.rs
+-rw-r--r--   0     1001      127     2082 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/no_align.rs
+-rw-r--r--   0     1001      127      353 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/powerpc/mod.rs
+-rw-r--r--   0     1001      127     6573 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/vita/mod.rs
+-rw-r--r--   0     1001      127       97 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/no_align.rs
+-rw-r--r--   0     1001      127      730 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/nto/aarch64.rs
+-rw-r--r--   0     1001      127   117100 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/nto/mod.rs
+-rw-r--r--   0     1001      127    42200 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/nto/neutrino.rs
+-rw-r--r--   0     1001      127     3479 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/nto/x86_64.rs
+-rw-r--r--   0     1001      127    46971 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/redox/mod.rs
+-rw-r--r--   0     1001      127     6492 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/compat.rs
+-rw-r--r--   0     1001      127     2814 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/illumos.rs
+-rw-r--r--   0     1001      127   113204 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/mod.rs
+-rw-r--r--   0     1001      127     3000 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/solaris.rs
+-rw-r--r--   0     1001      127      859 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/x86.rs
+-rw-r--r--   0     1001      127     6023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/x86_64.rs
+-rw-r--r--   0     1001      127     2717 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/x86_common.rs
+-rw-r--r--   0     1001      127       93 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/vxworks/aarch64.rs
+-rw-r--r--   0     1001      127       93 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/vxworks/arm.rs
+-rw-r--r--   0     1001      127    62286 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/vxworks/mod.rs
+-rw-r--r--   0     1001      127       93 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/vxworks/powerpc.rs
+-rw-r--r--   0     1001      127       93 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/vxworks/powerpc64.rs
+-rw-r--r--   0     1001      127       93 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/vxworks/x86.rs
+-rw-r--r--   0     1001      127       93 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/vxworks/x86_64.rs
+-rw-r--r--   0     1001      127    31119 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/wasi.rs
+-rw-r--r--   0     1001      127      525 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/windows/gnu/align.rs
+-rw-r--r--   0     1001      127      749 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/windows/gnu/mod.rs
+-rw-r--r--   0     1001      127    22035 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/windows/mod.rs
+-rw-r--r--   0     1001      127      639 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/windows/msvc/mod.rs
+-rw-r--r--   0     1001      127     1264 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/src/xous.rs
+-rw-r--r--   0     1001      127      220 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libc-0.2.149/tests/const_fn.rs
+-rw-r--r--   0     1001      127    11291 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1609 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/CHANGELOG.md
+-rw-r--r--   0     1001      127     3428 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/CONTRIBUTING.md
+-rw-r--r--   0     1001      127     1073 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1058 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/LICENSE-MIT
+-rw-r--r--   0     1001      127     1467 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/README.md
+-rw-r--r--   0     1001      127    15767 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/build.rs
+-rw-r--r--   0     1001      127     1461 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/lib.rs
+-rw-r--r--   0     1001      127     8395 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/libm_helper.rs
+-rw-r--r--   0     1001      127     3810 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/acos.rs
+-rw-r--r--   0     1001      127     2218 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/acosf.rs
+-rw-r--r--   0     1001      127      867 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/acosh.rs
+-rw-r--r--   0     1001      127      823 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/acoshf.rs
+-rw-r--r--   0     1001      127     4288 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/asin.rs
+-rw-r--r--   0     1001      127     2054 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/asinf.rs
+-rw-r--r--   0     1001      127     1162 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/asinh.rs
+-rw-r--r--   0     1001      127     1133 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/asinhf.rs
+-rw-r--r--   0     1001      127     5774 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atan.rs
+-rw-r--r--   0     1001      127     4355 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atan2.rs
+-rw-r--r--   0     1001      127     2894 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atan2f.rs
+-rw-r--r--   0     1001      127     3149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atanf.rs
+-rw-r--r--   0     1001      127      970 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atanh.rs
+-rw-r--r--   0     1001      127      968 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atanhf.rs
+-rw-r--r--   0     1001      127     4343 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cbrt.rs
+-rw-r--r--   0     1001      127     2149 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cbrtf.rs
+-rw-r--r--   0     1001      127     2333 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ceil.rs
+-rw-r--r--   0     1001      127     1750 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ceilf.rs
+-rw-r--r--   0     1001      127      403 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/copysign.rs
+-rw-r--r--   0     1001      127      406 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/copysignf.rs
+-rw-r--r--   0     1001      127     2255 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cos.rs
+-rw-r--r--   0     1001      127     2438 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cosf.rs
+-rw-r--r--   0     1001      127      993 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cosh.rs
+-rw-r--r--   0     1001      127      910 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/coshf.rs
+-rw-r--r--   0     1001      127    12647 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/erf.rs
+-rw-r--r--   0     1001      127     7600 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/erff.rs
+-rw-r--r--   0     1001      127     5099 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp.rs
+-rw-r--r--   0     1001      127      754 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp10.rs
+-rw-r--r--   0     1001      127      735 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp10f.rs
+-rw-r--r--   0     1001      127    16436 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp2.rs
+-rw-r--r--   0     1001      127     4725 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp2f.rs
+-rw-r--r--   0     1001      127     3032 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/expf.rs
+-rw-r--r--   0     1001      127     4321 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/expm1.rs
+-rw-r--r--   0     1001      127     3951 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/expm1f.rs
+-rw-r--r--   0     1001      127      568 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/expo2.rs
+-rw-r--r--   0     1001      127     1189 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fabs.rs
+-rw-r--r--   0     1001      127     1302 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fabsf.rs
+-rw-r--r--   0     1001      127      470 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fdim.rs
+-rw-r--r--   0     1001      127      471 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fdimf.rs
+-rw-r--r--   0     1001      127      478 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fenv.rs
+-rw-r--r--   0     1001      127     2333 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/floor.rs
+-rw-r--r--   0     1001      127     1783 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/floorf.rs
+-rw-r--r--   0     1001      127     6706 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fma.rs
+-rw-r--r--   0     1001      127     4135 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmaf.rs
+-rw-r--r--   0     1001      127      771 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmax.rs
+-rw-r--r--   0     1001      127      772 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmaxf.rs
+-rw-r--r--   0     1001      127      771 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmin.rs
+-rw-r--r--   0     1001      127      772 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fminf.rs
+-rw-r--r--   0     1001      127     1637 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmod.rs
+-rw-r--r--   0     1001      127     1649 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmodf.rs
+-rw-r--r--   0     1001      127      492 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/frexp.rs
+-rw-r--r--   0     1001      127      485 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/frexpf.rs
+-rw-r--r--   0     1001      127     1780 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/hypot.rs
+-rw-r--r--   0     1001      127     1000 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/hypotf.rs
+-rw-r--r--   0     1001      127      726 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ilogb.rs
+-rw-r--r--   0     1001      127      716 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ilogbf.rs
+-rw-r--r--   0     1001      127    15469 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/j0.rs
+-rw-r--r--   0     1001      127    10448 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/j0f.rs
+-rw-r--r--   0     1001      127    14881 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/j1.rs
+-rw-r--r--   0     1001      127    10641 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/j1f.rs
+-rw-r--r--   0     1001      127    10179 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/jn.rs
+-rw-r--r--   0     1001      127     6930 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/jnf.rs
+-rw-r--r--   0     1001      127     2985 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_cos.rs
+-rw-r--r--   0     1001      127     1132 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_cosf.rs
+-rw-r--r--   0     1001      127      566 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_expo2.rs
+-rw-r--r--   0     1001      127      542 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_expo2f.rs
+-rw-r--r--   0     1001      127     2470 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_sin.rs
+-rw-r--r--   0     1001      127     1137 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_sinf.rs
+-rw-r--r--   0     1001      127     4236 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_tan.rs
+-rw-r--r--   0     1001      127     1924 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_tanf.rs
+-rw-r--r--   0     1001      127      124 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ldexp.rs
+-rw-r--r--   0     1001      127      126 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ldexpf.rs
+-rw-r--r--   0     1001      127      133 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/lgamma.rs
+-rw-r--r--   0     1001      127    12707 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/lgamma_r.rs
+-rw-r--r--   0     1001      127      136 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/lgammaf.rs
+-rw-r--r--   0     1001      127     8573 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/lgammaf_r.rs
+-rw-r--r--   0     1001      127     4552 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log.rs
+-rw-r--r--   0     1001      127     3767 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log10.rs
+-rw-r--r--   0     1001      127     2561 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log10f.rs
+-rw-r--r--   0     1001      127     4769 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log1p.rs
+-rw-r--r--   0     1001      127     2836 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log1pf.rs
+-rw-r--r--   0     1001      127     3225 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log2.rs
+-rw-r--r--   0     1001      127     2378 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log2f.rs
+-rw-r--r--   0     1001      127     2076 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/logf.rs
+-rw-r--r--   0     1001      127     8036 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/mod.rs
+-rw-r--r--   0     1001      127      730 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/modf.rs
+-rw-r--r--   0     1001      127      739 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/modff.rs
+-rw-r--r--   0     1001      127      886 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/nextafter.rs
+-rw-r--r--   0     1001      127      920 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/nextafterf.rs
+-rw-r--r--   0     1001      127    21546 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/pow.rs
+-rw-r--r--   0     1001      127    10039 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/powf.rs
+-rw-r--r--   0     1001      127     7501 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rem_pio2.rs
+-rw-r--r--   0     1001      127    20354 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rem_pio2_large.rs
+-rw-r--r--   0     1001      127     2323 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rem_pio2f.rs
+-rw-r--r--   0     1001      127      158 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/remainder.rs
+-rw-r--r--   0     1001      127      160 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/remainderf.rs
+-rw-r--r--   0     1001      127     2462 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/remquo.rs
+-rw-r--r--   0     1001      127     2159 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/remquof.rs
+-rw-r--r--   0     1001      127     1776 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rint.rs
+-rw-r--r--   0     1001      127     1783 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rintf.rs
+-rw-r--r--   0     1001      127      635 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/round.rs
+-rw-r--r--   0     1001      127      775 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/roundf.rs
+-rw-r--r--   0     1001      127      964 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/scalbn.rs
+-rw-r--r--   0     1001      127      807 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/scalbnf.rs
+-rw-r--r--   0     1001      127     2803 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sin.rs
+-rw-r--r--   0     1001      127     3569 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sincos.rs
+-rw-r--r--   0     1001      127     5286 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sincosf.rs
+-rw-r--r--   0     1001      127     2647 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sinf.rs
+-rw-r--r--   0     1001      127     1261 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sinh.rs
+-rw-r--r--   0     1001      127      693 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sinhf.rs
+-rw-r--r--   0     1001      127     9295 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sqrt.rs
+-rw-r--r--   0     1001      127     4842 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sqrtf.rs
+-rw-r--r--   0     1001      127     2248 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tan.rs
+-rw-r--r--   0     1001      127     2411 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tanf.rs
+-rw-r--r--   0     1001      127     1360 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tanh.rs
+-rw-r--r--   0     1001      127      902 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tanhf.rs
+-rw-r--r--   0     1001      127     5518 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tgamma.rs
+-rw-r--r--   0     1001      127      142 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tgammaf.rs
+-rw-r--r--   0     1001      127      962 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/trunc.rs
+-rw-r--r--   0     1001      127     1078 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/libm-0.2.8/src/math/truncf.rs
+-rw-r--r--   0     1001      127     1037 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1348 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/LICENSE-MIT
+-rw-r--r--   0     1001      127     4233 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/README.md
+-rw-r--r--   0     1001      127     9498 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/src/lib.rs
+-rw-r--r--   0     1001      127     2339 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/tests/compiletest/mod.rs
+-rw-r--r--   0     1001      127     4891 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/tests/test.rs
+-rw-r--r--   0     1001      127      100 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/tests/ui/async-fn.rs
+-rw-r--r--   0     1001      127      254 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/tests/ui/async-fn.stderr
+-rw-r--r--   0     1001      127      121 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/tests/ui/trait-fn.rs
+-rw-r--r--   0     1001      127       96 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/no-panic-0.1.26/tests/ui/trait-fn.stderr
+-rw-r--r--   0     1001      127     2261 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1294 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1071 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/LICENSE-MIT
+-rw-r--r--   0     1001      127     1796 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/README.md
+-rw-r--r--   0     1001      127    11754 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/RELEASES.md
+-rw-r--r--   0     1001      127      799 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/build.rs
+-rw-r--r--   0     1001      127     3870 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/bounds.rs
+-rw-r--r--   0     1001      127    26072 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/cast.rs
+-rw-r--r--   0     1001      127    64284 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/float.rs
+-rw-r--r--   0     1001      127     4595 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/identities.rs
+-rw-r--r--   0     1001      127    15915 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/int.rs
+-rw-r--r--   0     1001      127    21755 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/lib.rs
+-rw-r--r--   0     1001      127     1397 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/macros.rs
+-rw-r--r--   0     1001      127    11368 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/bytes.rs
+-rw-r--r--   0     1001      127    10040 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/checked.rs
+-rw-r--r--   0     1001      127    10278 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/euclid.rs
+-rw-r--r--   0     1001      127      931 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/inv.rs
+-rw-r--r--   0     1001      127      137 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/mod.rs
+-rw-r--r--   0     1001      127     3983 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/mul_add.rs
+-rw-r--r--   0     1001      127     4283 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/overflowing.rs
+-rw-r--r--   0     1001      127     5103 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/saturating.rs
+-rw-r--r--   0     1001      127    11260 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/wrapping.rs
+-rw-r--r--   0     1001      127     6574 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/pow.rs
+-rw-r--r--   0     1001      127    22158 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/real.rs
+-rw-r--r--   0     1001      127     5877 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/src/sign.rs
+-rw-r--r--   0     1001      127    12080 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/num-traits-0.2.17/tests/cast.rs
+-rw-r--r--   0     1001      127     2279 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/.cargo-checksum.json
+-rw-r--r--   0     1001      127     6036 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/CHANGELOG.md
+-rw-r--r--   0     1001      127     4884 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/Cargo.lock
+-rw-r--r--   0     1001      127     2012 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/LICENSE-MIT
+-rw-r--r--   0     1001      127     2186 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/README.md
+-rw-r--r--   0     1001      127       50 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/bors.toml
+-rw-r--r--   0     1001      127      831 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/bench.rs
+-rw-r--r--   0     1001      127     1344 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/bench_acquire.rs
+-rw-r--r--   0     1001      127     1036 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/lazy_static.rs
+-rw-r--r--   0     1001      127      351 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/reentrant_init_deadlocks.rs
+-rw-r--r--   0     1001      127     1663 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/regex.rs
+-rw-r--r--   0     1001      127     1225 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/test_synchronization.rs
+-rw-r--r--   0     1001      127     2485 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/src/imp_cs.rs
+-rw-r--r--   0     1001      127     5803 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/src/imp_pl.rs
+-rw-r--r--   0     1001      127    12743 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/src/imp_std.rs
+-rw-r--r--   0     1001      127    46956 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/src/lib.rs
+-rw-r--r--   0     1001      127    13279 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/src/race.rs
+-rw-r--r--   0     1001      127      297 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/main.rs
+-rw-r--r--   0     1001      127     3055 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/race.rs
+-rw-r--r--   0     1001      127     3389 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/race_once_box.rs
+-rw-r--r--   0     1001      127     3685 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/sync_lazy.rs
+-rw-r--r--   0     1001      127     7663 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/sync_once_cell.rs
+-rw-r--r--   0     1001      127     2765 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/unsync_lazy.rs
+-rw-r--r--   0     1001      127     3853 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/unsync_once_cell.rs
+-rw-r--r--   0     1001      127    20422 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1903 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1071 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/LICENSE-MIT
+-rw-r--r--   0     1001      127     6869 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/README.md
+-rw-r--r--   0     1001      127       56 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/bors.toml
+-rw-r--r--   0     1001      127      195 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/build.rs
+-rwxr-xr-x   0     1001      127      848 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/all.sh
+-rw-r--r--   0     1001      127      735 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/android-install-ndk.sh
+-rw-r--r--   0     1001      127     1664 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/android-install-sdk.sh
+-rw-r--r--   0     1001      127     1664 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/android-sysimage.sh
+-rwxr-xr-x   0     1001      127      821 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/benchmark.sh
+-rw-r--r--   0     1001      127     5815 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/deploy_and_run_on_ios_simulator.rs
+-rw-r--r--   0     1001      127     1230 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/aarch64-linux-android/Dockerfile
+-rw-r--r--   0     1001      127      415 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/aarch64-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127      463 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/arm-unknown-linux-gnueabi/Dockerfile
+-rw-r--r--   0     1001      127      422 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/arm-unknown-linux-gnueabihf/Dockerfile
+-rw-r--r--   0     1001      127     1222 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/armv7-linux-androideabi/Dockerfile
+-rw-r--r--   0     1001      127      426 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/armv7-unknown-linux-gnueabihf/Dockerfile
+-rw-r--r--   0     1001      127      152 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/i586-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127      152 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/i686-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127      448 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/mips-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127      456 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/mips64-unknown-linux-gnuabi64/Dockerfile
+-rw-r--r--   0     1001      127      464 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/mips64el-unknown-linux-gnuabi64/Dockerfile
+-rw-r--r--   0     1001      127      849 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/mipsel-unknown-linux-musl/Dockerfile
+-rw-r--r--   0     1001      127      489 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/powerpc-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127      499 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/powerpc64-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127      491 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/powerpc64le-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127      554 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/s390x-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127      603 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/sparc64-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127     1238 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/thumbv7neon-linux-androideabi/Dockerfile
+-rw-r--r--   0     1001      127      438 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/thumbv7neon-unknown-linux-gnueabihf/Dockerfile
+-rw-r--r--   0     1001      127     1345 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/wasm32-unknown-unknown/Dockerfile
+-rw-r--r--   0     1001      127      892 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/x86_64-linux-android/Dockerfile
+-rw-r--r--   0     1001      127      180 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/x86_64-unknown-linux-gnu/Dockerfile
+-rw-r--r--   0     1001      127      451 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/x86_64-unknown-linux-gnu-emulated/Dockerfile
+-rwxr-xr-x   0     1001      127      663 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/dox.sh
+-rw-r--r--   0     1001      127      515 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/linux-s390x.sh
+-rw-r--r--   0     1001      127      433 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/linux-sparc64.sh
+-rw-r--r--   0     1001      127      282 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/lld-shim.rs
+-rwxr-xr-x   0     1001      127      281 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/max_line_width.sh
+-rwxr-xr-x   0     1001      127      976 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/run-docker.sh
+-rwxr-xr-x   0     1001      127     3275 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/run.sh
+-rw-r--r--   0     1001      127     1881 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/run_examples.sh
+-rw-r--r--   0     1001      127     1365 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/runtest-android.rs
+-rwxr-xr-x   0     1001      127      180 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/setup_benchmarks.sh
+-rwxr-xr-x   0     1001      127      454 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/test-runner-linux
+-rw-r--r--   0     1001      127     2956 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/contributing.md
+-rw-r--r--   0     1001      127      296 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/book.toml
+-rw-r--r--   0     1001      127      794 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/SUMMARY.md
+-rw-r--r--   0     1001      127      134 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/ascii.css
+-rw-r--r--   0     1001      127      911 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/bound_checks.md
+-rw-r--r--   0     1001      127      265 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/float-math/approx.md
+-rw-r--r--   0     1001      127      186 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/float-math/fma.md
+-rw-r--r--   0     1001      127      108 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/float-math/fp.md
+-rw-r--r--   0     1001      127      165 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/float-math/svml.md
+-rw-r--r--   0     1001      127      638 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/introduction.md
+-rw-r--r--   0     1001      127     3476 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/linux.md
+-rw-r--r--   0     1001      127     3629 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/mca.md
+-rw-r--r--   0     1001      127      738 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/profiling.md
+-rw-r--r--   0     1001      127       91 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/attribute.md
+-rw-r--r--   0     1001      127      745 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/features.md
+-rw-r--r--   0     1001      127       97 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/inlining.md
+-rw-r--r--   0     1001      127     1486 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/practice.md
+-rw-r--r--   0     1001      127       82 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/runtime.md
+-rw-r--r--   0     1001      127     2625 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/rustflags.md
+-rw-r--r--   0     1001      127     2719 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/vert-hor-ops.md
+-rw-r--r--   0     1001      127        8 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/rust-toolchain
+-rw-r--r--   0     1001      127      112 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/rustfmt.toml
+-rw-r--r--   0     1001      127     5477 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/bit_manip.rs
+-rw-r--r--   0     1001      127     3075 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/bitmask.rs
+-rw-r--r--   0     1001      127     2435 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/macros.rs
+-rw-r--r--   0     1001      127     4101 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v128.rs
+-rw-r--r--   0     1001      127      870 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v16.rs
+-rw-r--r--   0     1001      127     4066 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v256.rs
+-rw-r--r--   0     1001      127     1629 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v32.rs
+-rw-r--r--   0     1001      127     3202 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v512.rs
+-rw-r--r--   0     1001      127     2531 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v64.rs
+-rw-r--r--   0     1001      127     3070 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast.rs
+-rw-r--r--   0     1001      127      811 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/eq.rs
+-rw-r--r--   0     1001      127     1365 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/ord.rs
+-rw-r--r--   0     1001      127     2195 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/partial_eq.rs
+-rw-r--r--   0     1001      127    11164 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/partial_ord.rs
+-rw-r--r--   0     1001      127     4094 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/vertical.rs
+-rw-r--r--   0     1001      127      176 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp.rs
+-rw-r--r--   0     1001      127      997 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/default.rs
+-rw-r--r--   0     1001      127     2258 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/binary.rs
+-rw-r--r--   0     1001      127     2418 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/debug.rs
+-rw-r--r--   0     1001      127     2270 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/lower_hex.rs
+-rw-r--r--   0     1001      127     2258 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/octal.rs
+-rw-r--r--   0     1001      127     2274 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/upper_hex.rs
+-rw-r--r--   0     1001      127      161 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt.rs
+-rw-r--r--   0     1001      127     4759 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/from/from_array.rs
+-rw-r--r--   0     1001      127     2153 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/from/from_vector.rs
+-rw-r--r--   0     1001      127      113 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/from.rs
+-rw-r--r--   0     1001      127     1857 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/hash.rs
+-rw-r--r--   0     1001      127     7989 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/arch_specific.rs
+-rw-r--r--   0     1001      127     2761 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/macros.rs
+-rw-r--r--   0     1001      127     3049 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v128.rs
+-rw-r--r--   0     1001      127      312 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v16.rs
+-rw-r--r--   0     1001      127     3087 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v256.rs
+-rw-r--r--   0     1001      127      520 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v32.rs
+-rw-r--r--   0     1001      127     3138 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v512.rs
+-rw-r--r--   0     1001      127      972 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v64.rs
+-rw-r--r--   0     1001      127     1223 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits.rs
+-rw-r--r--   0     1001      127      981 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/abs.rs
+-rw-r--r--   0     1001      127     2687 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/consts.rs
+-rw-r--r--   0     1001      127     1569 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/cos.rs
+-rw-r--r--   0     1001      127     1183 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/exp.rs
+-rw-r--r--   0     1001      127     1157 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/ln.rs
+-rw-r--r--   0     1001      127     1700 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/mul_add.rs
+-rw-r--r--   0     1001      127     2016 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/mul_adde.rs
+-rw-r--r--   0     1001      127     1312 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/powf.rs
+-rw-r--r--   0     1001      127     1292 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/recpre.rs
+-rw-r--r--   0     1001      127     1496 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/rsqrte.rs
+-rw-r--r--   0     1001      127     1759 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/sin.rs
+-rw-r--r--   0     1001      127     1179 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/sqrt.rs
+-rw-r--r--   0     1001      127     1593 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/sqrte.rs
+-rw-r--r--   0     1001      127      871 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/tanh.rs
+-rw-r--r--   0     1001      127      957 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float.rs
+-rw-r--r--   0     1001      127       65 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math.rs
+-rw-r--r--   0     1001      127     6798 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/minimal/iuf.rs
+-rw-r--r--   0     1001      127     6833 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/minimal/mask.rs
+-rw-r--r--   0     1001      127    58636 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/minimal/ptr.rs
+-rw-r--r--   0     1001      127       67 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/minimal.rs
+-rw-r--r--   0     1001      127     7094 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_arithmetic.rs
+-rw-r--r--   0     1001      127     5612 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_bitwise.rs
+-rw-r--r--   0     1001      127     4673 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_mask_bitwise.rs
+-rw-r--r--   0     1001      127     4166 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_shifts.rs
+-rw-r--r--   0     1001      127     5010 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_arithmetic.rs
+-rw-r--r--   0     1001      127     4285 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_bitwise.rs
+-rw-r--r--   0     1001      127     2920 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_float_min_max.rs
+-rw-r--r--   0     1001      127     2037 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_int_min_max.rs
+-rw-r--r--   0     1001      127     3832 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_mask_bitwise.rs
+-rw-r--r--   0     1001      127     1569 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_neg.rs
+-rw-r--r--   0     1001      127     4106 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_rotates.rs
+-rw-r--r--   0     1001      127     4052 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_shifts.rs
+-rw-r--r--   0     1001      127      462 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops.rs
+-rw-r--r--   0     1001      127     8262 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ptr/gather_scatter.rs
+-rw-r--r--   0     1001      127       57 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ptr.rs
+-rw-r--r--   0     1001      127     6109 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/bitwise.rs
+-rw-r--r--   0     1001      127    13834 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/float_arithmetic.rs
+-rw-r--r--   0     1001      127     8030 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/integer_arithmetic.rs
+-rw-r--r--   0     1001      127     3573 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/mask.rs
+-rw-r--r--   0     1001      127    17484 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/min_max.rs
+-rw-r--r--   0     1001      127      163 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions.rs
+-rw-r--r--   0     1001      127     2516 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/select.rs
+-rw-r--r--   0     1001      127     6595 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/shuffle.rs
+-rw-r--r--   0     1001      127     6570 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/shuffle1_dyn.rs
+-rw-r--r--   0     1001      127     9045 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/slice/from_slice.rs
+-rw-r--r--   0     1001      127     9000 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/slice/write_to_slice.rs
+-rw-r--r--   0     1001      127       90 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/slice.rs
+-rw-r--r--   0     1001      127     7085 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/swap_bytes.rs
+-rw-r--r--   0     1001      127    13620 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api.rs
+-rw-r--r--   0     1001      127    13558 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/bit_manip.rs
+-rw-r--r--   0     1001      127     3842 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/llvm.rs
+-rw-r--r--   0     1001      127     3752 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/abs.rs
+-rw-r--r--   0     1001      127     3749 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/cos.rs
+-rw-r--r--   0     1001      127     2827 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/cos_pi.rs
+-rw-r--r--   0     1001      127     4276 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/exp.rs
+-rw-r--r--   0     1001      127     4237 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/ln.rs
+-rw-r--r--   0     1001      127    18033 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/macros.rs
+-rw-r--r--   0     1001      127     4150 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/mul_add.rs
+-rw-r--r--   0     1001      127     2093 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/mul_adde.rs
+-rw-r--r--   0     1001      127     4471 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/powf.rs
+-rw-r--r--   0     1001      127     3750 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin.rs
+-rw-r--r--   0     1001      127     6535 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin_cos_pi.rs
+-rw-r--r--   0     1001      127     2830 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin_pi.rs
+-rw-r--r--   0     1001      127     3756 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sqrt.rs
+-rw-r--r--   0     1001      127     2603 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sqrte.rs
+-rw-r--r--   0     1001      127     4289 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/tanh.rs
+-rw-r--r--   0     1001      127      425 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float.rs
+-rw-r--r--   0     1001      127       52 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math.rs
+-rw-r--r--   0     1001      127      908 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/pointer_sized_int.rs
+-rw-r--r--   0     1001      127     2309 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/aarch64.rs
+-rw-r--r--   0     1001      127     1845 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/arm.rs
+-rw-r--r--   0     1001      127      182 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/fallback.rs
+-rw-r--r--   0     1001      127     6614 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/fallback_impl.rs
+-rw-r--r--   0     1001      127     3692 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/avx.rs
+-rw-r--r--   0     1001      127     1351 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/avx2.rs
+-rw-r--r--   0     1001      127     1322 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/sse.rs
+-rw-r--r--   0     1001      127     2581 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/sse2.rs
+-rw-r--r--   0     1001      127     5387 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86.rs
+-rw-r--r--   0     1001      127     1745 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask.rs
+-rw-r--r--   0     1001      127       21 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions.rs
+-rw-r--r--   0     1001      127     5876 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/shuffle.rs
+-rw-r--r--   0     1001      127    15039 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/shuffle1_dyn.rs
+-rw-r--r--   0     1001      127     5365 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/swap_bytes.rs
+-rw-r--r--   0     1001      127     1251 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v128.rs
+-rw-r--r--   0     1001      127      187 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v16.rs
+-rw-r--r--   0     1001      127     1871 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v256.rs
+-rw-r--r--   0     1001      127      350 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v32.rs
+-rw-r--r--   0     1001      127     3082 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v512.rs
+-rw-r--r--   0     1001      127      778 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v64.rs
+-rw-r--r--   0     1001      127     1231 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/vPtr.rs
+-rw-r--r--   0     1001      127      823 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/vSize.rs
+-rw-r--r--   0     1001      127     1475 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen.rs
+-rw-r--r--   0     1001      127    11525 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/lib.rs
+-rw-r--r--   0     1001      127     3436 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/masks.rs
+-rw-r--r--   0     1001      127     1147 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/sealed.rs
+-rw-r--r--   0     1001      127     1916 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/testing/macros.rs
+-rw-r--r--   0     1001      127     4512 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/testing/utils.rs
+-rw-r--r--   0     1001      127      115 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/testing.rs
+-rw-r--r--   0     1001      127     3079 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v128.rs
+-rw-r--r--   0     1001      127      447 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v16.rs
+-rw-r--r--   0     1001      127     3462 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v256.rs
+-rw-r--r--   0     1001      127      895 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v32.rs
+-rw-r--r--   0     1001      127     4555 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v512.rs
+-rw-r--r--   0     1001      127     2379 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v64.rs
+-rw-r--r--   0     1001      127      966 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/vPtr.rs
+-rw-r--r--   0     1001      127     1484 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/vSize.rs
+-rw-r--r--   0     1001      127     7391 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/packed_simd-0.3.9/tests/endianness.rs
+-rw-r--r--   0     1001      127     1845 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1675 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/LICENSE-MIT
+-rw-r--r--   0     1001      127     3866 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/README.md
+-rw-r--r--   0     1001      127     4230 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/build.rs
+-rw-r--r--   0     1001      127       38 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/rust-toolchain.toml
+-rw-r--r--   0     1001      127     2703 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/detection.rs
+-rw-r--r--   0     1001      127     2565 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/extra.rs
+-rw-r--r--   0     1001      127    29816 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/fallback.rs
+-rw-r--r--   0     1001      127    43477 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/lib.rs
+-rw-r--r--   0     1001      127      872 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/location.rs
+-rw-r--r--   0     1001      127      499 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/marker.rs
+-rw-r--r--   0     1001      127    28375 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/parse.rs
+-rw-r--r--   0     1001      127     2901 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/rcvec.rs
+-rw-r--r--   0     1001      127    26672 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/wrapper.rs
+-rw-r--r--   0     1001      127     3425 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/comments.rs
+-rw-r--r--   0     1001      127      152 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/features.rs
+-rw-r--r--   0     1001      127     2705 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/marker.rs
+-rw-r--r--   0     1001      127    22341 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/test.rs
+-rw-r--r--   0     1001      127     1312 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/test_fmt.rs
+-rw-r--r--   0     1001      127     1365 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/test_size.rs
+-rw-r--r--   0     1001      127      743 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1459 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/Cargo.toml
+-rw-r--r--   0     1001      127    10781 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1107 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/LICENSE-MIT
+-rw-r--r--   0     1001      127     2498 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/build.rs
+-rw-r--r--   0     1001      127     3898 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/src/errors.rs
+-rw-r--r--   0     1001      127    90650 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/src/impl_.rs
+-rw-r--r--   0     1001      127     2032 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/src/import_lib.rs
+-rw-r--r--   0     1001      127     9381 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/src/lib.rs
+-rw-r--r--   0     1001      127     8015 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/.cargo-checksum.json
+-rw-r--r--   0     1001      127      266 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/ACKNOWLEDGEMENTS
+-rw-r--r--   0     1001      127     1593 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/Cargo.toml
+-rw-r--r--   0     1001      127    10781 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1107 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/LICENSE-MIT
+-rw-r--r--   0     1001      127     6375 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/README.md
+-rw-r--r--   0     1001      127     4018 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/build.rs
+-rw-r--r--   0     1001      127    15383 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/abstract_.rs
+-rw-r--r--   0     1001      127      233 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/bltinmodule.rs
+-rw-r--r--   0     1001      127     1294 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/boolobject.rs
+-rw-r--r--   0     1001      127     1874 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/bytearrayobject.rs
+-rw-r--r--   0     1001      127     2355 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/bytesobject.rs
+-rw-r--r--   0     1001      127     4431 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/ceval.rs
+-rw-r--r--   0     1001      127       53 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/code.rs
+-rw-r--r--   0     1001      127     2632 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/codecs.rs
+-rw-r--r--   0     1001      127      257 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/compile.rs
+-rw-r--r--   0     1001      127     2127 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/complexobject.rs
+-rw-r--r--   0     1001      127     1604 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/context.rs
+-rw-r--r--   0     1001      127     9978 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/abstract_.rs
+-rw-r--r--   0     1001      127      556 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/bytesobject.rs
+-rw-r--r--   0     1001      127      733 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/ceval.rs
+-rw-r--r--   0     1001      127     9164 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/code.rs
+-rw-r--r--   0     1001      127     3206 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/compile.rs
+-rw-r--r--   0     1001      127     1790 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/descrobject.rs
+-rw-r--r--   0     1001      127     2163 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/dictobject.rs
+-rw-r--r--   0     1001      127      572 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/floatobject.rs
+-rw-r--r--   0     1001      127     2530 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/frameobject.rs
+-rw-r--r--   0     1001      127     3495 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/funcobject.rs
+-rw-r--r--   0     1001      127     2586 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/genobject.rs
+-rw-r--r--   0     1001      127     1927 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/import.rs
+-rw-r--r--   0     1001      127     6136 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/initconfig.rs
+-rw-r--r--   0     1001      127      968 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/listobject.rs
+-rw-r--r--   0     1001      127     1741 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/methodobject.rs
+-rw-r--r--   0     1001      127     1879 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/mod.rs
+-rw-r--r--   0     1001      127    13622 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/object.rs
+-rw-r--r--   0     1001      127     1809 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/objimpl.rs
+-rw-r--r--   0     1001      127     2784 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pydebug.rs
+-rw-r--r--   0     1001      127     4597 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pyerrors.rs
+-rw-r--r--   0     1001      127       53 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pyframe.rs
+-rw-r--r--   0     1001      127     2642 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pylifecycle.rs
+-rw-r--r--   0     1001      127     1645 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pymem.rs
+-rw-r--r--   0     1001      127     3422 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pystate.rs
+-rw-r--r--   0     1001      127     7235 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pythonrun.rs
+-rw-r--r--   0     1001      127      875 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/tupleobject.rs
+-rw-r--r--   0     1001      127    22871 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/unicodeobject.rs
+-rw-r--r--   0     1001      127      465 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/weakrefobject.rs
+-rw-r--r--   0     1001      127    20094 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/datetime.rs
+-rw-r--r--   0     1001      127     4760 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/descrobject.rs
+-rw-r--r--   0     1001      127     4507 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/dictobject.rs
+-rw-r--r--   0     1001      127      191 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/enumobject.rs
+-rw-r--r--   0     1001      127     1382 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/fileobject.rs
+-rw-r--r--   0     1001      127      274 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/fileutils.rs
+-rw-r--r--   0     1001      127     1545 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/floatobject.rs
+-rw-r--r--   0     1001      127     3192 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/import.rs
+-rw-r--r--   0     1001      127      642 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/intrcheck.rs
+-rw-r--r--   0     1001      127      790 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/iterobject.rs
+-rw-r--r--   0     1001      127    13409 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/lib.rs
+-rw-r--r--   0     1001      127     2666 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/listobject.rs
+-rw-r--r--   0     1001      127     5383 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/longobject.rs
+-rw-r--r--   0     1001      127      755 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/marshal.rs
+-rw-r--r--   0     1001      127     1369 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/memoryobject.rs
+-rw-r--r--   0     1001      127     7821 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/methodobject.rs
+-rw-r--r--   0     1001      127     5558 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/modsupport.rs
+-rw-r--r--   0     1001      127     3556 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/moduleobject.rs
+-rw-r--r--   0     1001      127    24032 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/object.rs
+-rw-r--r--   0     1001      127     3256 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/objimpl.rs
+-rw-r--r--   0     1001      127      158 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/osmodule.rs
+-rw-r--r--   0     1001      127       25 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pyarena.rs
+-rw-r--r--   0     1001      127     4630 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pybuffer.rs
+-rw-r--r--   0     1001      127     2176 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pycapsule.rs
+-rw-r--r--   0     1001      127    17662 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pyerrors.rs
+-rw-r--r--   0     1001      127      427 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pyframe.rs
+-rw-r--r--   0     1001      127     1298 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pyhash.rs
+-rw-r--r--   0     1001      127     1754 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pylifecycle.rs
+-rw-r--r--   0     1001      127      510 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pymem.rs
+-rw-r--r--   0     1001      127      726 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pyport.rs
+-rw-r--r--   0     1001      127     3096 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pystate.rs
+-rw-r--r--   0     1001      127     1164 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pystrtod.rs
+-rw-r--r--   0     1001      127     1992 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pythonrun.rs
+-rw-r--r--   0     1001      127      469 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/rangeobject.rs
+-rw-r--r--   0     1001      127     4408 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/setobject.rs
+-rw-r--r--   0     1001      127     2354 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/sliceobject.rs
+-rw-r--r--   0     1001      127     1100 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/structmember.rs
+-rw-r--r--   0     1001      127     1892 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/structseq.rs
+-rw-r--r--   0     1001      127     1369 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/sysmodule.rs
+-rw-r--r--   0     1001      127      813 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/traceback.rs
+-rw-r--r--   0     1001      127     1490 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/tupleobject.rs
+-rw-r--r--   0     1001      127     3057 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/typeslots.rs
+-rw-r--r--   0     1001      127    13599 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/unicodeobject.rs
+-rw-r--r--   0     1001      127      959 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/warnings.rs
+-rw-r--r--   0     1001      127     2007 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/weakrefobject.rs
+-rw-r--r--   0     1001      127     2744 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1322 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/LICENSE-MIT
+-rw-r--r--   0     1001      127     9302 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/README.md
+-rw-r--r--   0     1001      127       38 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/rust-toolchain.toml
+-rw-r--r--   0     1001      127     2739 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/src/ext.rs
+-rw-r--r--   0     1001      127     4796 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/src/format.rs
+-rw-r--r--   0     1001      127     2309 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/src/ident_fragment.rs
+-rw-r--r--   0     1001      127    44977 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/src/lib.rs
+-rw-r--r--   0     1001      127    16224 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/src/runtime.rs
+-rw-r--r--   0     1001      127     1112 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/src/spanned.rs
+-rw-r--r--   0     1001      127     5454 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/src/to_tokens.rs
+-rw-r--r--   0     1001      127      166 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/compiletest.rs
+-rw-r--r--   0     1001      127    12980 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/test.rs
+-rw-r--r--   0     1001      127      209 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated-dup.rs
+-rw-r--r--   0     1001      127      559 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated-dup.stderr
+-rw-r--r--   0     1001      127      201 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated.rs
+-rw-r--r--   0     1001      127      539 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated.stderr
+-rw-r--r--   0     1001      127       55 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-separated.rs
+-rw-r--r--   0     1001      127      444 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-separated.stderr
+-rw-r--r--   0     1001      127       54 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter.rs
+-rw-r--r--   0     1001      127      432 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter.stderr
+-rw-r--r--   0     1001      127      119 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/not-quotable.rs
+-rw-r--r--   0     1001      127      659 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/not-quotable.stderr
+-rw-r--r--   0     1001      127      106 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/not-repeatable.rs
+-rw-r--r--   0     1001      127     1464 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/not-repeatable.stderr
+-rw-r--r--   0     1001      127      109 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/wrong-type-span.rs
+-rw-r--r--   0     1001      127      346 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/wrong-type-span.stderr
+-rw-r--r--   0     1001      127     2936 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1157 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/LICENSE-MIT
+-rw-r--r--   0     1001      127     4317 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/README.md
+-rw-r--r--   0     1001      127     2340 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/build/build.rs
+-rw-r--r--   0     1001      127     3661 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/build/rustc.rs
+-rw-r--r--   0     1001      127      886 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/attr.rs
+-rw-r--r--   0     1001      127     1982 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/bound.rs
+-rw-r--r--   0     1001      127     1827 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/constfn.rs
+-rw-r--r--   0     1001      127     1406 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/date.rs
+-rw-r--r--   0     1001      127     1714 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/error.rs
+-rw-r--r--   0     1001      127     2746 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/expand.rs
+-rw-r--r--   0     1001      127     5189 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/expr.rs
+-rw-r--r--   0     1001      127     1061 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/iter.rs
+-rw-r--r--   0     1001      127     7698 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/lib.rs
+-rw-r--r--   0     1001      127      929 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/release.rs
+-rw-r--r--   0     1001      127     1408 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/time.rs
+-rw-r--r--   0     1001      127     2442 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/token.rs
+-rw-r--r--   0     1001      127      289 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/src/version.rs
+-rw-r--r--   0     1001      127      166 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/compiletest.rs
+-rw-r--r--   0     1001      127      800 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/test_const.rs
+-rw-r--r--   0     1001      127      307 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/test_eval.rs
+-rw-r--r--   0     1001      127     2522 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/test_parse.rs
+-rw-r--r--   0     1001      127      100 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/bad-bound.rs
+-rw-r--r--   0     1001      127      374 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/bad-bound.stderr
+-rw-r--r--   0     1001      127      104 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/bad-date.rs
+-rw-r--r--   0     1001      127      312 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/bad-date.stderr
+-rw-r--r--   0     1001      127       90 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/bad-not.rs
+-rw-r--r--   0     1001      127      239 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/bad-not.stderr
+-rw-r--r--   0     1001      127      104 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/bad-version.rs
+-rw-r--r--   0     1001      127      322 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/bad-version.stderr
+-rw-r--r--   0     1001      127       63 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/const-not-fn.rs
+-rw-r--r--   0     1001      127      148 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/ui/const-not-fn.stderr
+-rw-r--r--   0     1001      127     2765 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/.cargo-checksum.json
+-rw-r--r--   0     1001      127     3777 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/Cargo.lock
+-rw-r--r--   0     1001      127     1311 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1338 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/LICENSE-BOOST
+-rw-r--r--   0     1001      127     3702 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/README.md
+-rw-r--r--   0     1001      127     1532 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/benches/bench.rs
+-rw-r--r--   0     1001      127     2189 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/examples/upstream_benchmark.rs
+-rw-r--r--   0     1001      127     5138 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/buffer/mod.rs
+-rw-r--r--   0     1001      127     3237 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/common.rs
+-rw-r--r--   0     1001      127    11284 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/d2s.rs
+-rw-r--r--   0     1001      127    32886 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/d2s_full_table.rs
+-rw-r--r--   0     1001      127     2567 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/d2s_intrinsics.rs
+-rw-r--r--   0     1001      127     5370 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/d2s_small_table.rs
+-rw-r--r--   0     1001      127     1203 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/digit_table.rs
+-rw-r--r--   0     1001      127     6959 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/f2s.rs
+-rw-r--r--   0     1001      127     3700 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/f2s_intrinsics.rs
+-rw-r--r--   0     1001      127     4039 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/lib.rs
+-rw-r--r--   0     1001      127      479 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/parse.rs
+-rw-r--r--   0     1001      127     1242 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/pretty/exponent.rs
+-rw-r--r--   0     1001      127     2391 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/pretty/mantissa.rs
+-rw-r--r--   0     1001      127     8015 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/pretty/mod.rs
+-rw-r--r--   0     1001      127     7756 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/s2d.rs
+-rw-r--r--   0     1001      127     8315 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/src/s2f.rs
+-rw-r--r--   0     1001      127     2497 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/tests/common_test.rs
+-rw-r--r--   0     1001      127     1698 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/tests/d2s_table_test.rs
+-rw-r--r--   0     1001      127     9617 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/tests/d2s_test.rs
+-rw-r--r--   0     1001      127     1613 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/tests/exhaustive.rs
+-rw-r--r--   0     1001      127     4572 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/tests/f2s_test.rs
+-rw-r--r--   0     1001      127      183 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/tests/macros/mod.rs
+-rw-r--r--   0     1001      127     5059 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/tests/s2d_test.rs
+-rw-r--r--   0     1001      127     3152 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/ryu-1.0.15/tests/s2f_test.rs
+-rw-r--r--   0     1001      127     2207 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1565 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/LICENSE-MIT
+-rw-r--r--   0     1001      127     4366 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/README.md
+-rw-r--r--   0     1001      127     3138 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/build.rs
+-rw-r--r--   0     1001      127     2538 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/crates-io.md
+-rw-r--r--   0     1001      127      726 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/de/format.rs
+-rw-r--r--   0     1001      127     6154 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/de/ignored_any.rs
+-rw-r--r--   0     1001      127    91490 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/de/impls.rs
+-rw-r--r--   0     1001      127    80313 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/de/mod.rs
+-rw-r--r--   0     1001      127      563 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/de/seed.rs
+-rw-r--r--   0     1001      127      644 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/de/size_hint.rs
+-rw-r--r--   0     1001      127    44831 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/de/value.rs
+-rw-r--r--   0     1001      127      243 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/integer128.rs
+-rw-r--r--   0     1001      127    13294 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/lib.rs
+-rw-r--r--   0     1001      127     8264 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/macros.rs
+-rw-r--r--   0     1001      127    86931 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/private/de.rs
+-rw-r--r--   0     1001      127     4888 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/private/doc.rs
+-rw-r--r--   0     1001      127     1567 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/private/mod.rs
+-rw-r--r--   0     1001      127    40321 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/private/ser.rs
+-rw-r--r--   0     1001      127     4169 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/ser/fmt.rs
+-rw-r--r--   0     1001      127    28630 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/ser/impls.rs
+-rw-r--r--   0     1001      127     5287 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/ser/impossible.rs
+-rw-r--r--   0     1001      127    62995 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/ser/mod.rs
+-rw-r--r--   0     1001      127     1347 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde-1.0.188/src/std_error.rs
+-rw-r--r--   0     1001      127     1973 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1412 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/LICENSE-MIT
+-rw-r--r--   0     1001      127     4366 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/README.md
+-rw-r--r--   0     1001      127     2538 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/crates-io.md
+-rw-r--r--   0     1001      127    14709 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/bound.rs
+-rw-r--r--   0     1001      127   109306 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/de.rs
+-rw-r--r--   0     1001      127      611 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/dummy.rs
+-rw-r--r--   0     1001      127     2116 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/fragment.rs
+-rw-r--r--   0     1001      127     6601 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/ast.rs
+-rw-r--r--   0     1001      127    68804 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/attr.rs
+-rw-r--r--   0     1001      127     7121 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/case.rs
+-rw-r--r--   0     1001      127    16638 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/check.rs
+-rw-r--r--   0     1001      127     2021 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/ctxt.rs
+-rw-r--r--   0     1001      127      381 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/mod.rs
+-rw-r--r--   0     1001      127    10519 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/receiver.rs
+-rw-r--r--   0     1001      127      451 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/respan.rs
+-rw-r--r--   0     1001      127     2523 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/symbol.rs
+-rw-r--r--   0     1001      127     3000 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/lib.rs
+-rw-r--r--   0     1001      127     5718 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/pretend.rs
+-rw-r--r--   0     1001      127    45209 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/ser.rs
+-rw-r--r--   0     1001      127     1007 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/this.rs
+-rw-r--r--   0     1001      127     7848 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1733 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/CONTRIBUTING.md
+-rw-r--r--   0     1001      127     2170 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/LICENSE-MIT
+-rw-r--r--   0     1001      127    14217 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/README.md
+-rw-r--r--   0     1001      127      521 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/build.rs
+-rw-r--r--   0     1001      127    85485 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/de.rs
+-rw-r--r--   0     1001      127    16571 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/error.rs
+-rw-r--r--   0     1001      127       80 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/features_check/error.rs
+-rw-r--r--   0     1001      127      269 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/features_check/mod.rs
+-rw-r--r--   0     1001      127     1739 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/io/core.rs
+-rw-r--r--   0     1001      127      684 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/io/mod.rs
+-rw-r--r--   0     1001      127     1848 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/iter.rs
+-rw-r--r--   0     1001      127     6154 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/algorithm.rs
+-rw-r--r--   0     1001      127     7039 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/bhcomp.rs
+-rw-r--r--   0     1001      127      654 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/bignum.rs
+-rw-r--r--   0     1001      127     2156 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/cached.rs
+-rw-r--r--   0     1001      127     5782 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/cached_float80.rs
+-rw-r--r--   0     1001      127      444 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/digit.rs
+-rw-r--r--   0     1001      127     5082 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/errors.rs
+-rw-r--r--   0     1001      127     1578 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/exponent.rs
+-rw-r--r--   0     1001      127     5482 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/float.rs
+-rw-r--r--   0     1001      127      232 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/large_powers.rs
+-rw-r--r--   0     1001      127    15360 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/large_powers32.rs
+-rw-r--r--   0     1001      127    15877 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/large_powers64.rs
+-rw-r--r--   0     1001      127    26259 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/math.rs
+-rw-r--r--   0     1001      127     1041 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/mod.rs
+-rw-r--r--   0     1001      127    11811 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/num.rs
+-rw-r--r--   0     1001      127     2241 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/parse.rs
+-rw-r--r--   0     1001      127     7396 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/rounding.rs
+-rw-r--r--   0     1001      127     1235 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/shift.rs
+-rw-r--r--   0     1001      127     1318 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/small_powers.rs
+-rw-r--r--   0     1001      127    13642 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lib.rs
+-rw-r--r--   0     1001      127    10129 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/macros.rs
+-rw-r--r--   0     1001      127    24860 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/map.rs
+-rw-r--r--   0     1001      127    24054 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/number.rs
+-rw-r--r--   0     1001      127    21194 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/raw.rs
+-rw-r--r--   0     1001      127    31338 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/read.rs
+-rw-r--r--   0     1001      127    62121 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/ser.rs
+-rw-r--r--   0     1001      127    38943 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/de.rs
+-rw-r--r--   0     1001      127     5962 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/from.rs
+-rw-r--r--   0     1001      127     8789 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/index.rs
+-rw-r--r--   0     1001      127    29737 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/mod.rs
+-rw-r--r--   0     1001      127     2371 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/partial_eq.rs
+-rw-r--r--   0     1001      127    27587 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/ser.rs
+-rw-r--r--   0     1001      127      166 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/compiletest.rs
+-rw-r--r--   0     1001      127     1995 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/debug.rs
+-rw-r--r--   0     1001      127     3867 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/algorithm.rs
+-rw-r--r--   0     1001      127     1548 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/exponent.rs
+-rw-r--r--   0     1001      127    14186 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/float.rs
+-rw-r--r--   0     1001      127     5418 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/math.rs
+-rw-r--r--   0     1001      127     1642 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/num.rs
+-rw-r--r--   0     1001      127    17154 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/parse.rs
+-rw-r--r--   0     1001      127     9038 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/rounding.rs
+-rw-r--r--   0     1001      127     1080 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical.rs
+-rw-r--r--   0     1001      127     1511 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/macros/mod.rs
+-rw-r--r--   0     1001      127     1268 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/map.rs
+-rw-r--r--   0     1001      127      362 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/regression/issue1004.rs
+-rw-r--r--   0     1001      127      401 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/regression/issue520.rs
+-rw-r--r--   0     1001      127     1605 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/regression/issue795.rs
+-rw-r--r--   0     1001      127     1895 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/regression/issue845.rs
+-rw-r--r--   0     1001      127      236 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/regression/issue953.rs
+-rw-r--r--   0     1001      127       58 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/regression.rs
+-rw-r--r--   0     1001      127     5130 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/stream.rs
+-rw-r--r--   0     1001      127    74363 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/test.rs
+-rw-r--r--   0     1001      127       57 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/missing_colon.rs
+-rw-r--r--   0     1001      127      448 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/missing_colon.stderr
+-rw-r--r--   0     1001      127       69 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/missing_comma.rs
+-rw-r--r--   0     1001      127      377 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/missing_comma.stderr
+-rw-r--r--   0     1001      127       59 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/missing_value.rs
+-rw-r--r--   0     1001      127      452 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/missing_value.stderr
+-rw-r--r--   0     1001      127       61 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/not_found.rs
+-rw-r--r--   0     1001      127      162 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/not_found.stderr
+-rw-r--r--   0     1001      127       61 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/parse_expr.rs
+-rw-r--r--   0     1001      127      305 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/parse_expr.stderr
+-rw-r--r--   0     1001      127       65 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/parse_key.rs
+-rw-r--r--   0     1001      127      139 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/parse_key.stderr
+-rw-r--r--   0     1001      127       61 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/unexpected_after_array_element.rs
+-rw-r--r--   0     1001      127      241 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/unexpected_after_array_element.stderr
+-rw-r--r--   0     1001      127       66 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/unexpected_after_map_entry.rs
+-rw-r--r--   0     1001      127      247 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/unexpected_after_map_entry.stderr
+-rw-r--r--   0     1001      127       60 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/unexpected_colon.rs
+-rw-r--r--   0     1001      127      219 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/unexpected_colon.stderr
+-rw-r--r--   0     1001      127       69 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/unexpected_comma.rs
+-rw-r--r--   0     1001      127      232 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/ui/unexpected_comma.stderr
+-rw-r--r--   0     1001      127     2259 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/.cargo-checksum.json
+-rw-r--r--   0     1001      127     2729 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/CHANGELOG.md
+-rw-r--r--   0     1001      127      152 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/Cargo.lock
+-rw-r--r--   0     1001      127     1464 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      127    10173 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/LICENSE-Apache
+-rw-r--r--   0     1001      127     1035 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/LICENSE-MIT
+-rw-r--r--   0     1001      127     9360 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/README.md
+-rw-r--r--   0     1001      127     1063 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/examples/streaming.rs
+-rw-r--r--   0     1001      127      952 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/release.toml
+-rw-r--r--   0     1001      127       14 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/rustfmt.toml
+-rw-r--r--   0     1001      127    10608 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/basic.rs
+-rw-r--r--   0     1001      127     4838 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/compat.rs
+-rw-r--r--   0     1001      127     1479 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/aarch64/mod.rs
+-rw-r--r--   0     1001      127     6044 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/aarch64/neon.rs
+-rw-r--r--   0     1001      127    23187 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/algorithm.rs
+-rw-r--r--   0     1001      127     3620 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/helpers.rs
+-rw-r--r--   0     1001      127     2537 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/mod.rs
+-rw-r--r--   0     1001      127     1304 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/wasm32/mod.rs
+-rw-r--r--   0     1001      127     6185 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/wasm32/simd128.rs
+-rw-r--r--   0     1001      127     7088 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/x86/avx2.rs
+-rw-r--r--   0     1001      127     5494 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/x86/mod.rs
+-rw-r--r--   0     1001      127     6525 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/x86/sse42.rs
+-rw-r--r--   0     1001      127     5414 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      127    16410 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/tests/tests.rs
+-rw-r--r--   0     1001      127     1475 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/simdutf8-0.1.4/wasm32-development.md
+-rw-r--r--   0     1001      127     1302 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1684 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1072 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/LICENSE-MIT
+-rw-r--r--   0     1001      127      649 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/README.md
+-rw-r--r--   0     1001      127     8567 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/benches/bench.rs
+-rw-r--r--   0     1001      127     5231 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/debug_metadata/README.md
+-rw-r--r--   0     1001      127     1561 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/debug_metadata/smallvec.natvis
+-rw-r--r--   0     1001      127      730 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/scripts/run_miri.sh
+-rw-r--r--   0     1001      127      570 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/src/arbitrary.rs
+-rw-r--r--   0     1001      127    78554 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/src/lib.rs
+-rw-r--r--   0     1001      127      611 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/src/specialization.rs
+-rw-r--r--   0     1001      127    25779 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/src/tests.rs
+-rw-r--r--   0     1001      127     1888 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/tests/debugger_visualizer.rs
+-rw-r--r--   0     1001      127      542 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/smallvec-1.11.1/tests/macro.rs
+-rw-r--r--   0     1001      127     1380 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/.cargo-checksum.json
+-rw-r--r--   0     1001      127     6229 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/CHANGELOG.md
+-rw-r--r--   0     1001      127     1411 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/Cargo.toml
+-rw-r--r--   0     1001      127    11358 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1072 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/LICENSE-MIT
+-rw-r--r--   0     1001      127     7437 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/README.md
+-rw-r--r--   0     1001      127     1734 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_cfg.rs
+-rw-r--r--   0     1001      127     1405 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_eq_align.rs
+-rw-r--r--   0     1001      127     3450 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_eq_size.rs
+-rw-r--r--   0     1001      127     1865 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_fields.rs
+-rw-r--r--   0     1001      127    12894 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_impl.rs
+-rw-r--r--   0     1001      127     2381 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_obj_safe.rs
+-rw-r--r--   0     1001      127     3106 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_trait.rs
+-rw-r--r--   0     1001      127     2854 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_type.rs
+-rw-r--r--   0     1001      127     2994 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/const_assert.rs
+-rw-r--r--   0     1001      127     3450 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/lib.rs
+-rw-r--r--   0     1001      127     8306 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/.cargo-checksum.json
+-rw-r--r--   0     1001      127     2678 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/LICENSE-MIT
+-rw-r--r--   0     1001      127    10396 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/README.md
+-rw-r--r--   0     1001      127     1331 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/benches/file.rs
+-rw-r--r--   0     1001      127     4956 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/benches/rust.rs
+-rw-r--r--   0     1001      127    26351 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/attr.rs
+-rw-r--r--   0     1001      127     1610 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/bigint.rs
+-rw-r--r--   0     1001      127    15994 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/buffer.rs
+-rw-r--r--   0     1001      127     7826 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/custom_keyword.rs
+-rw-r--r--   0     1001      127     9061 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/custom_punctuation.rs
+-rw-r--r--   0     1001      127     9777 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/data.rs
+-rw-r--r--   0     1001      127     8263 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/derive.rs
+-rw-r--r--   0     1001      127     9053 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/discouraged.rs
+-rw-r--r--   0     1001      127     1430 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/drops.rs
+-rw-r--r--   0     1001      127    14065 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/error.rs
+-rw-r--r--   0     1001      127     1584 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/export.rs
+-rw-r--r--   0     1001      127   112265 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/expr.rs
+-rw-r--r--   0     1001      127     3886 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/ext.rs
+-rw-r--r--   0     1001      127     3749 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/file.rs
+-rw-r--r--   0     1001      127    69617 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/clone.rs
+-rw-r--r--   0     1001      127   126176 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/debug.rs
+-rw-r--r--   0     1001      127    84324 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/eq.rs
+-rw-r--r--   0     1001      127   102480 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/fold.rs
+-rw-r--r--   0     1001      127    72585 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/hash.rs
+-rw-r--r--   0     1001      127    97057 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/visit.rs
+-rw-r--r--   0     1001      127   101467 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/visit_mut.rs
+-rw-r--r--   0     1001      127      840 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/gen_helper.rs
+-rw-r--r--   0     1001      127    41419 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/generics.rs
+-rw-r--r--   0     1001      127     7922 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/group.rs
+-rw-r--r--   0     1001      127     3122 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/ident.rs
+-rw-r--r--   0     1001      127   117455 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/item.rs
+-rw-r--r--   0     1001      127    31818 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/lib.rs
+-rw-r--r--   0     1001      127     3825 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/lifetime.rs
+-rw-r--r--   0     1001      127    49150 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/lit.rs
+-rw-r--r--   0     1001      127     5345 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/lookahead.rs
+-rw-r--r--   0     1001      127     7463 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/mac.rs
+-rw-r--r--   0     1001      127     4653 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/macros.rs
+-rw-r--r--   0     1001      127    14112 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/meta.rs
+-rw-r--r--   0     1001      127     8429 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/op.rs
+-rw-r--r--   0     1001      127    44840 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/parse.rs
+-rw-r--r--   0     1001      127     3497 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/parse_macro_input.rs
+-rw-r--r--   0     1001      127     5373 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/parse_quote.rs
+-rw-r--r--   0     1001      127    29968 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/pat.rs
+-rw-r--r--   0     1001      127    30668 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/path.rs
+-rw-r--r--   0     1001      127      390 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/print.rs
+-rw-r--r--   0     1001      127    29942 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/punctuated.rs
+-rw-r--r--   0     1001      127     5815 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/restriction.rs
+-rw-r--r--   0     1001      127       87 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/sealed.rs
+-rw-r--r--   0     1001      127     1197 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/span.rs
+-rw-r--r--   0     1001      127     3763 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/spanned.rs
+-rw-r--r--   0     1001      127    15355 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/stmt.rs
+-rw-r--r--   0     1001      127     1904 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/thread.rs
+-rw-r--r--   0     1001      127    37419 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/token.rs
+-rw-r--r--   0     1001      127     3727 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/tt.rs
+-rw-r--r--   0     1001      127    41263 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/ty.rs
+-rw-r--r--   0     1001      127     1216 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/verbatim.rs
+-rw-r--r--   0     1001      127     2103 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/src/whitespace.rs
+-rw-r--r--   0     1001      127    30636 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/common/eq.rs
+-rw-r--r--   0     1001      127      760 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/common/mod.rs
+-rw-r--r--   0     1001      127     1399 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/common/parse.rs
+-rw-r--r--   0     1001      127   188757 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/debug/gen.rs
+-rw-r--r--   0     1001      127     3199 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/debug/mod.rs
+-rw-r--r--   0     1001      127     2275 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/macros/mod.rs
+-rw-r--r--   0     1001      127       97 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/regression/issue1108.rs
+-rw-r--r--   0     1001      127      932 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/regression/issue1235.rs
+-rw-r--r--   0     1001      127      132 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/regression.rs
+-rw-r--r--   0     1001      127    15054 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/repo/mod.rs
+-rw-r--r--   0     1001      127      844 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/repo/progress.rs
+-rw-r--r--   0     1001      127      728 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_asyncness.rs
+-rw-r--r--   0     1001      127     4429 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_attribute.rs
+-rw-r--r--   0     1001      127    21384 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_derive_input.rs
+-rw-r--r--   0     1001      127     8562 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_expr.rs
+-rw-r--r--   0     1001      127     8906 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_generics.rs
+-rw-r--r--   0     1001      127     1518 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_grouping.rs
+-rw-r--r--   0     1001      127     1288 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_ident.rs
+-rw-r--r--   0     1001      127     7974 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_item.rs
+-rw-r--r--   0     1001      127     1774 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_iterators.rs
+-rw-r--r--   0     1001      127     8512 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_lit.rs
+-rw-r--r--   0     1001      127     3128 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_meta.rs
+-rw-r--r--   0     1001      127     2686 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_parse_buffer.rs
+-rw-r--r--   0     1001      127      311 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_parse_stream.rs
+-rw-r--r--   0     1001      127     3244 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_pat.rs
+-rw-r--r--   0     1001      127     3700 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_path.rs
+-rw-r--r--   0     1001      127    16304 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_precedence.rs
+-rw-r--r--   0     1001      127     8290 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_receiver.rs
+-rw-r--r--   0     1001      127     8115 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_round_trip.rs
+-rw-r--r--   0     1001      127     1655 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_shebang.rs
+-rw-r--r--   0     1001      127      915 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_should_parse.rs
+-rw-r--r--   0     1001      127      780 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_size.rs
+-rw-r--r--   0     1001      127     6398 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_stmt.rs
+-rw-r--r--   0     1001      127      675 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_token_trees.rs
+-rw-r--r--   0     1001      127    10949 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_ty.rs
+-rw-r--r--   0     1001      127     3704 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_visibility.rs
+-rw-r--r--   0     1001      127     1098 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/syn-2.0.38/tests/zzz_stable.rs
+-rw-r--r--   0     1001      127     1250 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1012 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/Cargo.lock
+-rw-r--r--   0     1001      127     1172 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/Cargo.toml
+-rw-r--r--   0     1001      127    12243 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/LICENSE
+-rw-r--r--   0     1001      127      957 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/README.md
+-rw-r--r--   0     1001      127     5117 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/build.rs
+-rw-r--r--   0     1001      127      208 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/examples/host.rs
+-rw-r--r--   0     1001      127      405 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/examples/misc.rs
+-rwxr-xr-x   0     1001      127      212 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/scripts/rust-targets.sh
+-rw-r--r--   0     1001      127     3160 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/data_model.rs
+-rw-r--r--   0     1001      127     1557 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/host.rs
+-rw-r--r--   0     1001      127     3098 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/lib.rs
+-rw-r--r--   0     1001      127     1208 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/parse_error.rs
+-rw-r--r--   0     1001      127    54160 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/targets.rs
+-rw-r--r--   0     1001      127    18653 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/triple.rs
+-rw-r--r--   0     1001      127     1641 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/.cargo-checksum.json
+-rw-r--r--   0     1001      127     1594 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/Cargo.toml
+-rw-r--r--   0     1001      127     9723 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/LICENSE-MIT
+-rw-r--r--   0     1001      127     2315 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/LICENSE-UNICODE
+-rw-r--r--   0     1001      127    12498 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/README.md
+-rw-r--r--   0     1001      127     4020 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/benches/xid.rs
+-rw-r--r--   0     1001      127    12596 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/src/lib.rs
+-rw-r--r--   0     1001      127    62702 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/src/tables.rs
+-rw-r--r--   0     1001      127     1790 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/compare.rs
+-rw-r--r--   0     1001      127      385 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/fst/mod.rs
+-rw-r--r--   0     1001      127    73249 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/fst/xid_continue.fst
+-rw-r--r--   0     1001      127    65487 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/fst/xid_start.fst
+-rw-r--r--   0     1001      127      502 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/roaring/mod.rs
+-rw-r--r--   0     1001      127     2456 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/static_size.rs
+-rw-r--r--   0     1001      127      144 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/tables/mod.rs
+-rw-r--r--   0     1001      127    23400 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/tables/tables.rs
+-rw-r--r--   0     1001      127      179 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/trie/mod.rs
+-rw-r--r--   0     1001      127    30278 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/trie/trie.rs
+-rw-r--r--   0     1001      127      741 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/version_check-0.9.4/.cargo-checksum.json
+-rw-r--r--   0     1001      127      890 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/version_check-0.9.4/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/version_check-0.9.4/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1085 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/version_check-0.9.4/LICENSE-MIT
+-rw-r--r--   0     1001      127     2669 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/version_check-0.9.4/README.md
+-rw-r--r--   0     1001      127     5425 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/version_check-0.9.4/src/channel.rs
+-rw-r--r--   0     1001      127     6198 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/version_check-0.9.4/src/date.rs
+-rw-r--r--   0     1001      127    19153 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/version_check-0.9.4/src/lib.rs
+-rw-r--r--   0     1001      127    10435 2023-10-12 23:01:36.000000 orjson-3.9.9/include/cargo/version_check-0.9.4/src/version.rs
+-rw-r--r--   0        0        0    49257 1970-01-01 00:00:00.000000 orjson-3.9.9/PKG-INFO
```

### Comparing `orjson-3.9.8/Cargo.toml` & `orjson-3.9.9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "orjson"
-version = "3.9.8"
+version = "3.9.9"
 authors = ["ijl <ijl@mailbox.org>"]
 description = "Fast, correct Python JSON library supporting dataclasses, datetimes, and numpy"
 edition = "2021"
 resolver = "2"
 rust-version = "1.65"
 license = "Apache-2.0 OR MIT"
 repository = "https://github.com/ijl/orjson"
@@ -55,24 +55,24 @@
 bytecount = { version = "^0.6.4", default_features = false, features = ["runtime-dispatch-simd"] }
 chrono = { version = "^0.4.24", default_features = false }
 compact_str = { version = "0.7", default_features = false, features = ["serde"] }
 encoding_rs = { version = "0.8", default_features = false }
 itoa = { version = "1", default_features = false }
 itoap = { version = "1", features = ["std", "simd"] }
 once_cell = { version = "1", default_features = false, features = ["race"] }
-pyo3-ffi = { version = "^0.19.2", default_features = false, features = ["extension-module"]}
+pyo3-ffi = { version = "^0.20", default_features = false, features = ["extension-module"]}
 ryu = { version = "1", default_features = false }
 serde = { version = "1", default_features = false }
 serde_json = { version = "1", default_features = false, features = ["std", "float_roundtrip"] }
 simdutf8 = { version = "0.1", default_features = false, features = ["std", "aarch64_neon"] }
 smallvec = { version = "^1.11", default_features = false, features = ["union", "write"] }
 
 [build-dependencies]
 cc = { version = "1" }
-pyo3-build-config = { version = "^0.19.2" }
+pyo3-build-config = { version = "^0.20" }
 version_check = { version = "0.9" }
 
 [profile.dev]
 codegen-units = 1
 debug = 2
 debug-assertions = true
 incremental = false
```

### Comparing `orjson-3.9.8/CHANGELOG.md` & `orjson-3.9.9/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 3.9.9 - 2023-10-12
+
+### Changed
+
+- `orjson` module metadata explicitly marks subinterpreters as not supported.
+
 
 ## 3.9.8 - 2023-10-10
 
 ### Changed
 
 - Improve performance.
 - Drop support for Python 3.7.
```

### Comparing `orjson-3.9.8/LICENSE-APACHE` & `orjson-3.9.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/LICENSE-MIT` & `orjson-3.9.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/README.md` & `orjson-3.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 support for 64-bit
 * does not provide `load()` or `dump()` functions for reading from/writing to
 file-like objects
 
 orjson supports CPython 3.8, 3.9, 3.10, 3.11, and 3.12. It distributes
 amd64/x86_64, aarch64/armv8, arm7, POWER/ppc64le, and s390x wheels for Linux,
 amd64 and aarch64 wheels for macOS, and amd64 and i686/x86 wheels for Windows.
-orjson  does not support PyPy. Releases follow semantic versioning and
+orjson does not and will not support PyPy. orjson does not and will not
+support PEP 554 subinterpreters. Releases follow semantic versioning and
 serializing a new object type without an opt-in flag is considered a
 breaking change.
 
 orjson is licensed under both the Apache 2.0 and MIT licenses. The
 repository and issue tracker is
 [github.com/ijl/orjson](https://github.com/ijl/orjson), and patches may be
 submitted there. There is a
@@ -1173,18 +1174,14 @@
 handle errors etc. This is addressed by data validation libraries a
 level above this.
 
 ### Will it serialize to `str`?
 
 No. `bytes` is the correct type for a serialized blob.
 
-### Will it support PyPy?
-
-Probably not.
-
 ## Packaging
 
 To package orjson requires at least [Rust](https://www.rust-lang.org/) 1.65
 and the [maturin](https://github.com/PyO3/maturin) build tool. The recommended
 build command is:
 
 ```sh
```

### Comparing `orjson-3.9.8/data/blns.txt.xz` & `orjson-3.9.9/data/blns.txt.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/data/canada.json.xz` & `orjson-3.9.9/data/canada.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/data/citm_catalog.json.xz` & `orjson-3.9.9/data/citm_catalog.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/data/github.json.xz` & `orjson-3.9.9/data/github.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/data/issue331_1.json.xz` & `orjson-3.9.9/data/issue331_1.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/data/issue331_2.json.xz` & `orjson-3.9.9/data/issue331_2.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/data/jsonchecker/pass01.json` & `orjson-3.9.9/data/jsonchecker/pass01.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/data/twitter.json.xz` & `orjson-3.9.9/data/twitter.json.xz`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/yyjson/yyjson.c` & `orjson-3.9.9/include/yyjson/yyjson.c`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/yyjson/yyjson.h` & `orjson-3.9.9/include/yyjson/yyjson.h`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/deserialize/cache.rs` & `orjson-3.9.9/src/deserialize/cache.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/deserialize/deserializer.rs` & `orjson-3.9.9/src/deserialize/deserializer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/deserialize/error.rs` & `orjson-3.9.9/src/deserialize/error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/deserialize/json.rs` & `orjson-3.9.9/src/deserialize/json.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/deserialize/pyobject.rs` & `orjson-3.9.9/src/deserialize/pyobject.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/deserialize/utf8.rs` & `orjson-3.9.9/src/deserialize/utf8.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/deserialize/yyjson.rs` & `orjson-3.9.9/src/deserialize/yyjson.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/ffi/buffer.rs` & `orjson-3.9.9/src/ffi/buffer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/ffi/fragment.rs` & `orjson-3.9.9/src/ffi/fragment.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/ffi/list.rs` & `orjson-3.9.9/src/ffi/list.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/ffi/long.rs` & `orjson-3.9.9/src/ffi/long.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/ffi/yyjson.rs` & `orjson-3.9.9/src/ffi/yyjson.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/lib.rs` & `orjson-3.9.9/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -139,24 +139,34 @@
 
     add!(mptr, "JSONDecodeError\0", typeref::JsonDecodeError);
     add!(mptr, "JSONEncodeError\0", typeref::JsonEncodeError);
 
     0
 }
 
+#[cfg(not(Py_3_12))]
+const PYMODULEDEF_LEN: usize = 2;
+#[cfg(Py_3_12)]
+const PYMODULEDEF_LEN: usize = 3;
+
 #[allow(non_snake_case)]
 #[no_mangle]
 #[cold]
 #[cfg_attr(feature = "optimize", optimize(size))]
 pub unsafe extern "C" fn PyInit_orjson() -> *mut PyModuleDef {
-    let mod_slots: Box<[PyModuleDef_Slot; 2]> = Box::new([
+    let mod_slots: Box<[PyModuleDef_Slot; PYMODULEDEF_LEN]> = Box::new([
         PyModuleDef_Slot {
             slot: Py_mod_exec,
             value: orjson_init_exec as *mut c_void,
         },
+        #[cfg(Py_3_12)]
+        PyModuleDef_Slot {
+            slot: Py_mod_multiple_interpreters,
+            value: Py_MOD_MULTIPLE_INTERPRETERS_NOT_SUPPORTED,
+        },
         PyModuleDef_Slot {
             slot: 0,
             value: null_mut(),
         },
     ]);
 
     let init = Box::new(PyModuleDef {
```

### Comparing `orjson-3.9.8/src/opt.rs` & `orjson-3.9.9/src/opt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/error.rs` & `orjson-3.9.9/src/serialize/error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/json.rs` & `orjson-3.9.9/src/serialize/json.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/dataclass.rs` & `orjson-3.9.9/src/serialize/per_type/dataclass.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/datetime.rs` & `orjson-3.9.9/src/serialize/per_type/datetime.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/datetimelike.rs` & `orjson-3.9.9/src/serialize/per_type/datetimelike.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/default.rs` & `orjson-3.9.9/src/serialize/per_type/default.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/dict.rs` & `orjson-3.9.9/src/serialize/per_type/dict.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/float.rs` & `orjson-3.9.9/src/serialize/per_type/float.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/fragment.rs` & `orjson-3.9.9/src/serialize/per_type/fragment.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/int.rs` & `orjson-3.9.9/src/serialize/per_type/int.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/list.rs` & `orjson-3.9.9/src/serialize/per_type/list.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/mod.rs` & `orjson-3.9.9/src/serialize/per_type/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/numpy.rs` & `orjson-3.9.9/src/serialize/per_type/numpy.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/pybool.rs` & `orjson-3.9.9/src/serialize/per_type/pybool.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/pyenum.rs` & `orjson-3.9.9/src/serialize/per_type/pyenum.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/tuple.rs` & `orjson-3.9.9/src/serialize/per_type/tuple.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/unicode.rs` & `orjson-3.9.9/src/serialize/per_type/unicode.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/per_type/uuid.rs` & `orjson-3.9.9/src/serialize/per_type/uuid.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/serializer.rs` & `orjson-3.9.9/src/serialize/serializer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/serialize/writer.rs` & `orjson-3.9.9/src/serialize/writer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/str/check.rs` & `orjson-3.9.9/src/str/check.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/str/create.rs` & `orjson-3.9.9/src/str/create.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/str/ffi.rs` & `orjson-3.9.9/src/str/ffi.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/typeref.rs` & `orjson-3.9.9/src/typeref.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/src/util.rs` & `orjson-3.9.9/src/util.rs`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     };
 }
 
 #[cfg(Py_3_12)]
 macro_rules! reverse_pydict_incref {
     ($op:expr) => {
         unsafe {
-            if crate::ffi::_Py_IsImmortal($op) == 0 {
+            if pyo3_ffi::_Py_IsImmortal($op) == 0 {
                 debug_assert!(ffi!(Py_REFCNT($op)) >= 2);
                 (*$op).ob_refcnt.ob_refcnt -= 1;
             }
         }
     };
 }
```

### Comparing `orjson-3.9.8/test/test_api.py` & `orjson-3.9.9/test/test_api.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_append_newline.py` & `orjson-3.9.9/test/test_append_newline.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_canonical.py` & `orjson-3.9.9/test/test_canonical.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_circular.py` & `orjson-3.9.9/test/test_circular.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_dataclass.py` & `orjson-3.9.9/test/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_datetime.py` & `orjson-3.9.9/test/test_datetime.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_default.py` & `orjson-3.9.9/test/test_default.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_dict.py` & `orjson-3.9.9/test/test_dict.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_enum.py` & `orjson-3.9.9/test/test_enum.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_error.py` & `orjson-3.9.9/test/test_error.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_fake.py` & `orjson-3.9.9/test/test_fake.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_fixture.py` & `orjson-3.9.9/test/test_fixture.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_fragment.py` & `orjson-3.9.9/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_indent.py` & `orjson-3.9.9/test/test_indent.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_issue331.py` & `orjson-3.9.9/test/test_issue331.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_jsonchecker.py` & `orjson-3.9.9/test/test_jsonchecker.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_memory.py` & `orjson-3.9.9/test/test_memory.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_non_str_keys.py` & `orjson-3.9.9/test/test_non_str_keys.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_numpy.py` & `orjson-3.9.9/test/test_numpy.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_parsing.py` & `orjson-3.9.9/test/test_parsing.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_roundtrip.py` & `orjson-3.9.9/test/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_sort_keys.py` & `orjson-3.9.9/test/test_sort_keys.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_subclass.py` & `orjson-3.9.9/test/test_subclass.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_transform.py` & `orjson-3.9.9/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_type.py` & `orjson-3.9.9/test/test_type.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_ujson.py` & `orjson-3.9.9/test/test_ujson.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/test_uuid.py` & `orjson-3.9.9/test/test_uuid.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/test/util.py` & `orjson-3.9.9/test/util.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/Cargo.lock` & `orjson-3.9.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "orjson"
-version = "3.9.8"
+version = "3.9.9"
 dependencies = [
  "ahash",
  "arrayvec",
  "associative-cache",
  "beef",
  "bytecount",
  "cc",
@@ -206,27 +206,27 @@
 checksum = "134c189feb4956b20f6f547d2cf727d4c0fe06722b20a0eec87ed445a97f92da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "a96fe70b176a89cff78f2fa7b3c930081e163d5379b4dcdf993e3ae29ca662e5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "214929900fd25e6604661ed9cf349727c8920d47deff196c4e28165a6ef2a96b"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `orjson-3.9.8/pyproject.toml` & `orjson-3.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/pysrc/orjson/__init__.py` & `orjson-3.9.9/pysrc/orjson/__init__.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/pysrc/orjson/__init__.pyi` & `orjson-3.9.9/pysrc/orjson/__init__.pyi`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/build.rs` & `orjson-3.9.9/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/ahash-0.8.3/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/Cargo.toml` & `orjson-3.9.9/include/cargo/ahash-0.8.3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/FAQ.md` & `orjson-3.9.9/include/cargo/ahash-0.8.3/FAQ.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/ahash-0.8.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/LICENSE-MIT` & `orjson-3.9.9/include/cargo/ahash-0.8.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/README.md` & `orjson-3.9.9/include/cargo/ahash-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/build.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/aes_hash.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/aes_hash.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/convert.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/convert.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/fallback_hash.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/fallback_hash.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/hash_map.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/hash_map.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/hash_quality_test.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/hash_quality_test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/hash_set.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/hash_set.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/lib.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/operations.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/operations.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/random_state.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/random_state.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/src/specialize.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/src/specialize.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/tests/bench.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/tests/bench.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/tests/map_tests.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/tests/map_tests.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ahash-0.8.3/tests/nopanic.rs` & `orjson-3.9.9/include/cargo/ahash-0.8.3/tests/nopanic.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/CHANGELOG.md` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/Cargo.toml` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/LICENSE-MIT` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/README.md` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/benches/arraystring.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/benches/arraystring.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/benches/extend.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/benches/extend.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/array_string.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/array_string.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/arrayvec.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/arrayvec.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/arrayvec_impl.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/arrayvec_impl.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/char.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/char.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/errors.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/errors.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/src/lib.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/tests/serde.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/tests/serde.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/arrayvec-0.7.4/tests/tests.rs` & `orjson-3.9.9/include/cargo/arrayvec-0.7.4/tests/tests.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/Cargo.toml` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/README.md` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/capacity.rs` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/capacity.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/entry.rs` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/entry.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/indices.rs` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/indices.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/iter.rs` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/iter.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/lib.rs` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/replacement/lru.rs` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/replacement/lru.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/associative-cache-2.0.0/src/replacement.rs` & `orjson-3.9.9/include/cargo/associative-cache-2.0.0/src/replacement.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/Cargo.toml` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/LICENSE-MIT` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/README.md` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/examples/paths.rs` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/examples/paths.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/examples/traits.rs` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/examples/traits.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/src/error.rs` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/src/lib.rs` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/src/tests.rs` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/src/tests.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/src/version.rs` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/src/version.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/autocfg-1.1.0/tests/rustflags.rs` & `orjson-3.9.9/include/cargo/autocfg-1.1.0/tests/rustflags.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/beef-0.5.2/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/Cargo.toml` & `orjson-3.9.9/include/cargo/beef-0.5.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/beef-0.5.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/LICENSE-MIT` & `orjson-3.9.9/include/cargo/beef-0.5.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/README.md` & `orjson-3.9.9/include/cargo/beef-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/benches/bench.rs` & `orjson-3.9.9/include/cargo/beef-0.5.2/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/src/generic.rs` & `orjson-3.9.9/include/cargo/beef-0.5.2/src/generic.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/src/lean.rs` & `orjson-3.9.9/include/cargo/beef-0.5.2/src/lean.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/src/lib.rs` & `orjson-3.9.9/include/cargo/beef-0.5.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/src/serde.rs` & `orjson-3.9.9/include/cargo/beef-0.5.2/src/serde.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/src/traits.rs` & `orjson-3.9.9/include/cargo/beef-0.5.2/src/traits.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/beef-0.5.2/src/wide.rs` & `orjson-3.9.9/include/cargo/beef-0.5.2/src/wide.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/Cargo.toml` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/LICENSE.Apache2` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/LICENSE.Apache2`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/LICENSE.MIT` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/README.md` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/benches/bench.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/src/integer_simd.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/src/integer_simd.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/src/lib.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/src/naive.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/src/naive.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/aarch64.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/aarch64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/generic.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/generic.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/mod.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/x86_avx2.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/x86_avx2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/src/simd/x86_sse2.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/src/simd/x86_sse2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/bytecount-0.6.4/tests/check.rs` & `orjson-3.9.9/include/cargo/bytecount-0.6.4/tests/check.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/castaway-0.2.2/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/castaway-0.2.2/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/castaway-0.2.2/Cargo.toml` & `orjson-3.9.9/include/cargo/castaway-0.2.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/castaway-0.2.2/LICENSE` & `orjson-3.9.9/include/cargo/castaway-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/castaway-0.2.2/README.md` & `orjson-3.9.9/include/cargo/castaway-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/castaway-0.2.2/src/internal.rs` & `orjson-3.9.9/include/cargo/castaway-0.2.2/src/internal.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/castaway-0.2.2/src/lib.rs` & `orjson-3.9.9/include/cargo/castaway-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/castaway-0.2.2/src/lifetime_free.rs` & `orjson-3.9.9/include/cargo/castaway-0.2.2/src/lifetime_free.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/castaway-0.2.2/src/utils.rs` & `orjson-3.9.9/include/cargo/castaway-0.2.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/cc-1.0.83/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/Cargo.lock` & `orjson-3.9.9/include/cargo/cc-1.0.83/Cargo.lock`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/Cargo.toml` & `orjson-3.9.9/include/cargo/cc-1.0.83/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/cc-1.0.83/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/LICENSE-MIT` & `orjson-3.9.9/include/cargo/cc-1.0.83/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/README.md` & `orjson-3.9.9/include/cargo/cc-1.0.83/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/bin/gcc-shim.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/bin/gcc-shim.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/com.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/com.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/lib.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/os_pipe/unix.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/os_pipe/unix.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/os_pipe/windows.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/os_pipe/windows.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/os_pipe.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/os_pipe.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/registry.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/registry.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/setup_config.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/setup_config.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/vs_instances.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/vs_instances.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/winapi.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/winapi.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/windows_registry.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/windows_registry.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/src/windows_sys.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/src/windows_sys.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/tests/cc_env.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/tests/cc_env.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/tests/support/mod.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/tests/support/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cc-1.0.83/tests/test.rs` & `orjson-3.9.9/include/cargo/cc-1.0.83/tests/test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cfg-if-1.0.0/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/cfg-if-1.0.0/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cfg-if-1.0.0/Cargo.toml` & `orjson-3.9.9/include/cargo/cfg-if-1.0.0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cfg-if-1.0.0/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/cfg-if-1.0.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cfg-if-1.0.0/LICENSE-MIT` & `orjson-3.9.9/include/cargo/cfg-if-1.0.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cfg-if-1.0.0/README.md` & `orjson-3.9.9/include/cargo/cfg-if-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/cfg-if-1.0.0/src/lib.rs` & `orjson-3.9.9/include/cargo/cfg-if-1.0.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/chrono-0.4.31/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/CHANGELOG.md` & `orjson-3.9.9/include/cargo/chrono-0.4.31/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/CITATION.cff` & `orjson-3.9.9/include/cargo/chrono-0.4.31/CITATION.cff`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/Cargo.toml` & `orjson-3.9.9/include/cargo/chrono-0.4.31/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/LICENSE.txt` & `orjson-3.9.9/include/cargo/chrono-0.4.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/README.md` & `orjson-3.9.9/include/cargo/chrono-0.4.31/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/date.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/date.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/datetime/mod.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/datetime/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/datetime/rustc_serialize.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/datetime/rustc_serialize.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/datetime/serde.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/datetime/serde.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/datetime/tests.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/datetime/tests.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/duration.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/duration.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/formatting.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/formatting.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/locales.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/locales.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/mod.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/parse.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/parse.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/parsed.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/parsed.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/scan.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/scan.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/format/strftime.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/format/strftime.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/lib.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/month.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/month.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/date.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/date.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/datetime/mod.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/datetime/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/datetime/rustc_serialize.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/datetime/rustc_serialize.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/datetime/serde.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/datetime/serde.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/datetime/tests.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/datetime/tests.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/internals.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/internals.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/isoweek.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/isoweek.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/mod.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/time/mod.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/time/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/time/rustc_serialize.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/time/rustc_serialize.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/time/serde.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/time/serde.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/naive/time/tests.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/naive/time/tests.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/fixed.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/fixed.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/mod.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/tz_info/mod.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/tz_info/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/tz_info/parser.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/tz_info/parser.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/tz_info/rule.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/tz_info/rule.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/tz_info/timezone.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/tz_info/timezone.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/unix.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/unix.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/win_bindings.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/win_bindings.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/local/windows.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/local/windows.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/mod.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/offset/utc.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/offset/utc.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/round.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/round.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/traits.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/traits.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/src/weekday.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/src/weekday.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/tests/dateutils.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/tests/dateutils.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/tests/wasm.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/tests/wasm.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/chrono-0.4.31/tests/win_bindings.rs` & `orjson-3.9.9/include/cargo/chrono-0.4.31/tests/win_bindings.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/Cargo.toml` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/LICENSE` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/README.md` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/arbitrary.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/arbitrary.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/bytes.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/bytes.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/markup.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/markup.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/proptest.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/proptest.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/quickcheck.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/quickcheck.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/rkyv.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/rkyv.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/serde.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/serde.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/features/smallvec.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/features/smallvec.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/lib.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/macros.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/bytes.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/bytes.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/capacity.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/capacity.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/heap.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/heap.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/inline.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/inline.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/iter.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/iter.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/mod.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/nonmax.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/nonmax.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/num.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/num.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/smallvec.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/smallvec.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/repr/traits.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/repr/traits.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/tests.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/tests.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/compact_str-0.7.1/src/traits.rs` & `orjson-3.9.9/include/cargo/compact_str-0.7.1/src/traits.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/CONTRIBUTING.md` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/COPYRIGHT` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/Cargo.toml` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/Ideas.md` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/Ideas.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/LICENSE-MIT` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/LICENSE-WHATWG` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/LICENSE-WHATWG`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/README.md` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/Big5.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/Big5.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/EUC-JP.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/EUC-JP.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/EUC-KR.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/EUC-KR.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/GBK.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/GBK.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-2022-JP.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-2022-JP.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-7.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-7.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-8-I.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-8-I.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-8.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/ISO-8859-8.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/gb18030.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/gb18030.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/doc/windows-1258.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/doc/windows-1258.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/generate-encoding-data.py` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/generate-encoding-data.py`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/ascii.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/ascii.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/big5.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/big5.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/data.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/data.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/euc_jp.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/euc_jp.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/euc_kr.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/euc_kr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/gb18030.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/gb18030.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/handles.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/handles.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/iso_2022_jp.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/iso_2022_jp.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/lib.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/macros.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/mem.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/mem.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/replacement.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/replacement.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/shift_jis.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/shift_jis.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/simd_funcs.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/simd_funcs.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/single_byte.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/single_byte.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/big5_in.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/big5_in.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/big5_in_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/big5_in_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/big5_out.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/big5_out.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/big5_out_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/big5_out_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_in.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_in.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_in_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_in_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_out.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_out.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_out_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/euc_kr_out_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_in.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_in.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_in_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_in_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_out.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_out.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_out_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/gb18030_out_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_in.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_in.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_in_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_in_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_out.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_out.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_out_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/iso_2022_jp_out_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_in.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_in.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_in_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_in_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_out.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_out.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_out_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0208_out_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0212_in.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0212_in.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/jis0212_in_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/jis0212_in_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_in.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_in.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_in_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_in_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_out.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_out.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_out_ref.txt` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_data/shift_jis_out_ref.txt`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/test_labels_names.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/test_labels_names.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/testing.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/testing.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/utf_16.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/utf_16.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/utf_8.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/utf_8.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/variant.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/variant.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/encoding_rs-0.8.33/src/x_user_defined.rs` & `orjson-3.9.9/include/cargo/encoding_rs-0.8.33/src/x_user_defined.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoa-1.0.9/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/itoa-1.0.9/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoa-1.0.9/Cargo.toml` & `orjson-3.9.9/include/cargo/itoa-1.0.9/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoa-1.0.9/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/itoa-1.0.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoa-1.0.9/LICENSE-MIT` & `orjson-3.9.9/include/cargo/itoa-1.0.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoa-1.0.9/README.md` & `orjson-3.9.9/include/cargo/itoa-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoa-1.0.9/benches/bench.rs` & `orjson-3.9.9/include/cargo/itoa-1.0.9/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoa-1.0.9/src/lib.rs` & `orjson-3.9.9/include/cargo/itoa-1.0.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoa-1.0.9/src/udiv128.rs` & `orjson-3.9.9/include/cargo/itoa-1.0.9/src/udiv128.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoa-1.0.9/tests/test.rs` & `orjson-3.9.9/include/cargo/itoa-1.0.9/tests/test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/itoap-1.0.1/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/Cargo.toml` & `orjson-3.9.9/include/cargo/itoap-1.0.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/LICENSE` & `orjson-3.9.9/include/cargo/itoap-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/README.md` & `orjson-3.9.9/include/cargo/itoap-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/bench.png` & `orjson-3.9.9/include/cargo/itoap-1.0.1/bench.png`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/benches/bench.rs` & `orjson-3.9.9/include/cargo/itoap-1.0.1/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/src/common.rs` & `orjson-3.9.9/include/cargo/itoap-1.0.1/src/common.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/src/fallback.rs` & `orjson-3.9.9/include/cargo/itoap-1.0.1/src/fallback.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/src/lib.rs` & `orjson-3.9.9/include/cargo/itoap-1.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/itoap-1.0.1/src/sse2.rs` & `orjson-3.9.9/include/cargo/itoap-1.0.1/src/sse2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/libc-0.2.149/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/CONTRIBUTING.md` & `orjson-3.9.9/include/cargo/libc-0.2.149/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/Cargo.toml` & `orjson-3.9.9/include/cargo/libc-0.2.149/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/libc-0.2.149/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/LICENSE-MIT` & `orjson-3.9.9/include/cargo/libc-0.2.149/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/README.md` & `orjson-3.9.9/include/cargo/libc-0.2.149/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/build.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/fixed_width_ints.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/fixed_width_ints.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/aarch64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/aarch64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/no_align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/no_align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/riscv64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/riscv64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/fuchsia/x86_64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/fuchsia/x86_64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/hermit/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/hermit/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/lib.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/macros.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/psp.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/psp.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/sgx.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/sgx.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/solid/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/solid/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/switch.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/switch.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/teeos/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/teeos/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/aix/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/aix/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/aix/powerpc64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/aix/powerpc64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b32/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b32/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/aarch64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/aarch64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/x86_64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/b64/x86_64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/apple/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/apple/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/dragonfly/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/dragonfly/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/aarch64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/aarch64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/arm.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/arm.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd11/b64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd11/b64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd11/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd11/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/b64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/b64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd12/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/b64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/b64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd13/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/b64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/b64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/x86_64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/freebsd14/x86_64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/powerpc.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/powerpc.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/powerpc64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/powerpc64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/riscv64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/riscv64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86_64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86_64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86_64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/freebsd/x86_64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/freebsdlike/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/aarch64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/aarch64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/arm.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/arm.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/powerpc.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/powerpc.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/x86_64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/netbsd/x86_64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/aarch64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/aarch64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/x86_64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/bsd/netbsdlike/openbsd/x86_64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/haiku/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/haiku/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/haiku/native.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/haiku/native.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/haiku/x86_64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/haiku/x86_64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/hurd/b32.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/hurd/b32.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/hurd/b64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/hurd/b64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/hurd/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/hurd/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/arm.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/arm.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/x86/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b32/x86/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/aarch64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/riscv64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/riscv64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/x86_64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/b64/x86_64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/android/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/android/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/lfs64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/lfs64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/no_align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/emscripten/no_align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/generic/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/mips/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/mips/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/powerpc/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/powerpc/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/sparc/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/arch/sparc/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/arm/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/arm/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/arm/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/arm/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/csky/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/csky/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/m68k/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/m68k/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mips/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mips/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/powerpc.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/powerpc.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/riscv32/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/riscv32/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/riscv32/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/riscv32/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/sparc/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/sparc/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/x86/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b32/x86/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/ilp32.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/ilp32.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/lp64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/lp64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/aarch64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/loongarch64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/loongarch64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/loongarch64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/loongarch64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mips64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mips64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/powerpc64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/powerpc64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/riscv64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/riscv64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/riscv64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/riscv64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/s390x.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/s390x.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/sparc64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/sparc64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/not_x32.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/not_x32.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/x32.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/b64/x86_64/x32.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/gnu/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/arm/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/arm/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/hexagon.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/hexagon.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mips/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mips/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/powerpc.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/powerpc.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/riscv32/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/riscv32/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/x86/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b32/x86/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/aarch64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/mips64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/mips64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/powerpc64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/powerpc64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/riscv64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/riscv64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/riscv64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/riscv64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/s390x.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/s390x.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/x86_64/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/x86_64/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/x86_64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/b64/x86_64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/lfs64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/lfs64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/musl/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/no_align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/no_align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/arm/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/arm/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips32/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips32/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mips64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mips/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/no_align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/no_align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/l4re.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/l4re.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/linux/uclibc/x86_64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/linux_like/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/linux_like/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/aarch64/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/aarch64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/arm/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/arm/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/espidf/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/espidf/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/generic.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/generic.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/horizon/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/horizon/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/no_align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/no_align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/newlib/vita/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/newlib/vita/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/nto/aarch64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/nto/aarch64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/nto/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/nto/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/nto/neutrino.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/nto/neutrino.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/nto/x86_64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/nto/x86_64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/redox/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/redox/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/compat.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/compat.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/illumos.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/illumos.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/solaris.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/solaris.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/x86.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/x86.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/x86_64.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/x86_64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/unix/solarish/x86_common.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/unix/solarish/x86_common.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/vxworks/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/vxworks/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/wasi.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/wasi.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/windows/gnu/align.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/windows/gnu/align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/windows/gnu/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/windows/gnu/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/windows/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/windows/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/windows/msvc/mod.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/windows/msvc/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libc-0.2.149/src/xous.rs` & `orjson-3.9.9/include/cargo/libc-0.2.149/src/xous.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/libm-0.2.8/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/CHANGELOG.md` & `orjson-3.9.9/include/cargo/libm-0.2.8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/CONTRIBUTING.md` & `orjson-3.9.9/include/cargo/libm-0.2.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/Cargo.toml` & `orjson-3.9.9/include/cargo/libm-0.2.8/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/libm-0.2.8/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/LICENSE-MIT` & `orjson-3.9.9/include/cargo/libm-0.2.8/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/README.md` & `orjson-3.9.9/include/cargo/libm-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/build.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/lib.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/libm_helper.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/libm_helper.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/acos.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/acos.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/acosf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/acosf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/acosh.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/acosh.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/acoshf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/acoshf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/asin.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/asin.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/asinf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/asinf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/asinh.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/asinh.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/asinhf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/asinhf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atan.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atan.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atan2.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atan2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atan2f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atan2f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atanf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atanf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atanh.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atanh.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/atanhf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/atanhf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cbrt.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cbrt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cbrtf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cbrtf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ceil.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ceil.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ceilf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ceilf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cos.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cos.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cosf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cosf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/cosh.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/cosh.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/coshf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/coshf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/erf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/erf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/erff.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/erff.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp10.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp10.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp10f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp10f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp2.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/exp2f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/exp2f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/expf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/expf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/expm1.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/expm1.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/expm1f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/expm1f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/expo2.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/expo2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fabs.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fabs.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fabsf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fabsf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/floor.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/floor.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/floorf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/floorf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fma.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fma.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmaf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmaf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmax.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmax.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmaxf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmaxf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmin.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmin.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fminf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fminf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmod.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/fmodf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/fmodf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/hypot.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/hypot.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/hypotf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/hypotf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ilogb.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ilogb.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/ilogbf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/ilogbf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/j0.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/j0.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/j0f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/j0f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/j1.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/j1.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/j1f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/j1f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/jn.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/jn.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/jnf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/jnf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_cos.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_cos.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_cosf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_cosf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_expo2.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_expo2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_expo2f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_expo2f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_sin.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_sin.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_sinf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_sinf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_tan.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_tan.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/k_tanf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/k_tanf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/lgamma_r.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/lgamma_r.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/lgammaf_r.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/lgammaf_r.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log10.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log10.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log10f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log10f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log1p.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log1p.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log1pf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log1pf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log2.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/log2f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/log2f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/logf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/logf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/mod.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/modf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/modf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/modff.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/modff.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/nextafter.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/nextafter.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/nextafterf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/nextafterf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/pow.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/pow.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/powf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/powf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rem_pio2.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rem_pio2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rem_pio2_large.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rem_pio2_large.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rem_pio2f.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rem_pio2f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/remquo.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/remquo.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/remquof.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/remquof.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rint.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rint.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/rintf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/rintf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/round.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/round.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/roundf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/roundf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/scalbn.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/scalbn.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/scalbnf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/scalbnf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sin.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sin.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sincos.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sincos.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sincosf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sincosf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sinf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sinf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sinh.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sinh.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sinhf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sinhf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sqrt.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sqrt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/sqrtf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/sqrtf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tan.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tan.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tanf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tanf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tanh.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tanh.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tanhf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tanhf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/tgamma.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/tgamma.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/trunc.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/trunc.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/libm-0.2.8/src/math/truncf.rs` & `orjson-3.9.9/include/cargo/libm-0.2.8/src/math/truncf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/no-panic-0.1.26/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/no-panic-0.1.26/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/no-panic-0.1.26/Cargo.toml` & `orjson-3.9.9/include/cargo/no-panic-0.1.26/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/no-panic-0.1.26/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/no-panic-0.1.26/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/no-panic-0.1.26/LICENSE-MIT` & `orjson-3.9.9/include/cargo/no-panic-0.1.26/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/no-panic-0.1.26/README.md` & `orjson-3.9.9/include/cargo/no-panic-0.1.26/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/no-panic-0.1.26/src/lib.rs` & `orjson-3.9.9/include/cargo/no-panic-0.1.26/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/no-panic-0.1.26/tests/compiletest/mod.rs` & `orjson-3.9.9/include/cargo/no-panic-0.1.26/tests/compiletest/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/no-panic-0.1.26/tests/test.rs` & `orjson-3.9.9/include/cargo/no-panic-0.1.26/tests/test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/Cargo.toml` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/LICENSE-MIT` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/README.md` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/RELEASES.md` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/RELEASES.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/build.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/bounds.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/bounds.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/cast.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/cast.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/float.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/float.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/identities.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/identities.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/int.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/int.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/lib.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/macros.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/bytes.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/bytes.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/checked.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/checked.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/euclid.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/euclid.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/inv.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/inv.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/mul_add.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/mul_add.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/overflowing.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/overflowing.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/saturating.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/saturating.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/ops/wrapping.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/ops/wrapping.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/pow.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/pow.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/real.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/real.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/src/sign.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/src/sign.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/num-traits-0.2.17/tests/cast.rs` & `orjson-3.9.9/include/cargo/num-traits-0.2.17/tests/cast.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/CHANGELOG.md` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/Cargo.lock` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/Cargo.lock`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/Cargo.toml` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/LICENSE-MIT` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/README.md` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/bench.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/bench.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/bench_acquire.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/bench_acquire.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/lazy_static.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/lazy_static.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/regex.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/regex.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/examples/test_synchronization.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/examples/test_synchronization.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/src/imp_cs.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/src/imp_cs.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/src/imp_pl.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/src/imp_pl.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/src/imp_std.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/src/imp_std.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/src/lib.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/src/race.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/src/race.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/race.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/race.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/race_once_box.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/race_once_box.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/sync_lazy.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/sync_lazy.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/sync_once_cell.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/sync_once_cell.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/unsync_lazy.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/unsync_lazy.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/once_cell-1.18.0/tests/it/unsync_once_cell.rs` & `orjson-3.9.9/include/cargo/once_cell-1.18.0/tests/it/unsync_once_cell.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/Cargo.toml` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/LICENSE-MIT` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/README.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/all.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/all.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/android-install-ndk.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/android-install-ndk.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/android-install-sdk.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/android-install-sdk.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/android-sysimage.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/android-sysimage.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/benchmark.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/benchmark.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/deploy_and_run_on_ios_simulator.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/deploy_and_run_on_ios_simulator.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/aarch64-linux-android/Dockerfile` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/aarch64-linux-android/Dockerfile`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/armv7-linux-androideabi/Dockerfile` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/armv7-linux-androideabi/Dockerfile`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/mipsel-unknown-linux-musl/Dockerfile` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/mipsel-unknown-linux-musl/Dockerfile`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/s390x-unknown-linux-gnu/Dockerfile` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/s390x-unknown-linux-gnu/Dockerfile`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/sparc64-unknown-linux-gnu/Dockerfile` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/sparc64-unknown-linux-gnu/Dockerfile`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/thumbv7neon-linux-androideabi/Dockerfile` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/thumbv7neon-linux-androideabi/Dockerfile`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/wasm32-unknown-unknown/Dockerfile` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/wasm32-unknown-unknown/Dockerfile`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/docker/x86_64-linux-android/Dockerfile` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/docker/x86_64-linux-android/Dockerfile`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/dox.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/dox.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/linux-s390x.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/linux-s390x.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/run-docker.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/run-docker.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/run.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/run.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/run_examples.sh` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/run_examples.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/ci/runtest-android.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/ci/runtest-android.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/contributing.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/contributing.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/SUMMARY.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/bound_checks.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/bound_checks.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/introduction.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/introduction.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/linux.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/linux.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/mca.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/mca.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/profiling.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/prof/profiling.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/features.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/features.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/practice.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/practice.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/rustflags.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/target-feature/rustflags.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/perf-guide/src/vert-hor-ops.md` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/perf-guide/src/vert-hor-ops.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/bit_manip.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/bit_manip.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/bitmask.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/bitmask.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/macros.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v128.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v128.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v16.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v16.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v256.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v256.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v32.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v32.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v512.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v512.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast/v64.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast/v64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cast.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cast.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/eq.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/eq.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/ord.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/ord.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/partial_eq.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/partial_eq.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/partial_ord.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/partial_ord.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/cmp/vertical.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/cmp/vertical.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/default.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/default.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/binary.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/binary.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/debug.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/debug.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/lower_hex.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/lower_hex.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/octal.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/octal.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/fmt/upper_hex.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/fmt/upper_hex.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/from/from_array.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/from/from_array.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/from/from_vector.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/from/from_vector.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/hash.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/hash.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/arch_specific.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/arch_specific.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/macros.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v128.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v128.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v256.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v256.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v32.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v32.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v512.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v512.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits/v64.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits/v64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/into_bits.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/into_bits.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/abs.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/abs.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/consts.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/consts.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/cos.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/cos.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/exp.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/exp.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/ln.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/ln.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/mul_add.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/mul_add.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/mul_adde.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/mul_adde.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/powf.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/powf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/recpre.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/recpre.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/rsqrte.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/rsqrte.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/sin.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/sin.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/sqrt.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/sqrt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/sqrte.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/sqrte.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float/tanh.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float/tanh.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/math/float.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/math/float.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/minimal/iuf.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/minimal/iuf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/minimal/mask.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/minimal/mask.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/minimal/ptr.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/minimal/ptr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_arithmetic.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_bitwise.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_bitwise.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_mask_bitwise.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_mask_bitwise.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_shifts.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/scalar_shifts.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_arithmetic.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_bitwise.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_bitwise.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_float_min_max.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_float_min_max.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_int_min_max.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_int_min_max.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_mask_bitwise.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_mask_bitwise.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_neg.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_neg.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_rotates.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_rotates.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ops/vector_shifts.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ops/vector_shifts.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/ptr/gather_scatter.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/ptr/gather_scatter.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/bitwise.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/bitwise.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/float_arithmetic.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/float_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/integer_arithmetic.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/integer_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/mask.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/mask.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/reductions/min_max.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/reductions/min_max.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/select.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/select.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/shuffle.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/shuffle.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/shuffle1_dyn.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/shuffle1_dyn.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/slice/from_slice.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/slice/from_slice.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/slice/write_to_slice.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/slice/write_to_slice.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api/swap_bytes.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api/swap_bytes.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/api.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/api.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/bit_manip.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/bit_manip.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/llvm.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/llvm.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/abs.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/abs.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/cos.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/cos.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/cos_pi.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/cos_pi.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/exp.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/exp.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/ln.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/ln.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/macros.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/mul_add.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/mul_add.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/mul_adde.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/mul_adde.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/powf.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/powf.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin_cos_pi.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin_cos_pi.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin_pi.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sin_pi.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sqrt.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sqrt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sqrte.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/sqrte.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/math/float/tanh.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/math/float/tanh.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/pointer_sized_int.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/pointer_sized_int.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/aarch64.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/aarch64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/arm.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/arm.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/fallback_impl.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/fallback_impl.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/avx.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/avx.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/avx2.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/avx2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/sse.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/sse.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/sse2.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86/sse2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask/x86.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/reductions/mask.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/shuffle.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/shuffle.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/shuffle1_dyn.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/shuffle1_dyn.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/swap_bytes.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/swap_bytes.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v128.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v128.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v256.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v256.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v512.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v512.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/v64.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/v64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/vPtr.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/vPtr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen/vSize.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen/vSize.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/codegen.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/codegen.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/lib.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/masks.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/masks.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/sealed.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/sealed.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/testing/macros.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/testing/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/testing/utils.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/testing/utils.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v128.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v128.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v256.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v256.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v32.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v32.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v512.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v512.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/v64.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/v64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/vPtr.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/vPtr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/src/vSize.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/src/vSize.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/packed_simd-0.3.9/tests/endianness.rs` & `orjson-3.9.9/include/cargo/packed_simd-0.3.9/tests/endianness.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/Cargo.toml` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/LICENSE-MIT` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/README.md` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/build.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/detection.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/detection.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/extra.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/extra.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/fallback.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/fallback.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/lib.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/location.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/location.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/parse.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/parse.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/rcvec.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/rcvec.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/src/wrapper.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/src/wrapper.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/comments.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/comments.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/marker.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/marker.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/test.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/test_fmt.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/test_fmt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/proc-macro2-1.0.69/tests/test_size.rs` & `orjson-3.9.9/include/cargo/proc-macro2-1.0.69/tests/test_size.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/Cargo.toml` & `orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 # to registry (e.g., crates.io) dependencies.
 #
 # If you are reading this file be aware that the original Cargo.toml
 # will likely look very different (and much more reasonable).
 # See Cargo.toml.orig for the original contents.
 
 [package]
-edition = "2018"
+edition = "2021"
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.20.0"
 authors = ["PyO3 Project and Contributors <https://github.com/PyO3>"]
 description = "Build configuration for the PyO3 ecosystem"
 homepage = "https://github.com/pyo3/pyo3"
 keywords = [
     "pyo3",
     "python",
     "cpython",
     "ffi",
 ]
 categories = [
     "api-bindings",
     "development-tools::ffi",
 ]
-license = "Apache-2.0"
+license = "MIT OR Apache-2.0"
 repository = "https://github.com/pyo3/pyo3"
 
 [package.metadata.docs.rs]
 features = ["resolve-config"]
 
 [dependencies.once_cell]
 version = "1"
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/LICENSE` & `orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/build.rs` & `orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/src/errors.rs` & `orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/src/errors.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/src/impl_.rs` & `orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/src/impl_.rs`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             implementation,
             shared,
             abi3,
             lib_name: Some(lib_name),
             lib_dir,
             executable: map.get("executable").cloned(),
             pointer_width: Some(calcsize_pointer * 8),
-            build_flags: BuildFlags::from_interpreter(interpreter)?.fixup(version),
+            build_flags: BuildFlags::from_interpreter(interpreter)?,
             suppress_build_script_link_lines: false,
             extra_build_script_lines: vec![],
         })
     }
 
     /// Generate from parsed sysconfigdata file
     ///
@@ -345,15 +345,15 @@
             version,
             implementation,
             sysconfigdata.get_value("LDVERSION"),
         ));
         let pointer_width = parse_key!(sysconfigdata, "SIZEOF_VOID_P")
             .map(|bytes_width: u32| bytes_width * 8)
             .ok();
-        let build_flags = BuildFlags::from_sysconfigdata(sysconfigdata).fixup(version);
+        let build_flags = BuildFlags::from_sysconfigdata(sysconfigdata);
 
         Ok(InterpreterConfig {
             implementation,
             version,
             shared: shared || framework,
             abi3: is_abi3(),
             lib_dir,
@@ -1015,14 +1015,15 @@
                 .filter(|flag| {
                     config_map
                         .get_value(&flag.to_string())
                         .map_or(false, |value| value == "1")
                 })
                 .collect(),
         )
+        .fixup()
     }
 
     /// Examine python's compile flags to pass to cfg by launching
     /// the interpreter and printing variables of interest from
     /// sysconfig.get_config_vars.
     fn from_interpreter(interpreter: impl AsRef<Path>) -> Result<Self> {
         // sysconfig is missing all the flags on windows, so we can't actually
@@ -1049,24 +1050,20 @@
         let flags = BuildFlags::ALL
             .iter()
             .zip(split_stdout)
             .filter(|(_, flag_value)| *flag_value == "1")
             .map(|(flag, _)| flag.clone())
             .collect();
 
-        Ok(Self(flags))
+        Ok(Self(flags).fixup())
     }
 
-    fn fixup(mut self, version: PythonVersion) -> Self {
+    fn fixup(mut self) -> Self {
         if self.0.contains(&BuildFlag::Py_DEBUG) {
             self.0.insert(BuildFlag::Py_REF_DEBUG);
-            if version <= PythonVersion::PY37 {
-                // Py_DEBUG only implies Py_TRACE_REFS until Python 3.7
-                self.0.insert(BuildFlag::Py_TRACE_REFS);
-            }
         }
 
         self
     }
 }
 
 impl Display for BuildFlags {
@@ -1128,15 +1125,15 @@
 }
 
 /// Parse sysconfigdata file
 ///
 /// The sysconfigdata is simply a dictionary containing all the build time variables used for the
 /// python executable and library. This function necessitates a python interpreter on the host
 /// machine to work. Here it is read into a `Sysconfigdata` (hash map), which can be turned into an
-/// [`InterpreterConfig`](InterpreterConfig) using
+/// [`InterpreterConfig`] using
 /// [`from_sysconfigdata`](InterpreterConfig::from_sysconfigdata).
 pub fn parse_sysconfigdata(sysconfigdata_path: impl AsRef<Path>) -> Result<Sysconfigdata> {
     let sysconfigdata_path = sysconfigdata_path.as_ref();
     let mut script = fs::read_to_string(sysconfigdata_path).with_context(|| {
         format!(
             "failed to read config from {}",
             sysconfigdata_path.display()
@@ -1931,33 +1928,25 @@
         assert_eq!(
             BuildFlags::from_sysconfigdata(&sysconfigdata).0,
             expected_flags
         );
     }
 
     #[test]
-    fn build_flags_fixup_py37_debug() {
+    fn build_flags_fixup() {
         let mut build_flags = BuildFlags::new();
-        build_flags.0.insert(BuildFlag::Py_DEBUG);
 
-        build_flags = build_flags.fixup(PythonVersion { major: 3, minor: 7 });
+        build_flags = build_flags.fixup();
+        assert!(build_flags.0.is_empty());
 
-        // On 3.7, Py_DEBUG implies Py_REF_DEBUG and Py_TRACE_REFS
-        assert!(build_flags.0.contains(&BuildFlag::Py_REF_DEBUG));
-        assert!(build_flags.0.contains(&BuildFlag::Py_TRACE_REFS));
-    }
-
-    #[test]
-    fn build_flags_fixup_py38_debug() {
-        let mut build_flags = BuildFlags::new();
         build_flags.0.insert(BuildFlag::Py_DEBUG);
 
-        build_flags = build_flags.fixup(PythonVersion { major: 3, minor: 8 });
+        build_flags = build_flags.fixup();
 
-        // On 3.8, Py_DEBUG implies Py_REF_DEBUG
+        // Py_DEBUG implies Py_REF_DEBUG
         assert!(build_flags.0.contains(&BuildFlag::Py_REF_DEBUG));
     }
 
     #[test]
     fn parse_script_output() {
         let output = "foo bar\nbar foobar\n\n";
         let map = super::parse_script_output(output);
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/src/import_lib.rs` & `orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/src/import_lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-build-config-0.19.2/src/lib.rs` & `orjson-3.9.9/include/cargo/pyo3-build-config-0.20.0/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -138,37 +138,22 @@
             return None;
         }
         pieces.next()?.parse().ok()
     }
 
     let rustc_minor_version = rustc_minor_version().unwrap_or(0);
 
-    // Enable use of const generics on Rust 1.51 and greater
-    if rustc_minor_version >= 51 {
-        println!("cargo:rustc-cfg=min_const_generics");
-    }
-
-    // Enable use of std::ptr::addr_of! on Rust 1.51 and greater
-    if rustc_minor_version >= 51 {
-        println!("cargo:rustc-cfg=addr_of");
-    }
-
-    // Enable use of Option::insert on Rust 1.53 and greater
-    if rustc_minor_version >= 53 {
-        println!("cargo:rustc-cfg=option_insert");
-    }
-
     // Enable use of const initializer for thread_local! on Rust 1.59 and greater
     if rustc_minor_version >= 59 {
         println!("cargo:rustc-cfg=thread_local_const_init");
     }
 
-    // Enable use of `#[cfg(panic = "...")]` on Rust 1.60 and greater
-    if rustc_minor_version >= 60 {
-        println!("cargo:rustc-cfg=panic_unwind");
+    // invalid_from_utf8 lint was added in Rust 1.74
+    if rustc_minor_version >= 74 {
+        println!("cargo:rustc-cfg=invalid_from_utf8_lint");
     }
 }
 
 /// Private exports used in PyO3's build.rs
 ///
 /// Please don't use these - they could change at any time.
 #[doc(hidden)]
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/.cargo-checksum.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6744505494505495%*

 * *Differences: {"'files'": "{'Cargo.toml': '887651795562158db6ccfb2868f081028de97ae79a525d31de39f75f43a6b2c7', "*

 * *            "'README.md': '055b259a47487be2976d504753d4b8b19a32527ac5ae44bf61c619a11ce4fb1e', "*

 * *            "'build.rs': '0848bebb8ce4feac8e012c4843cf37c248b71e7652091fe4873fa7bd354d24ca', "*

 * *            "'src/boolobject.rs': "*

 * *            "'fa5de2264fde326d121502bc155f5c7034afaec8547ceefdd33ba4b9226c7a35', "*

 * *            "'src/bytearrayobject.rs': "*

 * *            "'7e62a32a435838c18690296b71aec69e5ccacde2754574a8e […]*

```diff
@@ -1,91 +1,95 @@
 {
     "files": {
-        "Cargo.toml": "aa1dd019c1a2ae50af6fab262838fb9b949a0bca13355c8672972e2986b628e0",
-        "LICENSE": "8e206a2c586acb73f513a3782923354d5798bd4712ebad666e946499bcfdea9e",
-        "README.md": "c038d5f4562e89c8cfa9b7aad7ceea4d3abd485d8a3f47ee347fedade3083b87",
-        "build.rs": "5a98a98eef4e5738c3ce0a9299a51bdb2dacbd675d72b78f8988bc91fd988153",
+        "ACKNOWLEDGEMENTS": "a895ab531efd09aae5db905f6a62033d81469c233d42a5c200e1b1965a145020",
+        "Cargo.toml": "887651795562158db6ccfb2868f081028de97ae79a525d31de39f75f43a6b2c7",
+        "LICENSE-APACHE": "71073d492e996de196dbe1eb1e4c94c27c014c841b288161265b2efd06d0af28",
+        "LICENSE-MIT": "afcbe3b2e6b37172b5a9ca869ee4c0b8cdc09316e5d4384864154482c33e5af6",
+        "README.md": "055b259a47487be2976d504753d4b8b19a32527ac5ae44bf61c619a11ce4fb1e",
+        "build.rs": "0848bebb8ce4feac8e012c4843cf37c248b71e7652091fe4873fa7bd354d24ca",
         "src/abstract_.rs": "37bfcc40d1cf828e7474d7aa7d5ca221c18e6dda7aed6b58cf46a58c4ec52be0",
         "src/bltinmodule.rs": "05f18e034fffafba89d8255a7502b05d6debec5ef79f37c9657fd605f2a6a39b",
-        "src/boolobject.rs": "9b79341691402406bdef4a7e320fb1204f38352cc116c45baf217f7b7c5d9fce",
-        "src/bytearrayobject.rs": "ce12c676ec90be26bf0529db1101764c9897c2db57c491b6758cc8120b50ca07",
-        "src/bytesobject.rs": "1b311c0e3cd850bdeec8044c2aac55d44f4c01a2cf33bcb4b20c913e3f6a71bc",
+        "src/boolobject.rs": "fa5de2264fde326d121502bc155f5c7034afaec8547ceefdd33ba4b9226c7a35",
+        "src/bytearrayobject.rs": "7e62a32a435838c18690296b71aec69e5ccacde2754574a8ef9b3f33bc0f9c21",
+        "src/bytesobject.rs": "88a9d10e750d7d7917a6dd0d1259a1f86f3ca6a593a8b37c92356569bc2c5071",
         "src/ceval.rs": "a2abc504100b91898e3c924af39348cfbd01125c13fc1389f3781d7bd6c78f6c",
         "src/code.rs": "be9b7b82edaadbb478365c38bcc9323a4c6dc7eb37bc0992c0ff39e18f2af61d",
         "src/codecs.rs": "0c86ae7c1d3d67be9a2ac3c80f6ccdd77aa0c72c46b8dc37eda23eb7619ab0b2",
         "src/compile.rs": "9a7bdc36c8a7c9d0ae14c6db8d9c712d947458b424c8d1348f207c62c9c97b3b",
-        "src/complexobject.rs": "74f20d9a7a971b362395587bbfefa5f372a5a40d2e2541db0e53607a6bca8b38",
-        "src/context.rs": "d31db0dad618b23219ac05a88dabcfe51013384e60d716716ee860494f75fdc5",
+        "src/complexobject.rs": "6120ce16b49afa9dfec99fdbda52fc6957bb66a35c0491129e9825db1a37f80e",
+        "src/context.rs": "12cac9b5b794d869492a7714227ef0375d41c4a13f22193523ac2b539f52b004",
         "src/cpython/abstract_.rs": "5eed09592ee72a4790ec6d36ebf99bb8702e2ea6b091c4aff3bf915e62ff5c40",
         "src/cpython/bytesobject.rs": "ee072b05f47a41b54f825e78693491db3ac0180c11db6522cee71d99a269b917",
-        "src/cpython/ceval.rs": "b9759c9dbccac534fb7e622ebdf54a1f0b686a5dad243b7c61e07052fd065836",
-        "src/cpython/code.rs": "eb97cb0641daaa813614dca85bed08883234616b4cef4a913537db35bb1870f5",
+        "src/cpython/ceval.rs": "3cf69dc673e8cfcb0d40307dc7955526ed3002074d65cb277c282eaabd766160",
+        "src/cpython/code.rs": "74034a0cd3dff9e8266dcc778961a78a8d64f4871d655fd1c4efbaf8fff3df44",
         "src/cpython/compile.rs": "b604854c2a75e7ec5c29c7900266f8a572cba51584224160fcc5a9cc08bdb5a3",
         "src/cpython/descrobject.rs": "ff8341bcf19600cbaddcc02164ff0e789b0c1ec3502537076c4bc57bb5c14570",
         "src/cpython/dictobject.rs": "6c224875f3ae769f7a1a07cfccce36874a78c09adcad628ca66029be327e31e0",
         "src/cpython/floatobject.rs": "0855a592bfff14ca8efdfee7bb777dba75b7096c4ebd734d18f999d831de9d4e",
-        "src/cpython/frameobject.rs": "e06b4e2ce6440df5776b09aed62fd4222e178ae87aed106541b41b01d19a4d17",
-        "src/cpython/funcobject.rs": "eb9a5d48507199e3470d4e56e600f82b20c0f0919c3d49f9fb7f2df49a36de2d",
-        "src/cpython/genobject.rs": "62445231997fa0010a4f2387f718aa4633be0ebe062c55e342176c154a76c6dd",
+        "src/cpython/frameobject.rs": "66401317162699fd9b009ddfa773cd539da262f8f85df3c61287a053287f38c9",
+        "src/cpython/funcobject.rs": "60d658bec418c11400dc6cda95d07f9a5ca5e90f47cbab6e84fbc5b9b618d63f",
+        "src/cpython/genobject.rs": "8d35c4a1bae3060c587bc1aa47a662ae4c994b4a513b0f691f6029b8c40c70ca",
         "src/cpython/import.rs": "bf4a85fb6f9ac58e689a9d5536109bf93b17209c7949e27c6c108565a90ef14b",
         "src/cpython/initconfig.rs": "f289bc41b57eb9929db525cb8645d56f4d418a481dce5b351641ab6314dc6438",
         "src/cpython/listobject.rs": "6808198262f8824cb80aee6edf97c1b8fa76b66e1c879421f08ba2e1142677a8",
-        "src/cpython/methodobject.rs": "91514c017304dc74efd8bae5346571bdbeac9cc48d57e046e3c6186ffa1b49cf",
-        "src/cpython/mod.rs": "51071fd7e315a1503bd69a94e1d3be01d60e26cc45a5657b0ad50b42a56314aa",
-        "src/cpython/object.rs": "e24596c175b27b99300307f6a821154ab81e8c9698cf575b1a43ab30f8e5df57",
-        "src/cpython/pydebug.rs": "ffef916032730599e36403501c3c194218a0fcd681de008dc21ed7749da5d973",
+        "src/cpython/methodobject.rs": "66a232e8ce13903f726c1a9624408ff7b23c03a44f17442e8d81785343b5796f",
+        "src/cpython/mod.rs": "a7f47c2e5cc01c4e3297fbc203a8532a323a99834bc7909b57092cba20e2335e",
+        "src/cpython/object.rs": "b68bb46e164d8d0b393ad29def32da0e043466678f16399ee8341a9e3c2fd6ab",
+        "src/cpython/objimpl.rs": "2f2d030e9e6cc39579c6565a006ab3758865e6fc1c6113e9c383a34ef1f071be",
+        "src/cpython/pydebug.rs": "041988d8ee709ce499b729942b2f815be97d9b1f26e060db93813aa93d850c1f",
         "src/cpython/pyerrors.rs": "84e3329f2ee9b1f3dd41a131c51dda828bb5ebc24d465a2d5c24039422f959e5",
-        "src/cpython/pylifecycle.rs": "810fd56a53a62ce0efff1a929165d25072130d130da2f1f7fbf4576fab251c4d",
+        "src/cpython/pyframe.rs": "d99e567a14a3fbf6dfecf9342c4fa5839f55ac0f64cc22fe28dac8b27751a187",
+        "src/cpython/pylifecycle.rs": "c6440b0085c69d41dcdbf9622fcb8da7d16e8252bf511e1c61c0a945ce362d66",
         "src/cpython/pymem.rs": "74b692ff8cb6cbc1e855d4fd8ef71c73202c93cba5307ad803c923d11ebf668c",
-        "src/cpython/pystate.rs": "76356f5684d0e7409b7bbae9e958828e36ada67601c0ca77586fb236239976d2",
+        "src/cpython/pystate.rs": "371d81e613fe9a083413eaeb49c2a50523663f6fdf7b6e1aee266414e6efdaf6",
         "src/cpython/pythonrun.rs": "56f8edd7af5feacdc382994bb6b3b7b8686f5c716c2d619f870f7627abf49308",
         "src/cpython/tupleobject.rs": "7c6c7eddbcc0ef0c5b73c0b554ec6e363dfdbd00f7850f6fb435463525dd2a98",
-        "src/cpython/unicodeobject.rs": "2f01c301d4398630908452ad27954dd64e1ce4a7da965542b62438f6266c0737",
+        "src/cpython/unicodeobject.rs": "81de5ef91635b33b5c541a51f019dec6be3e28f940c9bf839d81fed14d3ed008",
         "src/cpython/weakrefobject.rs": "16e6d97a3bde80cbd9605652c9594136d35d8b8527468824f7062e0bfed01d28",
         "src/datetime.rs": "85ef113a4c8c32c199bd13aec78113cdf26359719f728e025366ed91e85ad1d4",
-        "src/descrobject.rs": "d2fef3e6391013ac44869f69f35cbd860c5cb202888a3583a05677964e743b30",
-        "src/dictobject.rs": "a32b5cccf0be9844ccfb0ec41c5487140cfe5ba6cc29cd6358130ba3d18acbe9",
+        "src/descrobject.rs": "3abc7bd7fa71a61352a438b100fff2643a24fd79409403833dd6708b7602dac9",
+        "src/dictobject.rs": "54f89a490c11141224f5b7d2d97b4da6bd52c64cf11f5c90793dd97daf3f240b",
         "src/enumobject.rs": "1c0f2ab3f7ab48d92147a3bebc0c0f1251adfed6904d53a9b2bf64f32560aeda",
-        "src/fileobject.rs": "b0b5f431e7f2a28fe70f28b1d3d0cc4890b0ed7a4bcc9c2b88b3390fa2ff4396",
+        "src/fileobject.rs": "494421b1779b93e8f27d052c53c857e83b5bb2c7a47870ff00ecbcd320042afe",
         "src/fileutils.rs": "ebec882c3f1ab47686da7bd05dec5f87f653fd115c26c3a1e475aadbf8dd729d",
-        "src/floatobject.rs": "76758f849ba7c90b2a64f41a657657e40b3ce947806b0596c6dad01493e6afd6",
+        "src/floatobject.rs": "cedc182ffeb692386c0f2e588431e18652945739adb3c412401521e3f12a5fcb",
         "src/import.rs": "94b49da77ae6f997d0efcbb6892e3b76973891e03a16f0c7c4a31c3a8ab747f5",
         "src/intrcheck.rs": "0b4e6ca30e123caf1892ab58cf53245f94b456d00333b93058965c08721a3523",
-        "src/iterobject.rs": "98fbb9680592c5c69da8001bb5c2d001d1b74c1a9c9a851f73bf38552f3c5c0b",
-        "src/lib.rs": "eb8ca1bdae1ce38954237ac9bdc117780019e26784a02761b1324aeba95d5752",
-        "src/listobject.rs": "e7b1ea5631df52ec45e40f8c549fdcc2e71909e21d9cf154f6b331b918fe6718",
-        "src/longobject.rs": "d3ee5edf42524f6756a4982b05b085aa170a58540464204a4e40d25acb1f9d94",
+        "src/iterobject.rs": "df4f345519a755ee43acde00c79480bebb34e9f21772f753820e652f4395741f",
+        "src/lib.rs": "8ebbbdadc5307f528f2b1e92cf27622f159728fa1276d6c7aa26806ced38bf02",
+        "src/listobject.rs": "f9cad784876ef33c0f7f8b1bbe93ed69691d56c4a9549be74e7433dd3ba23b3b",
+        "src/longobject.rs": "373ed2c1d80026710caecd70bbfd8f0f1e418e1efc565e1c880eb9c1699b9feb",
         "src/marshal.rs": "d1a51042497871a33adcd16f4c35e373405f5143be2c9666d4e726dbd3636aa6",
-        "src/memoryobject.rs": "be1ccf13e03ab079b113156c38219d2329d01fd785183b31e460e95d7447b105",
-        "src/methodobject.rs": "65168e371a0abdabb1ecbf0b772e5ce86e24f4b8e3a751a6fccb1a716a0459e8",
+        "src/memoryobject.rs": "941e8123288bea557fd59bdf10bcf90dcea2473fdc088463b06e16429c38b1ce",
+        "src/methodobject.rs": "239bba483d978ec28bf4a8af0ea229ebea13cc6a6146f8210a4029758852424b",
         "src/modsupport.rs": "f8c5d909d77660d0891f345b33caf9329b728f7224e7eaca7116aabbeb8ec83b",
-        "src/moduleobject.rs": "fc15a5fc90693037bd3f8f69c16c58c82958cd7ae9961da2f55e94694dfd3ca2",
-        "src/object.rs": "0add95de47e8d684a6e2cfd4c3dbdf022dea1feaf9e61a655b763569330acbf4",
-        "src/objimpl.rs": "39a42249650afcde4e1525cdd7807e2805f80f2fabfffd504ea47bf85fd753e9",
-        "src/osmodule.rs": "1b93ae4d5e4456da2f54938d79d3cd7d400b4f58bf7d4944ca75cad0bc221fc4",
+        "src/moduleobject.rs": "4ecc0512f36e29bbdfc4c86a4bb93ce471cd15ec4ab4494da64e8181b5fd89a8",
+        "src/object.rs": "9be1b276010f6fe34f7b8cb6c867748452eb78eeb97796058b7c79f70220b008",
+        "src/objimpl.rs": "534a7c422cfd386aa39826d6d4070c9f3f3b9a5bedeb9413a307ede89e97b267",
+        "src/osmodule.rs": "522f0e9265167d67675d01c14f657a31a95795e3dec423dee8af7f830f6946ac",
         "src/pyarena.rs": "53b929cf467bdb3fe7dc5fc22720dddeb6d43836d5e741f291d231c38462c4ab",
         "src/pybuffer.rs": "f18d9251c02a9e19522f606788effb9036b2642615225833591faa480cc3c229",
-        "src/pycapsule.rs": "1a366b3b377a4c02f8dd206cf4a9161b83a5aedbaaeba6e8d761859a8029bd0d",
+        "src/pycapsule.rs": "47191e027a978ecb2e03efdb9e2853bef68e305ee519b12ed2241801bc48c2db",
         "src/pyerrors.rs": "9bf052b4ba5b0d30a9397c23251091f9c27b99bba2c12e73f12a1293d5c6e029",
         "src/pyframe.rs": "54705aeb1eeb82c22749f80791785266a092cb91996bc2c1a1ba4d1bf6dca7f1",
         "src/pyhash.rs": "36321736b14510382dda796431a33deb54296317bf5bfb2288651665fbe6496e",
         "src/pylifecycle.rs": "a6c40c102d61095adbc7237c1b1cfcad5dc85d8af0cf089505a718b6cf0f00c3",
         "src/pymem.rs": "ae18180aded033401a5354bbb4ab313f07af2ac29b7e8f1216964308124a12f1",
         "src/pyport.rs": "5e5ebd10606ca299cc6f4085dd165006b11355b98d3d0a10fddbf974d27c7ca2",
         "src/pystate.rs": "0f37aea4ed472ad38b25f794cdbac0cfbb973597f837f0a10b6164c08fe2aa9b",
         "src/pystrtod.rs": "b29ccd17fc7d82642b5d167fb77d1071acab57c4fa6e56a5309c265aeb483aa3",
         "src/pythonrun.rs": "e8ef3a7d0c8d88d7b4a51c6916b311d3be83f153824d174e38f36da7dd7ffc7a",
-        "src/rangeobject.rs": "2f3fc54c0de9cc1c6c9d923ec6dcf4ed608ef8cf6204c5ff02ad7fad537021d9",
-        "src/setobject.rs": "f45ce23feac62d111131315575c99683f72ea6b31dcc13e3b40211918894332f",
-        "src/sliceobject.rs": "2e0f5ba0d02f159c9d0bf15cd9915ad68365392102d6b088e70f708be844f686",
-        "src/structmember.rs": "fc19aebb745d000d2cc5b09163b17661ff7b47239e5231e6f084ab0516250884",
+        "src/rangeobject.rs": "80761feb600397deb2a940cf94ede3693c47c4920be0a95cf5dbe3f123a6b1c1",
+        "src/setobject.rs": "ffb9e1e594420db06e7dbf42f40f8acd100a97d5af87cf0508a90f501ac81fc2",
+        "src/sliceobject.rs": "aa04238e6494857cf270c4fe946e0dcdb7f8d67ad3d6808569c66e906c9cd929",
+        "src/structmember.rs": "264e411d84160f91f992d8bf08f2c2c54b259a802dc77ded5267d32cc3115b7a",
         "src/structseq.rs": "f4ac63c6aff966da1eee44f2f221328d00351f091e9fd5976dccc00de8ac4809",
         "src/sysmodule.rs": "22b2e98c23f0a6e15fcd2c068c4cae39a5e20f2cad5be25925aea8309d1dd8fd",
-        "src/traceback.rs": "7217666791e559328734b2a7259c013a0bbce42fb1ef7f52596636fddc501153",
-        "src/tupleobject.rs": "c660e8efd1cbb78881b5db75887eabc85fb1708ac5ae3a6f136a52bced8fc6af",
+        "src/traceback.rs": "0b5fd918f33d88784e0eeb62c7d91ef55fa33aa9ead274cea1ad87fd88004a77",
+        "src/tupleobject.rs": "e2fb9e8ca46aaaf828f9eef3b5f35d9cbb4f2ae324b3cc6b8e58e0788c0a8c25",
         "src/typeslots.rs": "0fb9ad514b91d07f4465398276a9c8e40969da3dd30216cbfe905e998e4c9d80",
-        "src/unicodeobject.rs": "fdd136fb02ddd4ddec9d5b9aeb9451f39959ba0d02ff73940fa1b5a5e361c68d",
+        "src/unicodeobject.rs": "6200b5c9bdcc0d3797025d221be938af9ed72451cf2d822777be4b5d90ddf078",
         "src/warnings.rs": "7e53c5a45da1af53110ab09d8d7485bfbf0154a7f0e531ac9b74f3b953ab4d11",
-        "src/weakrefobject.rs": "9a1bf20ed73cde94aee7b3f736a3d1ab896103fc1650596d2107ffdd644d6d1d"
+        "src/weakrefobject.rs": "f7905fbc285ea770b0f8197d616fd87a5d2bcbd7d8468028f6daec72b3807d9a"
     },
-    "package": "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+    "package": "214929900fd25e6604661ed9cf349727c8920d47deff196c4e28165a6ef2a96b"
 }
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/Cargo.toml` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # to registry (e.g., crates.io) dependencies.
 #
 # If you are reading this file be aware that the original Cargo.toml
 # will likely look very different (and much more reasonable).
 # See Cargo.toml.orig for the original contents.
 
 [package]
-edition = "2018"
+edition = "2021"
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.20.0"
 authors = ["PyO3 Project and Contributors <https://github.com/PyO3>"]
 links = "python"
 description = "Python-API bindings for the PyO3 ecosystem"
 homepage = "https://github.com/pyo3/pyo3"
 readme = "README.md"
 keywords = [
     "pyo3",
@@ -24,22 +24,22 @@
     "cpython",
     "ffi",
 ]
 categories = [
     "api-bindings",
     "development-tools::ffi",
 ]
-license = "Apache-2.0"
+license = "MIT OR Apache-2.0"
 repository = "https://github.com/pyo3/pyo3"
 
 [dependencies.libc]
 version = "0.2.62"
 
 [build-dependencies.pyo3-build-config]
-version = "0.19.2"
+version = "0.20.0"
 features = ["resolve-config"]
 
 [features]
 abi3 = ["pyo3-build-config/abi3"]
 abi3-py310 = [
     "abi3-py311",
     "pyo3-build-config/abi3-py310",
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/README.md` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 basically copying the documentation from CPython. Consult the [Python/C API Reference
 Manual][capi] for up-to-date documentation.
 
 # Minimum supported Rust and Python versions
 
 PyO3 supports the following software versions:
   - Python 3.7 and up (CPython and PyPy)
-  - Rust 1.48 and up
+  - Rust 1.56 and up
 
 # Example: Building Python Native modules
 
 PyO3 can be used to generate a native Python module. The easiest way to try this out for the
 first time is to use [`maturin`]. `maturin` is a tool for building and publishing Rust-based
 Python packages with minimal configuration. The following steps set up some files for an example
 Python module, install `maturin`, and then show how to build and import the Python module.
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/build.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     interpreter_config.emit_pyo3_cfgs();
 
     // Extra lines come last, to support last write wins.
     for line in &interpreter_config.extra_build_script_lines {
         println!("{}", line);
     }
 
-    // Emit cfgs like `addr_of` and `min_const_generics`
+    // Emit cfgs like `thread_local_const_init`
     print_feature_cfgs();
 
     Ok(())
 }
 
 fn print_config_and_exit(config: &InterpreterConfig) {
     println!("\n-- PYO3_PRINT_CONFIG=1 is set, printing configuration and halting compile --");
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/abstract_.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/abstract_.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/boolobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/boolobject.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 use crate::longobject::PyLongObject;
 use crate::object::*;
 use std::os::raw::{c_int, c_long};
+use std::ptr::addr_of_mut;
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyBool_Type")]
     pub static mut PyBool_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyBool_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyBool_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyBool_Type)) as c_int
 }
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "_PyPy_FalseStruct")]
     static mut _Py_FalseStruct: PyLongObject;
     #[cfg_attr(PyPy, link_name = "_PyPy_TrueStruct")]
     static mut _Py_TrueStruct: PyLongObject;
 }
 
 #[inline]
 pub unsafe fn Py_False() -> *mut PyObject {
-    addr_of_mut_shim!(_Py_FalseStruct) as *mut PyObject
+    addr_of_mut!(_Py_FalseStruct) as *mut PyObject
 }
 
 #[inline]
 pub unsafe fn Py_True() -> *mut PyObject {
-    addr_of_mut_shim!(_Py_TrueStruct) as *mut PyObject
+    addr_of_mut!(_Py_TrueStruct) as *mut PyObject
 }
 
 #[inline]
 pub unsafe fn Py_IsTrue(x: *mut PyObject) -> c_int {
     Py_Is(x, Py_True())
 }
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/bytearrayobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/bytearrayobject.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 use std::os::raw::{c_char, c_int};
+use std::ptr::addr_of_mut;
 
 #[cfg(not(any(PyPy, Py_LIMITED_API)))]
 #[repr(C)]
 #[derive(Copy, Clone)]
 pub struct PyByteArrayObject {
     pub ob_base: PyVarObject,
     pub ob_alloc: Py_ssize_t,
@@ -25,20 +26,20 @@
     pub static mut PyByteArray_Type: PyTypeObject;
 
     pub static mut PyByteArrayIter_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyByteArray_Check(op: *mut PyObject) -> c_int {
-    PyObject_TypeCheck(op, addr_of_mut_shim!(PyByteArray_Type))
+    PyObject_TypeCheck(op, addr_of_mut!(PyByteArray_Type))
 }
 
 #[inline]
 pub unsafe fn PyByteArray_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyByteArray_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyByteArray_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyByteArray_FromObject")]
     pub fn PyByteArray_FromObject(o: *mut PyObject) -> *mut PyObject;
     #[cfg_attr(PyPy, link_name = "PyPyByteArray_Concat")]
     pub fn PyByteArray_Concat(a: *mut PyObject, b: *mut PyObject) -> *mut PyObject;
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/bytesobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/bytesobject.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 use std::os::raw::{c_char, c_int};
+use std::ptr::addr_of_mut;
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyBytes_Type")]
     pub static mut PyBytes_Type: PyTypeObject;
     pub static mut PyBytesIter_Type: PyTypeObject;
 }
@@ -12,15 +13,15 @@
 #[inline]
 pub unsafe fn PyBytes_Check(op: *mut PyObject) -> c_int {
     PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_BYTES_SUBCLASS)
 }
 
 #[inline]
 pub unsafe fn PyBytes_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyBytes_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyBytes_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyBytes_FromStringAndSize")]
     pub fn PyBytes_FromStringAndSize(arg1: *const c_char, arg2: Py_ssize_t) -> *mut PyObject;
     pub fn PyBytes_FromString(arg1: *const c_char) -> *mut PyObject;
     #[cfg_attr(PyPy, link_name = "PyPyBytes_FromObject")]
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/ceval.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/ceval.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/codecs.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/codecs.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/complexobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/complexobject.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use crate::object::*;
 use std::os::raw::{c_double, c_int};
+use std::ptr::addr_of_mut;
 
 #[repr(C)]
 #[derive(Copy, Clone)]
 // non-limited
 pub struct Py_complex {
     pub real: c_double,
     pub imag: c_double,
@@ -36,20 +37,20 @@
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyComplex_Type")]
     pub static mut PyComplex_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyComplex_Check(op: *mut PyObject) -> c_int {
-    PyObject_TypeCheck(op, addr_of_mut_shim!(PyComplex_Type))
+    PyObject_TypeCheck(op, addr_of_mut!(PyComplex_Type))
 }
 
 #[inline]
 pub unsafe fn PyComplex_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyComplex_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyComplex_Type)) as c_int
 }
 
 extern "C" {
     // skipped non-limited PyComplex_FromCComplex
     #[cfg_attr(PyPy, link_name = "PyPyComplex_FromDoubles")]
     pub fn PyComplex_FromDoubles(real: c_double, imag: c_double) -> *mut PyObject;
     #[cfg_attr(PyPy, link_name = "PyPyComplex_RealAsDouble")]
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/context.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/context.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 use crate::object::{PyObject, PyTypeObject, Py_TYPE};
 use std::os::raw::{c_char, c_int};
+use std::ptr::addr_of_mut;
 
 extern "C" {
     pub static mut PyContext_Type: PyTypeObject;
     // skipped non-limited opaque PyContext
     pub static mut PyContextVar_Type: PyTypeObject;
     // skipped non-limited opaque PyContextVar
     pub static mut PyContextToken_Type: PyTypeObject;
     // skipped non-limited opaque PyContextToken
 }
 
 #[inline]
 pub unsafe fn PyContext_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyContext_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyContext_Type)) as c_int
 }
 
 #[inline]
 pub unsafe fn PyContextVar_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyContextVar_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyContextVar_Type)) as c_int
 }
 
 #[inline]
 pub unsafe fn PyContextToken_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyContextToken_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyContextToken_Type)) as c_int
 }
 
 extern "C" {
     pub fn PyContext_New() -> *mut PyObject;
     pub fn PyContext_Copy(ctx: *mut PyObject) -> *mut PyObject;
     pub fn PyContext_CopyCurrent() -> *mut PyObject;
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/abstract_.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/abstract_.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/bytesobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/bytesobject.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/code.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/code.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 
 #[allow(unused_imports)]
 use std::os::raw::{c_char, c_int, c_short, c_uchar, c_void};
+#[cfg(not(PyPy))]
+use std::ptr::addr_of_mut;
 
 #[cfg(all(Py_3_8, not(PyPy), not(Py_3_11)))]
 opaque_struct!(_PyOpcache);
 
-pub const _PY_MONITORING_UNGROUPED_EVENTS: usize = 14;
-pub const _PY_MONITORING_EVENTS: usize = 16;
+#[cfg(Py_3_12)]
+pub const _PY_MONITORING_LOCAL_EVENTS: usize = 10;
+#[cfg(Py_3_12)]
+pub const _PY_MONITORING_UNGROUPED_EVENTS: usize = 15;
+#[cfg(Py_3_12)]
+pub const _PY_MONITORING_EVENTS: usize = 17;
 
 #[cfg(Py_3_12)]
 #[repr(C)]
-#[derive(Copy, Clone)]
-pub struct _Py_Monitors {
+#[derive(Clone, Copy)]
+pub struct _Py_LocalMonitors {
+    pub tools: [u8; _PY_MONITORING_UNGROUPED_EVENTS],
+}
+
+#[cfg(Py_3_12)]
+#[repr(C)]
+#[derive(Clone, Copy)]
+pub struct _Py_GlobalMonitors {
     pub tools: [u8; _PY_MONITORING_UNGROUPED_EVENTS],
 }
 
 // skipped _Py_CODEUNIT
 
 // skipped _Py_OPCODE
 // skipped _Py_OPARG
@@ -47,16 +60,16 @@
     pub line_delta: i8,
 }
 
 #[cfg(Py_3_12)]
 #[repr(C)]
 #[derive(Copy, Clone)]
 pub struct _PyCoMonitoringData {
-    pub local_monitors: _Py_Monitors,
-    pub active_monitors: _Py_Monitors,
+    pub local_monitors: _Py_LocalMonitors,
+    pub active_monitors: _Py_LocalMonitors,
     pub tools: *mut u8,
     pub lines: *mut _PyCoLineInstrumentationData,
     pub line_tools: *mut u8,
     pub per_instruction_opcodes: *mut u8,
     pub per_instruction_tools: *mut u8,
 }
 
@@ -221,15 +234,15 @@
 extern "C" {
     pub static mut PyCode_Type: PyTypeObject;
 }
 
 #[inline]
 #[cfg(not(PyPy))]
 pub unsafe fn PyCode_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyCode_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyCode_Type)) as c_int
 }
 
 #[inline]
 #[cfg(all(not(PyPy), Py_3_10, not(Py_3_11)))]
 pub unsafe fn PyCode_GetNumFree(op: *mut PyCodeObject) -> Py_ssize_t {
     crate::PyTuple_GET_SIZE((*op).co_freevars)
 }
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/compile.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/compile.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/descrobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/descrobject.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/dictobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/dictobject.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/floatobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/floatobject.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/frameobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/frameobject.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use crate::cpython::code::PyCodeObject;
 use crate::object::*;
 use crate::pystate::PyThreadState;
 #[cfg(not(any(PyPy, Py_3_11)))]
 use std::os::raw::c_char;
 use std::os::raw::c_int;
+use std::ptr::addr_of_mut;
 
 #[cfg(not(any(PyPy, Py_3_11)))]
 pub type PyFrameState = c_char;
 
 #[repr(C)]
 #[derive(Copy, Clone)]
 #[cfg(not(any(PyPy, Py_3_11)))]
@@ -60,15 +61,15 @@
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     pub static mut PyFrame_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyFrame_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyFrame_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyFrame_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyFrame_New")]
     pub fn PyFrame_New(
         tstate: *mut PyThreadState,
         code: *mut PyCodeObject,
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/funcobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/funcobject.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 use std::os::raw::c_int;
+#[cfg(not(all(PyPy, not(Py_3_8))))]
+use std::ptr::addr_of_mut;
 
 use crate::PyObject;
 
 #[cfg(all(not(PyPy), not(Py_3_10)))]
 #[repr(C)]
 pub struct PyFunctionObject {
     pub ob_base: PyObject,
@@ -59,15 +61,15 @@
     #[cfg_attr(PyPy, link_name = "PyPyFunction_Type")]
     pub static mut PyFunction_Type: crate::PyTypeObject;
 }
 
 #[cfg(not(all(PyPy, not(Py_3_8))))]
 #[inline]
 pub unsafe fn PyFunction_Check(op: *mut PyObject) -> c_int {
-    (crate::Py_TYPE(op) == addr_of_mut_shim!(PyFunction_Type)) as c_int
+    (crate::Py_TYPE(op) == addr_of_mut!(PyFunction_Type)) as c_int
 }
 
 extern "C" {
     pub fn PyFunction_New(code: *mut PyObject, globals: *mut PyObject) -> *mut PyObject;
     pub fn PyFunction_NewWithQualName(
         code: *mut PyObject,
         globals: *mut PyObject,
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/genobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/genobject.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use crate::object::*;
 use crate::PyFrameObject;
 #[cfg(not(PyPy))]
 use crate::_PyErr_StackItem;
 #[cfg(Py_3_11)]
 use std::os::raw::c_char;
 use std::os::raw::c_int;
+use std::ptr::addr_of_mut;
 
 #[cfg(not(PyPy))]
 #[repr(C)]
 #[derive(Copy, Clone)]
 pub struct PyGenObject {
     pub ob_base: PyObject,
     #[cfg(not(Py_3_11))]
@@ -38,20 +39,20 @@
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     pub static mut PyGen_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyGen_Check(op: *mut PyObject) -> c_int {
-    PyObject_TypeCheck(op, addr_of_mut_shim!(PyGen_Type))
+    PyObject_TypeCheck(op, addr_of_mut!(PyGen_Type))
 }
 
 #[inline]
 pub unsafe fn PyGen_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyGen_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyGen_Type)) as c_int
 }
 
 extern "C" {
     pub fn PyGen_New(frame: *mut PyFrameObject) -> *mut PyObject;
     // skipped PyGen_NewWithQualName
     // skipped _PyGen_SetStopIterationValue
     // skipped _PyGen_FetchStopIterationValue
@@ -68,15 +69,15 @@
 extern "C" {
     pub static mut PyCoro_Type: PyTypeObject;
     pub static mut _PyCoroWrapper_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyCoro_CheckExact(op: *mut PyObject) -> c_int {
-    PyObject_TypeCheck(op, addr_of_mut_shim!(PyCoro_Type))
+    PyObject_TypeCheck(op, addr_of_mut!(PyCoro_Type))
 }
 
 // skipped _PyCoro_GetAwaitableIter
 // skipped PyCoro_New
 
 // skipped PyAsyncGenObject
 
@@ -88,11 +89,11 @@
     // skipped _PyAsyncGenAThrow_Type
 }
 
 // skipped PyAsyncGen_New
 
 #[inline]
 pub unsafe fn PyAsyncGen_CheckExact(op: *mut PyObject) -> c_int {
-    PyObject_TypeCheck(op, addr_of_mut_shim!(PyAsyncGen_Type))
+    PyObject_TypeCheck(op, addr_of_mut!(PyAsyncGen_Type))
 }
 
 // skipped _PyAsyncGenValueWrapperNew
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/import.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/import.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/initconfig.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/initconfig.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/listobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/listobject.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/methodobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/methodobject.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 use crate::object::*;
 use crate::{PyCFunctionObject, PyMethodDefPointer, METH_METHOD, METH_STATIC};
 use std::os::raw::c_int;
+use std::ptr::addr_of_mut;
 
 pub struct PyCMethodObject {
     pub func: PyCFunctionObject,
     pub mm_class: *mut PyTypeObject,
 }
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     pub static mut PyCMethod_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyCMethod_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyCMethod_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyCMethod_Type)) as c_int
 }
 
 #[inline]
 pub unsafe fn PyCMethod_Check(op: *mut PyObject) -> c_int {
-    PyObject_TypeCheck(op, addr_of_mut_shim!(PyCMethod_Type))
+    PyObject_TypeCheck(op, addr_of_mut!(PyCMethod_Type))
 }
 
 #[inline]
 pub unsafe fn PyCFunction_GET_FUNCTION(func: *mut PyObject) -> PyMethodDefPointer {
     debug_assert_eq!(PyCMethod_Check(func), 1);
 
     let func = func.cast::<PyCFunctionObject>();
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/mod.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -17,23 +17,26 @@
 #[cfg(all(Py_3_8, not(PyPy)))]
 pub(crate) mod initconfig;
 // skipped interpreteridobject.h
 pub(crate) mod listobject;
 #[cfg(all(Py_3_9, not(PyPy)))]
 pub(crate) mod methodobject;
 pub(crate) mod object;
+pub(crate) mod objimpl;
 pub(crate) mod pydebug;
 pub(crate) mod pyerrors;
 #[cfg(all(Py_3_8, not(PyPy)))]
 pub(crate) mod pylifecycle;
 pub(crate) mod pymem;
 pub(crate) mod pystate;
 pub(crate) mod pythonrun;
 // skipped sysmodule.h
 pub(crate) mod floatobject;
+#[cfg(not(PyPy))]
+pub(crate) mod pyframe;
 pub(crate) mod tupleobject;
 pub(crate) mod unicodeobject;
 pub(crate) mod weakrefobject;
 
 pub use self::abstract_::*;
 pub use self::bytesobject::*;
 #[cfg(not(PyPy))]
@@ -50,16 +53,19 @@
 pub use self::import::*;
 #[cfg(all(Py_3_8, not(PyPy)))]
 pub use self::initconfig::*;
 pub use self::listobject::*;
 #[cfg(all(Py_3_9, not(PyPy)))]
 pub use self::methodobject::*;
 pub use self::object::*;
+pub use self::objimpl::*;
 pub use self::pydebug::*;
 pub use self::pyerrors::*;
+#[cfg(not(PyPy))]
+pub use self::pyframe::*;
 #[cfg(all(Py_3_8, not(PyPy)))]
 pub use self::pylifecycle::*;
 pub use self::pymem::*;
 pub use self::pystate::*;
 pub use self::pythonrun::*;
 pub use self::tupleobject::*;
 pub use self::unicodeobject::*;
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/object.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/object.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-use crate::object;
 #[cfg(Py_3_8)]
 use crate::vectorcallfunc;
-use crate::{PyObject, Py_ssize_t};
+use crate::{object, PyGetSetDef, PyMemberDef, PyMethodDef, PyObject, Py_ssize_t};
 use std::mem;
 use std::os::raw::{c_char, c_int, c_uint, c_ulong, c_void};
 
 // skipped _Py_NewReference
 // skipped _Py_ForgetReference
 // skipped _Py_GetRefTotal
 
@@ -243,17 +242,17 @@
     pub tp_doc: *const c_char,
     pub tp_traverse: Option<object::traverseproc>,
     pub tp_clear: Option<object::inquiry>,
     pub tp_richcompare: Option<object::richcmpfunc>,
     pub tp_weaklistoffset: Py_ssize_t,
     pub tp_iter: Option<object::getiterfunc>,
     pub tp_iternext: Option<object::iternextfunc>,
-    pub tp_methods: *mut crate::methodobject::PyMethodDef,
-    pub tp_members: *mut crate::structmember::PyMemberDef,
-    pub tp_getset: *mut crate::descrobject::PyGetSetDef,
+    pub tp_methods: *mut PyMethodDef,
+    pub tp_members: *mut PyMemberDef,
+    pub tp_getset: *mut PyGetSetDef,
     pub tp_base: *mut PyTypeObject,
     pub tp_dict: *mut object::PyObject,
     pub tp_descr_get: Option<object::descrgetfunc>,
     pub tp_descr_set: Option<object::descrsetfunc>,
     pub tp_dictoffset: Py_ssize_t,
     pub tp_init: Option<object::initproc>,
     pub tp_alloc: Option<object::allocfunc>,
@@ -323,20 +322,18 @@
     #[inline]
     fn default() -> Self {
         unsafe { mem::zeroed() }
     }
 }
 
 #[inline]
-pub unsafe fn PyHeapType_GET_MEMBERS(
-    etype: *mut PyHeapTypeObject,
-) -> *mut crate::structmember::PyMemberDef {
+pub unsafe fn PyHeapType_GET_MEMBERS(etype: *mut PyHeapTypeObject) -> *mut PyMemberDef {
     let py_type = object::Py_TYPE(etype as *mut object::PyObject);
     let ptr = etype.offset((*py_type).tp_basicsize);
-    ptr as *mut crate::structmember::PyMemberDef
+    ptr as *mut PyMemberDef
 }
 
 // skipped _PyType_Name
 // skipped _PyType_Lookup
 // skipped _PyType_LookupId
 // skipped _PyObject_LookupSpecial
 // skipped _PyType_CalculateMetaclass
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pyerrors.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pyerrors.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pymem.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pymem.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pystate.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pystate.rs`

 * *Files 2% similar despite different names*

```diff
@@ -65,21 +65,28 @@
     #[cfg(not(PyPy))]
     pub fn PyThreadState_Next(tstate: *mut PyThreadState) -> *mut PyThreadState;
 
     #[cfg_attr(PyPy, link_name = "PyPyThreadState_DeleteCurrent")]
     pub fn PyThreadState_DeleteCurrent();
 }
 
-#[cfg(Py_3_9)]
+#[cfg(all(Py_3_9, not(Py_3_11)))]
 pub type _PyFrameEvalFunction = extern "C" fn(
     *mut crate::PyThreadState,
     *mut crate::PyFrameObject,
     c_int,
 ) -> *mut crate::object::PyObject;
 
+#[cfg(Py_3_11)]
+pub type _PyFrameEvalFunction = extern "C" fn(
+    *mut crate::PyThreadState,
+    *mut crate::_PyInterpreterFrame,
+    c_int,
+) -> *mut crate::object::PyObject;
+
 #[cfg(Py_3_9)]
 extern "C" {
     /// Get the frame evaluation function.
     pub fn _PyInterpreterState_GetEvalFrameFunc(
         interp: *mut PyInterpreterState,
     ) -> _PyFrameEvalFunction;
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/pythonrun.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/pythonrun.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/tupleobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/tupleobject.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/cpython/unicodeobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/cpython/unicodeobject.rs`

 * *Files 1% similar despite different names*

```diff
@@ -258,27 +258,30 @@
     pub state: u32,
     #[cfg(not(Py_3_12))]
     pub wstr: *mut wchar_t,
 }
 
 /// Interacting with the bitfield is not actually well-defined, so we mark these APIs unsafe.
 impl PyASCIIObject {
+    #[cfg_attr(not(Py_3_12), allow(rustdoc::broken_intra_doc_links))] // SSTATE_INTERNED_IMMORTAL_STATIC requires 3.12
     /// Get the `interned` field of the [`PyASCIIObject`] state bitfield.
     ///
     /// Returns one of: [`SSTATE_NOT_INTERNED`], [`SSTATE_INTERNED_MORTAL`],
-    /// or [`SSTATE_INTERNED_IMMORTAL`].
+    /// [`SSTATE_INTERNED_IMMORTAL`], or [`SSTATE_INTERNED_IMMORTAL_STATIC`].
     #[inline]
     pub unsafe fn interned(&self) -> c_uint {
         PyASCIIObjectState::from(self.state).interned()
     }
 
+    #[cfg_attr(not(Py_3_12), allow(rustdoc::broken_intra_doc_links))] // SSTATE_INTERNED_IMMORTAL_STATIC requires 3.12
     /// Set the `interned` field of the [`PyASCIIObject`] state bitfield.
     ///
     /// Calling this function with an argument that is not [`SSTATE_NOT_INTERNED`],
-    /// [`SSTATE_INTERNED_MORTAL`], or [`SSTATE_INTERNED_IMMORTAL`] is invalid.
+    /// [`SSTATE_INTERNED_MORTAL`], [`SSTATE_INTERNED_IMMORTAL`], or
+    /// [`SSTATE_INTERNED_IMMORTAL_STATIC`] is invalid.
     #[inline]
     pub unsafe fn set_interned(&mut self, val: c_uint) {
         let mut state = PyASCIIObjectState::from(self.state);
         state.set_interned(val);
         self.state = u32::from(state);
     }
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/datetime.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/datetime.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/descrobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/objimpl.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,94 @@
-use crate::methodobject::PyMethodDef;
-use crate::object::{PyObject, PyTypeObject};
-use crate::structmember::PyMemberDef;
-use std::os::raw::{c_char, c_int, c_void};
-use std::ptr;
-
-pub type getter = unsafe extern "C" fn(slf: *mut PyObject, closure: *mut c_void) -> *mut PyObject;
-pub type setter =
-    unsafe extern "C" fn(slf: *mut PyObject, value: *mut PyObject, closure: *mut c_void) -> c_int;
-
-#[repr(C)]
-#[derive(Copy, Clone, Debug, Eq, PartialEq)]
-pub struct PyGetSetDef {
-    pub name: *const c_char,
-    pub get: Option<getter>,
-    pub set: Option<setter>,
-    pub doc: *const c_char,
-    pub closure: *mut c_void,
-}
+use libc::size_t;
+use std::os::raw::{c_int, c_void};
 
-impl Default for PyGetSetDef {
-    fn default() -> PyGetSetDef {
-        PyGetSetDef {
-            name: ptr::null(),
-            get: None,
-            set: None,
-            doc: ptr::null(),
-            closure: ptr::null_mut(),
-        }
-    }
-}
+use crate::object::*;
+use crate::pyport::Py_ssize_t;
 
-#[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
-    #[cfg_attr(PyPy, link_name = "PyPyClassMethodDescr_Type")]
-    pub static mut PyClassMethodDescr_Type: PyTypeObject;
-    #[cfg_attr(PyPy, link_name = "PyPyGetSetDescr_Type")]
-    pub static mut PyGetSetDescr_Type: PyTypeObject;
-    #[cfg_attr(PyPy, link_name = "PyPyMemberDescr_Type")]
-    pub static mut PyMemberDescr_Type: PyTypeObject;
-    #[cfg_attr(PyPy, link_name = "PyPyMethodDescr_Type")]
-    pub static mut PyMethodDescr_Type: PyTypeObject;
-    #[cfg_attr(PyPy, link_name = "PyPyWrapperDescr_Type")]
-    pub static mut PyWrapperDescr_Type: PyTypeObject;
-    #[cfg_attr(PyPy, link_name = "PyPyDictProxy_Type")]
-    pub static mut PyDictProxy_Type: PyTypeObject;
-    #[cfg_attr(PyPy, link_name = "PyPyProperty_Type")]
-    pub static mut PyProperty_Type: PyTypeObject;
+    #[cfg_attr(PyPy, link_name = "PyPyObject_Malloc")]
+    pub fn PyObject_Malloc(size: size_t) -> *mut c_void;
+    #[cfg_attr(PyPy, link_name = "PyPyObject_Calloc")]
+    pub fn PyObject_Calloc(nelem: size_t, elsize: size_t) -> *mut c_void;
+    #[cfg_attr(PyPy, link_name = "PyPyObject_Realloc")]
+    pub fn PyObject_Realloc(ptr: *mut c_void, new_size: size_t) -> *mut c_void;
+    #[cfg_attr(PyPy, link_name = "PyPyObject_Free")]
+    pub fn PyObject_Free(ptr: *mut c_void);
+
+    // skipped PyObject_MALLOC
+    // skipped PyObject_REALLOC
+    // skipped PyObject_FREE
+    // skipped PyObject_Del
+    // skipped PyObject_DEL
+
+    #[cfg_attr(PyPy, link_name = "PyPyObject_Init")]
+    pub fn PyObject_Init(arg1: *mut PyObject, arg2: *mut PyTypeObject) -> *mut PyObject;
+    #[cfg_attr(PyPy, link_name = "PyPyObject_InitVar")]
+    pub fn PyObject_InitVar(
+        arg1: *mut PyVarObject,
+        arg2: *mut PyTypeObject,
+        arg3: Py_ssize_t,
+    ) -> *mut PyVarObject;
+
+    // skipped PyObject_INIT
+    // skipped PyObject_INIT_VAR
+
+    #[cfg_attr(PyPy, link_name = "_PyPyObject_New")]
+    pub fn _PyObject_New(arg1: *mut PyTypeObject) -> *mut PyObject;
+    #[cfg_attr(PyPy, link_name = "_PyPyObject_NewVar")]
+    pub fn _PyObject_NewVar(arg1: *mut PyTypeObject, arg2: Py_ssize_t) -> *mut PyVarObject;
+
+    // skipped PyObject_New
+    // skipped PyObject_NEW
+    // skipped PyObject_NewVar
+    // skipped PyObject_NEW_VAR
+
+    pub fn PyGC_Collect() -> Py_ssize_t;
+
+    #[cfg(Py_3_10)]
+    #[cfg_attr(PyPy, link_name = "PyPyGC_Enable")]
+    pub fn PyGC_Enable() -> c_int;
+
+    #[cfg(Py_3_10)]
+    #[cfg_attr(PyPy, link_name = "PyPyGC_Disable")]
+    pub fn PyGC_Disable() -> c_int;
+
+    #[cfg(Py_3_10)]
+    #[cfg_attr(PyPy, link_name = "PyPyGC_IsEnabled")]
+    pub fn PyGC_IsEnabled() -> c_int;
+
+    // skipped PyUnstable_GC_VisitObjects
+}
+
+#[inline]
+pub unsafe fn PyType_IS_GC(t: *mut PyTypeObject) -> c_int {
+    PyType_HasFeature(t, Py_TPFLAGS_HAVE_GC)
 }
 
 extern "C" {
-    pub fn PyDescr_NewMethod(arg1: *mut PyTypeObject, arg2: *mut PyMethodDef) -> *mut PyObject;
-    #[cfg_attr(PyPy, link_name = "PyPyDescr_NewClassMethod")]
-    pub fn PyDescr_NewClassMethod(arg1: *mut PyTypeObject, arg2: *mut PyMethodDef)
-        -> *mut PyObject;
-    #[cfg_attr(PyPy, link_name = "PyPyDescr_NewMember")]
-    pub fn PyDescr_NewMember(arg1: *mut PyTypeObject, arg2: *mut PyMemberDef) -> *mut PyObject;
-    #[cfg_attr(PyPy, link_name = "PyPyDescr_NewGetSet")]
-    pub fn PyDescr_NewGetSet(arg1: *mut PyTypeObject, arg2: *mut PyGetSetDef) -> *mut PyObject;
-
-    #[cfg_attr(PyPy, link_name = "PyPyDictProxy_New")]
-    pub fn PyDictProxy_New(arg1: *mut PyObject) -> *mut PyObject;
-    pub fn PyWrapper_New(arg1: *mut PyObject, arg2: *mut PyObject) -> *mut PyObject;
+    pub fn _PyObject_GC_Resize(arg1: *mut PyVarObject, arg2: Py_ssize_t) -> *mut PyVarObject;
+
+    // skipped PyObject_GC_Resize
+
+    #[cfg_attr(PyPy, link_name = "_PyPyObject_GC_New")]
+    pub fn _PyObject_GC_New(arg1: *mut PyTypeObject) -> *mut PyObject;
+    #[cfg_attr(PyPy, link_name = "_PyPyObject_GC_NewVar")]
+    pub fn _PyObject_GC_NewVar(arg1: *mut PyTypeObject, arg2: Py_ssize_t) -> *mut PyVarObject;
+    #[cfg(not(PyPy))]
+    pub fn PyObject_GC_Track(arg1: *mut c_void);
+    #[cfg(not(PyPy))]
+    pub fn PyObject_GC_UnTrack(arg1: *mut c_void);
+    #[cfg_attr(PyPy, link_name = "PyPyObject_GC_Del")]
+    pub fn PyObject_GC_Del(arg1: *mut c_void);
+
+    // skipped PyObject_GC_New
+    // skipped PyObject_GC_NewVar
+
+    #[cfg(any(all(Py_3_9, not(PyPy)), Py_3_10))] // added in 3.9, or 3.10 on PyPy
+    #[cfg_attr(PyPy, link_name = "PyPyObject_GC_IsTracked")]
+    pub fn PyObject_GC_IsTracked(arg1: *mut PyObject) -> c_int;
+    #[cfg(any(all(Py_3_9, not(PyPy)), Py_3_10))] // added in 3.9, or 3.10 on PyPy
+    #[cfg_attr(PyPy, link_name = "PyPyObject_GC_IsFinalized")]
+    pub fn PyObject_GC_IsFinalized(arg1: *mut PyObject) -> c_int;
 }
+
+// skipped Py_VISIT
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/dictobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/dictobject.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 use std::os::raw::{c_char, c_int};
+use std::ptr::addr_of_mut;
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyDict_Type")]
     pub static mut PyDict_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyDict_Check(op: *mut PyObject) -> c_int {
     PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_DICT_SUBCLASS)
 }
 
 #[inline]
 pub unsafe fn PyDict_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyDict_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyDict_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyDict_New")]
     pub fn PyDict_New() -> *mut PyObject;
     #[cfg_attr(PyPy, link_name = "PyPyDict_GetItem")]
     pub fn PyDict_GetItem(mp: *mut PyObject, key: *mut PyObject) -> *mut PyObject;
@@ -73,25 +74,25 @@
     pub static mut PyDictKeys_Type: PyTypeObject;
     pub static mut PyDictValues_Type: PyTypeObject;
     pub static mut PyDictItems_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyDictKeys_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyDictKeys_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyDictKeys_Type)) as c_int
 }
 
 #[inline]
 pub unsafe fn PyDictValues_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyDictValues_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyDictValues_Type)) as c_int
 }
 
 #[inline]
 pub unsafe fn PyDictItems_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyDictItems_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyDictItems_Type)) as c_int
 }
 
 #[inline]
 pub unsafe fn PyDictViewSet_Check(op: *mut PyObject) -> c_int {
     (PyDictKeys_Check(op) != 0 || PyDictItems_Check(op) != 0) as c_int
 }
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/fileobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/fileobject.rs`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     pub fn PyFile_WriteString(arg1: *const c_char, arg2: *mut PyObject) -> c_int;
     #[cfg_attr(PyPy, link_name = "PyPyFile_AsFileDescriptor")]
     pub fn PyObject_AsFileDescriptor(arg1: *mut PyObject) -> c_int;
 }
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
+    #[deprecated(note = "Python 3.12")]
     pub static mut Py_FileSystemDefaultEncoding: *const c_char;
+    #[deprecated(note = "Python 3.12")]
     pub static mut Py_FileSystemDefaultEncodeErrors: *const c_char;
+    #[deprecated(note = "Python 3.12")]
     pub static mut Py_HasFileSystemDefaultEncoding: c_int;
-    // skipped Python 3.7 / ex-non-limited Py_UTF8Mode
+    // skipped 3.12-deprecated Py_UTF8Mode
 }
 
 // skipped _PyIsSelectable_fd
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/floatobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/floatobject.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 use crate::object::*;
 use std::os::raw::{c_double, c_int};
+use std::ptr::addr_of_mut;
 
 #[cfg(Py_LIMITED_API)]
 // TODO: remove (see https://github.com/PyO3/pyo3/pull/1341#issuecomment-751515985)
 opaque_struct!(PyFloatObject);
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyFloat_Type")]
     pub static mut PyFloat_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyFloat_Check(op: *mut PyObject) -> c_int {
-    PyObject_TypeCheck(op, addr_of_mut_shim!(PyFloat_Type))
+    PyObject_TypeCheck(op, addr_of_mut!(PyFloat_Type))
 }
 
 #[inline]
 pub unsafe fn PyFloat_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyFloat_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyFloat_Type)) as c_int
 }
 
 // skipped Py_RETURN_NAN
 // skipped Py_RETURN_INF
 
 extern "C" {
     pub fn PyFloat_GetMax() -> c_double;
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/import.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/import.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/intrcheck.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/intrcheck.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/iterobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/iterobject.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 use crate::object::*;
 use std::os::raw::c_int;
+use std::ptr::addr_of_mut;
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     pub static mut PySeqIter_Type: PyTypeObject;
     pub static mut PyCallIter_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PySeqIter_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PySeqIter_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PySeqIter_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPySeqIter_New")]
     pub fn PySeqIter_New(arg1: *mut PyObject) -> *mut PyObject;
 }
 
 #[inline]
 pub unsafe fn PyCallIter_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyCallIter_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyCallIter_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyCallIter_New")]
     pub fn PyCallIter_New(arg1: *mut PyObject, arg2: *mut PyObject) -> *mut PyObject;
 }
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/lib.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 //! - `Py_LIMITED_API`: Marks code enabled when the `abi3` feature flag is enabled.
 //! - `PyPy` - Marks code enabled when compiling for PyPy.
 //!
 //! # Minimum supported Rust and Python versions
 //!
 //! PyO3 supports the following software versions:
 //!   - Python 3.7 and up (CPython and PyPy)
-//!   - Rust 1.48 and up
+//!   - Rust 1.56 and up
 //!
 //! # Example: Building Python Native modules
 //!
 //! PyO3 can be used to generate a native Python module. The easiest way to try this out for the
 //! first time is to use [`maturin`]. `maturin` is a tool for building and publishing Rust-based
 //! Python packages with minimal configuration. The following steps set up some files for an example
 //! Python module, install `maturin`, and then show how to build and import the Python module.
@@ -71,17 +71,15 @@
 //! #
 //! # Downstream Rust code (including code in `bin/`, `examples/`, and `tests/`) will not be able
 //! # to `use string_sum;` unless the "rlib" or "lib" crate type is also included, e.g.:
 //! # crate-type = ["cdylib", "rlib"]
 //! crate-type = ["cdylib"]
 //!
 //! [dependencies.pyo3-ffi]
-// workaround for `extended_key_value_attributes`: https://github.com/rust-lang/rust/issues/82768#issuecomment-803935643
-#![cfg_attr(docsrs, cfg_attr(docsrs, doc = concat!("version = \"", env!("CARGO_PKG_VERSION"),  "\"")))]
-#![cfg_attr(not(docsrs), doc = "version = \"*\"")]
+#![doc = concat!("version = \"", env!("CARGO_PKG_VERSION"),  "\"")]
 //! features = ["extension-module"]
 //! ```
 //!
 //! **`src/lib.rs`**
 //! ```rust
 //! use std::os::raw::c_char;
 //! use std::ptr;
@@ -254,27 +252,14 @@
 macro_rules! opaque_struct {
     ($name:ident) => {
         #[repr(C)]
         pub struct $name([u8; 0]);
     };
 }
 
-macro_rules! addr_of_mut_shim {
-    ($place:expr) => {{
-        #[cfg(addr_of)]
-        {
-            ::std::ptr::addr_of_mut!($place)
-        }
-        #[cfg(not(addr_of))]
-        {
-            &mut $place as *mut _
-        }
-    }};
-}
-
 pub use self::abstract_::*;
 pub use self::bltinmodule::*;
 pub use self::boolobject::*;
 pub use self::bytearrayobject::*;
 pub use self::bytesobject::*;
 pub use self::ceval::*;
 pub use self::code::*;
@@ -292,14 +277,15 @@
 pub use self::fileutils::*;
 pub use self::floatobject::*;
 pub use self::import::*;
 pub use self::intrcheck::*;
 pub use self::iterobject::*;
 pub use self::listobject::*;
 pub use self::longobject::*;
+#[cfg(not(Py_LIMITED_API))]
 pub use self::marshal::*;
 pub use self::memoryobject::*;
 pub use self::methodobject::*;
 pub use self::modsupport::*;
 pub use self::moduleobject::*;
 pub use self::object::*;
 pub use self::objimpl::*;
@@ -362,15 +348,16 @@
 mod import;
 // skipped interpreteridobject.h
 mod intrcheck;
 mod iterobject;
 mod listobject;
 // skipped longintrepr.h
 mod longobject;
-pub(crate) mod marshal;
+#[cfg(not(Py_LIMITED_API))]
+pub mod marshal;
 mod memoryobject;
 mod methodobject;
 mod modsupport;
 mod moduleobject;
 // skipped namespaceobject.h
 mod object;
 mod objimpl;
@@ -418,14 +405,15 @@
 mod tupleobject;
 mod typeslots;
 mod unicodeobject;
 mod warnings;
 mod weakrefobject;
 
 // Additional headers that are not exported by Python.h
+#[deprecated(note = "Python 3.12")]
 pub mod structmember;
 
 // "Limited API" definitions matching Python's `include/cpython` directory.
 #[cfg(not(Py_LIMITED_API))]
 mod cpython;
 
 #[cfg(not(Py_LIMITED_API))]
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/listobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/listobject.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 use std::os::raw::c_int;
+use std::ptr::addr_of_mut;
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyList_Type")]
     pub static mut PyList_Type: PyTypeObject;
     pub static mut PyListIter_Type: PyTypeObject;
     pub static mut PyListRevIter_Type: PyTypeObject;
@@ -13,15 +14,15 @@
 #[inline]
 pub unsafe fn PyList_Check(op: *mut PyObject) -> c_int {
     PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_LIST_SUBCLASS)
 }
 
 #[inline]
 pub unsafe fn PyList_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyList_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyList_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyList_New")]
     pub fn PyList_New(size: Py_ssize_t) -> *mut PyObject;
     #[cfg_attr(PyPy, link_name = "PyPyList_Size")]
     pub fn PyList_Size(arg1: *mut PyObject) -> Py_ssize_t;
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/longobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/longobject.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 use libc::size_t;
 #[cfg(not(Py_LIMITED_API))]
 use std::os::raw::c_uchar;
 use std::os::raw::{c_char, c_double, c_int, c_long, c_longlong, c_ulong, c_ulonglong, c_void};
+use std::ptr::addr_of_mut;
 
 opaque_struct!(PyLongObject);
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyLong_Type")]
     pub static mut PyLong_Type: PyTypeObject;
@@ -16,15 +17,15 @@
 #[inline]
 pub unsafe fn PyLong_Check(op: *mut PyObject) -> c_int {
     PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_LONG_SUBCLASS)
 }
 
 #[inline]
 pub unsafe fn PyLong_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyLong_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyLong_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyLong_FromLong")]
     pub fn PyLong_FromLong(arg1: c_long) -> *mut PyObject;
     #[cfg_attr(PyPy, link_name = "PyPyLong_FromUnsignedLong")]
     pub fn PyLong_FromUnsignedLong(arg1: c_ulong) -> *mut PyObject;
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/marshal.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/marshal.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/memoryobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/memoryobject.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 use std::os::raw::{c_char, c_int};
+use std::ptr::addr_of_mut;
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg(not(Py_LIMITED_API))]
     pub static mut _PyManagedBuffer_Type: PyTypeObject;
 
     #[cfg_attr(PyPy, link_name = "PyPyMemoryView_Type")]
     pub static mut PyMemoryView_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PyMemoryView_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyMemoryView_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyMemoryView_Type)) as c_int
 }
 
 // skipped non-limited PyMemoryView_GET_BUFFER
 // skipped non-limited PyMemeryView_GET_BASE
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyMemoryView_FromObject")]
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/methodobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/methodobject.rs`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,27 @@
     #[cfg_attr(PyPy, link_name = "PyPyCFunction_Type")]
     pub static mut PyCFunction_Type: PyTypeObject;
 }
 
 #[cfg(Py_3_9)]
 #[inline]
 pub unsafe fn PyCFunction_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyCFunction_Type)) as c_int
+    (Py_TYPE(op) == ptr::addr_of_mut!(PyCFunction_Type)) as c_int
 }
 
 #[cfg(Py_3_9)]
 #[inline]
 pub unsafe fn PyCFunction_Check(op: *mut PyObject) -> c_int {
-    PyObject_TypeCheck(op, addr_of_mut_shim!(PyCFunction_Type))
+    PyObject_TypeCheck(op, ptr::addr_of_mut!(PyCFunction_Type))
 }
 
 #[cfg(not(Py_3_9))]
 #[inline]
 pub unsafe fn PyCFunction_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyCFunction_Type)) as c_int
+    (Py_TYPE(op) == ptr::addr_of_mut!(PyCFunction_Type)) as c_int
 }
 
 pub type PyCFunction =
     unsafe extern "C" fn(slf: *mut PyObject, args: *mut PyObject) -> *mut PyObject;
 
 #[cfg(any(Py_3_10, not(Py_LIMITED_API)))]
 pub type _PyCFunctionFast = unsafe extern "C" fn(
@@ -81,14 +81,19 @@
     pub fn PyCFunction_Call(
         f: *mut PyObject,
         args: *mut PyObject,
         kwds: *mut PyObject,
     ) -> *mut PyObject;
 }
 
+/// Represents the [PyMethodDef](https://docs.python.org/3/c-api/structures.html#c.PyMethodDef)
+/// structure.
+///
+/// Note that CPython may leave fields uninitialized. You must ensure that
+/// `ml_name` != NULL before dereferencing or reading other fields.
 #[repr(C)]
 #[derive(Copy, Clone, PartialEq, Eq)]
 pub struct PyMethodDef {
     pub ml_name: *const c_char,
     pub ml_meth: PyMethodDefPointer,
     pub ml_flags: c_int,
     pub ml_doc: *const c_char,
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/modsupport.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/modsupport.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/object.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/object.rs`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,16 @@
 }
 
 // PyLong_Type defined in longobject.rs
 // PyBool_Type defined in boolobject.rs
 
 #[inline]
 pub unsafe fn Py_SIZE(ob: *mut PyObject) -> Py_ssize_t {
-    debug_assert_ne!((*ob).ob_type, addr_of_mut_shim!(crate::PyLong_Type));
-    debug_assert_ne!((*ob).ob_type, addr_of_mut_shim!(crate::PyBool_Type));
+    debug_assert_ne!((*ob).ob_type, std::ptr::addr_of_mut!(crate::PyLong_Type));
+    debug_assert_ne!((*ob).ob_type, std::ptr::addr_of_mut!(crate::PyBool_Type));
     (*ob.cast::<PyVarObject>()).ob_size
 }
 
 #[inline]
 pub unsafe fn Py_IS_TYPE(ob: *mut PyObject, tp: *mut PyTypeObject) -> c_int {
     (Py_TYPE(ob) == tp) as c_int
 }
@@ -448,26 +448,22 @@
 } else {
     Py_TPFLAGS_HAVE_STACKLESS_EXTENSION | Py_TPFLAGS_HAVE_VERSION_TAG
 };
 
 pub const Py_TPFLAGS_HAVE_FINALIZE: c_ulong = 1;
 pub const Py_TPFLAGS_HAVE_VERSION_TAG: c_ulong = 1 << 18;
 
-#[cfg(all(py_sys_config = "Py_REF_DEBUG", not(Py_LIMITED_API)))]
 extern "C" {
-    pub fn _Py_NegativeRefCount(filename: *const c_char, lineno: c_int, op: *mut PyObject);
-    #[cfg(Py_3_12)]
-    #[link_name = "_Py_IncRefTotal_DO_NOT_USE_THIS"]
-    fn _Py_INC_REFTOTAL();
-    #[cfg(Py_3_12)]
-    #[link_name = "_Py_DecRefTotal_DO_NOT_USE_THIS"]
-    fn _Py_DEC_REFTOTAL();
-}
+    #[cfg(all(py_sys_config = "Py_REF_DEBUG", not(Py_LIMITED_API)))]
+    pub fn _Py_NegativeRefcount(filename: *const c_char, lineno: c_int, op: *mut PyObject);
+    #[cfg(all(Py_3_12, py_sys_config = "Py_REF_DEBUG", not(Py_LIMITED_API)))]
+    fn _Py_INCREF_IncRefTotal();
+    #[cfg(all(Py_3_12, py_sys_config = "Py_REF_DEBUG", not(Py_LIMITED_API)))]
+    fn _Py_DECREF_DecRefTotal();
 
-extern "C" {
     #[cfg_attr(PyPy, link_name = "_PyPy_Dealloc")]
     pub fn _Py_Dealloc(arg1: *mut PyObject);
 
     #[cfg_attr(PyPy, link_name = "PyPy_IncRef")]
     pub fn Py_IncRef(o: *mut PyObject);
     #[cfg_attr(PyPy, link_name = "PyPy_DecRef")]
     pub fn Py_DecRef(o: *mut PyObject);
@@ -496,17 +492,22 @@
 
     #[cfg(all(py_sys_config = "Py_REF_DEBUG", not(Py_3_10)))]
     {
         return Py_IncRef(op);
     }
 
     #[cfg(any(
-        not(Py_LIMITED_API),
         all(Py_LIMITED_API, not(Py_3_12)),
-        all(py_sys_config = "Py_REF_DEBUG", Py_3_12, not(Py_LIMITED_API))
+        all(
+            not(Py_LIMITED_API),
+            any(
+                not(py_sys_config = "Py_REF_DEBUG"),
+                all(py_sys_config = "Py_REF_DEBUG", Py_3_12),
+            )
+        ),
     ))]
     {
         #[cfg(all(Py_3_12, target_pointer_width = "64"))]
         {
             let cur_refcnt = (*op).ob_refcnt.ob_refcnt_split[crate::PY_BIG_ENDIAN];
             let new_refcnt = cur_refcnt.wrapping_add(1);
             if new_refcnt == 0 {
@@ -528,15 +529,15 @@
             (*op).ob_refcnt += 1
         }
 
         // Skipped _Py_INCREF_STAT_INC - if anyone wants this, please file an issue
         // or submit a PR supporting Py_STATS build option and pystats.h
 
         #[cfg(all(py_sys_config = "Py_REF_DEBUG", Py_3_12))]
-        _Py_INC_REFTOTAL();
+        _Py_INCREF_IncRefTotal();
     }
 }
 
 #[inline(always)]
 #[cfg_attr(
     all(py_sys_config = "Py_REF_DEBUG", Py_3_12, not(Py_LIMITED_API)),
     track_caller
@@ -556,38 +557,44 @@
 
     #[cfg(all(py_sys_config = "Py_REF_DEBUG", not(Py_3_10)))]
     {
         return Py_DecRef(op);
     }
 
     #[cfg(any(
-        not(Py_LIMITED_API),
         all(Py_LIMITED_API, not(Py_3_12)),
-        all(py_sys_config = "Py_REF_DEBUG", Py_3_12, not(Py_LIMITED_API))
+        all(
+            not(Py_LIMITED_API),
+            any(
+                not(py_sys_config = "Py_REF_DEBUG"),
+                all(py_sys_config = "Py_REF_DEBUG", Py_3_12),
+            )
+        ),
     ))]
     {
         #[cfg(Py_3_12)]
         if _Py_IsImmortal(op) != 0 {
             return;
         }
 
         // Skipped _Py_DECREF_STAT_INC - if anyone needs this, please file an issue
         // or submit a PR supporting Py_STATS build option and pystats.h
 
         #[cfg(all(py_sys_config = "Py_REF_DEBUG", Py_3_12))]
-        _Py_DEC_REFTOTAL();
+        _Py_DECREF_DecRefTotal();
 
         #[cfg(Py_3_12)]
         {
             (*op).ob_refcnt.ob_refcnt -= 1;
 
             #[cfg(py_sys_config = "Py_REF_DEBUG")]
             if (*op).ob_refcnt.ob_refcnt < 0 {
                 let location = std::panic::Location::caller();
-                _Py_NegativeRefcount(location.file(), location.line(), op);
+                let filename = std::ffi::CString::new(location.file()).unwrap();
+                _Py_NegativeRefcount(filename.as_ptr(), location.line() as i32, op);
             }
 
             if (*op).ob_refcnt.ob_refcnt == 0 {
                 _Py_Dealloc(op);
             }
         }
 
@@ -664,15 +671,15 @@
 extern "C" {
     #[cfg_attr(PyPy, link_name = "_PyPy_NoneStruct")]
     static mut _Py_NoneStruct: PyObject;
 }
 
 #[inline]
 pub unsafe fn Py_None() -> *mut PyObject {
-    addr_of_mut_shim!(_Py_NoneStruct)
+    ptr::addr_of_mut!(_Py_NoneStruct)
 }
 
 #[inline]
 pub unsafe fn Py_IsNone(x: *mut PyObject) -> c_int {
     Py_Is(x, Py_None())
 }
 
@@ -682,15 +689,15 @@
 extern "C" {
     #[cfg_attr(PyPy, link_name = "_PyPy_NotImplementedStruct")]
     static mut _Py_NotImplementedStruct: PyObject;
 }
 
 #[inline]
 pub unsafe fn Py_NotImplemented() -> *mut PyObject {
-    addr_of_mut_shim!(_Py_NotImplementedStruct)
+    ptr::addr_of_mut!(_Py_NotImplementedStruct)
 }
 
 // skipped Py_RETURN_NOTIMPLEMENTED
 
 /* Rich comparison opcodes */
 pub const Py_LT: c_int = 0;
 pub const Py_LE: c_int = 1;
@@ -730,9 +737,9 @@
 #[inline]
 pub unsafe fn PyType_Check(op: *mut PyObject) -> c_int {
     PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_TYPE_SUBCLASS)
 }
 
 #[inline]
 pub unsafe fn PyType_CheckExact(op: *mut PyObject) -> c_int {
-    Py_IS_TYPE(op, addr_of_mut_shim!(PyType_Type))
+    Py_IS_TYPE(op, ptr::addr_of_mut!(PyType_Type))
 }
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/objimpl.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/setobject.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,115 +1,150 @@
 use crate::object::*;
+#[cfg(not(any(Py_LIMITED_API, PyPy)))]
+use crate::pyport::Py_hash_t;
 use crate::pyport::Py_ssize_t;
-use libc::size_t;
-use std::os::raw::{c_int, c_void};
+use std::os::raw::c_int;
+use std::ptr::addr_of_mut;
 
-extern "C" {
-    #[cfg_attr(PyPy, link_name = "PyPyObject_Malloc")]
-    pub fn PyObject_Malloc(size: size_t) -> *mut c_void;
-    pub fn PyObject_Calloc(nelem: size_t, elsize: size_t) -> *mut c_void;
-    #[cfg_attr(PyPy, link_name = "PyPyObject_Realloc")]
-    pub fn PyObject_Realloc(ptr: *mut c_void, new_size: size_t) -> *mut c_void;
-    #[cfg_attr(PyPy, link_name = "PyPyObject_Free")]
-    pub fn PyObject_Free(ptr: *mut c_void);
+pub const PySet_MINSIZE: usize = 8;
 
-    #[cfg(not(Py_LIMITED_API))]
-    pub fn _Py_GetAllocatedBlocks() -> Py_ssize_t;
-    #[cfg_attr(PyPy, link_name = "PyPyObject_Init")]
-    pub fn PyObject_Init(arg1: *mut PyObject, arg2: *mut PyTypeObject) -> *mut PyObject;
-    #[cfg_attr(PyPy, link_name = "PyPyObject_InitVar")]
-    pub fn PyObject_InitVar(
-        arg1: *mut PyVarObject,
-        arg2: *mut PyTypeObject,
-        arg3: Py_ssize_t,
-    ) -> *mut PyVarObject;
-    #[cfg_attr(PyPy, link_name = "_PyPyObject_New")]
-    pub fn _PyObject_New(arg1: *mut PyTypeObject) -> *mut PyObject;
-    #[cfg_attr(PyPy, link_name = "_PyPyObject_NewVar")]
-    pub fn _PyObject_NewVar(arg1: *mut PyTypeObject, arg2: Py_ssize_t) -> *mut PyVarObject;
-
-    pub fn PyGC_Collect() -> Py_ssize_t;
-
-    #[cfg(Py_3_10)]
-    #[cfg_attr(PyPy, link_name = "PyPyGC_Enable")]
-    pub fn PyGC_Enable() -> c_int;
-
-    #[cfg(Py_3_10)]
-    #[cfg_attr(PyPy, link_name = "PyPyGC_Disable")]
-    pub fn PyGC_Disable() -> c_int;
-
-    #[cfg(Py_3_10)]
-    #[cfg_attr(PyPy, link_name = "PyPyGC_IsEnabled")]
-    pub fn PyGC_IsEnabled() -> c_int;
+#[cfg(not(any(Py_LIMITED_API, PyPy)))]
+#[repr(C)]
+#[derive(Debug)]
+pub struct setentry {
+    pub key: *mut PyObject,
+    pub hash: Py_hash_t,
 }
 
 #[cfg(not(any(Py_LIMITED_API, PyPy)))]
 #[repr(C)]
-#[derive(Copy, Clone)]
-pub struct PyObjectArenaAllocator {
-    pub ctx: *mut c_void,
-    pub alloc: Option<extern "C" fn(ctx: *mut c_void, size: size_t) -> *mut c_void>,
-    pub free: Option<extern "C" fn(ctx: *mut c_void, ptr: *mut c_void, size: size_t)>,
+#[derive(Debug)]
+pub struct PySetObject {
+    pub ob_base: PyObject,
+    pub fill: Py_ssize_t,
+    pub used: Py_ssize_t,
+    pub mask: Py_ssize_t,
+    pub table: *mut setentry,
+    pub hash: Py_hash_t,
+    pub finger: Py_ssize_t,
+    pub smalltable: [setentry; PySet_MINSIZE],
+    pub weakreflist: *mut PyObject,
 }
 
-#[cfg(not(any(Py_LIMITED_API, PyPy)))]
-impl Default for PyObjectArenaAllocator {
-    #[inline]
-    fn default() -> Self {
-        unsafe { std::mem::zeroed() }
-    }
+// skipped
+#[inline]
+#[cfg(all(not(PyPy), not(Py_LIMITED_API)))]
+pub unsafe fn PySet_GET_SIZE(so: *mut PyObject) -> Py_ssize_t {
+    debug_assert_eq!(PyAnySet_Check(so), 1);
+    let so = so.cast::<PySetObject>();
+    (*so).used
+}
+
+#[cfg(not(Py_LIMITED_API))]
+#[cfg_attr(windows, link(name = "pythonXY"))]
+extern "C" {
+    pub static mut _PySet_Dummy: *mut PyObject;
 }
 
 extern "C" {
-    #[cfg(not(any(Py_LIMITED_API, PyPy)))]
-    pub fn PyObject_GetArenaAllocator(allocator: *mut PyObjectArenaAllocator);
-    #[cfg(not(any(Py_LIMITED_API, PyPy)))]
-    pub fn PyObject_SetArenaAllocator(allocator: *mut PyObjectArenaAllocator);
+    #[cfg(not(Py_LIMITED_API))]
+    #[cfg_attr(PyPy, link_name = "_PyPySet_NextEntry")]
+    pub fn _PySet_NextEntry(
+        set: *mut PyObject,
+        pos: *mut Py_ssize_t,
+        key: *mut *mut PyObject,
+        hash: *mut super::Py_hash_t,
+    ) -> c_int;
+
+    // skipped non-limited _PySet_Update
+}
+
+#[cfg_attr(windows, link(name = "pythonXY"))]
+extern "C" {
+    #[cfg_attr(PyPy, link_name = "PyPySet_Type")]
+    pub static mut PySet_Type: PyTypeObject;
+    #[cfg_attr(PyPy, link_name = "PyPyFrozenSet_Type")]
+    pub static mut PyFrozenSet_Type: PyTypeObject;
+    pub static mut PySetIter_Type: PyTypeObject;
+}
+
+extern "C" {
+    #[cfg_attr(PyPy, link_name = "PyPySet_New")]
+    pub fn PySet_New(arg1: *mut PyObject) -> *mut PyObject;
+    #[cfg_attr(PyPy, link_name = "PyPyFrozenSet_New")]
+    pub fn PyFrozenSet_New(arg1: *mut PyObject) -> *mut PyObject;
+
+    #[cfg_attr(PyPy, link_name = "PyPySet_Add")]
+    pub fn PySet_Add(set: *mut PyObject, key: *mut PyObject) -> c_int;
+    #[cfg_attr(PyPy, link_name = "PyPySet_Clear")]
+    pub fn PySet_Clear(set: *mut PyObject) -> c_int;
+    #[cfg_attr(PyPy, link_name = "PyPySet_Contains")]
+    pub fn PySet_Contains(anyset: *mut PyObject, key: *mut PyObject) -> c_int;
+    #[cfg_attr(PyPy, link_name = "PyPySet_Discard")]
+    pub fn PySet_Discard(set: *mut PyObject, key: *mut PyObject) -> c_int;
+    #[cfg_attr(PyPy, link_name = "PyPySet_Pop")]
+    pub fn PySet_Pop(set: *mut PyObject) -> *mut PyObject;
+    #[cfg_attr(PyPy, link_name = "PyPySet_Size")]
+    pub fn PySet_Size(anyset: *mut PyObject) -> Py_ssize_t;
+
+    #[cfg(PyPy)]
+    #[link_name = "PyPyFrozenSet_CheckExact"]
+    pub fn PyFrozenSet_CheckExact(ob: *mut PyObject) -> c_int;
 }
 
-/// Test if a type has a GC head
 #[inline]
-pub unsafe fn PyType_IS_GC(t: *mut PyTypeObject) -> c_int {
-    PyType_HasFeature(t, Py_TPFLAGS_HAVE_GC)
+#[cfg(not(PyPy))]
+pub unsafe fn PyFrozenSet_CheckExact(ob: *mut PyObject) -> c_int {
+    (Py_TYPE(ob) == addr_of_mut!(PyFrozenSet_Type)) as c_int
+}
+
+extern "C" {
+    #[cfg(PyPy)]
+    #[link_name = "PyPyFrozenSet_Check"]
+    pub fn PyFrozenSet_Check(ob: *mut PyObject) -> c_int;
 }
 
-/// Test if an object has a GC head
 #[inline]
-#[cfg(not(Py_LIMITED_API))]
-pub unsafe fn PyObject_IS_GC(o: *mut PyObject) -> c_int {
-    (PyType_IS_GC(Py_TYPE(o)) != 0
-        && match (*Py_TYPE(o)).tp_is_gc {
-            Some(tp_is_gc) => tp_is_gc(o) != 0,
-            None => true,
-        }) as c_int
+#[cfg(not(PyPy))]
+pub unsafe fn PyFrozenSet_Check(ob: *mut PyObject) -> c_int {
+    (Py_TYPE(ob) == addr_of_mut!(PyFrozenSet_Type)
+        || PyType_IsSubtype(Py_TYPE(ob), addr_of_mut!(PyFrozenSet_Type)) != 0) as c_int
 }
 
 extern "C" {
-    pub fn _PyObject_GC_Resize(arg1: *mut PyVarObject, arg2: Py_ssize_t) -> *mut PyVarObject;
+    #[cfg(PyPy)]
+    #[link_name = "PyPyAnySet_CheckExact"]
+    pub fn PyAnySet_CheckExact(ob: *mut PyObject) -> c_int;
+}
 
-    #[cfg(not(Py_LIMITED_API))]
-    pub fn _PyObject_GC_Malloc(size: size_t) -> *mut PyObject;
-    #[cfg(not(Py_LIMITED_API))]
-    pub fn _PyObject_GC_Calloc(size: size_t) -> *mut PyObject;
-    #[cfg_attr(PyPy, link_name = "_PyPyObject_GC_New")]
-    pub fn _PyObject_GC_New(arg1: *mut PyTypeObject) -> *mut PyObject;
-    #[cfg_attr(PyPy, link_name = "_PyPyObject_GC_NewVar")]
-    pub fn _PyObject_GC_NewVar(arg1: *mut PyTypeObject, arg2: Py_ssize_t) -> *mut PyVarObject;
-    pub fn PyObject_GC_Track(arg1: *mut c_void);
-    pub fn PyObject_GC_UnTrack(arg1: *mut c_void);
-    #[cfg_attr(PyPy, link_name = "PyPyObject_GC_Del")]
-    pub fn PyObject_GC_Del(arg1: *mut c_void);
+#[inline]
+#[cfg(not(PyPy))]
+pub unsafe fn PyAnySet_CheckExact(ob: *mut PyObject) -> c_int {
+    (Py_TYPE(ob) == addr_of_mut!(PySet_Type) || Py_TYPE(ob) == addr_of_mut!(PyFrozenSet_Type))
+        as c_int
 }
 
-/// Test if a type supports weak references
 #[inline]
-#[cfg(not(Py_LIMITED_API))]
-pub unsafe fn PyType_SUPPORTS_WEAKREFS(t: *mut PyTypeObject) -> c_int {
-    ((*t).tp_weaklistoffset > 0) as c_int
+pub unsafe fn PyAnySet_Check(ob: *mut PyObject) -> c_int {
+    (PyAnySet_CheckExact(ob) != 0
+        || PyType_IsSubtype(Py_TYPE(ob), addr_of_mut!(PySet_Type)) != 0
+        || PyType_IsSubtype(Py_TYPE(ob), addr_of_mut!(PyFrozenSet_Type)) != 0) as c_int
 }
 
 #[inline]
-#[cfg(not(Py_LIMITED_API))]
-pub unsafe fn PyObject_GET_WEAKREFS_LISTPTR(o: *mut PyObject) -> *mut *mut PyObject {
-    let weaklistoffset = (*Py_TYPE(o)).tp_weaklistoffset;
-    o.offset(weaklistoffset) as *mut *mut PyObject
+#[cfg(Py_3_10)]
+pub unsafe fn PySet_CheckExact(op: *mut PyObject) -> c_int {
+    crate::Py_IS_TYPE(op, addr_of_mut!(PySet_Type))
+}
+
+extern "C" {
+    #[cfg(PyPy)]
+    #[link_name = "PyPySet_Check"]
+    pub fn PySet_Check(ob: *mut PyObject) -> c_int;
+}
+
+#[inline]
+#[cfg(not(PyPy))]
+pub unsafe fn PySet_Check(ob: *mut PyObject) -> c_int {
+    (Py_TYPE(ob) == addr_of_mut!(PySet_Type)
+        || PyType_IsSubtype(Py_TYPE(ob), addr_of_mut!(PySet_Type)) != 0) as c_int
 }
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pybuffer.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pybuffer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pycapsule.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pycapsule.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 use crate::object::*;
 use std::os::raw::{c_char, c_int, c_void};
+use std::ptr::addr_of_mut;
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyCapsule_Type")]
     pub static mut PyCapsule_Type: PyTypeObject;
 }
 
 pub type PyCapsule_Destructor = unsafe extern "C" fn(o: *mut PyObject);
 
 #[inline]
 pub unsafe fn PyCapsule_CheckExact(ob: *mut PyObject) -> c_int {
-    (Py_TYPE(ob) == addr_of_mut_shim!(PyCapsule_Type)) as c_int
+    (Py_TYPE(ob) == addr_of_mut!(PyCapsule_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyCapsule_New")]
     pub fn PyCapsule_New(
         pointer: *mut c_void,
         name: *const c_char,
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pyerrors.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pyerrors.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pyhash.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pyhash.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pylifecycle.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pylifecycle.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pyport.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pyport.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pystate.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pystate.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pystrtod.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pystrtod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/pythonrun.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/pythonrun.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/sliceobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/sliceobject.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 use std::os::raw::c_int;
+use std::ptr::addr_of_mut;
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "_PyPy_EllipsisObject")]
     static mut _Py_EllipsisObject: PyObject;
 }
 
 #[inline]
 pub unsafe fn Py_Ellipsis() -> *mut PyObject {
-    addr_of_mut_shim!(_Py_EllipsisObject)
+    addr_of_mut!(_Py_EllipsisObject)
 }
 
 #[cfg(not(Py_LIMITED_API))]
 #[repr(C)]
 pub struct PySliceObject {
     pub ob_base: PyObject,
     pub start: *mut PyObject,
@@ -27,15 +28,15 @@
     #[cfg_attr(PyPy, link_name = "PyPySlice_Type")]
     pub static mut PySlice_Type: PyTypeObject;
     pub static mut PyEllipsis_Type: PyTypeObject;
 }
 
 #[inline]
 pub unsafe fn PySlice_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PySlice_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PySlice_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPySlice_New")]
     pub fn PySlice_New(
         start: *mut PyObject,
         stop: *mut PyObject,
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/structseq.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/structseq.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/sysmodule.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/sysmodule.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/traceback.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/traceback.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 use crate::object::*;
 use std::os::raw::c_int;
+#[cfg(not(PyPy))]
+use std::ptr::addr_of_mut;
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyTraceBack_Here")]
     pub fn PyTraceBack_Here(arg1: *mut crate::PyFrameObject) -> c_int;
     #[cfg_attr(PyPy, link_name = "PyPyTraceBack_Print")]
     pub fn PyTraceBack_Print(arg1: *mut PyObject, arg2: *mut PyObject) -> c_int;
 }
@@ -17,9 +19,9 @@
     #[link_name = "PyPyTraceBack_Check"]
     pub fn PyTraceBack_Check(op: *mut PyObject) -> c_int;
 }
 
 #[inline]
 #[cfg(not(PyPy))]
 pub unsafe fn PyTraceBack_Check(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyTraceBack_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyTraceBack_Type)) as c_int
 }
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/tupleobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/tupleobject.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 use std::os::raw::c_int;
+use std::ptr::addr_of_mut;
 
 #[cfg_attr(windows, link(name = "pythonXY"))]
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyTuple_Type")]
     pub static mut PyTuple_Type: PyTypeObject;
     pub static mut PyTupleIter_Type: PyTypeObject;
 }
@@ -12,15 +13,15 @@
 #[inline]
 pub unsafe fn PyTuple_Check(op: *mut PyObject) -> c_int {
     PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_TUPLE_SUBCLASS)
 }
 
 #[inline]
 pub unsafe fn PyTuple_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyTuple_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyTuple_Type)) as c_int
 }
 
 extern "C" {
     #[cfg_attr(PyPy, link_name = "PyPyTuple_New")]
     pub fn PyTuple_New(size: Py_ssize_t) -> *mut PyObject;
     #[cfg_attr(PyPy, link_name = "PyPyTuple_Size")]
     pub fn PyTuple_Size(arg1: *mut PyObject) -> Py_ssize_t;
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/typeslots.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/typeslots.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/unicodeobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/unicodeobject.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use crate::object::*;
 use crate::pyport::Py_ssize_t;
 use libc::wchar_t;
 use std::os::raw::{c_char, c_int, c_void};
+#[cfg(not(PyPy))]
+use std::ptr::addr_of_mut;
 
 #[cfg(not(Py_LIMITED_API))]
 pub type Py_UNICODE = wchar_t;
 
 pub type Py_UCS4 = u32;
 pub type Py_UCS2 = u16;
 pub type Py_UCS1 = u8;
@@ -30,15 +32,15 @@
 pub unsafe fn PyUnicode_Check(op: *mut PyObject) -> c_int {
     PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_UNICODE_SUBCLASS)
 }
 
 #[inline]
 #[cfg(not(PyPy))]
 pub unsafe fn PyUnicode_CheckExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(PyUnicode_Type)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(PyUnicode_Type)) as c_int
 }
 
 pub const Py_UNICODE_REPLACEMENT_CHARACTER: Py_UCS4 = 0xFFFD;
 
 extern "C" {
 
     #[cfg_attr(PyPy, link_name = "PyPyUnicode_FromStringAndSize")]
```

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/warnings.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/warnings.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/pyo3-ffi-0.19.2/src/weakrefobject.rs` & `orjson-3.9.9/include/cargo/pyo3-ffi-0.20.0/src/weakrefobject.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 use crate::object::*;
 use std::os::raw::c_int;
+#[cfg(not(PyPy))]
+use std::ptr::addr_of_mut;
 
 #[cfg(all(not(PyPy), Py_LIMITED_API))]
 opaque_struct!(PyWeakReference);
 
 #[cfg(all(not(PyPy), not(Py_LIMITED_API)))]
 pub use crate::_PyWeakReference as PyWeakReference;
 
@@ -25,28 +27,28 @@
     #[link_name = "PyPyWeakref_CheckProxy"]
     pub fn PyWeakref_CheckProxy(op: *mut PyObject) -> c_int;
 }
 
 #[inline]
 #[cfg(not(PyPy))]
 pub unsafe fn PyWeakref_CheckRef(op: *mut PyObject) -> c_int {
-    PyObject_TypeCheck(op, addr_of_mut_shim!(_PyWeakref_RefType))
+    PyObject_TypeCheck(op, addr_of_mut!(_PyWeakref_RefType))
 }
 
 #[inline]
 #[cfg(not(PyPy))]
 pub unsafe fn PyWeakref_CheckRefExact(op: *mut PyObject) -> c_int {
-    (Py_TYPE(op) == addr_of_mut_shim!(_PyWeakref_RefType)) as c_int
+    (Py_TYPE(op) == addr_of_mut!(_PyWeakref_RefType)) as c_int
 }
 
 #[inline]
 #[cfg(not(PyPy))]
 pub unsafe fn PyWeakref_CheckProxy(op: *mut PyObject) -> c_int {
-    ((Py_TYPE(op) == addr_of_mut_shim!(_PyWeakref_ProxyType))
-        || (Py_TYPE(op) == addr_of_mut_shim!(_PyWeakref_CallableProxyType))) as c_int
+    ((Py_TYPE(op) == addr_of_mut!(_PyWeakref_ProxyType))
+        || (Py_TYPE(op) == addr_of_mut!(_PyWeakref_CallableProxyType))) as c_int
 }
 
 #[inline]
 pub unsafe fn PyWeakref_Check(op: *mut PyObject) -> c_int {
     (PyWeakref_CheckRef(op) != 0 || PyWeakref_CheckProxy(op) != 0) as c_int
 }
```

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/quote-1.0.33/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/Cargo.toml` & `orjson-3.9.9/include/cargo/quote-1.0.33/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/quote-1.0.33/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/LICENSE-MIT` & `orjson-3.9.9/include/cargo/quote-1.0.33/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/README.md` & `orjson-3.9.9/include/cargo/quote-1.0.33/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/src/ext.rs` & `orjson-3.9.9/include/cargo/quote-1.0.33/src/ext.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/src/format.rs` & `orjson-3.9.9/include/cargo/quote-1.0.33/src/format.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/src/ident_fragment.rs` & `orjson-3.9.9/include/cargo/quote-1.0.33/src/ident_fragment.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/src/lib.rs` & `orjson-3.9.9/include/cargo/quote-1.0.33/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/src/runtime.rs` & `orjson-3.9.9/include/cargo/quote-1.0.33/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/src/spanned.rs` & `orjson-3.9.9/include/cargo/quote-1.0.33/src/spanned.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/src/to_tokens.rs` & `orjson-3.9.9/include/cargo/quote-1.0.33/src/to_tokens.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/tests/test.rs` & `orjson-3.9.9/include/cargo/quote-1.0.33/tests/test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated-dup.stderr` & `orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated-dup.stderr`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated.stderr` & `orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/does-not-have-iter-interpolated.stderr`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/not-quotable.stderr` & `orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/not-quotable.stderr`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/quote-1.0.33/tests/ui/not-repeatable.stderr` & `orjson-3.9.9/include/cargo/quote-1.0.33/tests/ui/not-repeatable.stderr`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/Cargo.toml` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/LICENSE-MIT` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/README.md` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/build/build.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/build/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/build/rustc.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/build/rustc.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/attr.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/attr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/bound.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/bound.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/constfn.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/constfn.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/date.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/date.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/error.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/expand.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/expand.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/expr.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/expr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/iter.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/iter.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/lib.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/release.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/release.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/time.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/time.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/src/token.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/src/token.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/test_const.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/test_const.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/rustversion-1.0.14/tests/test_parse.rs` & `orjson-3.9.9/include/cargo/rustversion-1.0.14/tests/test_parse.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/ryu-1.0.15/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/Cargo.lock` & `orjson-3.9.9/include/cargo/ryu-1.0.15/Cargo.lock`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/Cargo.toml` & `orjson-3.9.9/include/cargo/ryu-1.0.15/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/ryu-1.0.15/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/LICENSE-BOOST` & `orjson-3.9.9/include/cargo/ryu-1.0.15/LICENSE-BOOST`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/README.md` & `orjson-3.9.9/include/cargo/ryu-1.0.15/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/benches/bench.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/examples/upstream_benchmark.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/examples/upstream_benchmark.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/buffer/mod.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/buffer/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/common.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/common.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/d2s.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/d2s.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/d2s_full_table.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/d2s_full_table.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/d2s_intrinsics.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/d2s_intrinsics.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/d2s_small_table.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/d2s_small_table.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/digit_table.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/digit_table.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/f2s.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/f2s.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/f2s_intrinsics.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/f2s_intrinsics.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/lib.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/pretty/exponent.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/pretty/exponent.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/pretty/mantissa.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/pretty/mantissa.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/pretty/mod.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/pretty/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/s2d.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/s2d.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/src/s2f.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/src/s2f.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/tests/common_test.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/tests/common_test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/tests/d2s_table_test.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/tests/d2s_table_test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/tests/d2s_test.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/tests/d2s_test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/tests/exhaustive.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/tests/exhaustive.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/tests/f2s_test.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/tests/f2s_test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/tests/s2d_test.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/tests/s2d_test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/ryu-1.0.15/tests/s2f_test.rs` & `orjson-3.9.9/include/cargo/ryu-1.0.15/tests/s2f_test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/serde-1.0.188/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/Cargo.toml` & `orjson-3.9.9/include/cargo/serde-1.0.188/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/serde-1.0.188/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/LICENSE-MIT` & `orjson-3.9.9/include/cargo/serde-1.0.188/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/README.md` & `orjson-3.9.9/include/cargo/serde-1.0.188/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/build.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/crates-io.md` & `orjson-3.9.9/include/cargo/serde-1.0.188/crates-io.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/de/format.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/de/format.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/de/ignored_any.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/de/ignored_any.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/de/impls.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/de/impls.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/de/mod.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/de/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/de/seed.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/de/seed.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/de/size_hint.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/de/size_hint.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/de/value.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/de/value.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/lib.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/macros.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/private/de.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/private/de.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/private/doc.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/private/doc.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/private/mod.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/private/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/private/ser.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/private/ser.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/ser/fmt.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/ser/fmt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/ser/impls.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/ser/impls.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/ser/impossible.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/ser/impossible.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/ser/mod.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/ser/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde-1.0.188/src/std_error.rs` & `orjson-3.9.9/include/cargo/serde-1.0.188/src/std_error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/Cargo.toml` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/LICENSE-MIT` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/README.md` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/crates-io.md` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/crates-io.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/bound.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/bound.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/de.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/de.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/dummy.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/dummy.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/fragment.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/fragment.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/ast.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/ast.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/attr.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/attr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/case.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/case.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/check.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/check.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/ctxt.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/ctxt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/receiver.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/receiver.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/internals/symbol.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/internals/symbol.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/lib.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/pretend.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/pretend.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/ser.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/ser.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_derive-1.0.188/src/this.rs` & `orjson-3.9.9/include/cargo/serde_derive-1.0.188/src/this.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/CONTRIBUTING.md` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/Cargo.toml` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/LICENSE-MIT` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/README.md` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/build.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/de.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/de.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/error.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/io/core.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/io/core.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/io/mod.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/io/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/iter.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/iter.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/algorithm.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/algorithm.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/bhcomp.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/bhcomp.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/bignum.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/bignum.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/cached.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/cached.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/cached_float80.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/cached_float80.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/errors.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/errors.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/exponent.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/exponent.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/float.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/float.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/large_powers32.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/large_powers32.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/large_powers64.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/large_powers64.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/math.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/math.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/mod.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/num.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/num.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/parse.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/parse.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/rounding.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/rounding.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/shift.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/shift.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lexical/small_powers.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lexical/small_powers.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/lib.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/macros.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/map.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/map.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/number.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/number.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/raw.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/raw.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/read.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/read.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/ser.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/ser.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/de.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/de.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/from.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/from.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/index.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/index.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/mod.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/partial_eq.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/partial_eq.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/src/value/ser.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/src/value/ser.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/debug.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/debug.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/algorithm.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/algorithm.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/exponent.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/exponent.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/float.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/float.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/math.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/math.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/num.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/num.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/parse.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/parse.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical/rounding.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical/rounding.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/lexical.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/lexical.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/macros/mod.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/macros/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/map.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/map.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/regression/issue795.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/regression/issue795.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/regression/issue845.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/regression/issue845.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/stream.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/stream.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/serde_json-1.0.107/tests/test.rs` & `orjson-3.9.9/include/cargo/serde_json-1.0.107/tests/test.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/CHANGELOG.md` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/Cargo.toml` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/LICENSE-Apache` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/LICENSE-Apache`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/LICENSE-MIT` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/README.md` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/examples/streaming.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/examples/streaming.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/release.toml` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/release.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/basic.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/basic.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/compat.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/compat.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/aarch64/mod.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/aarch64/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/aarch64/neon.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/aarch64/neon.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/algorithm.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/algorithm.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/helpers.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/helpers.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/mod.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/wasm32/mod.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/wasm32/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/wasm32/simd128.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/wasm32/simd128.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/x86/avx2.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/x86/avx2.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/x86/mod.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/x86/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/implementation/x86/sse42.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/implementation/x86/sse42.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/src/lib.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/tests/tests.rs` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/tests/tests.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/simdutf8-0.1.4/wasm32-development.md` & `orjson-3.9.9/include/cargo/simdutf8-0.1.4/wasm32-development.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/Cargo.toml` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/LICENSE-MIT` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/README.md` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/benches/bench.rs` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/debug_metadata/README.md` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/debug_metadata/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/debug_metadata/smallvec.natvis` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/debug_metadata/smallvec.natvis`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/scripts/run_miri.sh` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/scripts/run_miri.sh`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/src/arbitrary.rs` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/src/arbitrary.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/src/lib.rs` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/src/specialization.rs` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/src/specialization.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/src/tests.rs` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/src/tests.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/tests/debugger_visualizer.rs` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/tests/debugger_visualizer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/smallvec-1.11.1/tests/macro.rs` & `orjson-3.9.9/include/cargo/smallvec-1.11.1/tests/macro.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/CHANGELOG.md` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/Cargo.toml` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/LICENSE-MIT` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/README.md` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_cfg.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_cfg.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_eq_align.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_eq_align.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_eq_size.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_eq_size.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_fields.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_fields.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_impl.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_impl.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_obj_safe.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_obj_safe.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_trait.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_trait.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/assert_type.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/assert_type.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/const_assert.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/const_assert.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/static_assertions-1.1.0/src/lib.rs` & `orjson-3.9.9/include/cargo/static_assertions-1.1.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/syn-2.0.38/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/Cargo.toml` & `orjson-3.9.9/include/cargo/syn-2.0.38/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/syn-2.0.38/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/LICENSE-MIT` & `orjson-3.9.9/include/cargo/syn-2.0.38/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/README.md` & `orjson-3.9.9/include/cargo/syn-2.0.38/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/benches/file.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/benches/file.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/benches/rust.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/benches/rust.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/attr.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/attr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/bigint.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/bigint.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/buffer.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/buffer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/custom_keyword.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/custom_keyword.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/custom_punctuation.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/custom_punctuation.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/data.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/data.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/derive.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/derive.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/discouraged.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/discouraged.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/drops.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/drops.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/error.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/export.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/export.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/expr.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/expr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/ext.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/ext.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/file.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/file.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/clone.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/clone.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/debug.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/debug.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/eq.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/eq.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/fold.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/fold.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/hash.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/hash.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/visit.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/visit.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/gen/visit_mut.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/gen/visit_mut.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/gen_helper.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/gen_helper.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/generics.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/generics.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/group.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/group.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/ident.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/ident.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/item.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/item.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/lib.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/lifetime.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/lifetime.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/lit.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/lit.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/lookahead.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/lookahead.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/mac.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/mac.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/macros.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/macros.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/meta.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/meta.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/op.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/op.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/parse.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/parse.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/parse_macro_input.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/parse_macro_input.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/parse_quote.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/parse_quote.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/pat.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/pat.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/path.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/path.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/punctuated.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/punctuated.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/restriction.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/restriction.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/span.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/span.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/spanned.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/spanned.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/stmt.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/stmt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/thread.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/thread.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/token.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/token.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/tt.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/tt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/ty.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/ty.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/verbatim.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/verbatim.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/src/whitespace.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/src/whitespace.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/common/eq.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/common/eq.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/common/mod.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/common/parse.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/common/parse.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/debug/gen.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/debug/gen.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/debug/mod.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/debug/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/macros/mod.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/macros/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/regression/issue1235.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/regression/issue1235.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/repo/mod.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/repo/mod.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/repo/progress.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/repo/progress.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_asyncness.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_asyncness.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_attribute.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_attribute.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_derive_input.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_derive_input.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_expr.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_expr.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_generics.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_generics.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_grouping.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_grouping.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_ident.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_ident.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_item.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_item.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_iterators.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_iterators.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_lit.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_lit.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_meta.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_meta.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_parse_buffer.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_parse_buffer.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_pat.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_pat.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_path.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_path.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_precedence.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_precedence.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_receiver.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_receiver.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_round_trip.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_round_trip.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_shebang.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_shebang.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_should_parse.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_should_parse.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_size.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_size.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_stmt.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_stmt.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_token_trees.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_token_trees.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_ty.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_ty.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/test_visibility.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/test_visibility.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/syn-2.0.38/tests/zzz_stable.rs` & `orjson-3.9.9/include/cargo/syn-2.0.38/tests/zzz_stable.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/Cargo.lock` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/Cargo.lock`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/Cargo.toml` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/LICENSE` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/LICENSE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/README.md` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/build.rs` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/build.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/data_model.rs` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/data_model.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/host.rs` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/host.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/lib.rs` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/parse_error.rs` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/parse_error.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/targets.rs` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/targets.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/target-lexicon-0.12.11/src/triple.rs` & `orjson-3.9.9/include/cargo/target-lexicon-0.12.11/src/triple.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/Cargo.toml` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/LICENSE-MIT` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/LICENSE-UNICODE` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/LICENSE-UNICODE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/README.md` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/benches/xid.rs` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/benches/xid.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/src/lib.rs` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/src/tables.rs` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/src/tables.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/compare.rs` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/compare.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/fst/xid_continue.fst` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/fst/xid_continue.fst`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/fst/xid_start.fst` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/fst/xid_start.fst`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/static_size.rs` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/static_size.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/tables/tables.rs` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/tables/tables.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/unicode-ident-1.0.12/tests/trie/trie.rs` & `orjson-3.9.9/include/cargo/unicode-ident-1.0.12/tests/trie/trie.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/version_check-0.9.4/.cargo-checksum.json` & `orjson-3.9.9/include/cargo/version_check-0.9.4/.cargo-checksum.json`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/version_check-0.9.4/Cargo.toml` & `orjson-3.9.9/include/cargo/version_check-0.9.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/version_check-0.9.4/LICENSE-APACHE` & `orjson-3.9.9/include/cargo/version_check-0.9.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/version_check-0.9.4/LICENSE-MIT` & `orjson-3.9.9/include/cargo/version_check-0.9.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/version_check-0.9.4/README.md` & `orjson-3.9.9/include/cargo/version_check-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/version_check-0.9.4/src/channel.rs` & `orjson-3.9.9/include/cargo/version_check-0.9.4/src/channel.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/version_check-0.9.4/src/date.rs` & `orjson-3.9.9/include/cargo/version_check-0.9.4/src/date.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/version_check-0.9.4/src/lib.rs` & `orjson-3.9.9/include/cargo/version_check-0.9.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/include/cargo/version_check-0.9.4/src/version.rs` & `orjson-3.9.9/include/cargo/version_check-0.9.4/src/version.rs`

 * *Files identical despite different names*

### Comparing `orjson-3.9.8/PKG-INFO` & `orjson-3.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orjson
-Version: 3.9.8
+Version: 3.9.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -64,15 +64,16 @@
 support for 64-bit
 * does not provide `load()` or `dump()` functions for reading from/writing to
 file-like objects
 
 orjson supports CPython 3.8, 3.9, 3.10, 3.11, and 3.12. It distributes
 amd64/x86_64, aarch64/armv8, arm7, POWER/ppc64le, and s390x wheels for Linux,
 amd64 and aarch64 wheels for macOS, and amd64 and i686/x86 wheels for Windows.
-orjson  does not support PyPy. Releases follow semantic versioning and
+orjson does not and will not support PyPy. orjson does not and will not
+support PEP 554 subinterpreters. Releases follow semantic versioning and
 serializing a new object type without an opt-in flag is considered a
 breaking change.
 
 orjson is licensed under both the Apache 2.0 and MIT licenses. The
 repository and issue tracker is
 [github.com/ijl/orjson](https://github.com/ijl/orjson), and patches may be
 submitted there. There is a
@@ -1206,18 +1207,14 @@
 handle errors etc. This is addressed by data validation libraries a
 level above this.
 
 ### Will it serialize to `str`?
 
 No. `bytes` is the correct type for a serialized blob.
 
-### Will it support PyPy?
-
-Probably not.
-
 ## Packaging
 
 To package orjson requires at least [Rust](https://www.rust-lang.org/) 1.65
 and the [maturin](https://github.com/PyO3/maturin) build tool. The recommended
 build command is:
 
 ```sh
```

