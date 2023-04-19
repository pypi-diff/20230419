# Comparing `tmp/hak-0.0.1.tar.gz` & `tmp/hak-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hak-0.0.1.tar", last modified: Sun Apr 16 14:04:46 2023, max compression
+gzip compressed data, was "hak-0.0.2.tar", last modified: Wed Apr 19 03:16:26 2023, max compression
```

## Comparing `hak-0.0.1.tar` & `hak-0.0.2.tar`

### file list

```diff
@@ -1,363 +1,364 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.440691 hak-0.0.1/
--rw-rw-r--   0 j         (1000) j         (1000)     1068 2023-04-16 03:24:25.000000 hak-0.0.1/LICENSE
--rw-rw-r--   0 j         (1000) j         (1000)      893 2023-04-16 14:04:46.440691 hak-0.0.1/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      422 2023-04-16 05:07:28.000000 hak-0.0.1/README.md
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.320689 hak-0.0.1/hak/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 06:10:17.000000 hak-0.0.1/hak/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      140 2023-04-16 08:42:22.000000 hak-0.0.1/hak/a_equals_b.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.324689 hak-0.0.1/hak/bool/
--rw-rw-r--   0 j         (1000) j         (1000)       86 2023-04-16 08:44:03.000000 hak-0.0.1/hak/bool/fake.py
--rw-rw-r--   0 j         (1000) j         (1000)      103 2023-04-16 08:42:10.000000 hak-0.0.1/hak/bool/is_a.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.324689 hak-0.0.1/hak/bool/or_none/
--rw-rw-r--   0 j         (1000) j         (1000)      160 2023-04-16 08:45:15.000000 hak-0.0.1/hak/bool/or_none/fake.py
--rw-rw-r--   0 j         (1000) j         (1000)      125 2023-04-16 10:05:07.000000 hak-0.0.1/hak/bool/or_none/is_a.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.324689 hak-0.0.1/hak/bools/
--rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-16 10:05:53.000000 hak-0.0.1/hak/bools/count_true.py
--rw-rw-r--   0 j         (1000) j         (1000)      249 2023-04-16 10:06:38.000000 hak-0.0.1/hak/calculate_duration_bar_width.py
--rw-rw-r--   0 j         (1000) j         (1000)      758 2023-04-16 10:07:01.000000 hak-0.0.1/hak/check_if_ok_to_proceed.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.332689 hak-0.0.1/hak/date/
--rw-rw-r--   0 j         (1000) j         (1000)      143 2023-04-16 10:07:17.000000 hak-0.0.1/hak/date/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      347 2023-04-16 05:42:47.000000 hak-0.0.1/hak/date/is_first_second_or_third_day_of_month.py
--rw-rw-r--   0 j         (1000) j         (1000)      414 2023-04-16 05:43:44.000000 hak-0.0.1/hak/date/is_first_week_of_quarter.py
--rw-rw-r--   0 j         (1000) j         (1000)      208 2023-04-16 05:44:40.000000 hak-0.0.1/hak/date/is_monday.py
--rw-rw-r--   0 j         (1000) j         (1000)      462 2023-04-16 10:07:59.000000 hak-0.0.1/hak/date/is_weekday.py
--rw-rw-r--   0 j         (1000) j         (1000)      467 2023-04-16 10:08:30.000000 hak-0.0.1/hak/date/is_weekend.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.332689 hak-0.0.1/hak/date/public_holiday/
--rw-rw-r--   0 j         (1000) j         (1000)     5617 2023-04-16 05:41:31.000000 hak-0.0.1/hak/date/public_holiday/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      385 2023-04-16 08:43:58.000000 hak-0.0.1/hak/date/select_from_last_n_days.py
--rw-rw-r--   0 j         (1000) j         (1000)      146 2023-04-16 10:09:08.000000 hak-0.0.1/hak/date/to_dd_mm_yyyy_str.py
--rw-rw-r--   0 j         (1000) j         (1000)      568 2023-04-16 08:43:58.000000 hak-0.0.1/hak/date/to_timestamp.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.288689 hak-0.0.1/hak/date/year/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.332689 hak-0.0.1/hak/date/year/easter_sunday/
--rw-rw-r--   0 j         (1000) j         (1000)     1006 2023-04-16 05:41:31.000000 hak-0.0.1/hak/date/year/easter_sunday/get.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.332689 hak-0.0.1/hak/datetime/
--rw-rw-r--   0 j         (1000) j         (1000)      149 2023-04-16 10:09:36.000000 hak-0.0.1/hak/datetime/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      272 2023-04-16 10:10:01.000000 hak-0.0.1/hak/datetime/select_from_last_n_days.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.336689 hak-0.0.1/hak/dict/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 07:16:40.000000 hak-0.0.1/hak/dict/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      215 2023-04-16 10:13:51.000000 hak-0.0.1/hak/dict/convert_to_sql_insertable.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.336689 hak-0.0.1/hak/dict/frequencies/
--rw-rw-r--   0 j         (1000) j         (1000)      356 2023-04-16 05:43:02.000000 hak-0.0.1/hak/dict/frequencies/choose.py
--rw-rw-r--   0 j         (1000) j         (1000)      376 2023-04-16 05:44:08.000000 hak-0.0.1/hak/dict/frequencies/make_from_strings.py
--rw-rw-r--   0 j         (1000) j         (1000)      187 2023-04-16 10:14:30.000000 hak-0.0.1/hak/dict/get_or_default.py
--rw-rw-r--   0 j         (1000) j         (1000)      190 2023-04-16 11:34:27.000000 hak-0.0.1/hak/dict/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      116 2023-04-16 11:35:53.000000 hak-0.0.1/hak/dict/make_from_key_value_lists.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.336689 hak-0.0.1/hak/dict/proposed_dismantlement/
--rw-rw-r--   0 j         (1000) j         (1000)     1520 2023-04-16 08:42:22.000000 hak-0.0.1/hak/dict/proposed_dismantlement/show.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.336689 hak-0.0.1/hak/dict/test_durations/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 07:17:04.000000 hak-0.0.1/hak/dict/test_durations/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      134 2023-04-16 11:37:31.000000 hak-0.0.1/hak/dict/test_durations/to_tuple_list_sorted_by_duration.py
--rw-rw-r--   0 j         (1000) j         (1000)     4011 2023-04-16 08:43:58.000000 hak-0.0.1/hak/dict/to_max_line_width_str.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.340689 hak-0.0.1/hak/dicts/
--rw-rw-r--   0 j         (1000) j         (1000)      151 2023-04-16 11:39:13.000000 hak-0.0.1/hak/dicts/a_into_b.py
--rw-rw-r--   0 j         (1000) j         (1000)     1200 2023-04-16 06:15:59.000000 hak-0.0.1/hak/dicts/compare.py
--rw-rw-r--   0 j         (1000) j         (1000)      195 2023-04-16 11:40:55.000000 hak-0.0.1/hak/dicts/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      663 2023-04-16 06:17:02.000000 hak-0.0.1/hak/dicts/merge_freq_dicts.py
--rw-rw-r--   0 j         (1000) j         (1000)      251 2023-04-16 08:42:22.000000 hak-0.0.1/hak/dicts/reindex.py
--rw-rw-r--   0 j         (1000) j         (1000)      203 2023-04-16 11:43:35.000000 hak-0.0.1/hak/dicts/sort_by_key.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.340689 hak-0.0.1/hak/directories/
--rw-rw-r--   0 j         (1000) j         (1000)      567 2023-04-16 08:43:58.000000 hak-0.0.1/hak/directories/exist.py
--rw-rw-r--   0 j         (1000) j         (1000)      432 2023-04-16 06:21:38.000000 hak-0.0.1/hak/directories/make.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.344689 hak-0.0.1/hak/directory/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 06:57:25.000000 hak-0.0.1/hak/directory/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     1548 2023-04-16 06:22:08.000000 hak-0.0.1/hak/directory/compress_to_tar.py
--rw-rw-r--   0 j         (1000) j         (1000)      520 2023-04-16 11:43:54.000000 hak-0.0.1/hak/directory/empty.py
--rw-rw-r--   0 j         (1000) j         (1000)       88 2023-04-16 11:47:59.000000 hak-0.0.1/hak/directory/exists.py
--rw-rw-r--   0 j         (1000) j         (1000)      654 2023-04-16 05:41:33.000000 hak-0.0.1/hak/directory/make.py
--rw-rw-r--   0 j         (1000) j         (1000)      782 2023-04-16 05:41:33.000000 hak-0.0.1/hak/directory/remove.py
--rw-rw-r--   0 j         (1000) j         (1000)     3692 2023-04-16 08:42:22.000000 hak-0.0.1/hak/duration.py
--rw-rw-r--   0 j         (1000) j         (1000)     2021 2023-04-16 08:42:22.000000 hak-0.0.1/hak/duration_bar.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.344689 hak-0.0.1/hak/fake/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 06:44:53.000000 hak-0.0.1/hak/fake/__init__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.348689 hak-0.0.1/hak/fake/os/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 09:41:04.000000 hak-0.0.1/hak/fake/os/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      418 2023-04-16 08:43:58.000000 hak-0.0.1/hak/fake/os/system.py
--rw-rw-r--   0 j         (1000) j         (1000)      424 2023-04-16 08:43:58.000000 hak-0.0.1/hak/fake/printer.py
--rw-rw-r--   0 j         (1000) j         (1000)       45 2023-04-16 08:42:10.000000 hak-0.0.1/hak/fake/sleep.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.348689 hak-0.0.1/hak/fake/subprocess/
--rw-rw-r--   0 j         (1000) j         (1000)     5824 2023-04-16 06:39:03.000000 hak-0.0.1/hak/fake/subprocess/run.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.352690 hak-0.0.1/hak/file/
--rw-rw-r--   0 j         (1000) j         (1000)     1253 2023-04-16 08:42:22.000000 hak-0.0.1/hak/file/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      785 2023-04-16 06:40:55.000000 hak-0.0.1/hak/file/decrypt.py
--rw-rw-r--   0 j         (1000) j         (1000)      929 2023-04-16 06:41:14.000000 hak-0.0.1/hak/file/encrypt.py
--rw-rw-r--   0 j         (1000) j         (1000)      697 2023-04-16 05:41:31.000000 hak-0.0.1/hak/file/load.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.352690 hak-0.0.1/hak/file/pickle/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 06:55:47.000000 hak-0.0.1/hak/file/pickle/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     1253 2023-04-16 08:42:22.000000 hak-0.0.1/hak/file/pickle/load_if_exists.py
--rw-rw-r--   0 j         (1000) j         (1000)      906 2023-04-16 05:41:31.000000 hak-0.0.1/hak/file/pickle/save.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.356690 hak-0.0.1/hak/file/py/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 09:26:10.000000 hak-0.0.1/hak/file/py/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      546 2023-04-16 08:43:58.000000 hak-0.0.1/hak/file/py/create.py
--rw-rw-r--   0 j         (1000) j         (1000)     2644 2023-04-16 06:58:27.000000 hak-0.0.1/hak/file/py/dismantle.py
--rw-rw-r--   0 j         (1000) j         (1000)     3819 2023-04-16 06:58:40.000000 hak-0.0.1/hak/file/py/extract_fn.py
--rw-rw-r--   0 j         (1000) j         (1000)       84 2023-04-16 12:31:07.000000 hak-0.0.1/hak/file/py/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      337 2023-04-16 05:41:31.000000 hak-0.0.1/hak/file/remove.py
--rw-rw-r--   0 j         (1000) j         (1000)      956 2023-04-16 05:41:31.000000 hak-0.0.1/hak/file/save.py
--rw-rw-r--   0 j         (1000) j         (1000)      761 2023-04-16 06:58:56.000000 hak-0.0.1/hak/file/save_lines.py
--rw-rw-r--   0 j         (1000) j         (1000)      308 2023-04-16 12:31:28.000000 hak-0.0.1/hak/file/save_lines_or_string.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.292688 hak-0.0.1/hak/file/secret/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.356690 hak-0.0.1/hak/file/secret/password/
--rw-rw-r--   0 j         (1000) j         (1000)      680 2023-04-16 06:59:49.000000 hak-0.0.1/hak/file/secret/password/get.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.356690 hak-0.0.1/hak/file/secret/username/
--rw-rw-r--   0 j         (1000) j         (1000)      713 2023-04-16 07:00:01.000000 hak-0.0.1/hak/file/secret/username/get.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.356690 hak-0.0.1/hak/file/tar/
--rw-rw-r--   0 j         (1000) j         (1000)     1562 2023-04-16 07:00:34.000000 hak-0.0.1/hak/file/tar/extract.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.356690 hak-0.0.1/hak/file/zip/
--rw-rw-r--   0 j         (1000) j         (1000)      487 2023-04-16 07:01:10.000000 hak-0.0.1/hak/file/zip/extract.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.292688 hak-0.0.1/hak/files/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.356690 hak-0.0.1/hak/files/pyfiles/
--rw-rw-r--   0 j         (1000) j         (1000)     1760 2023-04-16 08:43:58.000000 hak-0.0.1/hak/files/pyfiles/dismantle.py
--rw-rw-r--   0 j         (1000) j         (1000)      100 2023-04-16 12:31:52.000000 hak-0.0.1/hak/find_first_parenthesis.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.360690 hak-0.0.1/hak/float/
--rw-rw-r--   0 j         (1000) j         (1000)       70 2023-04-16 12:32:12.000000 hak-0.0.1/hak/float/epsilon.py
--rw-rw-r--   0 j         (1000) j         (1000)      106 2023-04-16 12:32:36.000000 hak-0.0.1/hak/float/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      106 2023-04-16 12:32:57.000000 hak-0.0.1/hak/float/is_not.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.360690 hak-0.0.1/hak/float/nan/
--rw-rw-r--   0 j         (1000) j         (1000)      151 2023-04-16 08:42:22.000000 hak-0.0.1/hak/float/nan/to_none.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.360690 hak-0.0.1/hak/function/
--rw-rw-r--   0 j         (1000) j         (1000)      211 2023-04-16 08:43:58.000000 hak-0.0.1/hak/function/function.py
--rw-rw-r--   0 j         (1000) j         (1000)      423 2023-04-16 12:35:15.000000 hak-0.0.1/hak/function/write_to_file.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.360690 hak-0.0.1/hak/int/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.360690 hak-0.0.1/hak/int/days/
--rw-rw-r--   0 j         (1000) j         (1000)      227 2023-04-16 08:43:58.000000 hak-0.0.1/hak/int/days/a_to_b_inclusive.py
--rw-rw-r--   0 j         (1000) j         (1000)      661 2023-04-16 07:06:33.000000 hak-0.0.1/hak/int/get_prime_factorisation.py
--rw-rw-r--   0 j         (1000) j         (1000)      104 2023-04-16 12:37:04.000000 hak-0.0.1/hak/int/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      426 2023-04-16 08:43:58.000000 hak-0.0.1/hak/int/is_prime.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.364690 hak-0.0.1/hak/int/year/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.364690 hak-0.0.1/hak/int/year/days/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.364690 hak-0.0.1/hak/int/year/days/count/
--rw-rw-r--   0 j         (1000) j         (1000)      128 2023-04-16 12:37:28.000000 hak-0.0.1/hak/int/year/days/count/get.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.364690 hak-0.0.1/hak/int/year/days/first/
--rw-rw-r--   0 j         (1000) j         (1000)      154 2023-04-16 08:43:58.000000 hak-0.0.1/hak/int/year/days/first/get.py
--rw-rw-r--   0 j         (1000) j         (1000)      420 2023-04-16 08:43:58.000000 hak-0.0.1/hak/int/year/days/get.py
--rw-rw-r--   0 j         (1000) j         (1000)      153 2023-04-16 12:37:50.000000 hak-0.0.1/hak/int/year/now.py
--rw-rw-r--   0 j         (1000) j         (1000)      448 2023-04-16 08:43:48.000000 hak-0.0.1/hak/l.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.364690 hak-0.0.1/hak/list/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 08:09:27.000000 hak-0.0.1/hak/list/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      116 2023-04-16 12:39:15.000000 hak-0.0.1/hak/list/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      115 2023-04-16 12:41:47.000000 hak-0.0.1/hak/list/to_comma_separated_str.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.364690 hak-0.0.1/hak/lists/
--rw-rw-r--   0 j         (1000) j         (1000)      216 2023-04-16 12:42:12.000000 hak-0.0.1/hak/lists/merge.py
--rw-rw-r--   0 j         (1000) j         (1000)     1131 2023-04-16 08:43:58.000000 hak-0.0.1/hak/load_durations_if_exists.py
--rw-rw-r--   0 j         (1000) j         (1000)      123 2023-04-16 12:42:36.000000 hak-0.0.1/hak/log_2.py
--rw-rw-r--   0 j         (1000) j         (1000)       84 2023-04-16 12:42:54.000000 hak-0.0.1/hak/nop.py
--rw-rw-r--   0 j         (1000) j         (1000)       91 2023-04-16 12:43:08.000000 hak-0.0.1/hak/nop_state_x.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.364690 hak-0.0.1/hak/patch/
--rw-rw-r--   0 j         (1000) j         (1000)     3624 2023-04-16 14:00:42.000000 hak-0.0.1/hak/patch/do.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.368690 hak-0.0.1/hak/period/
--rw-rw-r--   0 j         (1000) j         (1000)      333 2023-04-16 12:43:27.000000 hak-0.0.1/hak/period/contains_day.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.368690 hak-0.0.1/hak/pip/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.368690 hak-0.0.1/hak/pip/dist_tar/
--rw-rw-r--   0 j         (1000) j         (1000)     2749 2023-04-16 08:43:58.000000 hak-0.0.1/hak/pip/dist_tar/make.py
--rw-rw-r--   0 j         (1000) j         (1000)      403 2023-04-16 07:14:24.000000 hak-0.0.1/hak/pip/dist_tar/remove.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.368690 hak-0.0.1/hak/pip/setup/
--rw-rw-r--   0 j         (1000) j         (1000)     1300 2023-04-16 08:43:58.000000 hak-0.0.1/hak/pip/setup/update.py
--rw-rw-r--   0 j         (1000) j         (1000)      920 2023-04-16 05:41:33.000000 hak-0.0.1/hak/pip/upload.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.368690 hak-0.0.1/hak/pip/version/
--rw-rw-r--   0 j         (1000) j         (1000)      837 2023-04-16 14:01:02.000000 hak-0.0.1/hak/pip/version/get.py
--rw-rw-r--   0 j         (1000) j         (1000)      120 2023-04-16 12:43:46.000000 hak-0.0.1/hak/pip/version/to_str.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.368690 hak-0.0.1/hak/pyfiles/
--rw-rw-r--   0 j         (1000) j         (1000)      157 2023-04-16 12:44:08.000000 hak-0.0.1/hak/pyfiles/format.py
--rw-rw-r--   0 j         (1000) j         (1000)      833 2023-04-16 08:42:22.000000 hak-0.0.1/hak/pyfiles/format_and_commit.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.372690 hak-0.0.1/hak/report/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.372690 hak-0.0.1/hak/report/fail/
--rw-rw-r--   0 j         (1000) j         (1000)      814 2023-04-16 08:43:58.000000 hak-0.0.1/hak/report/fail/no_xyz.py
--rw-rw-r--   0 j         (1000) j         (1000)     1914 2023-04-16 08:43:58.000000 hak-0.0.1/hak/report/fail/xyz.py
--rw-rw-r--   0 j         (1000) j         (1000)     1440 2023-04-16 08:43:58.000000 hak-0.0.1/hak/report/fail/z_return_neq_y_return.py
--rw-rw-r--   0 j         (1000) j         (1000)     1601 2023-04-16 08:43:58.000000 hak-0.0.1/hak/report/fail/z_stdo_neq_y_stdo.py
--rw-rw-r--   0 j         (1000) j         (1000)      887 2023-04-16 08:43:58.000000 hak-0.0.1/hak/report/property_failure.py
--rw-rw-r--   0 j         (1000) j         (1000)      729 2023-04-16 08:43:58.000000 hak-0.0.1/hak/report/success.py
--rw-rw-r--   0 j         (1000) j         (1000)      394 2023-04-16 08:42:22.000000 hak-0.0.1/hak/report/summarise_file.py
--rw-rw-r--   0 j         (1000) j         (1000)      758 2023-04-16 08:43:58.000000 hak-0.0.1/hak/save_durations.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.372690 hak-0.0.1/hak/schedule/
--rw-rw-r--   0 j         (1000) j         (1000)     3465 2023-04-16 07:21:00.000000 hak-0.0.1/hak/schedule/make.py
--rw-rw-r--   0 j         (1000) j         (1000)      559 2023-04-16 08:43:58.000000 hak-0.0.1/hak/select_text_colour_from_width.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.372690 hak-0.0.1/hak/session/
--rw-rw-r--   0 j         (1000) j         (1000)      146 2023-04-16 12:45:12.000000 hak-0.0.1/hak/session/is_a.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.376690 hak-0.0.1/hak/set/
--rw-rw-r--   0 j         (1000) j         (1000)      114 2023-04-16 12:48:59.000000 hak-0.0.1/hak/set/is_a.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.300689 hak-0.0.1/hak/setup/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.376690 hak-0.0.1/hak/setup/cfg/
--rw-rw-r--   0 j         (1000) j         (1000)     1412 2023-04-16 07:22:54.000000 hak-0.0.1/hak/setup/cfg/update.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.376690 hak-0.0.1/hak/setup/py/
--rw-rw-r--   0 j         (1000) j         (1000)     1465 2023-04-16 07:23:27.000000 hak-0.0.1/hak/setup/py/update.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.392690 hak-0.0.1/hak/string/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 06:22:58.000000 hak-0.0.1/hak/string/__init__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.392690 hak-0.0.1/hak/string/alphanumeric/
--rw-rw-r--   0 j         (1000) j         (1000)      264 2023-04-16 12:50:26.000000 hak-0.0.1/hak/string/alphanumeric/fake.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.392690 hak-0.0.1/hak/string/append/
--rw-rw-r--   0 j         (1000) j         (1000)       54 2023-04-16 12:52:07.000000 hak-0.0.1/hak/string/append/new_line.py
--rw-rw-r--   0 j         (1000) j         (1000)      541 2023-04-16 13:10:49.000000 hak-0.0.1/hak/string/camel_to_snake.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.396690 hak-0.0.1/hak/string/char/
--rw-rw-r--   0 j         (1000) j         (1000)      322 2023-04-16 13:11:18.000000 hak-0.0.1/hak/string/char/find_all_indices.py
--rw-rw-r--   0 j         (1000) j         (1000)      128 2023-04-16 13:13:11.000000 hak-0.0.1/hak/string/char/is_digit.py
--rw-rw-r--   0 j         (1000) j         (1000)      207 2023-04-16 13:14:37.000000 hak-0.0.1/hak/string/char/is_upper.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.396690 hak-0.0.1/hak/string/chars/
--rw-rw-r--   0 j         (1000) j         (1000)      561 2023-04-16 08:43:58.000000 hak-0.0.1/hak/string/chars/remove.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.400690 hak-0.0.1/hak/string/colour/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 06:23:13.000000 hak-0.0.1/hak/string/colour/__init__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.404690 hak-0.0.1/hak/string/colour/bright/
--rw-rw-r--   0 j         (1000) j         (1000)      162 2023-04-16 13:16:50.000000 hak-0.0.1/hak/string/colour/bright/blue.py
--rw-rw-r--   0 j         (1000) j         (1000)      162 2023-04-16 13:17:41.000000 hak-0.0.1/hak/string/colour/bright/cyan.py
--rw-rw-r--   0 j         (1000) j         (1000)      164 2023-04-16 13:20:07.000000 hak-0.0.1/hak/string/colour/bright/green.py
--rw-rw-r--   0 j         (1000) j         (1000)      168 2023-04-16 08:43:48.000000 hak-0.0.1/hak/string/colour/bright/magenta.py
--rw-rw-r--   0 j         (1000) j         (1000)      160 2023-04-16 13:21:30.000000 hak-0.0.1/hak/string/colour/bright/red.py
--rw-rw-r--   0 j         (1000) j         (1000)      164 2023-04-16 13:22:04.000000 hak-0.0.1/hak/string/colour/bright/white.py
--rw-rw-r--   0 j         (1000) j         (1000)      166 2023-04-16 13:22:53.000000 hak-0.0.1/hak/string/colour/bright/yellow.py
--rw-rw-r--   0 j         (1000) j         (1000)      130 2023-04-16 13:23:33.000000 hak-0.0.1/hak/string/colour/danger.py
--rw-rw-r--   0 j         (1000) j         (1000)      174 2023-04-16 13:25:12.000000 hak-0.0.1/hak/string/colour/danger_if_zero.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.408691 hak-0.0.1/hak/string/colour/dark/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-16 05:16:31.000000 hak-0.0.1/hak/string/colour/dark/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      148 2023-04-16 13:26:19.000000 hak-0.0.1/hak/string/colour/dark/blue.py
--rw-rw-r--   0 j         (1000) j         (1000)      148 2023-04-16 13:26:42.000000 hak-0.0.1/hak/string/colour/dark/cyan.py
--rw-rw-r--   0 j         (1000) j         (1000)      154 2023-04-16 13:28:45.000000 hak-0.0.1/hak/string/colour/dark/default.py
--rw-rw-r--   0 j         (1000) j         (1000)      150 2023-04-16 13:29:17.000000 hak-0.0.1/hak/string/colour/dark/green.py
--rw-rw-r--   0 j         (1000) j         (1000)      154 2023-04-16 13:29:49.000000 hak-0.0.1/hak/string/colour/dark/magenta.py
--rw-rw-r--   0 j         (1000) j         (1000)      146 2023-04-16 13:30:13.000000 hak-0.0.1/hak/string/colour/dark/red.py
--rw-rw-r--   0 j         (1000) j         (1000)      150 2023-04-16 13:30:47.000000 hak-0.0.1/hak/string/colour/dark/white.py
--rw-rw-r--   0 j         (1000) j         (1000)      152 2023-04-16 13:31:28.000000 hak-0.0.1/hak/string/colour/dark/yellow.py
--rw-rw-r--   0 j         (1000) j         (1000)       64 2023-04-15 06:25:57.000000 hak-0.0.1/hak/string/colour/data.py
--rw-rw-r--   0 j         (1000) j         (1000)      131 2023-04-16 08:43:48.000000 hak-0.0.1/hak/string/colour/info.py
--rw-rw-r--   0 j         (1000) j         (1000)      131 2023-04-16 13:32:19.000000 hak-0.0.1/hak/string/colour/primary.py
--rw-rw-r--   0 j         (1000) j         (1000)     2261 2023-04-16 08:35:41.000000 hak-0.0.1/hak/string/colour/rainbow.py
--rw-rw-r--   0 j         (1000) j         (1000)      134 2023-04-16 13:32:45.000000 hak-0.0.1/hak/string/colour/secondary.py
--rw-rw-r--   0 j         (1000) j         (1000)      267 2023-04-16 13:33:07.000000 hak-0.0.1/hak/string/colour/tgfr.py
--rw-rw-r--   0 j         (1000) j         (1000)      135 2023-04-16 13:33:53.000000 hak-0.0.1/hak/string/colour/warning.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.412690 hak-0.0.1/hak/string/contains/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 13:48:05.000000 hak-0.0.1/hak/string/contains/__init__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.412690 hak-0.0.1/hak/string/contains/function/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 13:47:58.000000 hak-0.0.1/hak/string/contains/function/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      341 2023-04-16 08:43:58.000000 hak-0.0.1/hak/string/contains/function/run.py
--rw-rw-r--   0 j         (1000) j         (1000)      192 2023-04-16 13:34:13.000000 hak-0.0.1/hak/string/contains/function/test.py
--rw-rw-r--   0 j         (1000) j         (1000)      224 2023-04-16 13:35:17.000000 hak-0.0.1/hak/string/contains/l.py
--rw-rw-r--   0 j         (1000) j         (1000)       76 2023-04-16 13:43:46.000000 hak-0.0.1/hak/string/contains/version.py
--rw-rw-r--   0 j         (1000) j         (1000)      105 2023-04-16 13:44:22.000000 hak-0.0.1/hak/string/count_x_in_y.py
--rw-rw-r--   0 j         (1000) j         (1000)      996 2023-04-16 08:37:46.000000 hak-0.0.1/hak/string/delete_character_safely.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.412690 hak-0.0.1/hak/string/digits/
--rw-rw-r--   0 j         (1000) j         (1000)      202 2023-04-16 13:44:51.000000 hak-0.0.1/hak/string/digits/remove.py
--rw-rw-r--   0 j         (1000) j         (1000)      111 2023-04-16 13:45:26.000000 hak-0.0.1/hak/string/double_single_quotes.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.412690 hak-0.0.1/hak/string/family_name/
--rw-rw-r--   0 j         (1000) j         (1000)   115522 2023-04-16 08:42:22.000000 hak-0.0.1/hak/string/family_name/fake.py
--rw-rw-r--   0 j         (1000) j         (1000)      303 2023-04-16 08:42:59.000000 hak-0.0.1/hak/string/family_name/is_a.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/filename/
--rw-rw-r--   0 j         (1000) j         (1000)      126 2023-04-16 08:44:52.000000 hak-0.0.1/hak/string/filename/to_module_name.py
--rw-rw-r--   0 j         (1000) j         (1000)      209 2023-04-16 10:04:54.000000 hak-0.0.1/hak/string/find_last_comma_index.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/fn_name/
--rw-rw-r--   0 j         (1000) j         (1000)      226 2023-04-16 10:05:22.000000 hak-0.0.1/hak/string/fn_name/is_ignorable.py
--rw-rw-r--   0 j         (1000) j         (1000)     5309 2023-04-16 10:06:24.000000 hak-0.0.1/hak/string/format.py
--rw-rw-r--   0 j         (1000) j         (1000)       73 2023-04-16 10:06:50.000000 hak-0.0.1/hak/string/has_at_symbol.py
--rw-rw-r--   0 j         (1000) j         (1000)      132 2023-04-16 10:07:09.000000 hak-0.0.1/hak/string/has_digit.py
--rw-rw-r--   0 j         (1000) j         (1000)      131 2023-04-16 10:07:29.000000 hak-0.0.1/hak/string/has_lowercase.py
--rw-rw-r--   0 j         (1000) j         (1000)      259 2023-04-16 10:08:06.000000 hak-0.0.1/hak/string/has_other_char.py
--rw-rw-r--   0 j         (1000) j         (1000)      172 2023-04-16 10:08:41.000000 hak-0.0.1/hak/string/has_seven_digits.py
--rw-rw-r--   0 j         (1000) j         (1000)      132 2023-04-16 10:09:25.000000 hak-0.0.1/hak/string/has_uppercase.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/hbar/
--rw-rw-r--   0 j         (1000) j         (1000)      122 2023-04-16 10:09:43.000000 hak-0.0.1/hak/string/hbar/make.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.308689 hak-0.0.1/hak/string/header/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/header/python_file/
--rw-rw-r--   0 j         (1000) j         (1000)      314 2023-04-16 10:12:58.000000 hak-0.0.1/hak/string/header/python_file/make.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/header/test_table/
--rw-rw-r--   0 j         (1000) j         (1000)      461 2023-04-16 10:13:59.000000 hak-0.0.1/hak/string/header/test_table/make.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/indent/
--rw-rw-r--   0 j         (1000) j         (1000)      137 2023-04-16 10:14:50.000000 hak-0.0.1/hak/string/indent/run_if_class_method.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/insert/
--rw-rw-r--   0 j         (1000) j         (1000)      602 2023-04-16 11:34:46.000000 hak-0.0.1/hak/string/insert/new_line_after_last_import_line.py
--rw-rw-r--   0 j         (1000) j         (1000)      278 2023-04-16 11:37:14.000000 hak-0.0.1/hak/string/insert/new_line_before_comment.py
--rw-rw-r--   0 j         (1000) j         (1000)      584 2023-04-16 11:38:19.000000 hak-0.0.1/hak/string/insert/new_line_before_def.py
--rw-rw-r--   0 j         (1000) j         (1000)      251 2023-04-16 11:39:20.000000 hak-0.0.1/hak/string/insert/new_line_before_if_main.py
--rw-rw-r--   0 j         (1000) j         (1000)      666 2023-04-16 11:43:21.000000 hak-0.0.1/hak/string/insert/new_line_before_lambda.py
--rw-rw-r--   0 j         (1000) j         (1000)      292 2023-04-16 11:43:44.000000 hak-0.0.1/hak/string/insert/new_line_before_new_line_and_cea_.py
--rw-rw-r--   0 j         (1000) j         (1000)      102 2023-04-16 11:44:07.000000 hak-0.0.1/hak/string/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      124 2023-04-16 12:29:51.000000 hak-0.0.1/hak/string/is_or_none.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/json/
--rw-rw-r--   0 j         (1000) j         (1000)      179 2023-04-16 12:30:57.000000 hak-0.0.1/hak/string/json/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      548 2023-04-16 12:31:15.000000 hak-0.0.1/hak/string/lambdarise.py
--rw-rw-r--   0 j         (1000) j         (1000)      360 2023-04-16 12:31:59.000000 hak-0.0.1/hak/string/make_content_without_function.py
--rw-rw-r--   0 j         (1000) j         (1000)      325 2023-04-16 12:32:19.000000 hak-0.0.1/hak/string/make_function_text.py
--rw-rw-r--   0 j         (1000) j         (1000)      338 2023-04-16 12:32:46.000000 hak-0.0.1/hak/string/make_initial_content.py
--rw-rw-r--   0 j         (1000) j         (1000)      319 2023-04-16 12:33:05.000000 hak-0.0.1/hak/string/make_new_function_text.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/password/
--rw-rw-r--   0 j         (1000) j         (1000)     1179 2023-04-16 12:36:53.000000 hak-0.0.1/hak/string/password/create.py
--rw-rw-r--   0 j         (1000) j         (1000)      534 2023-04-16 12:37:13.000000 hak-0.0.1/hak/string/password/has_chars_from_3_sets.py
--rw-rw-r--   0 j         (1000) j         (1000)      207 2023-04-16 12:37:37.000000 hak-0.0.1/hak/string/pop_left.py
--rw-rw-r--   0 j         (1000) j         (1000)      219 2023-04-16 12:37:57.000000 hak-0.0.1/hak/string/pop_right.py
--rw-rw-r--   0 j         (1000) j         (1000)      151 2023-04-16 12:39:03.000000 hak-0.0.1/hak/string/prepend_import.py
--rw-rw-r--   0 j         (1000) j         (1000)      756 2023-04-16 05:41:33.000000 hak-0.0.1/hak/string/print_and_return_false.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.416691 hak-0.0.1/hak/string/refactor/
--rw-rw-r--   0 j         (1000) j         (1000)     1213 2023-04-16 12:41:35.000000 hak-0.0.1/hak/string/refactor/by_two_char_combinations.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.424691 hak-0.0.1/hak/string/remove/
--rw-rw-r--   0 j         (1000) j         (1000)      211 2023-04-16 12:41:55.000000 hak-0.0.1/hak/string/remove/empty_line_spaces.py
--rw-rw-r--   0 j         (1000) j         (1000)      162 2023-04-16 12:42:26.000000 hak-0.0.1/hak/string/remove/empty_lines.py
--rw-rw-r--   0 j         (1000) j         (1000)      441 2023-04-16 12:42:44.000000 hak-0.0.1/hak/string/remove/extra_new_line_following_class_definition.py
--rw-rw-r--   0 j         (1000) j         (1000)      210 2023-04-16 12:43:01.000000 hak-0.0.1/hak/string/remove/first_new_line_if_starts_with_new_line.py
--rw-rw-r--   0 j         (1000) j         (1000)       81 2023-04-16 12:43:18.000000 hak-0.0.1/hak/string/remove/whitespace_between_newlines.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.428691 hak-0.0.1/hak/string/replace/
--rw-rw-r--   0 j         (1000) j         (1000)      241 2023-04-16 12:43:35.000000 hak-0.0.1/hak/string/replace/double_new_line_with_single_new_line.py
--rw-rw-r--   0 j         (1000) j         (1000)      129 2023-04-16 12:43:55.000000 hak-0.0.1/hak/string/replace/single_new_line_with_empty_string.py
--rw-rw-r--   0 j         (1000) j         (1000)      251 2023-04-16 12:44:17.000000 hak-0.0.1/hak/string/replace/triple_new_line_with_double_new_line.py
--rw-rw-r--   0 j         (1000) j         (1000)      483 2023-04-16 12:48:39.000000 hak-0.0.1/hak/string/replace_unprintable.py
--rw-rw-r--   0 j         (1000) j         (1000)     3361 2023-04-16 12:49:49.000000 hak-0.0.1/hak/string/separate_function_from_context.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.428691 hak-0.0.1/hak/string/single_line_function/
--rw-rw-r--   0 j         (1000) j         (1000)      428 2023-04-16 12:51:29.000000 hak-0.0.1/hak/string/single_line_function/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      463 2023-04-16 13:09:24.000000 hak-0.0.1/hak/string/single_line_function/to_lambda_str.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.428691 hak-0.0.1/hak/string/spaces/
--rw-rw-r--   0 j         (1000) j         (1000)      111 2023-04-16 13:10:59.000000 hak-0.0.1/hak/string/spaces/count.py
--rw-rw-r--   0 j         (1000) j         (1000)      320 2023-04-16 13:12:51.000000 hak-0.0.1/hak/string/split_fn_name_and_text.py
--rw-rw-r--   0 j         (1000) j         (1000)      344 2023-04-16 13:13:49.000000 hak-0.0.1/hak/string/strip_unprintable.py
--rw-rw-r--   0 j         (1000) j         (1000)      265 2023-04-16 13:14:54.000000 hak-0.0.1/hak/string/to_cond_freq_dict.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.428691 hak-0.0.1/hak/string/token/
--rw-rw-r--   0 j         (1000) j         (1000)     1263 2023-04-16 13:15:45.000000 hak-0.0.1/hak/string/token/substitute.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.428691 hak-0.0.1/hak/string/yyyymmdd/
--rw-rw-r--   0 j         (1000) j         (1000)      238 2023-04-16 13:16:58.000000 hak-0.0.1/hak/string/yyyymmdd/to_date.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.432691 hak-0.0.1/hak/strings/
--rw-rw-r--   0 j         (1000) j         (1000)      130 2023-04-16 13:19:55.000000 hak-0.0.1/hak/strings/add_src_funks_prefix.py
--rw-rw-r--   0 j         (1000) j         (1000)      586 2023-04-16 13:20:23.000000 hak-0.0.1/hak/strings/compare.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.432691 hak-0.0.1/hak/strings/contain/
--rw-rw-r--   0 j         (1000) j         (1000)      145 2023-04-16 13:20:43.000000 hak-0.0.1/hak/strings/contain/version.py
--rw-rw-r--   0 j         (1000) j         (1000)     2222 2023-04-16 13:21:14.000000 hak-0.0.1/hak/strings/find_first_diff.py
--rw-rw-r--   0 j         (1000) j         (1000)      434 2023-04-16 13:21:43.000000 hak-0.0.1/hak/strings/make_patch_version_change_to_py.py
--rw-rw-r--   0 j         (1000) j         (1000)      293 2023-04-16 13:22:16.000000 hak-0.0.1/hak/strings/module_names_from_py_filenames.py
--rw-rw-r--   0 j         (1000) j         (1000)      405 2023-04-16 13:23:14.000000 hak-0.0.1/hak/strings/patch_setup_cfg.py
--rw-rw-r--   0 j         (1000) j         (1000)      617 2023-04-16 13:24:27.000000 hak-0.0.1/hak/strings/patch_setup_py.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.432691 hak-0.0.1/hak/strings/pyfiles/
--rw-rw-r--   0 j         (1000) j         (1000)     1514 2023-04-16 13:25:35.000000 hak-0.0.1/hak/strings/pyfiles/filter_out_items.py
--rw-rw-r--   0 j         (1000) j         (1000)      761 2023-04-16 13:26:30.000000 hak-0.0.1/hak/strings/show_diff.py
--rw-rw-r--   0 j         (1000) j         (1000)      647 2023-04-16 13:28:32.000000 hak-0.0.1/hak/strings/to_dict.py
--rw-rw-r--   0 j         (1000) j         (1000)      357 2023-04-16 13:29:04.000000 hak-0.0.1/hak/strings/two_char_combinations.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.312689 hak-0.0.1/hak/subprocess/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.432691 hak-0.0.1/hak/subprocess/completed_process/
--rw-rw-r--   0 j         (1000) j         (1000)      655 2023-04-16 13:29:28.000000 hak-0.0.1/hak/subprocess/completed_process/to_str.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.432691 hak-0.0.1/hak/system/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 09:40:03.000000 hak-0.0.1/hak/system/__init__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.436691 hak-0.0.1/hak/system/git/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.436691 hak-0.0.1/hak/system/git/commit/
--rw-rw-r--   0 j         (1000) j         (1000)     2515 2023-04-16 13:32:06.000000 hak-0.0.1/hak/system/git/commit/run.py
--rw-rw-r--   0 j         (1000) j         (1000)      384 2023-04-16 13:32:31.000000 hak-0.0.1/hak/system/git/commit_if_test_and_app_ok.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.436691 hak-0.0.1/hak/system/git/gitignore/
--rw-rw-r--   0 j         (1000) j         (1000)      631 2023-04-16 13:32:55.000000 hak-0.0.1/hak/system/git/gitignore/make.py
--rw-rw-r--   0 j         (1000) j         (1000)      514 2023-04-16 13:33:18.000000 hak-0.0.1/hak/system/git/init.py
--rw-rw-r--   0 j         (1000) j         (1000)      725 2023-04-16 13:34:02.000000 hak-0.0.1/hak/system/git/log_oneline.py
--rw-rw-r--   0 j         (1000) j         (1000)      866 2023-04-16 13:34:58.000000 hak-0.0.1/hak/system/git/push_after_delay.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.436691 hak-0.0.1/hak/system/screen/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 09:40:15.000000 hak-0.0.1/hak/system/screen/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      786 2023-04-16 08:42:22.000000 hak-0.0.1/hak/system/screen/clear.py
--rw-rw-r--   0 j         (1000) j         (1000)     3119 2023-04-16 08:43:58.000000 hak-0.0.1/hak/terminal.py
--rw-rw-r--   0 j         (1000) j         (1000)      337 2023-04-16 08:43:58.000000 hak-0.0.1/hak/ternary.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.440691 hak-0.0.1/hak/test/
--rw-rw-r--   0 j         (1000) j         (1000)        0 2023-04-15 06:52:09.000000 hak-0.0.1/hak/test/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     2578 2023-04-16 05:45:38.000000 hak-0.0.1/hak/test/check_final_line.py
--rw-rw-r--   0 j         (1000) j         (1000)     2689 2023-04-16 05:47:48.000000 hak-0.0.1/hak/test/check_line_lengths.py
--rw-rw-r--   0 j         (1000) j         (1000)     2843 2023-04-16 13:43:08.000000 hak-0.0.1/hak/test/do.py
--rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-16 13:44:11.000000 hak-0.0.1/hak/test/final_line_check.py
--rw-rw-r--   0 j         (1000) j         (1000)      774 2023-04-16 13:44:42.000000 hak-0.0.1/hak/test/line_lengths_check.py
--rw-rw-r--   0 j         (1000) j         (1000)      926 2023-04-16 13:45:03.000000 hak-0.0.1/hak/test/oldest_file_print.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.440691 hak-0.0.1/hak/tup/
--rw-rw-r--   0 j         (1000) j         (1000)      176 2023-04-16 13:45:36.000000 hak-0.0.1/hak/tup/is_a.py
--rw-rw-r--   0 j         (1000) j         (1000)      617 2023-04-16 13:46:00.000000 hak-0.0.1/hak/update_duration.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-16 14:04:46.324689 hak-0.0.1/hak.egg-info/
--rw-rw-r--   0 j         (1000) j         (1000)      893 2023-04-16 14:04:46.000000 hak-0.0.1/hak.egg-info/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)     7710 2023-04-16 14:04:46.000000 hak-0.0.1/hak.egg-info/SOURCES.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2023-04-16 14:04:46.000000 hak-0.0.1/hak.egg-info/dependency_links.txt
--rw-rw-r--   0 j         (1000) j         (1000)     1591 2023-04-16 14:04:46.000000 hak-0.0.1/hak.egg-info/top_level.txt
--rw-rw-r--   0 j         (1000) j         (1000)      536 2023-04-16 14:04:46.440691 hak-0.0.1/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)     2732 2023-04-16 14:02:42.000000 hak-0.0.1/setup.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/
+-rw-rw-r--   0 a         (1009) a         (1010)     1068 2023-04-19 01:55:38.000000 hak-0.0.2/LICENSE
+-rw-rw-r--   0 a         (1009) a         (1010)     1018 2023-04-19 03:16:26.172838 hak-0.0.2/PKG-INFO
+-rw-rw-r--   0 a         (1009) a         (1010)      422 2023-04-19 01:55:38.000000 hak-0.0.2/README.md
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      140 2023-04-19 01:55:38.000000 hak-0.0.2/hak/a_equals_b.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/bool/
+-rw-rw-r--   0 a         (1009) a         (1010)       86 2023-04-19 01:55:38.000000 hak-0.0.2/hak/bool/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      103 2023-04-19 01:55:38.000000 hak-0.0.2/hak/bool/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/bool/or_none/
+-rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.2/hak/bool/or_none/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      125 2023-04-19 01:55:38.000000 hak-0.0.2/hak/bool/or_none/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/bools/
+-rw-rw-r--   0 a         (1009) a         (1010)      139 2023-04-19 01:55:38.000000 hak-0.0.2/hak/bools/count_true.py
+-rw-rw-r--   0 a         (1009) a         (1010)      249 2023-04-19 01:55:38.000000 hak-0.0.2/hak/calculate_duration_bar_width.py
+-rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.2/hak/check_if_ok_to_proceed.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/date/
+-rw-rw-r--   0 a         (1009) a         (1010)      143 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      347 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/is_first_second_or_third_day_of_month.py
+-rw-rw-r--   0 a         (1009) a         (1010)      414 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/is_first_week_of_quarter.py
+-rw-rw-r--   0 a         (1009) a         (1010)      208 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/is_monday.py
+-rw-rw-r--   0 a         (1009) a         (1010)      462 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/is_weekday.py
+-rw-rw-r--   0 a         (1009) a         (1010)      467 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/is_weekend.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/date/public_holiday/
+-rw-rw-r--   0 a         (1009) a         (1010)     5617 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/public_holiday/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      385 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/select_from_last_n_days.py
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/to_dd_mm_yyyy_str.py
+-rw-rw-r--   0 a         (1009) a         (1010)      605 2023-04-19 03:01:25.000000 hak-0.0.2/hak/date/to_utc_timestamp.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/date/year/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/date/year/easter_sunday/
+-rw-rw-r--   0 a         (1009) a         (1010)     1006 2023-04-19 01:55:38.000000 hak-0.0.2/hak/date/year/easter_sunday/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/datetime/
+-rw-rw-r--   0 a         (1009) a         (1010)      149 2023-04-19 01:55:38.000000 hak-0.0.2/hak/datetime/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      272 2023-04-19 01:55:38.000000 hak-0.0.2/hak/datetime/select_from_last_n_days.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/dict/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      215 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/convert_to_sql_insertable.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/dict/frequencies/
+-rw-rw-r--   0 a         (1009) a         (1010)      356 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/frequencies/choose.py
+-rw-rw-r--   0 a         (1009) a         (1010)      376 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/frequencies/make_from_strings.py
+-rw-rw-r--   0 a         (1009) a         (1010)      187 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/get_or_default.py
+-rw-rw-r--   0 a         (1009) a         (1010)      190 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/make_from_key_value_lists.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/dict/proposed_dismantlement/
+-rw-rw-r--   0 a         (1009) a         (1010)     1520 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/proposed_dismantlement/show.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/dict/test_durations/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/test_durations/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/test_durations/to_tuple_list_sorted_by_duration.py
+-rw-rw-r--   0 a         (1009) a         (1010)     4011 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dict/to_max_line_width_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/dicts/
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dicts/a_into_b.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1200 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dicts/compare.py
+-rw-rw-r--   0 a         (1009) a         (1010)      195 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dicts/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      663 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dicts/merge_freq_dicts.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dicts/reindex.py
+-rw-rw-r--   0 a         (1009) a         (1010)      203 2023-04-19 01:55:38.000000 hak-0.0.2/hak/dicts/sort_by_key.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/directories/
+-rw-rw-r--   0 a         (1009) a         (1010)      567 2023-04-19 01:55:38.000000 hak-0.0.2/hak/directories/exist.py
+-rw-rw-r--   0 a         (1009) a         (1010)      432 2023-04-19 01:55:38.000000 hak-0.0.2/hak/directories/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/directory/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/directory/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1548 2023-04-19 01:55:38.000000 hak-0.0.2/hak/directory/compress_to_tar.py
+-rw-rw-r--   0 a         (1009) a         (1010)      520 2023-04-19 01:55:38.000000 hak-0.0.2/hak/directory/empty.py
+-rw-rw-r--   0 a         (1009) a         (1010)       88 2023-04-19 01:55:38.000000 hak-0.0.2/hak/directory/exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)      650 2023-04-19 01:55:38.000000 hak-0.0.2/hak/directory/is_module.py
+-rw-rw-r--   0 a         (1009) a         (1010)      654 2023-04-19 01:55:38.000000 hak-0.0.2/hak/directory/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      782 2023-04-19 01:55:38.000000 hak-0.0.2/hak/directory/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3692 2023-04-19 01:55:38.000000 hak-0.0.2/hak/duration.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2021 2023-04-19 01:55:38.000000 hak-0.0.2/hak/duration_bar.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/fake/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/fake/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/fake/os/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/fake/os/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      418 2023-04-19 01:55:38.000000 hak-0.0.2/hak/fake/os/system.py
+-rw-rw-r--   0 a         (1009) a         (1010)      424 2023-04-19 01:55:38.000000 hak-0.0.2/hak/fake/printer.py
+-rw-rw-r--   0 a         (1009) a         (1010)       45 2023-04-19 01:55:38.000000 hak-0.0.2/hak/fake/sleep.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/fake/subprocess/
+-rw-rw-r--   0 a         (1009) a         (1010)     5824 2023-04-19 01:55:38.000000 hak-0.0.2/hak/fake/subprocess/run.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/file/
+-rw-rw-r--   0 a         (1009) a         (1010)     1253 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      785 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/decrypt.py
+-rw-rw-r--   0 a         (1009) a         (1010)      929 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/encrypt.py
+-rw-rw-r--   0 a         (1009) a         (1010)      697 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/load.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/file/pickle/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/pickle/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1253 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/pickle/load_if_exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)      906 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/pickle/save.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/file/py/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/py/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      546 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/py/create.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2644 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/py/dismantle.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3819 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/py/extract_fn.py
+-rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/py/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)      956 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/save.py
+-rw-rw-r--   0 a         (1009) a         (1010)      761 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/save_lines.py
+-rw-rw-r--   0 a         (1009) a         (1010)      308 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/save_lines_or_string.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/file/secret/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/file/secret/password/
+-rw-rw-r--   0 a         (1009) a         (1010)      680 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/secret/password/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/file/secret/username/
+-rw-rw-r--   0 a         (1009) a         (1010)      713 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/secret/username/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/file/tar/
+-rw-rw-r--   0 a         (1009) a         (1010)     1562 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/tar/extract.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/file/zip/
+-rw-rw-r--   0 a         (1009) a         (1010)      487 2023-04-19 01:55:38.000000 hak-0.0.2/hak/file/zip/extract.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/files/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/files/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)     1760 2023-04-19 01:55:38.000000 hak-0.0.2/hak/files/pyfiles/dismantle.py
+-rw-rw-r--   0 a         (1009) a         (1010)      100 2023-04-19 01:55:38.000000 hak-0.0.2/hak/find_first_parenthesis.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/float/
+-rw-rw-r--   0 a         (1009) a         (1010)       70 2023-04-19 01:55:38.000000 hak-0.0.2/hak/float/epsilon.py
+-rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.2/hak/float/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.2/hak/float/is_not.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/float/nan/
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.2/hak/float/nan/to_none.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/function/
+-rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.2/hak/function/function.py
+-rw-rw-r--   0 a         (1009) a         (1010)      423 2023-04-19 01:55:38.000000 hak-0.0.2/hak/function/write_to_file.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/int/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/int/days/
+-rw-rw-r--   0 a         (1009) a         (1010)      227 2023-04-19 01:55:38.000000 hak-0.0.2/hak/int/days/a_to_b_inclusive.py
+-rw-rw-r--   0 a         (1009) a         (1010)      661 2023-04-19 01:55:38.000000 hak-0.0.2/hak/int/get_prime_factorisation.py
+-rw-rw-r--   0 a         (1009) a         (1010)      104 2023-04-19 01:55:38.000000 hak-0.0.2/hak/int/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      426 2023-04-19 01:55:38.000000 hak-0.0.2/hak/int/is_prime.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/int/year/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/int/year/days/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/int/year/days/count/
+-rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.2/hak/int/year/days/count/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/int/year/days/first/
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.2/hak/int/year/days/first/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      420 2023-04-19 01:55:38.000000 hak-0.0.2/hak/int/year/days/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      153 2023-04-19 01:55:38.000000 hak-0.0.2/hak/int/year/now.py
+-rw-rw-r--   0 a         (1009) a         (1010)      448 2023-04-19 01:55:38.000000 hak-0.0.2/hak/l.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/list/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/list/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.2/hak/list/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      115 2023-04-19 01:55:38.000000 hak-0.0.2/hak/list/to_comma_separated_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/lists/
+-rw-rw-r--   0 a         (1009) a         (1010)      216 2023-04-19 01:55:38.000000 hak-0.0.2/hak/lists/merge.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1131 2023-04-19 01:55:38.000000 hak-0.0.2/hak/load_durations_if_exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)      123 2023-04-19 01:55:38.000000 hak-0.0.2/hak/log_2.py
+-rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.2/hak/nop.py
+-rw-rw-r--   0 a         (1009) a         (1010)       91 2023-04-19 01:55:38.000000 hak-0.0.2/hak/nop_state_x.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/patch/
+-rw-rw-r--   0 a         (1009) a         (1010)     3624 2023-04-19 01:55:38.000000 hak-0.0.2/hak/patch/do.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/period/
+-rw-rw-r--   0 a         (1009) a         (1010)      333 2023-04-19 01:55:38.000000 hak-0.0.2/hak/period/contains_day.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/pip/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/pip/dist_tar/
+-rw-rw-r--   0 a         (1009) a         (1010)     2749 2023-04-19 01:55:38.000000 hak-0.0.2/hak/pip/dist_tar/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      403 2023-04-19 01:55:38.000000 hak-0.0.2/hak/pip/dist_tar/remove.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/pip/setup/
+-rw-rw-r--   0 a         (1009) a         (1010)     1300 2023-04-19 01:55:38.000000 hak-0.0.2/hak/pip/setup/update.py
+-rw-rw-r--   0 a         (1009) a         (1010)      920 2023-04-19 01:55:38.000000 hak-0.0.2/hak/pip/upload.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/pip/version/
+-rw-rw-r--   0 a         (1009) a         (1010)      837 2023-04-19 01:55:38.000000 hak-0.0.2/hak/pip/version/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      120 2023-04-19 01:55:38.000000 hak-0.0.2/hak/pip/version/to_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)      157 2023-04-19 01:55:38.000000 hak-0.0.2/hak/pyfiles/format.py
+-rw-rw-r--   0 a         (1009) a         (1010)      833 2023-04-19 01:55:38.000000 hak-0.0.2/hak/pyfiles/format_and_commit.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/report/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/report/fail/
+-rw-rw-r--   0 a         (1009) a         (1010)      814 2023-04-19 01:55:38.000000 hak-0.0.2/hak/report/fail/no_xyz.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1914 2023-04-19 01:55:38.000000 hak-0.0.2/hak/report/fail/xyz.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1440 2023-04-19 01:55:38.000000 hak-0.0.2/hak/report/fail/z_return_neq_y_return.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1601 2023-04-19 01:55:38.000000 hak-0.0.2/hak/report/fail/z_stdo_neq_y_stdo.py
+-rw-rw-r--   0 a         (1009) a         (1010)      887 2023-04-19 01:55:38.000000 hak-0.0.2/hak/report/property_failure.py
+-rw-rw-r--   0 a         (1009) a         (1010)      729 2023-04-19 01:55:38.000000 hak-0.0.2/hak/report/success.py
+-rw-rw-r--   0 a         (1009) a         (1010)      394 2023-04-19 01:55:38.000000 hak-0.0.2/hak/report/summarise_file.py
+-rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.2/hak/save_durations.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/schedule/
+-rw-rw-r--   0 a         (1009) a         (1010)     3465 2023-04-19 01:55:38.000000 hak-0.0.2/hak/schedule/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      559 2023-04-19 01:55:38.000000 hak-0.0.2/hak/select_text_colour_from_width.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/session/
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.2/hak/session/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/set/
+-rw-rw-r--   0 a         (1009) a         (1010)      114 2023-04-19 01:55:38.000000 hak-0.0.2/hak/set/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/setup/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/setup/cfg/
+-rw-rw-r--   0 a         (1009) a         (1010)     1412 2023-04-19 01:55:38.000000 hak-0.0.2/hak/setup/cfg/update.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.164838 hak-0.0.2/hak/setup/py/
+-rw-rw-r--   0 a         (1009) a         (1010)     1465 2023-04-19 01:55:38.000000 hak-0.0.2/hak/setup/py/update.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/alphanumeric/
+-rw-rw-r--   0 a         (1009) a         (1010)      264 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/alphanumeric/fake.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/append/
+-rw-rw-r--   0 a         (1009) a         (1010)       54 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/append/new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      541 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/camel_to_snake.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/char/
+-rw-rw-r--   0 a         (1009) a         (1010)      322 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/char/find_all_indices.py
+-rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/char/is_digit.py
+-rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/char/is_upper.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/chars/
+-rw-rw-r--   0 a         (1009) a         (1010)      561 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/chars/remove.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/colour/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/colour/bright/
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/bright/blue.py
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/bright/cyan.py
+-rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/bright/green.py
+-rw-rw-r--   0 a         (1009) a         (1010)      168 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/bright/magenta.py
+-rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/bright/red.py
+-rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/bright/white.py
+-rw-rw-r--   0 a         (1009) a         (1010)      166 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/bright/yellow.py
+-rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/danger.py
+-rw-rw-r--   0 a         (1009) a         (1010)      174 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/danger_if_zero.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/colour/dark/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/dark/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/dark/blue.py
+-rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/dark/cyan.py
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/dark/default.py
+-rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/dark/green.py
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/dark/magenta.py
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/dark/red.py
+-rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/dark/white.py
+-rw-rw-r--   0 a         (1009) a         (1010)      152 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/dark/yellow.py
+-rw-rw-r--   0 a         (1009) a         (1010)       64 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/data.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/info.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/primary.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2261 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/rainbow.py
+-rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/secondary.py
+-rw-rw-r--   0 a         (1009) a         (1010)      267 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/tgfr.py
+-rw-rw-r--   0 a         (1009) a         (1010)      135 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/colour/warning.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/contains/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/contains/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/contains/function/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/contains/function/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      341 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/contains/function/run.py
+-rw-rw-r--   0 a         (1009) a         (1010)      192 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/contains/function/test.py
+-rw-rw-r--   0 a         (1009) a         (1010)      224 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/contains/l.py
+-rw-rw-r--   0 a         (1009) a         (1010)       76 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/contains/version.py
+-rw-rw-r--   0 a         (1009) a         (1010)      105 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/count_x_in_y.py
+-rw-rw-r--   0 a         (1009) a         (1010)      996 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/delete_character_safely.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/digits/
+-rw-rw-r--   0 a         (1009) a         (1010)      202 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/digits/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/double_single_quotes.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/family_name/
+-rw-rw-r--   0 a         (1009) a         (1010)   115522 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/family_name/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      303 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/family_name/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/filename/
+-rw-rw-r--   0 a         (1009) a         (1010)      126 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/filename/to_module_name.py
+-rw-rw-r--   0 a         (1009) a         (1010)      209 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/find_last_comma_index.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/fn_name/
+-rw-rw-r--   0 a         (1009) a         (1010)      226 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/fn_name/is_ignorable.py
+-rw-rw-r--   0 a         (1009) a         (1010)     5309 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/format.py
+-rw-rw-r--   0 a         (1009) a         (1010)       73 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/has_at_symbol.py
+-rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/has_digit.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/has_lowercase.py
+-rw-rw-r--   0 a         (1009) a         (1010)      259 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/has_other_char.py
+-rw-rw-r--   0 a         (1009) a         (1010)      172 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/has_seven_digits.py
+-rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/has_uppercase.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/hbar/
+-rw-rw-r--   0 a         (1009) a         (1010)      122 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/hbar/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/string/header/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/header/python_file/
+-rw-rw-r--   0 a         (1009) a         (1010)      314 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/header/python_file/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/header/test_table/
+-rw-rw-r--   0 a         (1009) a         (1010)      461 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/header/test_table/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/indent/
+-rw-rw-r--   0 a         (1009) a         (1010)      137 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/indent/run_if_class_method.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/insert/
+-rw-rw-r--   0 a         (1009) a         (1010)      602 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/insert/new_line_after_last_import_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      278 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/insert/new_line_before_comment.py
+-rw-rw-r--   0 a         (1009) a         (1010)      584 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/insert/new_line_before_def.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/insert/new_line_before_if_main.py
+-rw-rw-r--   0 a         (1009) a         (1010)      666 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/insert/new_line_before_lambda.py
+-rw-rw-r--   0 a         (1009) a         (1010)      292 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/insert/new_line_before_new_line_and_cea_.py
+-rw-rw-r--   0 a         (1009) a         (1010)      102 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      124 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/is_or_none.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/json/
+-rw-rw-r--   0 a         (1009) a         (1010)      179 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/json/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      548 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/lambdarise.py
+-rw-rw-r--   0 a         (1009) a         (1010)      360 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/make_content_without_function.py
+-rw-rw-r--   0 a         (1009) a         (1010)      325 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/make_function_text.py
+-rw-rw-r--   0 a         (1009) a         (1010)      338 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/make_initial_content.py
+-rw-rw-r--   0 a         (1009) a         (1010)      319 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/make_new_function_text.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/password/
+-rw-rw-r--   0 a         (1009) a         (1010)     1179 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/password/create.py
+-rw-rw-r--   0 a         (1009) a         (1010)      534 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/password/has_chars_from_3_sets.py
+-rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/pop_left.py
+-rw-rw-r--   0 a         (1009) a         (1010)      219 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/pop_right.py
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/prepend_import.py
+-rw-rw-r--   0 a         (1009) a         (1010)      756 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/print_and_return_false.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/refactor/
+-rw-rw-r--   0 a         (1009) a         (1010)     1213 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/refactor/by_two_char_combinations.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/remove/
+-rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/remove/empty_line_spaces.py
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/remove/empty_lines.py
+-rw-rw-r--   0 a         (1009) a         (1010)      441 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/remove/extra_new_line_following_class_definition.py
+-rw-rw-r--   0 a         (1009) a         (1010)      210 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/remove/first_new_line_if_starts_with_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)       81 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/remove/whitespace_between_newlines.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/replace/
+-rw-rw-r--   0 a         (1009) a         (1010)      241 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/replace/double_new_line_with_single_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      129 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/replace/single_new_line_with_empty_string.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/replace/triple_new_line_with_double_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      483 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/replace_unprintable.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3361 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/separate_function_from_context.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/single_line_function/
+-rw-rw-r--   0 a         (1009) a         (1010)      428 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/single_line_function/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      463 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/single_line_function/to_lambda_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/spaces/
+-rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/spaces/count.py
+-rw-rw-r--   0 a         (1009) a         (1010)      320 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/split_fn_name_and_text.py
+-rw-rw-r--   0 a         (1009) a         (1010)      344 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/strip_unprintable.py
+-rw-rw-r--   0 a         (1009) a         (1010)      265 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/to_cond_freq_dict.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/token/
+-rw-rw-r--   0 a         (1009) a         (1010)     1263 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/token/substitute.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/string/yyyymmdd/
+-rw-rw-r--   0 a         (1009) a         (1010)      238 2023-04-19 01:55:38.000000 hak-0.0.2/hak/string/yyyymmdd/to_date.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/strings/
+-rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/add_src_funks_prefix.py
+-rw-rw-r--   0 a         (1009) a         (1010)      586 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/compare.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.168838 hak-0.0.2/hak/strings/contain/
+-rw-rw-r--   0 a         (1009) a         (1010)      145 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/contain/version.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2222 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/find_first_diff.py
+-rw-rw-r--   0 a         (1009) a         (1010)      434 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/make_patch_version_change_to_py.py
+-rw-rw-r--   0 a         (1009) a         (1010)      293 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/module_names_from_py_filenames.py
+-rw-rw-r--   0 a         (1009) a         (1010)      405 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/patch_setup_cfg.py
+-rw-rw-r--   0 a         (1009) a         (1010)      617 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/patch_setup_py.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/hak/strings/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)     1514 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/pyfiles/filter_out_items.py
+-rw-rw-r--   0 a         (1009) a         (1010)      761 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/show_diff.py
+-rw-rw-r--   0 a         (1009) a         (1010)      647 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/to_dict.py
+-rw-rw-r--   0 a         (1009) a         (1010)      357 2023-04-19 01:55:38.000000 hak-0.0.2/hak/strings/two_char_combinations.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak/subprocess/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/hak/subprocess/completed_process/
+-rw-rw-r--   0 a         (1009) a         (1010)      655 2023-04-19 01:55:38.000000 hak-0.0.2/hak/subprocess/completed_process/to_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/hak/system/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/system/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/hak/system/git/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/hak/system/git/commit/
+-rw-rw-r--   0 a         (1009) a         (1010)     2515 2023-04-19 01:55:38.000000 hak-0.0.2/hak/system/git/commit/run.py
+-rw-rw-r--   0 a         (1009) a         (1010)      384 2023-04-19 01:55:38.000000 hak-0.0.2/hak/system/git/commit_if_test_and_app_ok.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/hak/system/git/gitignore/
+-rw-rw-r--   0 a         (1009) a         (1010)      631 2023-04-19 01:55:38.000000 hak-0.0.2/hak/system/git/gitignore/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      486 2023-04-19 03:03:56.000000 hak-0.0.2/hak/system/git/init.py
+-rw-rw-r--   0 a         (1009) a         (1010)      725 2023-04-19 01:55:38.000000 hak-0.0.2/hak/system/git/log_oneline.py
+-rw-rw-r--   0 a         (1009) a         (1010)      866 2023-04-19 01:55:38.000000 hak-0.0.2/hak/system/git/push_after_delay.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/hak/system/screen/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/system/screen/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      786 2023-04-19 01:55:38.000000 hak-0.0.2/hak/system/screen/clear.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 01:55:38.000000 hak-0.0.2/hak/terminal.py
+-rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.2/hak/ternary.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/hak/test/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.2/hak/test/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2578 2023-04-19 01:55:38.000000 hak-0.0.2/hak/test/check_final_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2689 2023-04-19 01:55:38.000000 hak-0.0.2/hak/test/check_line_lengths.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2843 2023-04-19 01:55:38.000000 hak-0.0.2/hak/test/do.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2450 2023-04-19 01:55:38.000000 hak-0.0.2/hak/test/final_line_check.py
+-rw-rw-r--   0 a         (1009) a         (1010)      774 2023-04-19 01:55:38.000000 hak-0.0.2/hak/test/line_lengths_check.py
+-rw-rw-r--   0 a         (1009) a         (1010)      926 2023-04-19 01:55:38.000000 hak-0.0.2/hak/test/oldest_file_print.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.172838 hak-0.0.2/hak/tup/
+-rw-rw-r--   0 a         (1009) a         (1010)      176 2023-04-19 01:55:38.000000 hak-0.0.2/hak/tup/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      617 2023-04-19 01:55:38.000000 hak-0.0.2/hak/update_duration.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 03:16:26.160838 hak-0.0.2/hak.egg-info/
+-rw-rw-r--   0 a         (1009) a         (1010)     1018 2023-04-19 03:16:26.000000 hak-0.0.2/hak.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1009) a         (1010)     7741 2023-04-19 03:16:26.000000 hak-0.0.2/hak.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1009) a         (1010)        1 2023-04-19 03:16:26.000000 hak-0.0.2/hak.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1009) a         (1010)     1591 2023-04-19 03:16:26.000000 hak-0.0.2/hak.egg-info/top_level.txt
+-rw-rw-r--   0 a         (1009) a         (1010)      536 2023-04-19 03:16:26.172838 hak-0.0.2/setup.cfg
+-rw-rw-r--   0 a         (1009) a         (1010)     2732 2023-04-19 03:16:26.000000 hak-0.0.2/setup.py
```

### Comparing `hak-0.0.1/LICENSE` & `hak-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/PKG-INFO` & `hak-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: hak
-Version: 0.0.1
+Version: 0.0.2
 Summary: Function Test Pair Toolbox
 Home-page: https://github.com/JohnForbes/hak
 Author: @JohnRForbes
 Author-email: john.robert.forbes@gmail.com
 License: MIT
