# Comparing `tmp/labxpipe-0.5.0.tar.gz` & `tmp/labxpipe-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labxpipe-0.5.0.tar", last modified: Wed Apr  5 16:31:51 2023, max compression
+gzip compressed data, was "labxpipe-0.6.0.tar", last modified: Wed Apr 19 16:00:19 2023, max compression
```

## Comparing `labxpipe-0.5.0.tar` & `labxpipe-0.6.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.696672 labxpipe-0.5.0/
--rw-r--r--   0 build     (1000) build     (1001)       17 2023-04-05 16:31:06.000000 labxpipe-0.5.0/.gitignore
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.683337 labxpipe-0.5.0/.sourcehut/
--rw-r--r--   0 build     (1000) build     (1001)     1272 2023-04-05 16:31:06.000000 labxpipe-0.5.0/.sourcehut/arch.yml
--rw-r--r--   0 build     (1000) build     (1001)    16726 2023-04-05 16:31:06.000000 labxpipe-0.5.0/LICENSE
--rw-r--r--   0 build     (1000) build     (1001)    12773 2023-04-05 16:31:51.696672 labxpipe-0.5.0/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)    12477 2023-04-05 16:31:06.000000 labxpipe-0.5.0/README.md
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.683337 labxpipe-0.5.0/config/
--rw-r--r--   0 build     (1000) build     (1001)     1065 2023-04-05 16:31:06.000000 labxpipe-0.5.0/config/labxpipe.json
--rw-r--r--   0 build     (1000) build     (1001)     1123 2023-04-05 16:31:06.000000 labxpipe-0.5.0/config/labxpipe_trackhub.json
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.686671 labxpipe-0.5.0/config/pipelines/
--rw-r--r--   0 build     (1000) build     (1001)     2189 2023-04-05 16:31:06.000000 labxpipe-0.5.0/config/pipelines/chip_seq.json
--rw-r--r--   0 build     (1000) build     (1001)     2440 2023-04-05 16:31:06.000000 labxpipe-0.5.0/config/pipelines/mrna_seq.json
--rw-r--r--   0 build     (1000) build     (1001)     2226 2023-04-05 16:31:06.000000 labxpipe-0.5.0/config/pipelines/mrna_seq_cufflinks.json
--rw-r--r--   0 build     (1000) build     (1001)     2898 2023-04-05 16:31:06.000000 labxpipe-0.5.0/config/pipelines/mrna_seq_no_db.json
--rw-r--r--   0 build     (1000) build     (1001)     2802 2023-04-05 16:31:06.000000 labxpipe-0.5.0/config/pipelines/mrna_seq_with_plotting.json
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.686671 labxpipe-0.5.0/img/
--rw-r--r--   0 build     (1000) build     (1001)     5728 2023-04-05 16:31:06.000000 labxpipe-0.5.0/img/logo.svg
--rw-r--r--   0 build     (1000) build     (1001)      581 2023-04-05 16:31:06.000000 labxpipe-0.5.0/pyproject.toml
--rw-r--r--   0 build     (1000) build     (1001)       38 2023-04-05 16:31:51.696672 labxpipe-0.5.0/setup.cfg
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.683337 labxpipe-0.5.0/src/
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.686671 labxpipe-0.5.0/src/labxpipe/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.690004 labxpipe-0.5.0/src/labxpipe/interfaces/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/interfaces/__init__.py
--rw-r--r--   0 build     (1000) build     (1001)     1547 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_bg2bw.py
--rw-r--r--   0 build     (1000) build     (1001)     5817 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_bowtie2.py
--rw-r--r--   0 build     (1000) build     (1001)     2336 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_cufflinks.py
--rw-r--r--   0 build     (1000) build     (1001)     8069 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_geneabacus.py
--rw-r--r--   0 build     (1000) build     (1001)     4564 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_readknead.py
--rw-r--r--   0 build     (1000) build     (1001)     2423 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_samtools.py
--rw-r--r--   0 build     (1000) build     (1001)     6569 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_star.py
--rw-r--r--   0 build     (1000) build     (1001)     2876 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/parallel_helpers.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.693338 labxpipe-0.5.0/src/labxpipe/steps/
--rw-r--r--   0 build     (1000) build     (1001)      423 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/steps/__init__.py
--rw-r--r--   0 build     (1000) build     (1001)     4022 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/steps/bowtie2.py
--rw-r--r--   0 build     (1000) build     (1001)     1431 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/steps/cleaning.py
--rw-r--r--   0 build     (1000) build     (1001)     2413 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/steps/cufflinks.py
--rw-r--r--   0 build     (1000) build     (1001)     6565 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/steps/geneabacus.py
--rw-r--r--   0 build     (1000) build     (1001)     5492 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/steps/readknead.py
--rw-r--r--   0 build     (1000) build     (1001)     2950 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/steps/samtools_sort.py
--rw-r--r--   0 build     (1000) build     (1001)     3625 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/steps/samtools_uniquify.py
--rw-r--r--   0 build     (1000) build     (1001)     3235 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/steps/star.py
--rw-r--r--   0 build     (1000) build     (1001)     8654 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/trackhub.py
--rw-r--r--   0 build     (1000) build     (1001)     1739 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe/utils.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.690004 labxpipe-0.5.0/src/labxpipe.egg-info/
--rw-r--r--   0 build     (1000) build     (1001)    12773 2023-04-05 16:31:51.000000 labxpipe-0.5.0/src/labxpipe.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)     1641 2023-04-05 16:31:51.000000 labxpipe-0.5.0/src/labxpipe.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1001)        1 2023-04-05 16:31:51.000000 labxpipe-0.5.0/src/labxpipe.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1001)       56 2023-04-05 16:31:51.000000 labxpipe-0.5.0/src/labxpipe.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1001)       44 2023-04-05 16:31:51.000000 labxpipe-0.5.0/src/labxpipe.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1001)       26 2023-04-05 16:31:51.000000 labxpipe-0.5.0/src/labxpipe.egg-info/top_level.txt
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-05 16:31:51.696672 labxpipe-0.5.0/src/labxpipe_scripts/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/__init__.py
--rwxr-xr-x   0 build     (1000) build     (1001)     2440 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/lxpipe.py
--rwxr-xr-x   0 build     (1000) build     (1001)    15408 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_demultiplex.py
--rwxr-xr-x   0 build     (1000) build     (1001)     7438 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_extract.py
--rwxr-xr-x   0 build     (1000) build     (1001)     7704 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_generate.py
--rwxr-xr-x   0 build     (1000) build     (1001)    17284 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_merge_count.py
--rwxr-xr-x   0 build     (1000) build     (1001)     4243 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_profile.py
--rwxr-xr-x   0 build     (1000) build     (1001)    13878 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_report.py
--rwxr-xr-x   0 build     (1000) build     (1001)    16815 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_run.py
--rwxr-xr-x   0 build     (1000) build     (1001)    21424 2023-04-05 16:31:06.000000 labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_trackhub.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.572254 labxpipe-0.6.0/
+-rw-r--r--   0 build     (1000) build     (1001)       17 2023-04-19 15:59:30.000000 labxpipe-0.6.0/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/.sourcehut/
+-rw-r--r--   0 build     (1000) build     (1001)     1272 2023-04-19 15:59:30.000000 labxpipe-0.6.0/.sourcehut/arch.yml
+-rw-r--r--   0 build     (1000) build     (1001)    16726 2023-04-19 15:59:30.000000 labxpipe-0.6.0/LICENSE
+-rw-r--r--   0 build     (1000) build     (1001)    12773 2023-04-19 16:00:19.568920 labxpipe-0.6.0/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)    12477 2023-04-19 15:59:30.000000 labxpipe-0.6.0/README.md
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/config/
+-rw-r--r--   0 build     (1000) build     (1001)     1065 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/labxpipe.json
+-rw-r--r--   0 build     (1000) build     (1001)     1123 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/labxpipe_trackhub.json
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/config/pipelines/
+-rw-r--r--   0 build     (1000) build     (1001)     2189 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/chip_seq.json
+-rw-r--r--   0 build     (1000) build     (1001)     2440 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/mrna_seq.json
+-rw-r--r--   0 build     (1000) build     (1001)     2226 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/mrna_seq_cufflinks.json
+-rw-r--r--   0 build     (1000) build     (1001)     2898 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/mrna_seq_no_db.json
+-rw-r--r--   0 build     (1000) build     (1001)     2802 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/mrna_seq_with_plotting.json
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/img/
+-rw-r--r--   0 build     (1000) build     (1001)     5728 2023-04-19 15:59:30.000000 labxpipe-0.6.0/img/logo.svg
+-rw-r--r--   0 build     (1000) build     (1001)      581 2023-04-19 15:59:30.000000 labxpipe-0.6.0/pyproject.toml
+-rw-r--r--   0 build     (1000) build     (1001)       38 2023-04-19 16:00:19.572254 labxpipe-0.6.0/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/src/
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.565586 labxpipe-0.6.0/src/labxpipe/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.565586 labxpipe-0.6.0/src/labxpipe/interfaces/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)     1547 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_bg2bw.py
+-rw-r--r--   0 build     (1000) build     (1001)     5817 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_bowtie2.py
+-rw-r--r--   0 build     (1000) build     (1001)     2336 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_cufflinks.py
+-rw-r--r--   0 build     (1000) build     (1001)     8069 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_geneabacus.py
+-rw-r--r--   0 build     (1000) build     (1001)     4642 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_minimap2.py
+-rw-r--r--   0 build     (1000) build     (1001)     4564 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_readknead.py
+-rw-r--r--   0 build     (1000) build     (1001)     2423 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_samtools.py
+-rw-r--r--   0 build     (1000) build     (1001)     6569 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_star.py
+-rw-r--r--   0 build     (1000) build     (1001)     2876 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/parallel_helpers.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.568920 labxpipe-0.6.0/src/labxpipe/steps/
+-rw-r--r--   0 build     (1000) build     (1001)      423 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)     4181 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/bowtie2.py
+-rw-r--r--   0 build     (1000) build     (1001)     1431 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/cleaning.py
+-rw-r--r--   0 build     (1000) build     (1001)     2413 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/cufflinks.py
+-rw-r--r--   0 build     (1000) build     (1001)     6565 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/geneabacus.py
+-rw-r--r--   0 build     (1000) build     (1001)     3677 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/minimap2.py
+-rw-r--r--   0 build     (1000) build     (1001)     5492 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/readknead.py
+-rw-r--r--   0 build     (1000) build     (1001)     2950 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/samtools_sort.py
+-rw-r--r--   0 build     (1000) build     (1001)     3625 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/samtools_uniquify.py
+-rw-r--r--   0 build     (1000) build     (1001)     3235 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/star.py
+-rw-r--r--   0 build     (1000) build     (1001)     8654 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/trackhub.py
+-rw-r--r--   0 build     (1000) build     (1001)     1739 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/utils.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.565586 labxpipe-0.6.0/src/labxpipe.egg-info/
+-rw-r--r--   0 build     (1000) build     (1001)    12773 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)     1715 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1001)        1 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1001)       56 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1001)       44 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1001)       26 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/top_level.txt
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.568920 labxpipe-0.6.0/src/labxpipe_scripts/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/__init__.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     2440 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    15493 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_demultiplex.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     7803 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_extract.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     7704 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_generate.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    17284 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_merge_count.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     4243 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_profile.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    13924 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_report.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    16815 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_run.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    21424 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_trackhub.py
```

### Comparing `labxpipe-0.5.0/.sourcehut/arch.yml` & `labxpipe-0.6.0/.sourcehut/arch.yml`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/LICENSE` & `labxpipe-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/PKG-INFO` & `labxpipe-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labxpipe
-Version: 0.5.0
+Version: 0.6.0
 Summary: Genomics pipelines
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: homepage, https://git.sr.ht/~vejnar/LabxPipe
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `labxpipe-0.5.0/README.md` & `labxpipe-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/config/labxpipe.json` & `labxpipe-0.6.0/config/labxpipe.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/config/labxpipe_trackhub.json` & `labxpipe-0.6.0/config/labxpipe_trackhub.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/config/pipelines/chip_seq.json` & `labxpipe-0.6.0/config/pipelines/chip_seq.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/config/pipelines/mrna_seq.json` & `labxpipe-0.6.0/config/pipelines/mrna_seq.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/config/pipelines/mrna_seq_cufflinks.json` & `labxpipe-0.6.0/config/pipelines/mrna_seq_cufflinks.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/config/pipelines/mrna_seq_no_db.json` & `labxpipe-0.6.0/config/pipelines/mrna_seq_no_db.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/config/pipelines/mrna_seq_with_plotting.json` & `labxpipe-0.6.0/config/pipelines/mrna_seq_with_plotting.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/img/logo.svg` & `labxpipe-0.6.0/img/logo.svg`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/pyproject.toml` & `labxpipe-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_bg2bw.py` & `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_bg2bw.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_bowtie2.py` & `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_bowtie2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_cufflinks.py` & `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_cufflinks.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_geneabacus.py` & `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_geneabacus.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_readknead.py` & `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_readknead.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_samtools.py` & `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_samtools.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/interfaces/if_exe_star.py` & `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_star.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/parallel_helpers.py` & `labxpipe-0.6.0/src/labxpipe/parallel_helpers.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/steps/bowtie2.py` & `labxpipe-0.6.0/src/labxpipe/steps/bowtie2.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,18 +24,22 @@
     return int((8 * 1024 * 1024 * 1024) / (num_processor * 0.2))
 
 
 def run(path_in, path_out, params):
     # Parameters
     logger = logging.getLogger(params['logger_name'] + '.' + params['step_name'])
 
-    # Check compress_sam and index_bam aren't used together
-    assert not (
-        params.get('compress_sam', False) and params.get('index_bam', False)
-    ), 'Options compress_sam and index_bam incompatible'
+    # Keep output SAM if BAM is requested by user
+    compress_sam_cmd = params.get('compress_sam_cmd')
+    if params.get('compress_sam', False) and compress_sam_cmd is None:
+        if params.get('create_bam', False) or params.get('index_bam', False):
+            compress_sam_cmd = ['zstd', '--keep', '-12']
+        else:
+            compress_sam_cmd = ['zstd', '--rm', '-12']
+        logger.info(f'Output compression using {compress_sam_cmd}')
 
     # Input
     fq_files = get_fastqs_per_end(path_in, params.get('paired'), params.get('fastq_exts'), params.get('read_regexs_in'))
     # Check input
     if len(fq_files) == 0:
         raise ValueError('No input FASTQ file found')
 
@@ -77,35 +81,34 @@
         fq_files[0],
         fq_files[1],
         quality_score=params.get('quality_scores'),
         outfile=os.path.join(path_out, params['output']),
         bwt_index=os.path.join(params['path_bowtie2_index'], params['index']),
         num_processor=str(params['num_processor']),
         compress_sam=params.get('compress_sam', False),
-        compress_sam_cmd=params.get('compress_sam_cmd'),
+        compress_sam_cmd=compress_sam_cmd,
         others=others,
         exe=bowtie2_exe,
         return_std=True,
         cwd=path_out,
         logger=logger,
     )
 
     # Create and index BAM file
     if params.get('create_bam', False):
-        if_exe_samtools.create_bam(os.path.join(path_out, params['output']), exe=bowtie2_exe, logger=logger)
+        if_exe_samtools.create_bam(os.path.join(path_out, params['output']), logger=logger)
     elif params.get('index_bam', False):
         if_exe_samtools.create_bam(
             os.path.join(path_out, params['output']),
             sort=True,
             max_memory=get_max_ram(params['num_processor']),
-            exe=bowtie2_exe,
             logger=logger,
         )
         if_exe_samtools.create_bam_index(
-            os.path.join(path_out, params['output'].replace('.sam', '.bam')), exe=bowtie2_exe, logger=logger
+            os.path.join(path_out, params['output'].replace('.sam', '.bam')), logger=logger
         )
 
     # Report
     logger.info('Report: Writing logs')
     with open(os.path.join(path_out, 'bowtie2_err.log'), 'wt') as f:
         f.write(stderr)
     with open(os.path.join(path_out, 'bowtie2_out.log'), 'wt') as f:
```

