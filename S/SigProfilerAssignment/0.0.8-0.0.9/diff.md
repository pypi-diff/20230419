# Comparing `tmp/SigProfilerAssignment-0.0.8.tar.gz` & `tmp/SigProfilerAssignment-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SigProfilerAssignment-0.0.8.tar", last modified: Wed Jul 20 23:29:50 2022, max compression
+gzip compressed data, was "SigProfilerAssignment-0.0.9.tar", last modified: Wed Aug  3 21:52:13 2022, max compression
```

## Comparing `SigProfilerAssignment-0.0.8.tar` & `SigProfilerAssignment-0.0.9.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.724985 SigProfilerAssignment-0.0.8/
--rw-r--r--   0 rvangara   (503) staff       (20)     1342 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/LICENSE.txt
--rw-r--r--   0 rvangara   (503) staff       (20)      542 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/MANIFEST.in
--rw-r--r--   0 rvangara   (503) staff       (20)     8267 2022-07-20 23:29:50.724442 SigProfilerAssignment-0.0.8/PKG-INFO
--rw-r--r--   0 rvangara   (503) staff       (20)     7901 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/README.md
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.664666 SigProfilerAssignment-0.0.8/SigProfilerAssignment/
--rw-r--r--   0 rvangara   (503) staff       (20)     2738 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/Analyzer.py
--rw-r--r--   0 rvangara   (503) staff       (20)       49 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/__init__.py
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.671016 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/
--rwxr-xr-x   0 rvangara   (503) staff       (20)     3342 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat
--rw-r--r--   0 rvangara   (503) staff       (20)     4864 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Accolade_fermante.png
--rw-r--r--   0 rvangara   (503) staff       (20)      803 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/CNV_features.tsv
--rw-r--r--   0 rvangara   (503) staff       (20)    15995 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/CNV_signatures.txt
--rw-r--r--   0 rvangara   (503) staff       (20)     1641 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/CN_classes_dictionary.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   128402 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.660902 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.676963 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/
--rw-r--r--   0 rvangara   (503) staff       (20)    14328 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt
--rwxr-xr-x   0 rvangara   (503) staff       (20)    36586 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17758 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    29489 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   137506 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17758 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    29489 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   109467 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   148966 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    18940 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17759 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    29808 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   149327 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17757 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    28686 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt
--rwxr-xr-x   0 rvangara   (503) staff       (20)   128501 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.681061 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/
--rw-r--r--   0 rvangara   (503) staff       (20)    39244 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    53205 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17833 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   138534 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17833 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   150027 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17825 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   150274 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17829 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   129685 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.684980 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/
--rw-r--r--   0 rvangara   (503) staff       (20)    39213 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    53208 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17834 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   138625 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17834 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   150107 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17836 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   150444 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17836 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   129718 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.689777 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/
--rw-r--r--   0 rvangara   (503) staff       (20)    39213 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    53199 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17839 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   138548 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17839 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   150036 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17842 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   150387 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17837 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   129655 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.694849 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/
--rw-r--r--   0 rvangara   (503) staff       (20)    39230 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    53187 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17837 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   138524 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17837 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   150001 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17838 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   150274 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)    17840 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   129663 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt
--rw-r--r--   0 rvangara   (503) staff       (20)   380152 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx
--rw-r--r--   0 rvangara   (503) staff       (20)     7124 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Samples.txt
--rw-r--r--   0 rvangara   (503) staff       (20)     3851 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/csvexample.csv
--rwxr-xr-x   0 rvangara   (503) staff       (20)     8338 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv
--rw-r--r--   0 rvangara   (503) staff       (20)    16970 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv
--rwxr-xr-x   0 rvangara   (503) staff       (20)    57422 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.712172 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/
--rw-r--r--   0 rvangara   (503) staff       (20)    42134 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3851a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   144692 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3890a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   132516 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3904a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   108261 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3905a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   243267 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3945a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   144314 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4005a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   217281 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4006a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)    63094 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4085a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)    51960 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4086a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)    40304 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4088a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   126650 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4103a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   243377 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4107a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   233696 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4109a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   235200 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4115a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   189909 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4116a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)  1672536 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4120a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)    92642 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4192a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)    35093 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4194a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   107668 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4198a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)   164069 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4199a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)    59915 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4248a.vcf
--rw-r--r--   0 rvangara   (503) staff       (20)    50659 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/decompose_sub_routines.py
--rw-r--r--   0 rvangara   (503) staff       (20)    24218 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/decomposition.py
--rw-r--r--   0 rvangara   (503) staff       (20)    35439 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/single_sample.py
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.713721 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/
--rw-r--r--   0 rvangara   (503) staff       (20)    12535 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/Accolade_fermante.png
--rw-r--r--   0 rvangara   (503) staff       (20)      165 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/CREDIT.md
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.714216 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/Fonts/
--rw-r--r--   0 rvangara   (503) staff       (20)   750984 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/Fonts/Arial Bold.ttf
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.723660 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/
--rw-r--r--   0 rvangara   (503) staff       (20)    13740 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS1248.all
--rw-r--r--   0 rvangara   (503) staff       (20)     1686 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS186.all
--rw-r--r--   0 rvangara   (503) staff       (20)    38700 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS2976.all
--rw-r--r--   0 rvangara   (503) staff       (20)      558 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS78.all
--rw-r--r--   0 rvangara   (503) staff       (20)      309 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID28.all
--rw-r--r--   0 rvangara   (503) staff       (20)     5407 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID415.all
--rw-r--r--   0 rvangara   (503) staff       (20)      926 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID83.all
--rw-r--r--   0 rvangara   (503) staff       (20)    16908 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS1536.all
--rw-r--r--   0 rvangara   (503) staff       (20)      180 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS24.all
--rw-r--r--   0 rvangara   (503) staff       (20)     4236 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS384.all
--rw-r--r--   0 rvangara   (503) staff       (20)       42 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS6.all
--rw-r--r--   0 rvangara   (503) staff       (20)    79884 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS6144.all
--rw-r--r--   0 rvangara   (503) staff       (20)      876 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS96.all
--rw-r--r--   0 rvangara   (503) staff       (20)      193 2022-07-20 23:29:49.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment/version.py
-drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-07-20 23:29:50.666497 SigProfilerAssignment-0.0.8/SigProfilerAssignment.egg-info/
--rw-r--r--   0 rvangara   (503) staff       (20)     8267 2022-07-20 23:29:50.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment.egg-info/PKG-INFO
--rw-r--r--   0 rvangara   (503) staff       (20)     7481 2022-07-20 23:29:50.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment.egg-info/SOURCES.txt
--rw-r--r--   0 rvangara   (503) staff       (20)        1 2022-07-20 23:29:50.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment.egg-info/dependency_links.txt
--rw-r--r--   0 rvangara   (503) staff       (20)        1 2022-07-20 23:29:50.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment.egg-info/not-zip-safe
--rw-r--r--   0 rvangara   (503) staff       (20)      241 2022-07-20 23:29:50.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment.egg-info/requires.txt
--rw-r--r--   0 rvangara   (503) staff       (20)       22 2022-07-20 23:29:50.000000 SigProfilerAssignment-0.0.8/SigProfilerAssignment.egg-info/top_level.txt
--rw-r--r--   0 rvangara   (503) staff       (20)       38 2022-07-20 23:29:50.725134 SigProfilerAssignment-0.0.8/setup.cfg
--rw-r--r--   0 rvangara   (503) staff       (20)     1667 2022-07-20 23:28:35.000000 SigProfilerAssignment-0.0.8/setup.py
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.973816 SigProfilerAssignment-0.0.9/
+-rw-r--r--   0 rvangara   (503) staff       (20)     1342 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/LICENSE.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)      542 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/MANIFEST.in
+-rw-r--r--   0 rvangara   (503) staff       (20)     8265 2022-08-03 21:52:13.973404 SigProfilerAssignment-0.0.9/PKG-INFO
+-rw-r--r--   0 rvangara   (503) staff       (20)     7899 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/README.md
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.913004 SigProfilerAssignment-0.0.9/SigProfilerAssignment/
+-rw-r--r--   0 rvangara   (503) staff       (20)     2738 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/Analyzer.py
+-rw-r--r--   0 rvangara   (503) staff       (20)       49 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/__init__.py
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.920185 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/
+-rwxr-xr-x   0 rvangara   (503) staff       (20)     3342 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat
+-rw-r--r--   0 rvangara   (503) staff       (20)     4864 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Accolade_fermante.png
+-rw-r--r--   0 rvangara   (503) staff       (20)      803 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/CNV_features.tsv
+-rw-r--r--   0 rvangara   (503) staff       (20)    15995 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/CNV_signatures.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)     1641 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/CN_classes_dictionary.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   128402 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.908617 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.930908 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/
+-rw-r--r--   0 rvangara   (503) staff       (20)    14328 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt
+-rwxr-xr-x   0 rvangara   (503) staff       (20)    36586 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17758 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    29489 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   137506 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17758 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    29489 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   109467 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   148966 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    18940 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17759 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    29808 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   149327 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17757 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    28686 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt
+-rwxr-xr-x   0 rvangara   (503) staff       (20)   128501 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.938063 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/
+-rw-r--r--   0 rvangara   (503) staff       (20)    39244 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    53205 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17833 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   138534 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17833 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   150027 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17825 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   150274 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17829 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   129685 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.943276 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/
+-rw-r--r--   0 rvangara   (503) staff       (20)    39213 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    53208 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17834 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   138625 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17834 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   150107 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17836 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   150444 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17836 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   129718 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.947630 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/
+-rw-r--r--   0 rvangara   (503) staff       (20)    39213 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    53199 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17839 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   138548 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17839 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   150036 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17842 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   150387 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17837 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   129655 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.952896 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/
+-rw-r--r--   0 rvangara   (503) staff       (20)    39230 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    53187 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17837 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   138524 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17837 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   150001 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17838 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   150274 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)    17840 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   129663 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)   380152 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx
+-rw-r--r--   0 rvangara   (503) staff       (20)     7124 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Samples.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)     3851 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/csvexample.csv
+-rwxr-xr-x   0 rvangara   (503) staff       (20)     8338 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv
+-rw-r--r--   0 rvangara   (503) staff       (20)    16970 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv
+-rwxr-xr-x   0 rvangara   (503) staff       (20)    57422 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.965959 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/
+-rw-r--r--   0 rvangara   (503) staff       (20)    42134 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3851a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   144692 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3890a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   132516 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3904a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   108261 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3905a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   243267 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3945a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   144314 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4005a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   217281 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4006a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)    63094 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4085a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)    51960 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4086a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)    40304 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4088a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   126650 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4103a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   243377 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4107a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   233696 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4109a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   235200 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4115a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   189909 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4116a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)  1672536 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4120a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)    92642 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4192a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)    35093 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4194a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   107668 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4198a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)   164069 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4199a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)    59915 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4248a.vcf
+-rw-r--r--   0 rvangara   (503) staff       (20)    50656 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/decompose_sub_routines.py
+-rw-r--r--   0 rvangara   (503) staff       (20)    24216 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/decomposition.py
+-rw-r--r--   0 rvangara   (503) staff       (20)    35439 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/single_sample.py
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.966975 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/
+-rw-r--r--   0 rvangara   (503) staff       (20)    12535 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/Accolade_fermante.png
+-rw-r--r--   0 rvangara   (503) staff       (20)      165 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/CREDIT.md
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.967303 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/Fonts/
+-rw-r--r--   0 rvangara   (503) staff       (20)   750984 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/Fonts/Arial Bold.ttf
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.972946 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/
+-rw-r--r--   0 rvangara   (503) staff       (20)    13740 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS1248.all
+-rw-r--r--   0 rvangara   (503) staff       (20)     1686 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS186.all
+-rw-r--r--   0 rvangara   (503) staff       (20)    38700 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS2976.all
+-rw-r--r--   0 rvangara   (503) staff       (20)      558 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS78.all
+-rw-r--r--   0 rvangara   (503) staff       (20)      309 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID28.all
+-rw-r--r--   0 rvangara   (503) staff       (20)     5407 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID415.all
+-rw-r--r--   0 rvangara   (503) staff       (20)      925 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID83.all
+-rw-r--r--   0 rvangara   (503) staff       (20)    16908 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS1536.all
+-rw-r--r--   0 rvangara   (503) staff       (20)      180 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS24.all
+-rw-r--r--   0 rvangara   (503) staff       (20)     4236 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS384.all
+-rw-r--r--   0 rvangara   (503) staff       (20)       42 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS6.all
+-rw-r--r--   0 rvangara   (503) staff       (20)    79884 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS6144.all
+-rw-r--r--   0 rvangara   (503) staff       (20)      876 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS96.all
+-rw-r--r--   0 rvangara   (503) staff       (20)      183 2022-08-03 21:52:13.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment/version.py
+drwxr-xr-x   0 rvangara   (503) staff       (20)        0 2022-08-03 21:52:13.914771 SigProfilerAssignment-0.0.9/SigProfilerAssignment.egg-info/
+-rw-r--r--   0 rvangara   (503) staff       (20)     8265 2022-08-03 21:52:13.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment.egg-info/PKG-INFO
+-rw-r--r--   0 rvangara   (503) staff       (20)     7481 2022-08-03 21:52:13.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment.egg-info/SOURCES.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)        1 2022-08-03 21:52:13.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment.egg-info/dependency_links.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)        1 2022-08-03 21:52:13.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment.egg-info/not-zip-safe
+-rw-r--r--   0 rvangara   (503) staff       (20)      239 2022-08-03 21:52:13.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment.egg-info/requires.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)       22 2022-08-03 21:52:13.000000 SigProfilerAssignment-0.0.9/SigProfilerAssignment.egg-info/top_level.txt
+-rw-r--r--   0 rvangara   (503) staff       (20)       38 2022-08-03 21:52:13.973947 SigProfilerAssignment-0.0.9/setup.cfg
+-rw-r--r--   0 rvangara   (503) staff       (20)     1655 2022-08-03 21:51:36.000000 SigProfilerAssignment-0.0.9/setup.py
```

### Comparing `SigProfilerAssignment-0.0.8/LICENSE.txt` & `SigProfilerAssignment-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/MANIFEST.in` & `SigProfilerAssignment-0.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/PKG-INFO` & `SigProfilerAssignment-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SigProfilerAssignment
-Version: 0.0.8
+Version: 0.0.9
 Summary: Mutational signatures attribution and decomposition tool
 Home-page: https://github.com/AlexandrovLab/SigProfilerAssignment.git
 Author: Raviteja Vangara
 Author-email: rvangara@health.ucsd.edu
 License: UCSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -44,15 +44,15 @@
 ```python
 signature_subgroups = ['remove_MMR_deficiency_signatures',
                        'remove_POL_deficiency_signatures',
                        'remove_HR_deficiency_signatures' ,
                        'remove_BER_deficiency_signatures',
                        'remove_Chemotherapy_signatures',
                        'remove_Immunosuppressants_signatures'
-                       'remove_Iatrogenic_signatures'
+                       'remove_Treatment_signatures'
                        'remove_APOBEC_signatures',
                        'remove_Tobacco_signatures',
                        'remove_UV_signatures',
                        'remove_AA_signatures',
                        'remove_Colibactin_signatures',
                        'remove_Artifact_signatures',
                        'remove_Lymphoid_signatures']
@@ -63,15 +63,15 @@
 | ----------- | ----------- |
 |MMR_deficiency_signatures|	6, 14, 15, 20, 21, 26, 44|
 |POL_deficiency_signatures|	10a, 10b, 10c, 10d, 28|
 |HR_deficiency_signatures|	3|
 |BER_deficiency_signatures|	30, 36|
 |Chemotherapy_signatures|	11, 25, 31, 35, 86, 87, 90|
 |Immunosuppressants_signatures|	32|
-|Iatrogenic_signatures|	11, 25, 31, 32, 35, 86, 87, 90|
+|Treatment_signatures|	11, 25, 31, 32, 35, 86, 87, 90|
 |APOBEC_signatures|	2, 13|
 |Tobacco_signatures	|4, 29, 92|
 |UV_signatures|	7a, 7b, 7c, 7d, 38|
 |AA_signatures|	22|
 |Colibactin_signatures|	88|
 |Artifact_signatures|	27, 43, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60|
 |Lymphoid_signatures|	9, 84, 85|
```