+Description: # hak
+        ===============
+        This project is a collection of function test pairs for common tasks.
+        Mostly for my own use but others are welcome to leverage it.
+        
+        ## Required configuration
+        `git config --global user.email "you@example.com"`
+        `git config --global user.name "Your Name`
+        
+        ## Required packages
+        * `sudo apt install twine`
+        
+        ## Recommended packages
+        * `sudo npm i -g nodemon`
+        
+        ## Test Cycle
+        `nodemon --exec python3 test.py`
+        
 Keywords: hak
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# hak
-===============
-This project is a collection of function test pairs for common tasks.
-Mostly for my own use but others are welcome to leverage it.
-
-## Required configuration
-`git config --global user.email "you@example.com"`
-`git config --global user.name "Your Name`
-
-## Required packages
-* `sudo apt install twine`
-
-## Recommended packages
-* `sudo npm i -g nodemon`
-
-## Test Cycle
-`nodemon --exec python3 test.py`
-
-
```

### Comparing `hak-0.0.1/hak/check_if_ok_to_proceed.py` & `hak-0.0.2/hak/check_if_ok_to_proceed.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/date/public_holiday/is_a.py` & `hak-0.0.2/hak/date/public_holiday/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/date/to_timestamp.py` & `hak-0.0.2/hak/date/to_utc_timestamp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from datetime import date
 from datetime import datetime as dt
 from hak.string.print_and_return_false import f as pf
