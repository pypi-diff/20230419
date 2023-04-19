# Comparing `tmp/pyriksprot-2023.4.2.tar.gz` & `tmp/pyriksprot-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksprot-2023.4.2.tar", max compression
+gzip compressed data, was "pyriksprot-2023.4.3.tar", max compression
```

## Comparing `pyriksprot-2023.4.2.tar` & `pyriksprot-2023.4.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2023.4.2/LICENSE
--rw-r--r--   0        0        0     7547 2023-04-13 10:55:09.499216 pyriksprot-2023.4.2/README.md
--rw-r--r--   0        0        0     3406 2023-04-17 14:56:36.929977 pyriksprot-2023.4.2/pyproject.toml
--rw-r--r--   0        0        0     1250 2023-04-17 14:55:11.204894 pyriksprot-2023.4.2/pyriksprot/__init__.py
--rw-r--r--   0        0        0      152 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/corpus/__init__.py
--rw-r--r--   0        0        0     4111 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/corpus_index.py
--rw-r--r--   0        0        0    11973 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/iterate.py
--rw-r--r--   0        0        0      243 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/__init__.py
--rw-r--r--   0        0        0     3528 2023-04-14 06:54:51.788513 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/convert.py
--rw-r--r--   0        0        0     2467 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/iterate.py
--rw-r--r--   0        0        0     5365 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/parse.py
--rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/__init__.py
--rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
--rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
--rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
--rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
--rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
--rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
--rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
--rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
--rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
--rw-r--r--   0        0        0     2266 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/tf.py
--rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/tagged/__init__.py
--rw-r--r--   0        0        0     1630 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/tagged/iterate.py
--rw-r--r--   0        0        0     5790 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/tagged/persist.py
--rw-r--r--   0        0        0     1515 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/utility.py
--rw-r--r--   0        0        0      113 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/dehyphenation/__init__.py
--rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/dehyphenation/flair_dehyphen.py
--rw-r--r--   0        0        0     8562 2023-04-17 14:55:11.248895 pyriksprot-2023.4.2/pyriksprot/dehyphenation/swe_dehyphen.py
--rw-r--r--   0        0        0      843 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/dehyphenation/utility.py
--rw-r--r--   0        0        0      438 2023-01-24 09:13:07.490512 pyriksprot-2023.4.2/pyriksprot/dispatch/__init__.py
--rw-r--r--   0        0        0    21549 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/dispatch/dispatch.py
--rw-r--r--   0        0        0     2100 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/dispatch/item.py
--rw-r--r--   0        0        0     4594 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/dispatch/merge.py
--rw-r--r--   0        0        0     4908 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/dispatch/utility.py
--rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/README.md
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/__init__.py
--rw-r--r--   0        0        0     2335 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/bettertokenizer.sv
--rw-r--r--   0        0        0      945 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens
--rw-r--r--   0        0        0    12236 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/foss/pos_tags.py
--rw-r--r--   0        0        0     7546 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/foss/sparv_tokenize.py
--rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/stopwords.py
--rw-r--r--   0        0        0     6119 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/foss/untangle.py
--rw-r--r--   0        0        0     3582 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/gitchen.py
--rw-r--r--   0        0        0    13080 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/interface.py
--rw-r--r--   0        0        0      769 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/metadata/__init__.py
--rw-r--r--   0        0        0     5145 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/codecs.py
--rw-r--r--   0        0        0    12475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/config.py
--rw-r--r--   0        0        0     7737 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/generate.py
--rw-r--r--   0        0        0    14671 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/person.py
--rw-r--r--   0        0        0     3125 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/repository.py
--rw-r--r--   0        0        0     2373 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/subset.py
--rw-r--r--   0        0        0     6384 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/utility.py
--rw-r--r--   0        0        0     1461 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/utterance.py
--rw-r--r--   0        0        0     4296 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/verify.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/scripts/__init__.py
--rw-r--r--   0        0        0     1596 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/csv2pgsql.py
--rw-r--r--   0        0        0     1648 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/fix_speaker_notes.py
--rw-r--r--   0        0        0     3543 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/metadata2db.py
--rw-r--r--   0        0        0     2695 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2speech.py
--rw-r--r--   0        0        0     3475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2speech_text.py
--rw-r--r--   0        0        0     2902 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2tagged.py
--rw-r--r--   0        0        0     4650 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2text.py
--rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2tfs.py
--rwxr-xr-x   0        0        0      680 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/speaker_note2csv
--rw-r--r--   0        0        0     2568 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/speech_index.py
--rw-r--r--   0        0        0     1196 2023-04-13 13:53:50.922546 pyriksprot-2023.4.2/pyriksprot/scripts/subset_corpus.py
--rw-r--r--   0        0        0     5266 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/utils.py
--rwxr-xr-x   0        0        0      541 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/xml2csv
--rw-r--r--   0        0        0      599 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/00_rename.sql
--rw-r--r--   0        0        0     4522 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/01_data_updates.sql
--rw-r--r--   0        0        0     2592 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/02_code_tables.sql
--rw-r--r--   0        0        0     2199 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/03_persons_of_interest.sql
--rw-r--r--   0        0        0     5973 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/04_terms_of_office.sql
--rw-r--r--   0        0        0     2818 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/05_person_party.sql
--rw-r--r--   0        0        0     1707 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/06_unknown.sql
--rw-r--r--   0        0        0     1344 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/09_cleanup.sql
--rw-r--r--   0        0        0      204 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/__init__.py
--rw-r--r--   0        0        0     7144 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/to_speech.py
--rw-r--r--   0        0        0    12974 2023-04-17 05:36:18.788607 pyriksprot-2023.4.2/pyriksprot/utility.py
--rw-r--r--   0        0        0      250 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/workflows/__init__.py
--rw-r--r--   0        0        0     1415 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/_extract_speech_ids.py
--rw-r--r--   0        0        0     4425 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/extract_speech_text.py
--rw-r--r--   0        0        0     6449 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/extract_tags.py
--rw-r--r--   0        0        0     4552 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/extract_text.py
--rw-r--r--   0        0        0     3254 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/workflows/speech_index.py
--rw-r--r--   0        0        0     2230 2023-04-13 13:53:26.190262 pyriksprot-2023.4.2/pyriksprot/workflows/subset_corpus.py
--rw-r--r--   0        0        0     6120 2023-04-17 14:55:10.780889 pyriksprot-2023.4.2/pyriksprot/workflows/tag.py
--rw-r--r--   0        0        0     4137 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/tf.py
--rw-r--r--   0        0        0     8732 1970-01-01 00:00:00.000000 pyriksprot-2023.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2023.4.3/LICENSE
+-rw-r--r--   0        0        0     7547 2023-04-13 10:55:09.499216 pyriksprot-2023.4.3/README.md
+-rw-r--r--   0        0        0     3536 2023-04-19 09:23:02.948346 pyriksprot-2023.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1250 2023-04-17 14:57:52.426931 pyriksprot-2023.4.3/pyriksprot/__init__.py
+-rw-r--r--   0        0        0      152 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/corpus/__init__.py
+-rw-r--r--   0        0        0     4111 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/corpus_index.py
+-rw-r--r--   0        0        0    11973 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/iterate.py
+-rw-r--r--   0        0        0      243 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/__init__.py
+-rw-r--r--   0        0        0     3528 2023-04-17 14:57:52.426931 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/convert.py
+-rw-r--r--   0        0        0     2467 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/iterate.py
+-rw-r--r--   0        0        0     5365 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/parse.py
+-rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/__init__.py
+-rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
+-rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
+-rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
+-rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
+-rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
+-rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
+-rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
+-rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
+-rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
+-rw-r--r--   0        0        0     2266 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/tf.py
+-rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/corpus/tagged/__init__.py
+-rw-r--r--   0        0        0     1630 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/tagged/iterate.py
+-rw-r--r--   0        0        0     5790 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/tagged/persist.py
+-rw-r--r--   0        0        0     1515 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/corpus/utility.py
+-rw-r--r--   0        0        0      113 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/dehyphenation/__init__.py
+-rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/dehyphenation/flair_dehyphen.py
+-rw-r--r--   0        0        0     8642 2023-04-19 09:21:24.587202 pyriksprot-2023.4.3/pyriksprot/dehyphenation/swe_dehyphen.py
+-rw-r--r--   0        0        0      843 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/dehyphenation/utility.py
+-rw-r--r--   0        0        0      438 2023-01-24 09:13:07.490512 pyriksprot-2023.4.3/pyriksprot/dispatch/__init__.py
+-rw-r--r--   0        0        0    21577 2023-04-19 09:21:24.587202 pyriksprot-2023.4.3/pyriksprot/dispatch/dispatch.py
+-rw-r--r--   0        0        0     2100 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/dispatch/item.py
+-rw-r--r--   0        0        0     4594 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/dispatch/merge.py
+-rw-r--r--   0        0        0     4908 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/dispatch/utility.py
+-rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/README.md
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/__init__.py
+-rw-r--r--   0        0        0     2335 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/bettertokenizer.sv
+-rw-r--r--   0        0        0      945 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/bettertokenizer.sv.saldo-tokens
+-rw-r--r--   0        0        0    12236 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/foss/pos_tags.py
+-rw-r--r--   0        0        0     7546 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/foss/sparv_tokenize.py
+-rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/foss/stopwords.py
+-rw-r--r--   0        0        0     6119 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/foss/untangle.py
+-rw-r--r--   0        0        0     3582 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/gitchen.py
+-rw-r--r--   0        0        0    13080 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/interface.py
+-rw-r--r--   0        0        0      769 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/metadata/__init__.py
+-rw-r--r--   0        0        0     5145 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/codecs.py
+-rw-r--r--   0        0        0    12475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/config.py
+-rw-r--r--   0        0        0     7737 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/generate.py
+-rw-r--r--   0        0        0    14671 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/person.py
+-rw-r--r--   0        0        0     3125 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/repository.py
+-rw-r--r--   0        0        0     2373 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/subset.py
+-rw-r--r--   0        0        0     6384 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/utility.py
+-rw-r--r--   0        0        0     1461 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/utterance.py
+-rw-r--r--   0        0        0     4296 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/metadata/verify.py
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.3/pyriksprot/scripts/__init__.py
+-rw-r--r--   0        0        0     1596 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/csv2pgsql.py
+-rw-r--r--   0        0        0     1648 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/fix_speaker_notes.py
+-rw-r--r--   0        0        0     3543 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/metadata2db.py
+-rw-r--r--   0        0        0     2789 2023-04-19 09:21:24.587202 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2speech.py
+-rw-r--r--   0        0        0     3475 2023-04-19 09:07:54.192237 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2speech_text.py
+-rw-r--r--   0        0        0     2902 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2tagged.py
+-rw-r--r--   0        0        0     4650 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2text.py
+-rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2tfs.py
+-rwxr-xr-x   0        0        0      680 2023-01-24 09:13:07.494512 pyriksprot-2023.4.3/pyriksprot/scripts/speaker_note2csv
+-rw-r--r--   0        0        0     2568 2023-01-24 09:13:07.494512 pyriksprot-2023.4.3/pyriksprot/scripts/speech_index.py
+-rw-r--r--   0        0        0     1162 2023-04-19 09:21:24.591202 pyriksprot-2023.4.3/pyriksprot/scripts/subset_corpus.py
+-rw-r--r--   0        0        0     5266 2023-01-24 09:13:07.494512 pyriksprot-2023.4.3/pyriksprot/scripts/utils.py
+-rwxr-xr-x   0        0        0      541 2023-01-24 09:13:07.494512 pyriksprot-2023.4.3/pyriksprot/scripts/xml2csv
+-rw-r--r--   0        0        0      599 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/00_rename.sql
+-rw-r--r--   0        0        0     4522 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/01_data_updates.sql
+-rw-r--r--   0        0        0     2592 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/02_code_tables.sql
+-rw-r--r--   0        0        0     2199 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/03_persons_of_interest.sql
+-rw-r--r--   0        0        0     5973 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/04_terms_of_office.sql
+-rw-r--r--   0        0        0     2818 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/05_person_party.sql
+-rw-r--r--   0        0        0     1707 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/06_unknown.sql
+-rw-r--r--   0        0        0     1344 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/09_cleanup.sql
+-rw-r--r--   0        0        0      204 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/sql/__init__.py
+-rw-r--r--   0        0        0     7144 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/to_speech.py
+-rw-r--r--   0        0        0    12974 2023-04-17 14:57:52.426931 pyriksprot-2023.4.3/pyriksprot/utility.py
+-rw-r--r--   0        0        0      250 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/workflows/__init__.py
+-rw-r--r--   0        0        0     1415 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/workflows/_extract_speech_ids.py
+-rw-r--r--   0        0        0     4425 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/workflows/extract_speech_text.py
+-rw-r--r--   0        0        0     6449 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/workflows/extract_tags.py
+-rw-r--r--   0        0        0     4552 2023-04-13 10:55:09.503216 pyriksprot-2023.4.3/pyriksprot/workflows/extract_text.py
+-rw-r--r--   0        0        0     3254 2023-03-27 13:27:29.397414 pyriksprot-2023.4.3/pyriksprot/workflows/speech_index.py
+-rw-r--r--   0        0        0     2230 2023-04-13 13:53:26.190262 pyriksprot-2023.4.3/pyriksprot/workflows/subset_corpus.py
+-rw-r--r--   0        0        0     6123 2023-04-19 09:21:24.591202 pyriksprot-2023.4.3/pyriksprot/workflows/tag.py
+-rw-r--r--   0        0        0     4159 2023-04-19 09:21:24.591202 pyriksprot-2023.4.3/pyriksprot/workflows/tf.py
+-rw-r--r--   0        0        0     8732 1970-01-01 00:00:00.000000 pyriksprot-2023.4.3/PKG-INFO
```

### Comparing `pyriksprot-2023.4.2/LICENSE` & `pyriksprot-2023.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/README.md` & `pyriksprot-2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyproject.toml` & `pyriksprot-2023.4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksprot"
-version = "2023.4.2"
+version = "2023.4.3"
 description = "Python API for Riksdagens Protokoll"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
     { include = "pyriksprot" },
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
@@ -52,14 +52,16 @@
 pyinstrument = "*"
 pytest-codeblocks = "*"
 
 [tool.poetry.scripts]
 riksprot2any = "pyriksprot.scripts.riksprot2any:main"
 riksprot2tfs = "pyriksprot.scripts.riksprot2tfs:main"
 riksprot2text = "pyriksprot.scripts.riksprot2text:main"
