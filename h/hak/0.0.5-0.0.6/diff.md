# Comparing `tmp/hak-0.0.5.tar.gz` & `tmp/hak-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hak-0.0.5.tar", last modified: Wed Apr 19 10:09:33 2023, max compression
+gzip compressed data, was "hak-0.0.6.tar", last modified: Wed Apr 19 10:12:37 2023, max compression
```

## Comparing `hak-0.0.5.tar` & `hak-0.0.6.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/
--rw-rw-r--   0 a         (1009) a         (1010)     1068 2023-04-19 01:55:38.000000 hak-0.0.5/LICENSE
--rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:09:33.059331 hak-0.0.5/PKG-INFO
--rw-rw-r--   0 a         (1009) a         (1010)      406 2023-04-19 03:24:53.000000 hak-0.0.5/README.md
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.047330 hak-0.0.5/hak/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      140 2023-04-19 01:55:38.000000 hak-0.0.5/hak/a_equals_b.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/bool/
--rw-rw-r--   0 a         (1009) a         (1010)       86 2023-04-19 01:55:38.000000 hak-0.0.5/hak/bool/fake.py
--rw-rw-r--   0 a         (1009) a         (1010)      103 2023-04-19 01:55:38.000000 hak-0.0.5/hak/bool/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/bool/or_none/
--rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.5/hak/bool/or_none/fake.py
--rw-rw-r--   0 a         (1009) a         (1010)      125 2023-04-19 01:55:38.000000 hak-0.0.5/hak/bool/or_none/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/bools/
--rw-rw-r--   0 a         (1009) a         (1010)      139 2023-04-19 01:55:38.000000 hak-0.0.5/hak/bools/count_true.py
--rw-rw-r--   0 a         (1009) a         (1010)      249 2023-04-19 01:55:38.000000 hak-0.0.5/hak/calculate_duration_bar_width.py
--rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.5/hak/check_if_ok_to_proceed.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/date/
--rw-rw-r--   0 a         (1009) a         (1010)      143 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      347 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/is_first_second_or_third_day_of_month.py
--rw-rw-r--   0 a         (1009) a         (1010)      414 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/is_first_week_of_quarter.py
--rw-rw-r--   0 a         (1009) a         (1010)      208 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/is_monday.py
--rw-rw-r--   0 a         (1009) a         (1010)      462 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/is_weekday.py
--rw-rw-r--   0 a         (1009) a         (1010)      467 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/is_weekend.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/date/public_holiday/
--rw-rw-r--   0 a         (1009) a         (1010)     5617 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/public_holiday/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      385 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/select_from_last_n_days.py
--rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/to_dd_mm_yyyy_str.py
--rw-rw-r--   0 a         (1009) a         (1010)      605 2023-04-19 03:01:25.000000 hak-0.0.5/hak/date/to_utc_timestamp.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.047330 hak-0.0.5/hak/date/year/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/date/year/easter_sunday/
--rw-rw-r--   0 a         (1009) a         (1010)     1006 2023-04-19 01:55:38.000000 hak-0.0.5/hak/date/year/easter_sunday/get.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/datetime/
--rw-rw-r--   0 a         (1009) a         (1010)      149 2023-04-19 01:55:38.000000 hak-0.0.5/hak/datetime/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      272 2023-04-19 01:55:38.000000 hak-0.0.5/hak/datetime/select_from_last_n_days.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/dict/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      215 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/convert_to_sql_insertable.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/dict/frequencies/
--rw-rw-r--   0 a         (1009) a         (1010)      356 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/frequencies/choose.py
--rw-rw-r--   0 a         (1009) a         (1010)      376 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/frequencies/make_from_strings.py
--rw-rw-r--   0 a         (1009) a         (1010)      187 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/get_or_default.py
--rw-rw-r--   0 a         (1009) a         (1010)      190 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/make_from_key_value_lists.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/dict/proposed_dismantlement/
--rw-rw-r--   0 a         (1009) a         (1010)     1520 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/proposed_dismantlement/show.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/dict/test_durations/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/test_durations/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/test_durations/to_tuple_list_sorted_by_duration.py
--rw-rw-r--   0 a         (1009) a         (1010)     4011 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dict/to_max_line_width_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/dicts/
--rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dicts/a_into_b.py
--rw-rw-r--   0 a         (1009) a         (1010)     1200 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dicts/compare.py
--rw-rw-r--   0 a         (1009) a         (1010)      195 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dicts/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      663 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dicts/merge_freq_dicts.py
--rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dicts/reindex.py
--rw-rw-r--   0 a         (1009) a         (1010)      203 2023-04-19 01:55:38.000000 hak-0.0.5/hak/dicts/sort_by_key.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/directories/
--rw-rw-r--   0 a         (1009) a         (1010)      567 2023-04-19 01:55:38.000000 hak-0.0.5/hak/directories/exist.py
--rw-rw-r--   0 a         (1009) a         (1010)      432 2023-04-19 01:55:38.000000 hak-0.0.5/hak/directories/make.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/directory/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/directory/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)     1548 2023-04-19 01:55:38.000000 hak-0.0.5/hak/directory/compress_to_tar.py
--rw-rw-r--   0 a         (1009) a         (1010)      674 2023-04-19 05:28:56.000000 hak-0.0.5/hak/directory/empty.py
--rw-rw-r--   0 a         (1009) a         (1010)       88 2023-04-19 01:55:38.000000 hak-0.0.5/hak/directory/exists.py
--rw-rw-r--   0 a         (1009) a         (1010)     1197 2023-04-19 04:40:12.000000 hak-0.0.5/hak/directory/get_most_recently_modified.py
--rw-rw-r--   0 a         (1009) a         (1010)      650 2023-04-19 01:55:38.000000 hak-0.0.5/hak/directory/is_module.py
--rw-rw-r--   0 a         (1009) a         (1010)      667 2023-04-19 10:09:14.000000 hak-0.0.5/hak/directory/make.py
--rw-rw-r--   0 a         (1009) a         (1010)      782 2023-04-19 01:55:38.000000 hak-0.0.5/hak/directory/remove.py
--rw-rw-r--   0 a         (1009) a         (1010)     3692 2023-04-19 01:55:38.000000 hak-0.0.5/hak/duration.py
--rw-rw-r--   0 a         (1009) a         (1010)     2021 2023-04-19 01:55:38.000000 hak-0.0.5/hak/duration_bar.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/fake/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/fake/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/fake/os/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/fake/os/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      418 2023-04-19 01:55:38.000000 hak-0.0.5/hak/fake/os/system.py
--rw-rw-r--   0 a         (1009) a         (1010)      424 2023-04-19 01:55:38.000000 hak-0.0.5/hak/fake/printer.py
--rw-rw-r--   0 a         (1009) a         (1010)       45 2023-04-19 01:55:38.000000 hak-0.0.5/hak/fake/sleep.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/fake/subprocess/
--rw-rw-r--   0 a         (1009) a         (1010)     5854 2023-04-19 04:41:24.000000 hak-0.0.5/hak/fake/subprocess/run.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/file/
--rw-rw-r--   0 a         (1009) a         (1010)     1253 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      785 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/decrypt.py
--rw-rw-r--   0 a         (1009) a         (1010)      929 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/encrypt.py
--rw-rw-r--   0 a         (1009) a         (1010)      697 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/load.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/file/pickle/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/pickle/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)     1253 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/pickle/load_if_exists.py
--rw-rw-r--   0 a         (1009) a         (1010)      906 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/pickle/save.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/file/py/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/py/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      546 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/py/create.py
--rw-rw-r--   0 a         (1009) a         (1010)     2644 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/py/dismantle.py
--rw-rw-r--   0 a         (1009) a         (1010)     3819 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/py/extract_fn.py
--rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/py/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/remove.py
--rw-rw-r--   0 a         (1009) a         (1010)      956 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/save.py
--rw-rw-r--   0 a         (1009) a         (1010)      761 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/save_lines.py
--rw-rw-r--   0 a         (1009) a         (1010)      308 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/save_lines_or_string.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.047330 hak-0.0.5/hak/file/secret/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/file/secret/password/
--rw-rw-r--   0 a         (1009) a         (1010)      680 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/secret/password/get.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/file/secret/username/
--rw-rw-r--   0 a         (1009) a         (1010)      713 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/secret/username/get.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/file/tar/
--rw-rw-r--   0 a         (1009) a         (1010)     1562 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/tar/extract.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/file/zip/
--rw-rw-r--   0 a         (1009) a         (1010)      487 2023-04-19 01:55:38.000000 hak-0.0.5/hak/file/zip/extract.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.047330 hak-0.0.5/hak/files/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/files/pyfiles/
--rw-rw-r--   0 a         (1009) a         (1010)     1765 2023-04-19 04:43:12.000000 hak-0.0.5/hak/files/pyfiles/dismantle.py
--rw-rw-r--   0 a         (1009) a         (1010)      100 2023-04-19 01:55:38.000000 hak-0.0.5/hak/find_first_parenthesis.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/float/
--rw-rw-r--   0 a         (1009) a         (1010)       70 2023-04-19 01:55:38.000000 hak-0.0.5/hak/float/epsilon.py
--rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.5/hak/float/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.5/hak/float/is_not.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/float/nan/
--rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.5/hak/float/nan/to_none.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/function/
--rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.5/hak/function/function.py
--rw-rw-r--   0 a         (1009) a         (1010)      423 2023-04-19 01:55:38.000000 hak-0.0.5/hak/function/write_to_file.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/int/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/int/days/
--rw-rw-r--   0 a         (1009) a         (1010)      227 2023-04-19 01:55:38.000000 hak-0.0.5/hak/int/days/a_to_b_inclusive.py
--rw-rw-r--   0 a         (1009) a         (1010)      661 2023-04-19 01:55:38.000000 hak-0.0.5/hak/int/get_prime_factorisation.py
--rw-rw-r--   0 a         (1009) a         (1010)      104 2023-04-19 01:55:38.000000 hak-0.0.5/hak/int/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      426 2023-04-19 01:55:38.000000 hak-0.0.5/hak/int/is_prime.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/int/year/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/int/year/days/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/int/year/days/count/
--rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.5/hak/int/year/days/count/get.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/int/year/days/first/
--rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.5/hak/int/year/days/first/get.py
--rw-rw-r--   0 a         (1009) a         (1010)      420 2023-04-19 01:55:38.000000 hak-0.0.5/hak/int/year/days/get.py
--rw-rw-r--   0 a         (1009) a         (1010)      153 2023-04-19 01:55:38.000000 hak-0.0.5/hak/int/year/now.py
--rw-rw-r--   0 a         (1009) a         (1010)      448 2023-04-19 01:55:38.000000 hak-0.0.5/hak/l.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/list/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/list/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.5/hak/list/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/list/strings/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/list/strings/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 04:41:08.000000 hak-0.0.5/hak/list/strings/add_src_funks_prefix.py
--rw-rw-r--   0 a         (1009) a         (1010)      586 2023-04-19 01:55:38.000000 hak-0.0.5/hak/list/strings/compare.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak/list/strings/contain/
--rw-rw-r--   0 a         (1009) a         (1010)      145 2023-04-19 04:43:23.000000 hak-0.0.5/hak/list/strings/contain/version.py
--rw-rw-r--   0 a         (1009) a         (1010)     2222 2023-04-19 04:44:27.000000 hak-0.0.5/hak/list/strings/find_first_diff.py
--rw-rw-r--   0 a         (1009) a         (1010)      434 2023-04-19 04:45:12.000000 hak-0.0.5/hak/list/strings/make_patch_version_change_to_py.py
--rw-rw-r--   0 a         (1009) a         (1010)      293 2023-04-19 04:47:46.000000 hak-0.0.5/hak/list/strings/module_names_from_py_filenames.py
--rw-rw-r--   0 a         (1009) a         (1010)      410 2023-04-19 04:48:58.000000 hak-0.0.5/hak/list/strings/patch_setup_cfg.py
--rw-rw-r--   0 a         (1009) a         (1010)      622 2023-04-19 04:51:45.000000 hak-0.0.5/hak/list/strings/patch_setup_py.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/list/strings/pyfiles/
--rw-rw-r--   0 a         (1009) a         (1010)     1514 2023-04-19 04:52:08.000000 hak-0.0.5/hak/list/strings/pyfiles/filter_out_items.py
--rw-rw-r--   0 a         (1009) a         (1010)      766 2023-04-19 05:00:37.000000 hak-0.0.5/hak/list/strings/show_diff.py
--rw-rw-r--   0 a         (1009) a         (1010)      647 2023-04-19 05:00:56.000000 hak-0.0.5/hak/list/strings/to_dict.py
--rw-rw-r--   0 a         (1009) a         (1010)      357 2023-04-19 05:01:35.000000 hak-0.0.5/hak/list/strings/two_char_combinations.py
--rw-rw-r--   0 a         (1009) a         (1010)      115 2023-04-19 01:55:38.000000 hak-0.0.5/hak/list/to_comma_separated_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/lists/
--rw-rw-r--   0 a         (1009) a         (1010)      216 2023-04-19 01:55:38.000000 hak-0.0.5/hak/lists/merge.py
--rw-rw-r--   0 a         (1009) a         (1010)     1131 2023-04-19 01:55:38.000000 hak-0.0.5/hak/load_durations_if_exists.py
--rw-rw-r--   0 a         (1009) a         (1010)      123 2023-04-19 01:55:38.000000 hak-0.0.5/hak/log_2.py
--rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.5/hak/nop.py
--rw-rw-r--   0 a         (1009) a         (1010)       91 2023-04-19 01:55:38.000000 hak-0.0.5/hak/nop_state_x.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/patch/
--rw-rw-r--   0 a         (1009) a         (1010)     7860 2023-04-19 09:15:38.000000 hak-0.0.5/hak/patch/do.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/period/
--rw-rw-r--   0 a         (1009) a         (1010)      333 2023-04-19 01:55:38.000000 hak-0.0.5/hak/period/contains_day.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/pip/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/pip/dist_tar/
--rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 07:21:09.000000 hak-0.0.5/hak/pip/dist_tar/make.py
--rw-rw-r--   0 a         (1009) a         (1010)      804 2023-04-19 07:34:45.000000 hak-0.0.5/hak/pip/dist_tar/remove.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/pip/setup/
--rw-rw-r--   0 a         (1009) a         (1010)     1305 2023-04-19 04:43:59.000000 hak-0.0.5/hak/pip/setup/update.py
--rw-rw-r--   0 a         (1009) a         (1010)     1792 2023-04-19 08:32:41.000000 hak-0.0.5/hak/pip/upload.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/pip/version/
--rw-rw-r--   0 a         (1009) a         (1010)      837 2023-04-19 01:55:38.000000 hak-0.0.5/hak/pip/version/get.py
--rw-rw-r--   0 a         (1009) a         (1010)      120 2023-04-19 01:55:38.000000 hak-0.0.5/hak/pip/version/to_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/pyfiles/
--rw-rw-r--   0 a         (1009) a         (1010)      157 2023-04-19 01:55:38.000000 hak-0.0.5/hak/pyfiles/format.py
--rw-rw-r--   0 a         (1009) a         (1010)      838 2023-04-19 04:33:37.000000 hak-0.0.5/hak/pyfiles/format_and_commit.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/report/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/report/fail/
--rw-rw-r--   0 a         (1009) a         (1010)      814 2023-04-19 01:55:38.000000 hak-0.0.5/hak/report/fail/no_xyz.py
--rw-rw-r--   0 a         (1009) a         (1010)     1914 2023-04-19 01:55:38.000000 hak-0.0.5/hak/report/fail/xyz.py
--rw-rw-r--   0 a         (1009) a         (1010)     1440 2023-04-19 01:55:38.000000 hak-0.0.5/hak/report/fail/z_return_neq_y_return.py
--rw-rw-r--   0 a         (1009) a         (1010)     1601 2023-04-19 01:55:38.000000 hak-0.0.5/hak/report/fail/z_stdo_neq_y_stdo.py
--rw-rw-r--   0 a         (1009) a         (1010)      887 2023-04-19 01:55:38.000000 hak-0.0.5/hak/report/property_failure.py
--rw-rw-r--   0 a         (1009) a         (1010)      729 2023-04-19 01:55:38.000000 hak-0.0.5/hak/report/success.py
--rw-rw-r--   0 a         (1009) a         (1010)      394 2023-04-19 01:55:38.000000 hak-0.0.5/hak/report/summarise_file.py
--rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.5/hak/save_durations.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/schedule/
--rw-rw-r--   0 a         (1009) a         (1010)     3465 2023-04-19 01:55:38.000000 hak-0.0.5/hak/schedule/make.py
--rw-rw-r--   0 a         (1009) a         (1010)      559 2023-04-19 01:55:38.000000 hak-0.0.5/hak/select_text_colour_from_width.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/session/
--rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.5/hak/session/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/set/
--rw-rw-r--   0 a         (1009) a         (1010)      114 2023-04-19 01:55:38.000000 hak-0.0.5/hak/set/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.047330 hak-0.0.5/hak/setup/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/setup/cfg/
--rw-rw-r--   0 a         (1009) a         (1010)     1531 2023-04-19 07:22:45.000000 hak-0.0.5/hak/setup/cfg/update.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/setup/py/
--rw-rw-r--   0 a         (1009) a         (1010)     1633 2023-04-19 07:24:59.000000 hak-0.0.5/hak/setup/py/update.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/alphanumeric/
--rw-rw-r--   0 a         (1009) a         (1010)      264 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/alphanumeric/fake.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/append/
--rw-rw-r--   0 a         (1009) a         (1010)       54 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/append/new_line.py
--rw-rw-r--   0 a         (1009) a         (1010)      541 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/camel_to_snake.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/char/
--rw-rw-r--   0 a         (1009) a         (1010)      322 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/char/find_all_indices.py
--rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/char/is_digit.py
--rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/char/is_upper.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/chars/
--rw-rw-r--   0 a         (1009) a         (1010)      561 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/chars/remove.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/colour/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/colour/bright/
--rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/bright/blue.py
--rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/bright/cyan.py
--rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/bright/green.py
--rw-rw-r--   0 a         (1009) a         (1010)      168 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/bright/magenta.py
--rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/bright/red.py
--rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/bright/white.py
--rw-rw-r--   0 a         (1009) a         (1010)      166 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/bright/yellow.py
--rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/danger.py
--rw-rw-r--   0 a         (1009) a         (1010)      174 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/danger_if_zero.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/colour/dark/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/dark/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/dark/blue.py
--rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/dark/cyan.py
--rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/dark/default.py
--rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/dark/green.py
--rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/dark/magenta.py
--rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/dark/red.py
--rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/dark/white.py
--rw-rw-r--   0 a         (1009) a         (1010)      152 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/dark/yellow.py
--rw-rw-r--   0 a         (1009) a         (1010)       64 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/data.py
--rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/info.py
--rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/primary.py
--rw-rw-r--   0 a         (1009) a         (1010)     2261 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/rainbow.py
--rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/secondary.py
--rw-rw-r--   0 a         (1009) a         (1010)      267 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/tgfr.py
--rw-rw-r--   0 a         (1009) a         (1010)      135 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/colour/warning.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/contains/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/contains/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/contains/function/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/contains/function/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      341 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/contains/function/run.py
--rw-rw-r--   0 a         (1009) a         (1010)      192 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/contains/function/test.py
--rw-rw-r--   0 a         (1009) a         (1010)      224 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/contains/l.py
--rw-rw-r--   0 a         (1009) a         (1010)       76 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/contains/version.py
--rw-rw-r--   0 a         (1009) a         (1010)      105 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/count_x_in_y.py
--rw-rw-r--   0 a         (1009) a         (1010)      996 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/delete_character_safely.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/digits/
--rw-rw-r--   0 a         (1009) a         (1010)      202 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/digits/remove.py
--rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/double_single_quotes.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/family_name/
--rw-rw-r--   0 a         (1009) a         (1010)   115522 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/family_name/fake.py
--rw-rw-r--   0 a         (1009) a         (1010)      303 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/family_name/is_a.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/filename/
--rw-rw-r--   0 a         (1009) a         (1010)      126 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/filename/to_module_name.py
--rw-rw-r--   0 a         (1009) a         (1010)      209 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/find_last_comma_index.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/fn_name/
--rw-rw-r--   0 a         (1009) a         (1010)      226 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/fn_name/is_ignorable.py
--rw-rw-r--   0 a         (1009) a         (1010)     5035 2023-04-19 05:00:49.000000 hak-0.0.5/hak/string/format.py
--rw-rw-r--   0 a         (1009) a         (1010)       73 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/has_at_symbol.py
--rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/has_digit.py
--rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/has_lowercase.py
--rw-rw-r--   0 a         (1009) a         (1010)      259 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/has_other_char.py
--rw-rw-r--   0 a         (1009) a         (1010)      172 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/has_seven_digits.py
--rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/has_uppercase.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/hbar/
--rw-rw-r--   0 a         (1009) a         (1010)      122 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/hbar/make.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.047330 hak-0.0.5/hak/string/header/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/header/python_file/
--rw-rw-r--   0 a         (1009) a         (1010)      314 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/header/python_file/make.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.055331 hak-0.0.5/hak/string/header/test_table/
--rw-rw-r--   0 a         (1009) a         (1010)      461 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/header/test_table/make.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/indent/
--rw-rw-r--   0 a         (1009) a         (1010)      137 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/indent/run_if_class_method.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/insert/
--rw-rw-r--   0 a         (1009) a         (1010)      602 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/insert/new_line_after_last_import_line.py
--rw-rw-r--   0 a         (1009) a         (1010)      278 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/insert/new_line_before_comment.py
--rw-rw-r--   0 a         (1009) a         (1010)      584 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/insert/new_line_before_def.py
--rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/insert/new_line_before_if_main.py
--rw-rw-r--   0 a         (1009) a         (1010)      666 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/insert/new_line_before_lambda.py
--rw-rw-r--   0 a         (1009) a         (1010)      292 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/insert/new_line_before_new_line_and_cea_.py
--rw-rw-r--   0 a         (1009) a         (1010)      102 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      124 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/is_or_none.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/json/
--rw-rw-r--   0 a         (1009) a         (1010)      179 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/json/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      548 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/lambdarise.py
--rw-rw-r--   0 a         (1009) a         (1010)      360 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/make_content_without_function.py
--rw-rw-r--   0 a         (1009) a         (1010)      325 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/make_function_text.py
--rw-rw-r--   0 a         (1009) a         (1010)      338 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/make_initial_content.py
--rw-rw-r--   0 a         (1009) a         (1010)      319 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/make_new_function_text.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/password/
--rw-rw-r--   0 a         (1009) a         (1010)     1179 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/password/create.py
--rw-rw-r--   0 a         (1009) a         (1010)      534 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/password/has_chars_from_3_sets.py
--rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/pop_left.py
--rw-rw-r--   0 a         (1009) a         (1010)      219 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/pop_right.py
--rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/prepend_import.py
--rw-rw-r--   0 a         (1009) a         (1010)      756 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/print_and_return_false.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/refactor/
--rw-rw-r--   0 a         (1009) a         (1010)     1218 2023-04-19 05:01:09.000000 hak-0.0.5/hak/string/refactor/by_two_char_combinations.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/remove/
--rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/remove/empty_line_spaces.py
--rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/remove/empty_lines.py
--rw-rw-r--   0 a         (1009) a         (1010)      441 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/remove/extra_new_line_following_class_definition.py
--rw-rw-r--   0 a         (1009) a         (1010)      210 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/remove/first_new_line_if_starts_with_new_line.py
--rw-rw-r--   0 a         (1009) a         (1010)       81 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/remove/whitespace_between_newlines.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/replace/
--rw-rw-r--   0 a         (1009) a         (1010)      241 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/replace/double_new_line_with_single_new_line.py
--rw-rw-r--   0 a         (1009) a         (1010)      129 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/replace/single_new_line_with_empty_string.py
--rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/replace/triple_new_line_with_double_new_line.py
--rw-rw-r--   0 a         (1009) a         (1010)      483 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/replace_unprintable.py
--rw-rw-r--   0 a         (1009) a         (1010)     3361 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/separate_function_from_context.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/single_line_function/
--rw-rw-r--   0 a         (1009) a         (1010)      428 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/single_line_function/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      463 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/single_line_function/to_lambda_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/spaces/
--rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/spaces/count.py
--rw-rw-r--   0 a         (1009) a         (1010)      320 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/split_fn_name_and_text.py
--rw-rw-r--   0 a         (1009) a         (1010)      344 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/strip_unprintable.py
--rw-rw-r--   0 a         (1009) a         (1010)      265 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/to_cond_freq_dict.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/token/
--rw-rw-r--   0 a         (1009) a         (1010)     1263 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/token/substitute.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/string/yyyymmdd/
--rw-rw-r--   0 a         (1009) a         (1010)      238 2023-04-19 01:55:38.000000 hak-0.0.5/hak/string/yyyymmdd/to_date.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.047330 hak-0.0.5/hak/subprocess/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/subprocess/completed_process/
--rw-rw-r--   0 a         (1009) a         (1010)      655 2023-04-19 01:55:38.000000 hak-0.0.5/hak/subprocess/completed_process/to_str.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/system/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/system/__init__.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/system/git/
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/system/git/commit/
--rw-rw-r--   0 a         (1009) a         (1010)     2515 2023-04-19 01:55:38.000000 hak-0.0.5/hak/system/git/commit/run.py
--rw-rw-r--   0 a         (1009) a         (1010)      384 2023-04-19 01:55:38.000000 hak-0.0.5/hak/system/git/commit_if_test_and_app_ok.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/system/git/gitignore/
--rw-rw-r--   0 a         (1009) a         (1010)      631 2023-04-19 01:55:38.000000 hak-0.0.5/hak/system/git/gitignore/make.py
--rw-rw-r--   0 a         (1009) a         (1010)      486 2023-04-19 03:03:56.000000 hak-0.0.5/hak/system/git/init.py
--rw-rw-r--   0 a         (1009) a         (1010)      725 2023-04-19 01:55:38.000000 hak-0.0.5/hak/system/git/log_oneline.py
--rw-rw-r--   0 a         (1009) a         (1010)      866 2023-04-19 01:55:38.000000 hak-0.0.5/hak/system/git/push_after_delay.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/system/screen/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/system/screen/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)      786 2023-04-19 01:55:38.000000 hak-0.0.5/hak/system/screen/clear.py
--rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 01:55:38.000000 hak-0.0.5/hak/terminal.py
--rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.5/hak/ternary.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/test/
--rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.5/hak/test/__init__.py
--rw-rw-r--   0 a         (1009) a         (1010)     2578 2023-04-19 01:55:38.000000 hak-0.0.5/hak/test/check_final_line.py
--rw-rw-r--   0 a         (1009) a         (1010)     2689 2023-04-19 01:55:38.000000 hak-0.0.5/hak/test/check_line_lengths.py
--rw-rw-r--   0 a         (1009) a         (1010)     2843 2023-04-19 01:55:38.000000 hak-0.0.5/hak/test/do.py
--rw-rw-r--   0 a         (1009) a         (1010)     2450 2023-04-19 01:55:38.000000 hak-0.0.5/hak/test/final_line_check.py
--rw-rw-r--   0 a         (1009) a         (1010)      774 2023-04-19 01:55:38.000000 hak-0.0.5/hak/test/line_lengths_check.py
--rw-rw-r--   0 a         (1009) a         (1010)      926 2023-04-19 01:55:38.000000 hak-0.0.5/hak/test/oldest_file_print.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.059331 hak-0.0.5/hak/tup/
--rw-rw-r--   0 a         (1009) a         (1010)      176 2023-04-19 01:55:38.000000 hak-0.0.5/hak/tup/is_a.py
--rw-rw-r--   0 a         (1009) a         (1010)      617 2023-04-19 01:55:38.000000 hak-0.0.5/hak/update_duration.py
-drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:09:33.051331 hak-0.0.5/hak.egg-info/
--rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:09:32.000000 hak-0.0.5/hak.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1009) a         (1010)     7874 2023-04-19 10:09:33.000000 hak-0.0.5/hak.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1009) a         (1010)        1 2023-04-19 10:09:32.000000 hak-0.0.5/hak.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1009) a         (1010)     1606 2023-04-19 10:09:32.000000 hak-0.0.5/hak.egg-info/top_level.txt
--rw-rw-r--   0 a         (1009) a         (1010)      536 2023-04-19 10:09:33.059331 hak-0.0.5/setup.cfg
--rw-rw-r--   0 a         (1009) a         (1010)     2747 2023-04-19 10:09:32.000000 hak-0.0.5/setup.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/
+-rw-rw-r--   0 a         (1009) a         (1010)     1068 2023-04-19 01:55:38.000000 hak-0.0.6/LICENSE
+-rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:12:37.334879 hak-0.0.6/PKG-INFO
+-rw-rw-r--   0 a         (1009) a         (1010)      406 2023-04-19 03:24:53.000000 hak-0.0.6/README.md
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.322878 hak-0.0.6/hak/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      140 2023-04-19 01:55:38.000000 hak-0.0.6/hak/a_equals_b.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.322878 hak-0.0.6/hak/bool/
+-rw-rw-r--   0 a         (1009) a         (1010)       86 2023-04-19 01:55:38.000000 hak-0.0.6/hak/bool/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      103 2023-04-19 01:55:38.000000 hak-0.0.6/hak/bool/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/bool/or_none/
+-rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.6/hak/bool/or_none/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      125 2023-04-19 01:55:38.000000 hak-0.0.6/hak/bool/or_none/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/bools/
+-rw-rw-r--   0 a         (1009) a         (1010)      139 2023-04-19 01:55:38.000000 hak-0.0.6/hak/bools/count_true.py
+-rw-rw-r--   0 a         (1009) a         (1010)      249 2023-04-19 01:55:38.000000 hak-0.0.6/hak/calculate_duration_bar_width.py
+-rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.6/hak/check_if_ok_to_proceed.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/date/
+-rw-rw-r--   0 a         (1009) a         (1010)      143 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      347 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/is_first_second_or_third_day_of_month.py
+-rw-rw-r--   0 a         (1009) a         (1010)      414 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/is_first_week_of_quarter.py
+-rw-rw-r--   0 a         (1009) a         (1010)      208 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/is_monday.py
+-rw-rw-r--   0 a         (1009) a         (1010)      462 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/is_weekday.py
+-rw-rw-r--   0 a         (1009) a         (1010)      467 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/is_weekend.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/date/public_holiday/
+-rw-rw-r--   0 a         (1009) a         (1010)     5617 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/public_holiday/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      385 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/select_from_last_n_days.py
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/to_dd_mm_yyyy_str.py
+-rw-rw-r--   0 a         (1009) a         (1010)      605 2023-04-19 03:01:25.000000 hak-0.0.6/hak/date/to_utc_timestamp.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.322878 hak-0.0.6/hak/date/year/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/date/year/easter_sunday/
+-rw-rw-r--   0 a         (1009) a         (1010)     1006 2023-04-19 01:55:38.000000 hak-0.0.6/hak/date/year/easter_sunday/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/datetime/
+-rw-rw-r--   0 a         (1009) a         (1010)      149 2023-04-19 01:55:38.000000 hak-0.0.6/hak/datetime/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      272 2023-04-19 01:55:38.000000 hak-0.0.6/hak/datetime/select_from_last_n_days.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/dict/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      215 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/convert_to_sql_insertable.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/dict/frequencies/
+-rw-rw-r--   0 a         (1009) a         (1010)      356 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/frequencies/choose.py
+-rw-rw-r--   0 a         (1009) a         (1010)      376 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/frequencies/make_from_strings.py
+-rw-rw-r--   0 a         (1009) a         (1010)      187 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/get_or_default.py
+-rw-rw-r--   0 a         (1009) a         (1010)      190 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/make_from_key_value_lists.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/dict/proposed_dismantlement/
+-rw-rw-r--   0 a         (1009) a         (1010)     1520 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/proposed_dismantlement/show.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/dict/test_durations/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/test_durations/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/test_durations/to_tuple_list_sorted_by_duration.py
+-rw-rw-r--   0 a         (1009) a         (1010)     4011 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dict/to_max_line_width_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/dicts/
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dicts/a_into_b.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1200 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dicts/compare.py
+-rw-rw-r--   0 a         (1009) a         (1010)      195 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dicts/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      663 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dicts/merge_freq_dicts.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dicts/reindex.py
+-rw-rw-r--   0 a         (1009) a         (1010)      203 2023-04-19 01:55:38.000000 hak-0.0.6/hak/dicts/sort_by_key.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/directories/
+-rw-rw-r--   0 a         (1009) a         (1010)      567 2023-04-19 01:55:38.000000 hak-0.0.6/hak/directories/exist.py
+-rw-rw-r--   0 a         (1009) a         (1010)      432 2023-04-19 01:55:38.000000 hak-0.0.6/hak/directories/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/directory/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/directory/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1548 2023-04-19 01:55:38.000000 hak-0.0.6/hak/directory/compress_to_tar.py
+-rw-rw-r--   0 a         (1009) a         (1010)      674 2023-04-19 05:28:56.000000 hak-0.0.6/hak/directory/empty.py
+-rw-rw-r--   0 a         (1009) a         (1010)       88 2023-04-19 01:55:38.000000 hak-0.0.6/hak/directory/exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1203 2023-04-19 10:11:56.000000 hak-0.0.6/hak/directory/get_most_recently_modified.py
+-rw-rw-r--   0 a         (1009) a         (1010)      650 2023-04-19 01:55:38.000000 hak-0.0.6/hak/directory/is_module.py
+-rw-rw-r--   0 a         (1009) a         (1010)      667 2023-04-19 10:09:51.000000 hak-0.0.6/hak/directory/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      782 2023-04-19 01:55:38.000000 hak-0.0.6/hak/directory/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3692 2023-04-19 01:55:38.000000 hak-0.0.6/hak/duration.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2021 2023-04-19 01:55:38.000000 hak-0.0.6/hak/duration_bar.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/fake/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/fake/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/fake/os/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/fake/os/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      418 2023-04-19 01:55:38.000000 hak-0.0.6/hak/fake/os/system.py
+-rw-rw-r--   0 a         (1009) a         (1010)      424 2023-04-19 01:55:38.000000 hak-0.0.6/hak/fake/printer.py
+-rw-rw-r--   0 a         (1009) a         (1010)       45 2023-04-19 01:55:38.000000 hak-0.0.6/hak/fake/sleep.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/fake/subprocess/
+-rw-rw-r--   0 a         (1009) a         (1010)     5854 2023-04-19 04:41:24.000000 hak-0.0.6/hak/fake/subprocess/run.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/file/
+-rw-rw-r--   0 a         (1009) a         (1010)     1253 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      785 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/decrypt.py
+-rw-rw-r--   0 a         (1009) a         (1010)      929 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/encrypt.py
+-rw-rw-r--   0 a         (1009) a         (1010)      697 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/load.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/file/pickle/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/pickle/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1253 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/pickle/load_if_exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)      906 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/pickle/save.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/file/py/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/py/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      546 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/py/create.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2644 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/py/dismantle.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3819 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/py/extract_fn.py
+-rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/py/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)      956 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/save.py
+-rw-rw-r--   0 a         (1009) a         (1010)      761 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/save_lines.py
+-rw-rw-r--   0 a         (1009) a         (1010)      308 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/save_lines_or_string.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.322878 hak-0.0.6/hak/file/secret/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/file/secret/password/
+-rw-rw-r--   0 a         (1009) a         (1010)      680 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/secret/password/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/file/secret/username/
+-rw-rw-r--   0 a         (1009) a         (1010)      713 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/secret/username/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/file/tar/
+-rw-rw-r--   0 a         (1009) a         (1010)     1562 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/tar/extract.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/file/zip/
+-rw-rw-r--   0 a         (1009) a         (1010)      487 2023-04-19 01:55:38.000000 hak-0.0.6/hak/file/zip/extract.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.322878 hak-0.0.6/hak/files/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/files/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)     1765 2023-04-19 04:43:12.000000 hak-0.0.6/hak/files/pyfiles/dismantle.py
+-rw-rw-r--   0 a         (1009) a         (1010)      100 2023-04-19 01:55:38.000000 hak-0.0.6/hak/find_first_parenthesis.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/float/
+-rw-rw-r--   0 a         (1009) a         (1010)       70 2023-04-19 01:55:38.000000 hak-0.0.6/hak/float/epsilon.py
+-rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.6/hak/float/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.6/hak/float/is_not.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/float/nan/
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.6/hak/float/nan/to_none.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/function/
+-rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.6/hak/function/function.py
+-rw-rw-r--   0 a         (1009) a         (1010)      423 2023-04-19 01:55:38.000000 hak-0.0.6/hak/function/write_to_file.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/int/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/int/days/
+-rw-rw-r--   0 a         (1009) a         (1010)      227 2023-04-19 01:55:38.000000 hak-0.0.6/hak/int/days/a_to_b_inclusive.py
+-rw-rw-r--   0 a         (1009) a         (1010)      661 2023-04-19 01:55:38.000000 hak-0.0.6/hak/int/get_prime_factorisation.py
+-rw-rw-r--   0 a         (1009) a         (1010)      104 2023-04-19 01:55:38.000000 hak-0.0.6/hak/int/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      426 2023-04-19 01:55:38.000000 hak-0.0.6/hak/int/is_prime.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/int/year/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/int/year/days/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/int/year/days/count/
+-rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.6/hak/int/year/days/count/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/int/year/days/first/
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.6/hak/int/year/days/first/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      420 2023-04-19 01:55:38.000000 hak-0.0.6/hak/int/year/days/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      153 2023-04-19 01:55:38.000000 hak-0.0.6/hak/int/year/now.py
+-rw-rw-r--   0 a         (1009) a         (1010)      448 2023-04-19 01:55:38.000000 hak-0.0.6/hak/l.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/list/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/list/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.6/hak/list/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/list/strings/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/list/strings/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 04:41:08.000000 hak-0.0.6/hak/list/strings/add_src_funks_prefix.py
+-rw-rw-r--   0 a         (1009) a         (1010)      586 2023-04-19 01:55:38.000000 hak-0.0.6/hak/list/strings/compare.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/list/strings/contain/
+-rw-rw-r--   0 a         (1009) a         (1010)      145 2023-04-19 04:43:23.000000 hak-0.0.6/hak/list/strings/contain/version.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2222 2023-04-19 04:44:27.000000 hak-0.0.6/hak/list/strings/find_first_diff.py
+-rw-rw-r--   0 a         (1009) a         (1010)      434 2023-04-19 04:45:12.000000 hak-0.0.6/hak/list/strings/make_patch_version_change_to_py.py
+-rw-rw-r--   0 a         (1009) a         (1010)      293 2023-04-19 04:47:46.000000 hak-0.0.6/hak/list/strings/module_names_from_py_filenames.py
+-rw-rw-r--   0 a         (1009) a         (1010)      410 2023-04-19 04:48:58.000000 hak-0.0.6/hak/list/strings/patch_setup_cfg.py
+-rw-rw-r--   0 a         (1009) a         (1010)      622 2023-04-19 04:51:45.000000 hak-0.0.6/hak/list/strings/patch_setup_py.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/list/strings/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)     1514 2023-04-19 04:52:08.000000 hak-0.0.6/hak/list/strings/pyfiles/filter_out_items.py
+-rw-rw-r--   0 a         (1009) a         (1010)      766 2023-04-19 05:00:37.000000 hak-0.0.6/hak/list/strings/show_diff.py
+-rw-rw-r--   0 a         (1009) a         (1010)      647 2023-04-19 05:00:56.000000 hak-0.0.6/hak/list/strings/to_dict.py
+-rw-rw-r--   0 a         (1009) a         (1010)      357 2023-04-19 05:01:35.000000 hak-0.0.6/hak/list/strings/two_char_combinations.py
+-rw-rw-r--   0 a         (1009) a         (1010)      115 2023-04-19 01:55:38.000000 hak-0.0.6/hak/list/to_comma_separated_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/lists/
+-rw-rw-r--   0 a         (1009) a         (1010)      216 2023-04-19 01:55:38.000000 hak-0.0.6/hak/lists/merge.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1131 2023-04-19 01:55:38.000000 hak-0.0.6/hak/load_durations_if_exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)      123 2023-04-19 01:55:38.000000 hak-0.0.6/hak/log_2.py
+-rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.6/hak/nop.py
+-rw-rw-r--   0 a         (1009) a         (1010)       91 2023-04-19 01:55:38.000000 hak-0.0.6/hak/nop_state_x.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/patch/
+-rw-rw-r--   0 a         (1009) a         (1010)     7860 2023-04-19 09:15:38.000000 hak-0.0.6/hak/patch/do.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/period/
+-rw-rw-r--   0 a         (1009) a         (1010)      333 2023-04-19 01:55:38.000000 hak-0.0.6/hak/period/contains_day.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.326879 hak-0.0.6/hak/pip/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/pip/dist_tar/
+-rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 07:21:09.000000 hak-0.0.6/hak/pip/dist_tar/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      804 2023-04-19 07:34:45.000000 hak-0.0.6/hak/pip/dist_tar/remove.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/pip/setup/
+-rw-rw-r--   0 a         (1009) a         (1010)     1305 2023-04-19 04:43:59.000000 hak-0.0.6/hak/pip/setup/update.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1792 2023-04-19 08:32:41.000000 hak-0.0.6/hak/pip/upload.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/pip/version/
+-rw-rw-r--   0 a         (1009) a         (1010)      837 2023-04-19 01:55:38.000000 hak-0.0.6/hak/pip/version/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      120 2023-04-19 01:55:38.000000 hak-0.0.6/hak/pip/version/to_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)      157 2023-04-19 01:55:38.000000 hak-0.0.6/hak/pyfiles/format.py
+-rw-rw-r--   0 a         (1009) a         (1010)      838 2023-04-19 04:33:37.000000 hak-0.0.6/hak/pyfiles/format_and_commit.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/report/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/report/fail/
+-rw-rw-r--   0 a         (1009) a         (1010)      814 2023-04-19 01:55:38.000000 hak-0.0.6/hak/report/fail/no_xyz.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1914 2023-04-19 01:55:38.000000 hak-0.0.6/hak/report/fail/xyz.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1440 2023-04-19 01:55:38.000000 hak-0.0.6/hak/report/fail/z_return_neq_y_return.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1601 2023-04-19 01:55:38.000000 hak-0.0.6/hak/report/fail/z_stdo_neq_y_stdo.py
+-rw-rw-r--   0 a         (1009) a         (1010)      887 2023-04-19 01:55:38.000000 hak-0.0.6/hak/report/property_failure.py
+-rw-rw-r--   0 a         (1009) a         (1010)      729 2023-04-19 01:55:38.000000 hak-0.0.6/hak/report/success.py
+-rw-rw-r--   0 a         (1009) a         (1010)      394 2023-04-19 01:55:38.000000 hak-0.0.6/hak/report/summarise_file.py
+-rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.6/hak/save_durations.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/schedule/
+-rw-rw-r--   0 a         (1009) a         (1010)     3465 2023-04-19 01:55:38.000000 hak-0.0.6/hak/schedule/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      559 2023-04-19 01:55:38.000000 hak-0.0.6/hak/select_text_colour_from_width.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/session/
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.6/hak/session/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/set/
+-rw-rw-r--   0 a         (1009) a         (1010)      114 2023-04-19 01:55:38.000000 hak-0.0.6/hak/set/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.322878 hak-0.0.6/hak/setup/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/setup/cfg/
+-rw-rw-r--   0 a         (1009) a         (1010)     1531 2023-04-19 07:22:45.000000 hak-0.0.6/hak/setup/cfg/update.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/setup/py/
+-rw-rw-r--   0 a         (1009) a         (1010)     1633 2023-04-19 07:24:59.000000 hak-0.0.6/hak/setup/py/update.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/alphanumeric/
+-rw-rw-r--   0 a         (1009) a         (1010)      264 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/alphanumeric/fake.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/append/
+-rw-rw-r--   0 a         (1009) a         (1010)       54 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/append/new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      541 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/camel_to_snake.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/char/
+-rw-rw-r--   0 a         (1009) a         (1010)      322 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/char/find_all_indices.py
+-rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/char/is_digit.py
+-rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/char/is_upper.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/chars/
+-rw-rw-r--   0 a         (1009) a         (1010)      561 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/chars/remove.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/colour/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/colour/bright/
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/bright/blue.py
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/bright/cyan.py
+-rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/bright/green.py
+-rw-rw-r--   0 a         (1009) a         (1010)      168 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/bright/magenta.py
+-rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/bright/red.py
+-rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/bright/white.py
+-rw-rw-r--   0 a         (1009) a         (1010)      166 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/bright/yellow.py
+-rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/danger.py
+-rw-rw-r--   0 a         (1009) a         (1010)      174 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/danger_if_zero.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/colour/dark/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/dark/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/dark/blue.py
+-rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/dark/cyan.py
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/dark/default.py
+-rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/dark/green.py
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/dark/magenta.py
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/dark/red.py
+-rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/dark/white.py
+-rw-rw-r--   0 a         (1009) a         (1010)      152 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/dark/yellow.py
+-rw-rw-r--   0 a         (1009) a         (1010)       64 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/data.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/info.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/primary.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2261 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/rainbow.py
+-rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/secondary.py
+-rw-rw-r--   0 a         (1009) a         (1010)      267 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/tgfr.py
+-rw-rw-r--   0 a         (1009) a         (1010)      135 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/colour/warning.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/contains/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/contains/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/contains/function/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/contains/function/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      341 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/contains/function/run.py
+-rw-rw-r--   0 a         (1009) a         (1010)      192 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/contains/function/test.py
+-rw-rw-r--   0 a         (1009) a         (1010)      224 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/contains/l.py
+-rw-rw-r--   0 a         (1009) a         (1010)       76 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/contains/version.py
+-rw-rw-r--   0 a         (1009) a         (1010)      105 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/count_x_in_y.py
+-rw-rw-r--   0 a         (1009) a         (1010)      996 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/delete_character_safely.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/digits/
+-rw-rw-r--   0 a         (1009) a         (1010)      202 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/digits/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/double_single_quotes.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/family_name/
+-rw-rw-r--   0 a         (1009) a         (1010)   115522 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/family_name/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      303 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/family_name/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/filename/
+-rw-rw-r--   0 a         (1009) a         (1010)      126 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/filename/to_module_name.py
+-rw-rw-r--   0 a         (1009) a         (1010)      209 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/find_last_comma_index.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/fn_name/
+-rw-rw-r--   0 a         (1009) a         (1010)      226 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/fn_name/is_ignorable.py
+-rw-rw-r--   0 a         (1009) a         (1010)     5035 2023-04-19 05:00:49.000000 hak-0.0.6/hak/string/format.py
+-rw-rw-r--   0 a         (1009) a         (1010)       73 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/has_at_symbol.py
+-rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/has_digit.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/has_lowercase.py
+-rw-rw-r--   0 a         (1009) a         (1010)      259 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/has_other_char.py
+-rw-rw-r--   0 a         (1009) a         (1010)      172 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/has_seven_digits.py
+-rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/has_uppercase.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/hbar/
+-rw-rw-r--   0 a         (1009) a         (1010)      122 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/hbar/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.322878 hak-0.0.6/hak/string/header/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/header/python_file/
+-rw-rw-r--   0 a         (1009) a         (1010)      314 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/header/python_file/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/header/test_table/
+-rw-rw-r--   0 a         (1009) a         (1010)      461 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/header/test_table/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/indent/
+-rw-rw-r--   0 a         (1009) a         (1010)      137 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/indent/run_if_class_method.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/insert/
+-rw-rw-r--   0 a         (1009) a         (1010)      602 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/insert/new_line_after_last_import_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      278 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/insert/new_line_before_comment.py
+-rw-rw-r--   0 a         (1009) a         (1010)      584 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/insert/new_line_before_def.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/insert/new_line_before_if_main.py
+-rw-rw-r--   0 a         (1009) a         (1010)      666 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/insert/new_line_before_lambda.py
+-rw-rw-r--   0 a         (1009) a         (1010)      292 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/insert/new_line_before_new_line_and_cea_.py
+-rw-rw-r--   0 a         (1009) a         (1010)      102 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      124 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/is_or_none.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.330879 hak-0.0.6/hak/string/json/
+-rw-rw-r--   0 a         (1009) a         (1010)      179 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/json/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      548 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/lambdarise.py
+-rw-rw-r--   0 a         (1009) a         (1010)      360 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/make_content_without_function.py
+-rw-rw-r--   0 a         (1009) a         (1010)      325 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/make_function_text.py
+-rw-rw-r--   0 a         (1009) a         (1010)      338 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/make_initial_content.py
+-rw-rw-r--   0 a         (1009) a         (1010)      319 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/make_new_function_text.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/string/password/
+-rw-rw-r--   0 a         (1009) a         (1010)     1179 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/password/create.py
+-rw-rw-r--   0 a         (1009) a         (1010)      534 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/password/has_chars_from_3_sets.py
+-rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/pop_left.py
+-rw-rw-r--   0 a         (1009) a         (1010)      219 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/pop_right.py
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/prepend_import.py
+-rw-rw-r--   0 a         (1009) a         (1010)      756 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/print_and_return_false.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/string/refactor/
+-rw-rw-r--   0 a         (1009) a         (1010)     1218 2023-04-19 05:01:09.000000 hak-0.0.6/hak/string/refactor/by_two_char_combinations.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/string/remove/
+-rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/remove/empty_line_spaces.py
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/remove/empty_lines.py
+-rw-rw-r--   0 a         (1009) a         (1010)      441 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/remove/extra_new_line_following_class_definition.py
+-rw-rw-r--   0 a         (1009) a         (1010)      210 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/remove/first_new_line_if_starts_with_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)       81 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/remove/whitespace_between_newlines.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/string/replace/
+-rw-rw-r--   0 a         (1009) a         (1010)      241 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/replace/double_new_line_with_single_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      129 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/replace/single_new_line_with_empty_string.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/replace/triple_new_line_with_double_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      483 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/replace_unprintable.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3361 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/separate_function_from_context.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/string/single_line_function/
+-rw-rw-r--   0 a         (1009) a         (1010)      428 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/single_line_function/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      463 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/single_line_function/to_lambda_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/string/spaces/
+-rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/spaces/count.py
+-rw-rw-r--   0 a         (1009) a         (1010)      320 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/split_fn_name_and_text.py
+-rw-rw-r--   0 a         (1009) a         (1010)      344 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/strip_unprintable.py
+-rw-rw-r--   0 a         (1009) a         (1010)      265 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/to_cond_freq_dict.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/string/token/
+-rw-rw-r--   0 a         (1009) a         (1010)     1263 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/token/substitute.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/string/yyyymmdd/
+-rw-rw-r--   0 a         (1009) a         (1010)      238 2023-04-19 01:55:38.000000 hak-0.0.6/hak/string/yyyymmdd/to_date.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.322878 hak-0.0.6/hak/subprocess/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/subprocess/completed_process/
+-rw-rw-r--   0 a         (1009) a         (1010)      655 2023-04-19 01:55:38.000000 hak-0.0.6/hak/subprocess/completed_process/to_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/system/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/system/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/system/git/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/system/git/commit/
+-rw-rw-r--   0 a         (1009) a         (1010)     2515 2023-04-19 01:55:38.000000 hak-0.0.6/hak/system/git/commit/run.py
+-rw-rw-r--   0 a         (1009) a         (1010)      384 2023-04-19 01:55:38.000000 hak-0.0.6/hak/system/git/commit_if_test_and_app_ok.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/system/git/gitignore/
+-rw-rw-r--   0 a         (1009) a         (1010)      631 2023-04-19 01:55:38.000000 hak-0.0.6/hak/system/git/gitignore/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      486 2023-04-19 03:03:56.000000 hak-0.0.6/hak/system/git/init.py
+-rw-rw-r--   0 a         (1009) a         (1010)      725 2023-04-19 01:55:38.000000 hak-0.0.6/hak/system/git/log_oneline.py
+-rw-rw-r--   0 a         (1009) a         (1010)      866 2023-04-19 01:55:38.000000 hak-0.0.6/hak/system/git/push_after_delay.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/system/screen/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/system/screen/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      786 2023-04-19 01:55:38.000000 hak-0.0.6/hak/system/screen/clear.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 01:55:38.000000 hak-0.0.6/hak/terminal.py
+-rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.6/hak/ternary.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/test/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.6/hak/test/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2578 2023-04-19 01:55:38.000000 hak-0.0.6/hak/test/check_final_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2689 2023-04-19 01:55:38.000000 hak-0.0.6/hak/test/check_line_lengths.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2843 2023-04-19 01:55:38.000000 hak-0.0.6/hak/test/do.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2450 2023-04-19 01:55:38.000000 hak-0.0.6/hak/test/final_line_check.py
+-rw-rw-r--   0 a         (1009) a         (1010)      774 2023-04-19 01:55:38.000000 hak-0.0.6/hak/test/line_lengths_check.py
+-rw-rw-r--   0 a         (1009) a         (1010)      926 2023-04-19 01:55:38.000000 hak-0.0.6/hak/test/oldest_file_print.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.334879 hak-0.0.6/hak/tup/
+-rw-rw-r--   0 a         (1009) a         (1010)      176 2023-04-19 01:55:38.000000 hak-0.0.6/hak/tup/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      617 2023-04-19 01:55:38.000000 hak-0.0.6/hak/update_duration.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:12:37.322878 hak-0.0.6/hak.egg-info/
+-rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:12:37.000000 hak-0.0.6/hak.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1009) a         (1010)     7874 2023-04-19 10:12:37.000000 hak-0.0.6/hak.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1009) a         (1010)        1 2023-04-19 10:12:37.000000 hak-0.0.6/hak.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1009) a         (1010)     1606 2023-04-19 10:12:37.000000 hak-0.0.6/hak.egg-info/top_level.txt
+-rw-rw-r--   0 a         (1009) a         (1010)      536 2023-04-19 10:12:37.334879 hak-0.0.6/setup.cfg
+-rw-rw-r--   0 a         (1009) a         (1010)     2747 2023-04-19 10:12:37.000000 hak-0.0.6/setup.py
```

### Comparing `hak-0.0.5/LICENSE` & `hak-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/PKG-INFO` & `hak-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hak
-Version: 0.0.5
+Version: 0.0.6
 Summary: Function Test Pair Toolbox
 Home-page: https://github.com/JohnForbes/hak
 Author: @JohnRForbes
 Author-email: john.robert.forbes@gmail.com
 License: MIT
 Description: # hak
         This project is a collection of function test pairs for common tasks.