+from time import timezone
 
-f = lambda x: dt(x.year, x.month, x.day).timestamp()
+f = lambda x: dt(x.year, x.month, x.day).timestamp() - timezone
 
 def t_0():
   x = date(1970,1,1)
   y = 0
   z = f(x)
   return y==z or pf([f'x: {x}', f'y: {y}', f'z: {z}'])
 
 def t_1():
   x = date(1970,1,2)
-  y = 50400
+  y = 86400
   z = f(x)
   return y==z or pf([f'x: {x}', f'y: {y}', f'z: {z}'])
 
 def t_2():
   x = date(2022,3,4)
-  y = 1646312400
+  y = 1646352000
   z = f(x)
   return y==z or pf([f'x: {x}', f'y: {y}', f'z: {z}'])
 
 def t():
   if not t_0(): return pf('t_0 failed')
   return True
```

### Comparing `hak-0.0.1/hak/date/year/easter_sunday/get.py` & `hak-0.0.2/hak/date/year/easter_sunday/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/dict/proposed_dismantlement/show.py` & `hak-0.0.2/hak/dict/proposed_dismantlement/show.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/dict/to_max_line_width_str.py` & `hak-0.0.2/hak/dict/to_max_line_width_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/dicts/compare.py` & `hak-0.0.2/hak/dicts/compare.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/dicts/merge_freq_dicts.py` & `hak-0.0.2/hak/dicts/merge_freq_dicts.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/directories/exist.py` & `hak-0.0.2/hak/directories/exist.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/directory/compress_to_tar.py` & `hak-0.0.2/hak/directory/compress_to_tar.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/directory/empty.py` & `hak-0.0.2/hak/directory/empty.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/directory/make.py` & `hak-0.0.2/hak/directory/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/directory/remove.py` & `hak-0.0.2/hak/directory/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/duration.py` & `hak-0.0.2/hak/duration.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/duration_bar.py` & `hak-0.0.2/hak/duration_bar.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/fake/subprocess/run.py` & `hak-0.0.2/hak/fake/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/__init__.py` & `hak-0.0.2/hak/file/__init__.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/decrypt.py` & `hak-0.0.2/hak/file/decrypt.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/encrypt.py` & `hak-0.0.2/hak/file/encrypt.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/load.py` & `hak-0.0.2/hak/file/load.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/pickle/load_if_exists.py` & `hak-0.0.2/hak/file/pickle/load_if_exists.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/pickle/save.py` & `hak-0.0.2/hak/file/pickle/save.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/py/create.py` & `hak-0.0.2/hak/file/py/create.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/py/dismantle.py` & `hak-0.0.2/hak/file/py/dismantle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/py/extract_fn.py` & `hak-0.0.2/hak/file/py/extract_fn.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/save.py` & `hak-0.0.2/hak/file/save.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/save_lines.py` & `hak-0.0.2/hak/file/save_lines.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/secret/password/get.py` & `hak-0.0.2/hak/file/secret/password/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/secret/username/get.py` & `hak-0.0.2/hak/file/secret/username/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/file/tar/extract.py` & `hak-0.0.2/hak/file/tar/extract.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/files/pyfiles/dismantle.py` & `hak-0.0.2/hak/files/pyfiles/dismantle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/int/get_prime_factorisation.py` & `hak-0.0.2/hak/int/get_prime_factorisation.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/load_durations_if_exists.py` & `hak-0.0.2/hak/load_durations_if_exists.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/patch/do.py` & `hak-0.0.2/hak/patch/do.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/pip/dist_tar/make.py` & `hak-0.0.2/hak/pip/dist_tar/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/pip/setup/update.py` & `hak-0.0.2/hak/pip/setup/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/pip/upload.py` & `hak-0.0.2/hak/pip/upload.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/pip/version/get.py` & `hak-0.0.2/hak/pip/version/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/pyfiles/format_and_commit.py` & `hak-0.0.2/hak/pyfiles/format_and_commit.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/report/fail/no_xyz.py` & `hak-0.0.2/hak/report/fail/no_xyz.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/report/fail/xyz.py` & `hak-0.0.2/hak/report/fail/xyz.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/report/fail/z_return_neq_y_return.py` & `hak-0.0.2/hak/report/fail/z_return_neq_y_return.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/report/fail/z_stdo_neq_y_stdo.py` & `hak-0.0.2/hak/report/fail/z_stdo_neq_y_stdo.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/report/property_failure.py` & `hak-0.0.2/hak/report/property_failure.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/report/success.py` & `hak-0.0.2/hak/report/success.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/save_durations.py` & `hak-0.0.2/hak/save_durations.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/schedule/make.py` & `hak-0.0.2/hak/schedule/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/select_text_colour_from_width.py` & `hak-0.0.2/hak/select_text_colour_from_width.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/setup/cfg/update.py` & `hak-0.0.2/hak/setup/cfg/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/setup/py/update.py` & `hak-0.0.2/hak/setup/py/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/camel_to_snake.py` & `hak-0.0.2/hak/string/camel_to_snake.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/chars/remove.py` & `hak-0.0.2/hak/string/chars/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/colour/rainbow.py` & `hak-0.0.2/hak/string/colour/rainbow.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/delete_character_safely.py` & `hak-0.0.2/hak/string/delete_character_safely.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/family_name/fake.py` & `hak-0.0.2/hak/string/family_name/fake.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/format.py` & `hak-0.0.2/hak/string/format.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/insert/new_line_after_last_import_line.py` & `hak-0.0.2/hak/string/insert/new_line_after_last_import_line.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/insert/new_line_before_def.py` & `hak-0.0.2/hak/string/insert/new_line_before_def.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/insert/new_line_before_lambda.py` & `hak-0.0.2/hak/string/insert/new_line_before_lambda.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/lambdarise.py` & `hak-0.0.2/hak/string/lambdarise.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/password/create.py` & `hak-0.0.2/hak/string/password/create.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/password/has_chars_from_3_sets.py` & `hak-0.0.2/hak/string/password/has_chars_from_3_sets.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/print_and_return_false.py` & `hak-0.0.2/hak/string/print_and_return_false.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/refactor/by_two_char_combinations.py` & `hak-0.0.2/hak/string/refactor/by_two_char_combinations.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/separate_function_from_context.py` & `hak-0.0.2/hak/string/separate_function_from_context.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/string/token/substitute.py` & `hak-0.0.2/hak/string/token/substitute.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/strings/compare.py` & `hak-0.0.2/hak/strings/compare.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/strings/find_first_diff.py` & `hak-0.0.2/hak/strings/find_first_diff.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/strings/patch_setup_py.py` & `hak-0.0.2/hak/strings/patch_setup_py.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/strings/pyfiles/filter_out_items.py` & `hak-0.0.2/hak/strings/pyfiles/filter_out_items.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/strings/show_diff.py` & `hak-0.0.2/hak/strings/show_diff.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/strings/to_dict.py` & `hak-0.0.2/hak/strings/to_dict.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/subprocess/completed_process/to_str.py` & `hak-0.0.2/hak/subprocess/completed_process/to_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/system/git/commit/run.py` & `hak-0.0.2/hak/system/git/commit/run.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/system/git/gitignore/make.py` & `hak-0.0.2/hak/system/git/gitignore/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/system/git/init.py` & `hak-0.0.2/hak/system/git/log_oneline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from subprocess import run as sprun
 from hak.directory.make import f as mkdir
 from hak.directory.remove import f as rmdir