+riksprot2speech = "pyriksprot.scripts.riksprot2speech:main"
+riksprot2speech_text = "pyriksprot.scripts.riksprot2speech_text:main"
 subset-corpus = "pyriksprot.scripts.subset_corpus:main"
 speech-index = "pyriksprot.scripts.speech_index:main"
 metadata2db = "pyriksprot.scripts.metadata2db:main"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-rfE", "-q", "-s"]
```

### Comparing `pyriksprot-2023.4.2/pyriksprot/__init__.py` & `pyriksprot-2023.4.3/pyriksprot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/corpus_index.py` & `pyriksprot-2023.4.3/pyriksprot/corpus/corpus_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/iterate.py` & `pyriksprot-2023.4.3/pyriksprot/corpus/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/convert.py` & `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/convert.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/iterate.py` & `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/parse.py` & `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/parse.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt` & `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt` & `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt` & `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/tf.py` & `pyriksprot-2023.4.3/pyriksprot/corpus/parlaclarin/tf.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/tagged/iterate.py` & `pyriksprot-2023.4.3/pyriksprot/corpus/tagged/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/tagged/persist.py` & `pyriksprot-2023.4.3/pyriksprot/corpus/tagged/persist.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/corpus/utility.py` & `pyriksprot-2023.4.3/pyriksprot/corpus/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/dehyphenation/flair_dehyphen.py` & `pyriksprot-2023.4.3/pyriksprot/dehyphenation/flair_dehyphen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/dehyphenation/swe_dehyphen.py` & `pyriksprot-2023.4.3/pyriksprot/dehyphenation/swe_dehyphen.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 """
 import re
 from dataclasses import dataclass, field
 from enum import IntEnum
 from os.path import isfile, join
 from typing import Callable
 
+from loguru import logger
+
 from .utility import load_dict, load_token_set, store_dict, store_token_set
 
 PARAGRAPH_MARKER = '##PARAGRAPH##'
 
 # pylint: disable=too-many-arguments
 jj = join
 
@@ -230,14 +232,15 @@
         self.whitelist = load_token_set(self.whitelist_filename)
         self.whitelist_log = load_dict(self.whitelist_log_filename)
         self.unresolved = load_token_set(self.unresolved_filename)
 
     @staticmethod
     def create_dehypen(data_folder: str, word_frequencies: str | dict = None) -> Callable[[str], str]:
         """Create a dehyphen service. Return wrapped dehyphen function."""
+        logger.info(f"dehyphen path: {data_folder}")
         dehyphenator: SwedishDehyphenator = SwedishDehyphenator(
             data_folder=data_folder, word_frequencies=word_frequencies
         )
 
         def dehyphen(text: str) -> str:
             """Remove hyphens from `text`."""
             dehyphenated_text = dehyphenator.dehyphen_text(text)
```

### Comparing `pyriksprot-2023.4.2/pyriksprot/dehyphenation/utility.py` & `pyriksprot-2023.4.3/pyriksprot/dehyphenation/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/dispatch/dispatch.py` & `pyriksprot-2023.4.3/pyriksprot/dispatch/dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,15 +498,15 @@
         self.token2id: defaultdict = defaultdict()
         self.tfs: defaultdict = defaultdict()
         self.token2id.default_factory = self.token2id.__len__
         self.pos_schema: PoS_Tag_Scheme = PoS_TAGS_SCHEMES.SUC
 
     def create_tagged_frame(self, item: IDispatchItem) -> pd.DataFrame:
         tagged_frame: pd.DataFrame = super().create_tagged_frame(item)
-        fg = self.token2id.get  # lambda t: self.token2id[t]
+        fg = lambda t: self.token2id[t]  # pylint: disable=unnecessary-lambda-assignment
         pg = self.pos_schema.pos_to_id.get  # pylint: disable=unnecessary-lambda-assignment
 
         if not self.skip_text:
             tagged_frame['token_id'] = tagged_frame.token.apply(fg)
 
         if not self.skip_lemma:
             tagged_frame['lemma_id'] = tagged_frame.lemma.apply(fg)
```

### Comparing `pyriksprot-2023.4.2/pyriksprot/dispatch/item.py` & `pyriksprot-2023.4.3/pyriksprot/dispatch/item.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/dispatch/merge.py` & `pyriksprot-2023.4.3/pyriksprot/dispatch/merge.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/dispatch/utility.py` & `pyriksprot-2023.4.3/pyriksprot/dispatch/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/foss/bettertokenizer.sv` & `pyriksprot-2023.4.3/pyriksprot/foss/bettertokenizer.sv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens` & `pyriksprot-2023.4.3/pyriksprot/foss/bettertokenizer.sv.saldo-tokens`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/foss/pos_tags.py` & `pyriksprot-2023.4.3/pyriksprot/foss/pos_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/foss/sparv_tokenize.py` & `pyriksprot-2023.4.3/pyriksprot/foss/sparv_tokenize.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/foss/stopwords.py` & `pyriksprot-2023.4.3/pyriksprot/foss/stopwords.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/foss/untangle.py` & `pyriksprot-2023.4.3/pyriksprot/foss/untangle.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/gitchen.py` & `pyriksprot-2023.4.3/pyriksprot/gitchen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/interface.py` & `pyriksprot-2023.4.3/pyriksprot/interface.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/__init__.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/codecs.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/codecs.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/config.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/config.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/generate.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/generate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/person.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/person.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/repository.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/repository.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/subset.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/subset.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/utility.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/utterance.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/utterance.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/metadata/verify.py` & `pyriksprot-2023.4.3/pyriksprot/metadata/verify.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/csv2pgsql.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/csv2pgsql.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/fix_speaker_notes.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/fix_speaker_notes.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/metadata2db.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/metadata2db.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2speech.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2tagged.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,103 @@
+import sys
+from inspect import currentframe, getargvalues
+from typing import Sequence
+
 import click
 
-from pyriksprot import interface, to_speech
+from pyriksprot import interface
 from pyriksprot.dispatch import dispatch
 from pyriksprot.scripts.utils import option2, update_arguments_from_options_file
 from pyriksprot.utility import strip_path_and_extension
 from pyriksprot.workflows import extract_tags
 
+sys.path.insert(0, '.')
+
+
+sys.path.insert(0, '.')
+
+
 # pylint: disable=too-many-arguments, unused-argument
 
 
+def get_kwargs():
+    keys, _, _, values = getargvalues(currentframe().f_back)
+    return {k: v for k, v in zip(keys, values) if k != 'self'}
+
+
+"""
+Extract an aggregated subset of a tagged ParlaCLARIN corpus.
+"""
+
+
 @click.command()
-@click.argument('source-folder', type=click.STRING)
+@click.argument('source-folder', type=click.STRING, required=False)
 @click.argument('metadata-filename', type=click.STRING)
-@click.argument('target-name', type=click.STRING)
+@click.argument('target-name', type=click.STRING, required=False)
 @option2('--options-filename')
 @option2('--target-type')
 @option2('--compress-type')
 @option2('--content-type')
-@option2('--merge-strategy')
-@option2('--multiproc-processes')
+@option2('--segment-level')
+@option2('--segment-skip-size')
+@option2('--temporal-key')
+@option2('--group-key')
+@option2('--years')
 @option2('--skip-lemma')
 @option2('--skip-text')
 @option2('--skip-puncts')
 @option2('--skip-stopwords')
-@option2('--lowercase')
+@option2('--multiproc-processes')
+@option2('--multiproc-keep-order')
 @option2('--force')
 def main(
     options_filename: str = None,
     source_folder: str = None,
     metadata_filename: str = None,
     target_name: str = None,
     target_type: str = None,
+    compress_type: str = "feather",
     content_type: str = 'tagged_frame',
-    merge_strategy: str = 'chain',
-    compress_type: str = 'feather',
-    multiproc_processes: int = 1,
+    segment_level: interface.SegmentLevel = None,
+    segment_skip_size: int = 1,
+    temporal_key: interface.TemporalKey = None,
+    group_key: Sequence[interface.GroupingKey] = None,
+    years: str = None,
     skip_lemma: bool = False,
     skip_text: bool = False,
     skip_puncts: bool = False,
     skip_stopwords: bool = False,
-    lowercase: bool = True,
+    multiproc_processes: int = 1,
+    multiproc_keep_order: str = None,
     force: bool = False,
 ):
-    arguments: dict = update_arguments_from_options_file(
-        arguments=locals(), filename_key='options_filename', suffix=strip_path_and_extension(target_name)
-    )
-    arguments['content_type'] = interface.ContentType(arguments['content_type'])
-    arguments['merge_strategy'] = to_speech.MergeStrategyType(arguments['merge_strategy'])
-    arguments['compress_type'] = dispatch.CompressType(arguments['compress_type'].lower())
-
-    extract_tags.extract_corpus_tags(
-        **{
-            **arguments,
-            **dict(
-                segment_level=interface.SegmentLevel.Speech,
-                segment_skip_size=1,
-                years=None,
-                temporal_key=None,
-                group_keys=None,
-                multiproc_keep_order=False,
-                multiproc_chunksize=10,
-            ),
-        }
-    )
+    try:
+        arguments: dict = update_arguments_from_options_file(
+            arguments=locals(), filename_key='options_filename', suffix=strip_path_and_extension(target_name)
+        )
+        arguments['content_type'] = interface.ContentType(arguments['content_type'])
+        arguments['compress_type'] = dispatch.CompressType(arguments['compress_type'].lower())
+
+        arguments['group_keys'] = arguments['group_key']
+        del arguments['group_key']
+
+        extract_tags.extract_corpus_tags(**arguments)
+
+    except Exception as ex:
+        click.echo(ex)
+        sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
 
     # from click.testing import CliRunner
+
     # runner = CliRunner()
     # result = runner.invoke(
     #     main,
     #     [
-    #         '/data/westac/riksdagen_corpus_data/tagged_frames',
-    #         '/data/westac/riksdagen_corpus_data/tagged-speech-corpus.feather',
-    #         '--target-type',
-    #         'feather',
-    #         # '--compression-type',
-    #         # 'LZMA',
-    #         '--processes',
-    #         1,
+    #         '--options-filename',
+    #         'sample_opts/riksprot2tagged_year_who.yml'
     #     ],
     # )
     # print(result.output)
```

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2speech_text.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2speech_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2tagged.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2speech.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,103 +1,85 @@
-import sys
-from inspect import currentframe, getargvalues
-from typing import Sequence
-
 import click
 
-from pyriksprot import interface
+from pyriksprot import interface, to_speech
 from pyriksprot.dispatch import dispatch
 from pyriksprot.scripts.utils import option2, update_arguments_from_options_file
 from pyriksprot.utility import strip_path_and_extension
 from pyriksprot.workflows import extract_tags
 
-sys.path.insert(0, '.')
-
-
-sys.path.insert(0, '.')
-
-
 # pylint: disable=too-many-arguments, unused-argument
 
 
-def get_kwargs():
-    keys, _, _, values = getargvalues(currentframe().f_back)
-    return {k: v for k, v in zip(keys, values) if k != 'self'}
-
-
-"""
-Extract an aggregated subset of a tagged ParlaCLARIN corpus.
-"""
-
-
 @click.command()
-@click.argument('source-folder', type=click.STRING, required=False)
+@click.argument('source-folder', type=click.STRING)
 @click.argument('metadata-filename', type=click.STRING)
-@click.argument('target-name', type=click.STRING, required=False)
+@click.argument('target-name', type=click.STRING)
 @option2('--options-filename')
 @option2('--target-type')
 @option2('--compress-type')
 @option2('--content-type')
-@option2('--segment-level')
-@option2('--segment-skip-size')
-@option2('--temporal-key')
-@option2('--group-key')
-@option2('--years')
+@option2('--merge-strategy')
+@option2('--multiproc-processes')
 @option2('--skip-lemma')
 @option2('--skip-text')
 @option2('--skip-puncts')
 @option2('--skip-stopwords')
-@option2('--multiproc-processes')
-@option2('--multiproc-keep-order')
+@option2('--lowercase')
 @option2('--force')
 def main(
     options_filename: str = None,
     source_folder: str = None,
     metadata_filename: str = None,
     target_name: str = None,
     target_type: str = None,
-    compress_type: str = "feather",
     content_type: str = 'tagged_frame',
-    segment_level: interface.SegmentLevel = None,
-    segment_skip_size: int = 1,
-    temporal_key: interface.TemporalKey = None,
-    group_key: Sequence[interface.GroupingKey] = None,
-    years: str = None,
+    merge_strategy: str = 'chain',
+    compress_type: str = 'feather',
+    multiproc_processes: int = 1,
     skip_lemma: bool = False,
     skip_text: bool = False,
     skip_puncts: bool = False,
     skip_stopwords: bool = False,
-    multiproc_processes: int = 1,
-    multiproc_keep_order: str = None,
+    lowercase: bool = True,
     force: bool = False,
 ):
-    try:
-        arguments: dict = update_arguments_from_options_file(
-            arguments=locals(), filename_key='options_filename', suffix=strip_path_and_extension(target_name)
-        )
-        arguments['content_type'] = interface.ContentType(arguments['content_type'])
-        arguments['compress_type'] = dispatch.CompressType(arguments['compress_type'].lower())
-
-        arguments['group_keys'] = arguments['group_key']
-        del arguments['group_key']
-
-        extract_tags.extract_corpus_tags(**arguments)
-
-    except Exception as ex:
-        click.echo(ex)
-        sys.exit(1)
+    arguments: dict = update_arguments_from_options_file(
+        arguments=locals(), filename_key='options_filename', suffix=strip_path_and_extension(target_name)
+    )
+    arguments['content_type'] = interface.ContentType(arguments['content_type'])
+    arguments['merge_strategy'] = to_speech.MergeStrategyType(arguments['merge_strategy'])
+    arguments['compress_type'] = dispatch.CompressType(arguments['compress_type'].lower())
+
+    extract_tags.extract_corpus_tags(
+        **{
+            **arguments,
+            **dict(
+                segment_level=interface.SegmentLevel.Speech,
+                segment_skip_size=1,
+                years=None,
+                temporal_key=None,
+                group_keys=None,
+                multiproc_keep_order=False,
+                multiproc_chunksize=10,
+            ),
+        }
+    )
 
 
 if __name__ == "__main__":
     main()
 
     # from click.testing import CliRunner
-
     # runner = CliRunner()
     # result = runner.invoke(
     #     main,
     #     [
     #         '--options-filename',
-    #         'sample_opts/riksprot2tagged_year_who.yml'
+    #         'data/swedeb-data/dataset-01/opts/tagged-speeches/tagged_frames_speeches_lemma.feather.yml',
+    #         '--force',
+    #         'data/swedeb-data/dataset-01/v0.6.0/tagged_frames',
+    #         'data/swedeb-data/dataset-01/v0.6.0/riksprot_metadata.db',
+    #         'data/swedeb-data/dataset-01/v0.6.0/speeches/tagged_frames_speeches_lemma.feather'
+
     #     ],
     # )
     # print(result.output)
```

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2text.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/riksprot2text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/speaker_note2csv` & `pyriksprot-2023.4.3/pyriksprot/scripts/speaker_note2csv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/speech_index.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/speech_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/subset_corpus.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/subset_corpus.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,11 +33,10 @@
 
 
 if __name__ == "__main__":
     # options = {
     #     'documents': 'swedeb-sample-protocols.txt',
     #     'target_folder': 'data/swedeb-samples/',
     #     'tag': 'v0.6.0',
-    #     'scripts_folder': None,
     # }
     # subset_corpus_and_metadata(**options)
     main()
```

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/utils.py` & `pyriksprot-2023.4.3/pyriksprot/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/scripts/xml2csv` & `pyriksprot-2023.4.3/pyriksprot/scripts/xml2csv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/sql/00_rename.sql` & `pyriksprot-2023.4.3/pyriksprot/sql/00_rename.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/sql/01_data_updates.sql` & `pyriksprot-2023.4.3/pyriksprot/sql/01_data_updates.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/sql/02_code_tables.sql` & `pyriksprot-2023.4.3/pyriksprot/sql/02_code_tables.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/sql/03_persons_of_interest.sql` & `pyriksprot-2023.4.3/pyriksprot/sql/03_persons_of_interest.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/sql/04_terms_of_office.sql` & `pyriksprot-2023.4.3/pyriksprot/sql/04_terms_of_office.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/sql/05_person_party.sql` & `pyriksprot-2023.4.3/pyriksprot/sql/05_person_party.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/sql/06_unknown.sql` & `pyriksprot-2023.4.3/pyriksprot/sql/06_unknown.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/sql/09_cleanup.sql` & `pyriksprot-2023.4.3/pyriksprot/sql/09_cleanup.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/to_speech.py` & `pyriksprot-2023.4.3/pyriksprot/to_speech.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/utility.py` & `pyriksprot-2023.4.3/pyriksprot/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/workflows/_extract_speech_ids.py` & `pyriksprot-2023.4.3/pyriksprot/workflows/_extract_speech_ids.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/workflows/extract_speech_text.py` & `pyriksprot-2023.4.3/pyriksprot/workflows/extract_speech_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/workflows/extract_tags.py` & `pyriksprot-2023.4.3/pyriksprot/workflows/extract_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/workflows/extract_text.py` & `pyriksprot-2023.4.3/pyriksprot/workflows/extract_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/workflows/speech_index.py` & `pyriksprot-2023.4.3/pyriksprot/workflows/speech_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/workflows/subset_corpus.py` & `pyriksprot-2023.4.3/pyriksprot/workflows/subset_corpus.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.2/pyriksprot/workflows/tag.py` & `pyriksprot-2023.4.3/pyriksprot/workflows/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     force: bool,
     recursive: bool = False,
 ):
     """Tags protocols in `source_folder`. Stores result in `target_folder`.
     Note: not used by Snakemake workflow (used by tag CLI script)
     """
 
-    source_files: list[str] = glob(join(source_folder, "prot-*.xml"), recursive=recursive)
+    source_files: list[str] = glob(join(source_folder, "**/prot-*.xml"), recursive=recursive)
     for source_file in tqdm(source_files):
         subfolder: str = split(dirname(source_file))[1] if recursive else ''
         target_file = join(target_folder, subfolder, f"{strip_path_and_extension(source_file)}.zip")
         if force or expired(target_file, source_file):
             tag_protocol_xml(source_file, target_file, tagger, storage_format="json", force=force)
         else:
             touch(target_file)
```

### Comparing `pyriksprot-2023.4.2/pyriksprot/workflows/tf.py` & `pyriksprot-2023.4.3/pyriksprot/workflows/tf.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         if isinstance(source, XmlUntangleSegmentIterator):
             texts = source
         else:
             if isinstance(source, str):
                 if os.path.isfile(source):
                     filenames = [source]
                 elif os.path.isdir(source):
-                    filenames = glob(os.path.join(source, "*.xml"))
+                    filenames = glob(os.path.join(source, "**", "*.xml"), recursive=True)
                 else:
                     filenames = glob(source)
             elif isinstance(source, list):
                 filenames = source
             else:
                 raise ValueError(f"unknown source of type {type(source)}")
```

### Comparing `pyriksprot-2023.4.2/PKG-INFO` & `pyriksprot-2023.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksprot
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Python API for Riksdagens Protokoll
 Home-page: https://westac.se
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
 Requires-Python: >=3.11.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
```