### Comparing `labxpipe-0.5.0/src/labxpipe/steps/cleaning.py` & `labxpipe-0.6.0/src/labxpipe/steps/cleaning.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/steps/cufflinks.py` & `labxpipe-0.6.0/src/labxpipe/steps/cufflinks.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/steps/geneabacus.py` & `labxpipe-0.6.0/src/labxpipe/steps/geneabacus.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/steps/readknead.py` & `labxpipe-0.6.0/src/labxpipe/steps/readknead.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/steps/samtools_sort.py` & `labxpipe-0.6.0/src/labxpipe/steps/samtools_sort.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/steps/samtools_uniquify.py` & `labxpipe-0.6.0/src/labxpipe/steps/samtools_uniquify.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/steps/star.py` & `labxpipe-0.6.0/src/labxpipe/steps/star.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/trackhub.py` & `labxpipe-0.6.0/src/labxpipe/trackhub.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe/utils.py` & `labxpipe-0.6.0/src/labxpipe/utils.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe.egg-info/PKG-INFO` & `labxpipe-0.6.0/src/labxpipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labxpipe
-Version: 0.5.0
+Version: 0.6.0
 Summary: Genomics pipelines
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: homepage, https://git.sr.ht/~vejnar/LabxPipe
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `labxpipe-0.5.0/src/labxpipe.egg-info/SOURCES.txt` & `labxpipe-0.6.0/src/labxpipe.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 src/labxpipe.egg-info/requires.txt
 src/labxpipe.egg-info/top_level.txt
 src/labxpipe/interfaces/__init__.py
 src/labxpipe/interfaces/if_exe_bg2bw.py
 src/labxpipe/interfaces/if_exe_bowtie2.py
 src/labxpipe/interfaces/if_exe_cufflinks.py
 src/labxpipe/interfaces/if_exe_geneabacus.py
+src/labxpipe/interfaces/if_exe_minimap2.py
 src/labxpipe/interfaces/if_exe_readknead.py
 src/labxpipe/interfaces/if_exe_samtools.py
 src/labxpipe/interfaces/if_exe_star.py
 src/labxpipe/steps/__init__.py
 src/labxpipe/steps/bowtie2.py
 src/labxpipe/steps/cleaning.py
 src/labxpipe/steps/cufflinks.py
 src/labxpipe/steps/geneabacus.py
+src/labxpipe/steps/minimap2.py
 src/labxpipe/steps/readknead.py
 src/labxpipe/steps/samtools_sort.py
 src/labxpipe/steps/samtools_uniquify.py
 src/labxpipe/steps/star.py
 src/labxpipe_scripts/__init__.py
 src/labxpipe_scripts/lxpipe.py
 src/labxpipe_scripts/lxpipe_demultiplex.py
```