-_root = '../temp_git_init'
+from hak.system.git.init import f as git_init
+from hak.file.save import f as save
+from hak.system.git.commit.run import f as git_commit
 
-def up(): mkdir(_root)
+_root = '../temp_git_log_oneline'
+
+def up():
+  mkdir(_root)
+  git_init(_root)
+  save(_root+'/foo.py', 'foo')
+  git_commit(do_pull=False, cwd=_root, do_push=False)
 
 def dn(): rmdir(_root)
-args = ['git', 'init', '--initial-branch', 'main']
+
+args = ['git', 'log', '--oneline']
 
 f = lambda cwd: sprun(cwd=cwd, capture_output=True, args=args)
 
 def t():
   up()
   z = f(_root)
   dn()
   return all([
     z.args==args,
     z.returncode==0,
-    'Initialized empty Git repository in' in z.stdout.decode('utf-8'),
+    'Added foo.py' in z.stdout.decode('utf-8'),
     not z.stderr.decode('utf-8')
   ])
```

### Comparing `hak-0.0.1/hak/system/git/push_after_delay.py` & `hak-0.0.2/hak/system/git/push_after_delay.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/system/screen/clear.py` & `hak-0.0.2/hak/system/screen/clear.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/terminal.py` & `hak-0.0.2/hak/terminal.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/test/check_final_line.py` & `hak-0.0.2/hak/test/check_final_line.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/test/check_line_lengths.py` & `hak-0.0.2/hak/test/check_line_lengths.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/test/do.py` & `hak-0.0.2/hak/test/do.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/test/final_line_check.py` & `hak-0.0.2/hak/test/final_line_check.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/test/line_lengths_check.py` & `hak-0.0.2/hak/test/line_lengths_check.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/test/oldest_file_print.py` & `hak-0.0.2/hak/test/oldest_file_print.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak/update_duration.py` & `hak-0.0.2/hak/update_duration.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/hak.egg-info/PKG-INFO` & `hak-0.0.2/hak.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: hak
-Version: 0.0.1
+Version: 0.0.2
 Summary: Function Test Pair Toolbox
 Home-page: https://github.com/JohnForbes/hak
 Author: @JohnRForbes
 Author-email: john.robert.forbes@gmail.com
 License: MIT