### Comparing `SigProfilerAssignment-0.0.8/README.md` & `SigProfilerAssignment-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ```python
 signature_subgroups = ['remove_MMR_deficiency_signatures',
                        'remove_POL_deficiency_signatures',
                        'remove_HR_deficiency_signatures' ,
                        'remove_BER_deficiency_signatures',
                        'remove_Chemotherapy_signatures',
                        'remove_Immunosuppressants_signatures'
-                       'remove_Iatrogenic_signatures'
+                       'remove_Treatment_signatures'
                        'remove_APOBEC_signatures',
                        'remove_Tobacco_signatures',
                        'remove_UV_signatures',
                        'remove_AA_signatures',
                        'remove_Colibactin_signatures',
                        'remove_Artifact_signatures',
                        'remove_Lymphoid_signatures']
@@ -51,15 +51,15 @@
 | ----------- | ----------- |
 |MMR_deficiency_signatures|	6, 14, 15, 20, 21, 26, 44|
 |POL_deficiency_signatures|	10a, 10b, 10c, 10d, 28|
 |HR_deficiency_signatures|	3|
 |BER_deficiency_signatures|	30, 36|
 |Chemotherapy_signatures|	11, 25, 31, 35, 86, 87, 90|
 |Immunosuppressants_signatures|	32|