### Comparing `labxpipe-0.5.0/src/labxpipe_scripts/lxpipe.py` & `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_demultiplex.py` & `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_demultiplex.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     for name, path_list in fastqs.items():
         # Get run info
         if dbl:
             search_criterion = []
             # Flowcell
             flowcells = set()
             for p in path_list:
-                r = labxdb.fastq.get_illumina_fastq_info(os.path.join(p['path'], p['fname']))
-                flowcells.add(r['flowcell'])
+                fastq_info = labxdb.fastq.get_fastq_info(os.path.join(p['path'], p['fname']), [labxdb.fastq.get_illumina_fastq_info, labxdb.fastq.get_pacbio_fastq_info])
+                flowcells.add(fastq_info['flowcell'])
             if len(flowcells) == 1:
                 flowcell = list(flowcells)[0]
                 search_criterion.append('3 flowcell FUZZY '+flowcell)
             else:
                 raise Error('Multiple flowcell detected in a single run')
             # Tube label
             search_criterion.append('3 tube_label EQUAL '+name)
```

### Comparing `labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_extract.py` & `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     parser = argparse.ArgumentParser(prog=prog, description='Extract & rename project output files.')
     parser.add_argument('-c', '--pipeline', dest='path_pipeline', action='store', required=True, help='Path to pipeline')
     parser.add_argument('-f', '--files', dest='files', action='store', required=True, help='Files to extract (comma separated list of step,filename pairs)')
     parser.add_argument('-o', '--path_extract', dest='path_extract', action='store', default='.', help='Path to output')
     parser.add_argument('-l', '--label', dest='use_label', action='store_true', help='Use label to rename')
     parser.add_argument('-r', '--reference', dest='use_reference', action='store_true', help='Use reference to rename')
     parser.add_argument('-w', '--lowercase', dest='lowercase', action='store_true', help='Lowercase filename')