+Description: # hak
+        ===============
+        This project is a collection of function test pairs for common tasks.
+        Mostly for my own use but others are welcome to leverage it.
+        
+        ## Required configuration
+        `git config --global user.email "you@example.com"`
+        `git config --global user.name "Your Name`
+        
+        ## Required packages
+        * `sudo apt install twine`
+        
+        ## Recommended packages
+        * `sudo npm i -g nodemon`
+        
+        ## Test Cycle
+        `nodemon --exec python3 test.py`
+        
 Keywords: hak
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# hak
-===============
-This project is a collection of function test pairs for common tasks.
-Mostly for my own use but others are welcome to leverage it.
-
-## Required configuration
-`git config --global user.email "you@example.com"`
-`git config --global user.name "Your Name`
-
-## Required packages
-* `sudo apt install twine`
-
-## Recommended packages
-* `sudo npm i -g nodemon`
-
-## Test Cycle
-`nodemon --exec python3 test.py`
-
-
```

### Comparing `hak-0.0.1/hak.egg-info/SOURCES.txt` & `hak-0.0.2/hak.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 hak/date/is_first_second_or_third_day_of_month.py
 hak/date/is_first_week_of_quarter.py
 hak/date/is_monday.py
 hak/date/is_weekday.py
 hak/date/is_weekend.py
 hak/date/select_from_last_n_days.py
 hak/date/to_dd_mm_yyyy_str.py