-|Iatrogenic_signatures|	11, 25, 31, 32, 35, 86, 87, 90|
+|Treatment_signatures|	11, 25, 31, 32, 35, 86, 87, 90|
 |APOBEC_signatures|	2, 13|
 |Tobacco_signatures	|4, 29, 92|
 |UV_signatures|	7a, 7b, 7c, 7d, 38|
 |AA_signatures|	22|
 |Colibactin_signatures|	88|
 |Artifact_signatures|	27, 43, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60|
 |Lymphoid_signatures|	9, 84, 85|
```

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/Analyzer.py` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/Analyzer.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Accolade_fermante.png` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Accolade_fermante.png`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/CNV_features.tsv` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/CNV_features.tsv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/CNV_signatures.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/CNV_signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/CN_classes_dictionary.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/CN_classes_dictionary.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/Samples.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/Samples.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/csvexample.csv` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/csvexample.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3851a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3851a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3890a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3890a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3904a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3904a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3905a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3905a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD3945a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD3945a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4005a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4005a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4006a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4006a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4085a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4085a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4086a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4086a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4088a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4088a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4103a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4103a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4107a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4107a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4109a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4109a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4115a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4115a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4116a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4116a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4120a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4120a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4192a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4192a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4194a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4194a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4198a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4198a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4199a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4199a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/data/vcftest/PD4248a.vcf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/data/vcftest/PD4248a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/decompose_sub_routines.py` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/decompose_sub_routines.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
         try:
             # import pdb
             # pdb.set_trace() 
             if mtype_par!="none" and make_decomposition_plots==True:
                 # Get the names of the columns for each dataframe
                 denovo_col_names = originalProcessAvg.columns
                 cosmic_col_names = sigDatabases_DF.columns
-                # Get the name for the MutationTypes column
+                # Get the name for the MutationType column
                 cosmic_mut_types_col = cosmic_col_names[0]
                 denovo_mut_types_col =  denovo_col_names[0]
                 # create lists of implemented columns
                 basis_cols = basis_names.copy()
                 basis_cols.insert(0,cosmic_mut_types_col)
                 denovo_cols=[denovo_mut_types_col, denovo_name]
                 byte_plot = sp.run_PlotDecomposition(originalProcessAvg[denovo_cols], denovo_name, sigDatabases_DF[basis_cols], basis_names, weights, nonzero_exposures/5000, directory, "test", mtype_par)
@@ -671,15 +671,15 @@
         # when use the exposures from the initial NMF
         else:
             exposureAvg=denovo_exposureAvg
 
     processAvg= pd.DataFrame(processAvg.astype(float))
     processes = processAvg.set_index(index)
     processes.columns = allsigids
-    processes = processes.rename_axis("MutationsType", axis="columns")
+    processes = processes.rename_axis("MutationType", axis="columns")
     processes.to_csv(layer_directory+"/Signatures"+"/"+solution_prefix+"_"+"Signatures.txt", "\t", float_format='%.8f',index_label=[processes.columns.name]) 
     exposureAvg = pd.DataFrame(exposureAvg.astype(int))
     allsigids = np.array(allsigids)
     exposures = exposureAvg.set_index(allsigids)
     exposures.columns = allcolnames
     exposures = exposures.T
     exposures = exposures.rename_axis("Samples", axis="columns")
@@ -877,15 +877,15 @@
         
         M = genomes[:,i][np.newaxis]
         probs = W*H[:,i]/M.T        
         probs = pd.DataFrame(probs)
         probs.columns = sigs
         col1 = [cols[i]]*len(rows)
         probs.insert(loc=0, column='Sample Names', value=col1)
-        probs.insert(loc=1, column='MutationTypes', value = rows)
+        probs.insert(loc=1, column='MutationType', value = rows)
         if i!=0:
             result = pd.concat([result, probs], axis=0)
         else:
             result = probs
     
         
     return result
```

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/decomposition.py` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,30 +93,30 @@
     
     default_subgroups_dict= {'remove_MMR_deficiency_signatures' :False,
                       'remove_POL_deficiency_signatures' :False,
                       'remove_HR_deficiency_signatures' :False,
                       'remove_BER_deficiency_signatures' :False,
                       'remove_Chemotherapy_signatures' :False,
                       'remove_Immunosuppressants_signatures' :False,
-                      'remove_Iatrogenic_signatures' :False,
+                      'remove_Treatment_signatures' :False,
                       'remove_APOBEC_signatures' :False,
                       'remove_Tobacco_signatures' :False,
                       'remove_UV_signatures' :False,
                       'remove_AA_signatures' :False,
                       'remove_Colibactin_signatures' :False,
                       'remove_Artifact_signatures' :False,
                       'remove_Lymphoid_signatures' :False}
                       
     default_subgroups_siglists= {'remove_MMR_deficiency_signatures' :['6', '14', '15', '20', '21', '26', '44'],
                       'remove_POL_deficiency_signatures' :['10a', '10b', '10c', '10d', '28'],
                       'remove_HR_deficiency_signatures' :['3'],
                       'remove_BER_deficiency_signatures' :['30','36'],
                       'remove_Chemotherapy_signatures' :['11','25','31','35','86','87','90'],
                       'remove_Immunosuppressants_signatures' :['32'],
-                      'remove_Iatrogenic_signatures' :['11','25','31','32','35','86','87','90'],
+                      'remove_Treatment_signatures' :['11','25','31','32','35','86','87','90'],
                       'remove_APOBEC_signatures' :['2','13'],
                       'remove_Tobacco_signatures' :['4','29','92'],
                       'remove_UV_signatures' :['7a','7b','7c','7d','38'],
                       'remove_AA_signatures' :['22'],
                       'remove_Colibactin_signatures' :['88'],
                       'remove_Artifact_signatures' :['27','43','45','46','47','48','49','50','51','52','53','54','55','56','57','58','59','60'],
                       'remove_Lymphoid_signatures' :['9','84','85']}
```

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/single_sample.py` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/single_sample.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/Accolade_fermante.png` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/Accolade_fermante.png`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/Fonts/Arial Bold.ttf` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/Fonts/Arial Bold.ttf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS1248.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS1248.all`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS186.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS186.all`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS2976.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS2976.all`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS78.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.DBS78.all`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID415.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID415.all`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID83.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.ID83.all`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MutationsType
+MutationType
 1:Del:C:0
 1:Del:C:1
 1:Del:C:2
 1:Del:C:3
 1:Del:C:4
 1:Del:C:5
 1:Del:T:0