```

### Comparing `hak-0.0.5/hak/check_if_ok_to_proceed.py` & `hak-0.0.6/hak/check_if_ok_to_proceed.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/date/public_holiday/is_a.py` & `hak-0.0.6/hak/date/public_holiday/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/date/to_utc_timestamp.py` & `hak-0.0.6/hak/date/to_utc_timestamp.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/date/year/easter_sunday/get.py` & `hak-0.0.6/hak/date/year/easter_sunday/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/dict/proposed_dismantlement/show.py` & `hak-0.0.6/hak/dict/proposed_dismantlement/show.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/dict/to_max_line_width_str.py` & `hak-0.0.6/hak/dict/to_max_line_width_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/dicts/compare.py` & `hak-0.0.6/hak/dicts/compare.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/dicts/merge_freq_dicts.py` & `hak-0.0.6/hak/dicts/merge_freq_dicts.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/directories/exist.py` & `hak-0.0.6/hak/directories/exist.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/directory/compress_to_tar.py` & `hak-0.0.6/hak/directory/compress_to_tar.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/directory/empty.py` & `hak-0.0.6/hak/directory/empty.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/directory/get_most_recently_modified.py` & `hak-0.0.6/hak/directory/get_most_recently_modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from hak.directory.make import f as mkdir
+from hak.directory.make import f as mkdirine
 from hak.file.save import f as save
 from hak.directory.remove import f as rmdir
 from hak.string.print_and_return_false import f as pf
 from os.path import getmtime
 from hak.list.strings.filepaths.get import f as get_filepaths
 
 def f(x):