+    parser.add_argument('-x', '--suffix', dest='suffix', action='store_true', help='Suffix input filename to output filename')
     parser.add_argument('-e', '--extensions', dest='search_extensions', action='store', help='File extensions to search (comma separated)')
     parser.add_argument('-d', '--dry_run', dest='dry_run', action='store_true', help='Dry run')
     parser.add_argument('--path_config', dest='path_config', action='store', help='Path to config')
     parser.add_argument('--http_url', '--labxdb_http_url', dest='labxdb_http_url', action='store', help='Database HTTP URL')
     parser.add_argument('--http_login', '--labxdb_http_login', dest='labxdb_http_login', action='store', help='Database HTTP login')
     parser.add_argument('--http_password', '--labxdb_http_password', dest='labxdb_http_password', action='store', help='Database HTTP password')
     parser.add_argument('--http_path', '--labxdb_http_path', dest='labxdb_http_path', action='store', help='Database HTTP path')
@@ -125,28 +126,33 @@
     for ref in labxpipe.utils.get_first_key(('run_refs', 'replicate_refs'), config):
         for step, fname in files:
             path_in = os.path.join(config['path_output'], ref, step, fname)
             if os.path.exists(path_in):
                 fname_ext = None
                 for ext in labxpipe.utils.all_exts + config['search_extensions']:
                     if fname.rfind(ext) != -1:
