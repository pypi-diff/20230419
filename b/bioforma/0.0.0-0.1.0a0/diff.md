# Comparing `tmp/bioforma-0.0.0.tar.gz` & `tmp/bioforma-0.1.0a0.tar.gz`

## Comparing `bioforma-0.0.0.tar` & `bioforma-0.1.0a0.tar`

### file list

```diff
@@ -1,20 +1,30 @@
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 bioforma-0.0.0/Cargo.toml
--rw-r--r--   0      501       20     2770 2023-03-10 17:23:11.000000 bioforma-0.0.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      327 2023-03-10 17:37:56.000000 bioforma-0.0.0/.gitignore
--rw-r--r--   0      501       20      176 2023-03-10 16:57:14.000000 bioforma-0.0.0/.idea/.gitignore
--rw-r--r--   0      501       20      329 2023-03-10 17:38:53.000000 bioforma-0.0.0/.idea/bioforma.iml
--rw-r--r--   0      501       20    13434 2023-03-10 16:58:20.000000 bioforma-0.0.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0      501       20      174 2023-03-10 16:58:20.000000 bioforma-0.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0      501       20      197 2023-03-10 17:38:53.000000 bioforma-0.0.0/.idea/misc.xml
--rw-r--r--   0      501       20      268 2023-03-10 16:58:20.000000 bioforma-0.0.0/.idea/modules.xml
--rw-r--r--   0      501       20      180 2023-03-10 16:58:20.000000 bioforma-0.0.0/.idea/vcs.xml
--rw-r--r--   0      501       20     5202 2023-03-10 18:14:14.000000 bioforma-0.0.0/.idea/workspace.xml
--rw-r--r--   0      501       20     1073 2023-03-10 16:56:36.000000 bioforma-0.0.0/LICENSE
--rw-r--r--   0      501       20       10 2023-03-10 16:56:36.000000 bioforma-0.0.0/README.md
--rw-r--r--   0      501       20       69 2023-03-10 18:14:09.000000 bioforma-0.0.0/bioforma/__init__.py
--rw-r--r--   0      501       20       17 2023-03-10 18:12:56.000000 bioforma-0.0.0/bioforma/_bioforma.pyi
--rw-r--r--   0      501       20      371 2023-03-10 17:29:21.000000 bioforma-0.0.0/pyproject.toml
--rw-r--r--   0      501       20      683 2023-03-10 18:12:56.000000 bioforma-0.0.0/src/lib.rs
--rw-r--r--   0      501       20      101 2023-03-10 18:01:00.000000 bioforma-0.0.0/test.py
--rw-r--r--   0      501       20     7652 2023-03-10 17:58:18.000000 bioforma-0.0.0/Cargo.lock
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 bioforma-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 bioforma-0.1.0a0/Cargo.toml
+-rw-r--r--   0     1001      123     1073 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/LICENSE
+-rw-r--r--   0     1001      123     2175 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/README.md
+-rw-r--r--   0     1001      123       63 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/__init__.py
+-rw-r--r--   0     1001      123       59 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/_bioforma.pyi
+-rw-r--r--   0     1001      123     2069 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/alignment/__init__.pyi
+-rw-r--r--   0     1001      123      338 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/alignment/distance.pyi
+-rw-r--r--   0     1001      123      758 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/alphabets/__init__.pyi
+-rw-r--r--   0     1001      123      262 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/alphabets/dna.pyi
+-rw-r--r--   0     1001      123      121 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/alphabets/protein.pyi
+-rw-r--r--   0     1001      123      262 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/alphabets/rna.pyi
+-rw-r--r--   0     1001      123      216 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/scores.pyi
+-rw-r--r--   0     1001      123        0 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/seq_analysis/__init__.pyi
+-rw-r--r--   0     1001      123       93 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/seq_analysis/gc.pyi
+-rw-r--r--   0     1001      123      388 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/bioforma/seq_analysis/orf.pyi
+-rw-r--r--   0     1001      123      156 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/build.rs
+-rw-r--r--   0     1001      123     1129 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/pyproject.toml
+-rw-r--r--   0     1001      123     9725 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/src/alignment.rs
+-rw-r--r--   0     1001      123     7026 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/src/alphabets.rs
+-rw-r--r--   0     1001      123     1665 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/src/lib.rs
+-rw-r--r--   0     1001      123     1379 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/src/scores.rs
+-rw-r--r--   0     1001      123     3050 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/src/seq_analysis.rs
+-rw-r--r--   0     1001      123        0 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/tests/__init__.py
+-rw-r--r--   0     1001      123     5029 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/tests/test_alignment.py
+-rw-r--r--   0     1001      123     3368 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/tests/test_alphabets.py
+-rw-r--r--   0     1001      123      152 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/tests/test_metadata.py
+-rw-r--r--   0     1001      123     1805 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/tests/test_scores.py
+-rw-r--r--   0     1001      123     1703 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/tests/test_seq_analysis.py
+-rw-r--r--   0     1001      123    25259 2023-04-19 05:26:20.000000 bioforma-0.1.0a0/Cargo.lock
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 bioforma-0.1.0a0/PKG-INFO
```

### Comparing `bioforma-0.0.0/LICENSE` & `bioforma-0.1.0a0/LICENSE`

 * *Files identical despite different names*