@@ -15,15 +15,15 @@
   return newest['file']
 
 def up():
   x = {}
   x['dir_name'] = './test_directory_get_most_recently_modified'
   
   # Create test directory
-  mkdir(x['dir_name'])
+  mkdirine(x['dir_name'])
 
   # create old file
   x['old_file_content'] = 'ABC'
   x['old_file_path'] = f"{x['dir_name']}/old_file.txt"
   save(x['old_file_path'], x['old_file_content'])
 
   # create new file
```

### Comparing `hak-0.0.5/hak/directory/is_module.py` & `hak-0.0.6/hak/directory/is_module.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/directory/make.py` & `hak-0.0.6/hak/directory/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/directory/remove.py` & `hak-0.0.6/hak/directory/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/duration.py` & `hak-0.0.6/hak/duration.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/duration_bar.py` & `hak-0.0.6/hak/duration_bar.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/fake/subprocess/run.py` & `hak-0.0.6/hak/fake/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/__init__.py` & `hak-0.0.6/hak/file/__init__.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/decrypt.py` & `hak-0.0.6/hak/file/decrypt.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/encrypt.py` & `hak-0.0.6/hak/file/encrypt.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/load.py` & `hak-0.0.6/hak/file/load.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/pickle/load_if_exists.py` & `hak-0.0.6/hak/file/pickle/load_if_exists.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/pickle/save.py` & `hak-0.0.6/hak/file/pickle/save.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/py/create.py` & `hak-0.0.6/hak/file/py/create.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/py/dismantle.py` & `hak-0.0.6/hak/file/py/dismantle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/py/extract_fn.py` & `hak-0.0.6/hak/file/py/extract_fn.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/save.py` & `hak-0.0.6/hak/file/save.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/save_lines.py` & `hak-0.0.6/hak/file/save_lines.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/secret/password/get.py` & `hak-0.0.6/hak/file/secret/password/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/secret/username/get.py` & `hak-0.0.6/hak/file/secret/username/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/file/tar/extract.py` & `hak-0.0.6/hak/file/tar/extract.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/files/pyfiles/dismantle.py` & `hak-0.0.6/hak/files/pyfiles/dismantle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/int/get_prime_factorisation.py` & `hak-0.0.6/hak/int/get_prime_factorisation.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/list/strings/compare.py` & `hak-0.0.6/hak/list/strings/compare.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/list/strings/find_first_diff.py` & `hak-0.0.6/hak/list/strings/find_first_diff.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/list/strings/patch_setup_py.py` & `hak-0.0.6/hak/list/strings/patch_setup_py.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/list/strings/pyfiles/filter_out_items.py` & `hak-0.0.6/hak/list/strings/pyfiles/filter_out_items.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/list/strings/show_diff.py` & `hak-0.0.6/hak/list/strings/show_diff.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/list/strings/to_dict.py` & `hak-0.0.6/hak/list/strings/to_dict.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/load_durations_if_exists.py` & `hak-0.0.6/hak/load_durations_if_exists.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/patch/do.py` & `hak-0.0.6/hak/patch/do.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/pip/dist_tar/make.py` & `hak-0.0.6/hak/pip/dist_tar/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/pip/dist_tar/remove.py` & `hak-0.0.6/hak/pip/dist_tar/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/pip/setup/update.py` & `hak-0.0.6/hak/pip/setup/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/pip/upload.py` & `hak-0.0.6/hak/pip/upload.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/pip/version/get.py` & `hak-0.0.6/hak/pip/version/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/pyfiles/format_and_commit.py` & `hak-0.0.6/hak/pyfiles/format_and_commit.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/report/fail/no_xyz.py` & `hak-0.0.6/hak/report/fail/no_xyz.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/report/fail/xyz.py` & `hak-0.0.6/hak/report/fail/xyz.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/report/fail/z_return_neq_y_return.py` & `hak-0.0.6/hak/report/fail/z_return_neq_y_return.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/report/fail/z_stdo_neq_y_stdo.py` & `hak-0.0.6/hak/report/fail/z_stdo_neq_y_stdo.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/report/property_failure.py` & `hak-0.0.6/hak/report/property_failure.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/report/success.py` & `hak-0.0.6/hak/report/success.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/save_durations.py` & `hak-0.0.6/hak/save_durations.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/schedule/make.py` & `hak-0.0.6/hak/schedule/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/select_text_colour_from_width.py` & `hak-0.0.6/hak/select_text_colour_from_width.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/setup/cfg/update.py` & `hak-0.0.6/hak/setup/cfg/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/setup/py/update.py` & `hak-0.0.6/hak/setup/py/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/camel_to_snake.py` & `hak-0.0.6/hak/string/camel_to_snake.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/chars/remove.py` & `hak-0.0.6/hak/string/chars/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/colour/rainbow.py` & `hak-0.0.6/hak/string/colour/rainbow.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/delete_character_safely.py` & `hak-0.0.6/hak/string/delete_character_safely.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/family_name/fake.py` & `hak-0.0.6/hak/string/family_name/fake.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/format.py` & `hak-0.0.6/hak/string/format.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/insert/new_line_after_last_import_line.py` & `hak-0.0.6/hak/string/insert/new_line_after_last_import_line.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/insert/new_line_before_def.py` & `hak-0.0.6/hak/string/insert/new_line_before_def.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/insert/new_line_before_lambda.py` & `hak-0.0.6/hak/string/insert/new_line_before_lambda.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/lambdarise.py` & `hak-0.0.6/hak/string/lambdarise.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/password/create.py` & `hak-0.0.6/hak/string/password/create.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/password/has_chars_from_3_sets.py` & `hak-0.0.6/hak/string/password/has_chars_from_3_sets.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/print_and_return_false.py` & `hak-0.0.6/hak/string/print_and_return_false.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/refactor/by_two_char_combinations.py` & `hak-0.0.6/hak/string/refactor/by_two_char_combinations.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/separate_function_from_context.py` & `hak-0.0.6/hak/string/separate_function_from_context.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/string/token/substitute.py` & `hak-0.0.6/hak/string/token/substitute.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/subprocess/completed_process/to_str.py` & `hak-0.0.6/hak/subprocess/completed_process/to_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/system/git/commit/run.py` & `hak-0.0.6/hak/system/git/commit/run.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/system/git/gitignore/make.py` & `hak-0.0.6/hak/system/git/gitignore/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/system/git/log_oneline.py` & `hak-0.0.6/hak/system/git/log_oneline.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/system/git/push_after_delay.py` & `hak-0.0.6/hak/system/git/push_after_delay.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/system/screen/clear.py` & `hak-0.0.6/hak/system/screen/clear.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/terminal.py` & `hak-0.0.6/hak/terminal.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/test/check_final_line.py` & `hak-0.0.6/hak/test/check_final_line.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/test/check_line_lengths.py` & `hak-0.0.6/hak/test/check_line_lengths.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/test/do.py` & `hak-0.0.6/hak/test/do.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/test/final_line_check.py` & `hak-0.0.6/hak/test/final_line_check.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/test/line_lengths_check.py` & `hak-0.0.6/hak/test/line_lengths_check.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/test/oldest_file_print.py` & `hak-0.0.6/hak/test/oldest_file_print.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak/update_duration.py` & `hak-0.0.6/hak/update_duration.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak.egg-info/PKG-INFO` & `hak-0.0.6/hak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hak
-Version: 0.0.5
+Version: 0.0.6
 Summary: Function Test Pair Toolbox
 Home-page: https://github.com/JohnForbes/hak
 Author: @JohnRForbes
 Author-email: john.robert.forbes@gmail.com
 License: MIT
 Description: # hak
         This project is a collection of function test pairs for common tasks.
```

### Comparing `hak-0.0.5/hak.egg-info/SOURCES.txt` & `hak-0.0.6/hak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/hak.egg-info/top_level.txt` & `hak-0.0.6/hak.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `hak-0.0.5/setup.cfg` & `hak-0.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hak
-version = 0.0.5
+version = 0.0.6
 author = John Forbes
 author_email = john.robert.forbes@gmail.com
 description = Function Test Pair Toolbox
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JohnForbes/hak
 license_files = LICENSE
```

### Comparing `hak-0.0.5/setup.py` & `hak-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 long_description = Path("./README.md").read_text()
 
 setup(
   name='hak',
-  version='0.0.5',
+  version='0.0.6',
   license='MIT',
   description='Function Test Pair Toolbox',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='@JohnRForbes',
   author_email='john.robert.forbes@gmail.com',
   url='https://github.com/JohnForbes/hak',
```