+                        fname_base = fname[: fname.rfind(ext)]
                         fname_ext = fname[fname.rfind(ext) :]
                         break
                 if fname_ext is None:
+                    fname_base = fname[: fname.rfind('.')]
                     fname_ext = fname[fname.rfind('.') :]
                 if fname_ext is None:
+                    fname_base = fname
                     fname_ext = fname
                 if args.use_label:
                     label = labxpipe.utils.label2var(config['ref_infos'][ref]['label_short'])
                 if args.use_label and args.use_reference:
                     name = f'{label}_{ref}'
                 elif args.use_label:
                     name = label
                 elif args.use_reference:
                     name = ref
+                if args.suffix:
+                    name += f'_{fname_base}'
                 if args.lowercase:
                     name = name.lower()
                 path_out = os.path.join(config['path_extract'], name + fname_ext)
                 moves.append((path_in, path_out))
 
     # Check move filenames are unique
     tmp = set()
```

### Comparing `labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_generate.py` & `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_generate.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_merge_count.py` & `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_merge_count.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_profile.py` & `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_profile.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_report.py` & `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,21 +97,22 @@
             path_report = os.path.join(path_root, step['step_name'], step['step_name']+'_report.json')
             # Parse report
             if os.path.exists(path_report):
                 parse_step(json.load(open(path_report)), (step['step_name'], ), all_report)
                 # Percent for spreadsheet
                 if spreadsheet:
                     all_report[(step['step_name'], '%')] = None