-hak/date/to_timestamp.py
+hak/date/to_utc_timestamp.py
 hak/date/public_holiday/is_a.py
 hak/date/year/easter_sunday/get.py
 hak/datetime/is_a.py
 hak/datetime/select_from_last_n_days.py
 hak/dict/__init__.py
 hak/dict/convert_to_sql_insertable.py
 hak/dict/get_or_default.py
@@ -60,14 +60,15 @@
 hak/dicts/sort_by_key.py
 hak/directories/exist.py
 hak/directories/make.py
 hak/directory/__init__.py
 hak/directory/compress_to_tar.py
 hak/directory/empty.py
 hak/directory/exists.py
+hak/directory/is_module.py
 hak/directory/make.py
 hak/directory/remove.py
 hak/fake/__init__.py
 hak/fake/printer.py
 hak/fake/sleep.py
 hak/fake/os/__init__.py
 hak/fake/os/system.py
```

### Comparing `hak-0.0.1/hak.egg-info/top_level.txt` & `hak-0.0.2/hak.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `hak-0.0.1/setup.cfg` & `hak-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hak
-version = 0.0.1
+version = 0.0.2
 author = John Forbes
 author_email = john.robert.forbes@gmail.com
 description = Function Test Pair Toolbox
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JohnForbes/hak
 license_files = LICENSE
```

### Comparing `hak-0.0.1/setup.py` & `hak-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 long_description = Path("./README.md").read_text()
 
 setup(
   name='hak',
-  version='0.0.1',
+  version='0.0.2',
   license='MIT',
   description='Function Test Pair Toolbox',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='@JohnRForbes',
   author_email='john.robert.forbes@gmail.com',
   url='https://github.com/JohnForbes/hak',
```