```

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS1536.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS1536.all`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS384.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS384.all`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS6144.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS6144.all`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS96.all` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment/src/FormatFiles/Sample_Files.SBS96.all`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment.egg-info/PKG-INFO` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SigProfilerAssignment
-Version: 0.0.8
+Version: 0.0.9
 Summary: Mutational signatures attribution and decomposition tool
 Home-page: https://github.com/AlexandrovLab/SigProfilerAssignment.git
 Author: Raviteja Vangara
 Author-email: rvangara@health.ucsd.edu
 License: UCSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -44,15 +44,15 @@
 ```python
 signature_subgroups = ['remove_MMR_deficiency_signatures',
                        'remove_POL_deficiency_signatures',
                        'remove_HR_deficiency_signatures' ,
                        'remove_BER_deficiency_signatures',
                        'remove_Chemotherapy_signatures',
                        'remove_Immunosuppressants_signatures'
-                       'remove_Iatrogenic_signatures'
+                       'remove_Treatment_signatures'
                        'remove_APOBEC_signatures',
                        'remove_Tobacco_signatures',
                        'remove_UV_signatures',
                        'remove_AA_signatures',
                        'remove_Colibactin_signatures',
                        'remove_Artifact_signatures',
                        'remove_Lymphoid_signatures']