-            elif step['step_name'] == 'counting':
+            elif 'features' in step:
                 for feat in step['features']:
-                    path_report = os.path.join(path_root, step['step_name'], feat['name']+'_report.json')
-                    if os.path.exists(path_report):
-                        parse_step(json.load(open(path_report)), (step['step_name'], feat['name']), all_report)
-                        if spreadsheet:
-                            all_report[(step['step_name'], feat['name'], '%')] = None
+                    if 'name' in feat:
+                        path_report = os.path.join(path_root, step['step_name'], feat['name']+'_report.json')
+                        if os.path.exists(path_report):
+                            parse_step(json.load(open(path_report)), (step['step_name'], feat['name']), all_report)
+                            if spreadsheet:
+                                all_report[(step['step_name'], feat['name'], '%')] = None
         # Get computing time
         path_compl = os.path.join(path_root, 'log', config['name']+'_compl.json')
         if os.path.exists(path_compl):
             compl_steps = json.load(open(path_compl))
             total_time = datetime.timedelta(0)
             for step in compl_steps:
                 if step['start'] and step['end']:
```

### Comparing `labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_run.py` & `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_run.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.5.0/src/labxpipe_scripts/lxpipe_trackhub.py` & `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_trackhub.py`

 * *Files identical despite different names*