@@ -63,15 +63,15 @@
 | ----------- | ----------- |
 |MMR_deficiency_signatures|	6, 14, 15, 20, 21, 26, 44|
 |POL_deficiency_signatures|	10a, 10b, 10c, 10d, 28|
 |HR_deficiency_signatures|	3|
 |BER_deficiency_signatures|	30, 36|
 |Chemotherapy_signatures|	11, 25, 31, 35, 86, 87, 90|
 |Immunosuppressants_signatures|	32|
-|Iatrogenic_signatures|	11, 25, 31, 32, 35, 86, 87, 90|
+|Treatment_signatures|	11, 25, 31, 32, 35, 86, 87, 90|
 |APOBEC_signatures|	2, 13|
 |Tobacco_signatures	|4, 29, 92|
 |UV_signatures|	7a, 7b, 7c, 7d, 38|
 |AA_signatures|	22|
 |Colibactin_signatures|	88|
 |Artifact_signatures|	27, 43, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60|
 |Lymphoid_signatures|	9, 84, 85|
```

### Comparing `SigProfilerAssignment-0.0.8/SigProfilerAssignment.egg-info/SOURCES.txt` & `SigProfilerAssignment-0.0.9/SigProfilerAssignment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.0.8/setup.py` & `SigProfilerAssignment-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 import shutil
 import os
 
 #remove the dist folder first if exists
 if os.path.exists("dist"):
     shutil.rmtree("dist")
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 
 with open('README.md') as f:
 	long_description = f.read()
 
 def write_version_py(filename='SigProfilerAssignment/version.py'):
     # Copied from numpy setup.py
     cnt = """
 # THIS FILE IS GENERATED FROM SigProfilerAssignment SETUP.PY
 short_version = '%(version)s'
 version = '%(version)s'
-Update = '1.Copy number Signatures support 2. Fixed bugs on signature subtypes'
+Update = '1. Make consistent MutationType column 2. Update subgroups'
     
     """
     fh = open(filename, 'w')
     fh.write(cnt % {'version': VERSION,})
     fh.close()
 requirements=[
           'scipy>=1.6.3',
           'numpy>=1.21.2',
           'pandas>=1.2.4', 
-          'SigProfilerExtractor>=1.1.7',
-          'SigProfilerMatrixGenerator>=1.1.30', 
-          'sigProfilerPlotting>=1.1.15', 
+          'SigProfilerExtractor>=1.1.9',
+          'SigProfilerMatrixGenerator>=1.2.9', 
+          'sigProfilerPlotting>=1.2.2', 
           'pillow',
           'statsmodels>=0.9.0',
           'scikit-learn>=0.24.2',
           'psutil>=5.6.1',
           'reportlab>=3.5.42',
           'PyPDF2>=1.26.0',
           'alive_progress'
```

