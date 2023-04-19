# Comparing `tmp/eQTac-1.0.4.tar.gz` & `tmp/eQTac-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eQTac-1.0.4.tar", last modified: Wed Apr 19 08:10:21 2023, max compression
+gzip compressed data, was "eQTac-1.0.5.tar", last modified: Wed Apr 19 09:10:48 2023, max compression
```

## Comparing `eQTac-1.0.4.tar` & `eQTac-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 08:10:21.222872 eQTac-1.0.4/
--rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3900 2023-04-19 08:10:21.220876 eQTac-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3428 2023-04-19 06:43:03.000000 eQTac-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 08:10:21.114162 eQTac-1.0.4/eQTac/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:08:46.000000 eQTac-1.0.4/eQTac/__init__.py
--rw-rw-rw-   0        0        0     1860 2023-04-18 09:28:48.000000 eQTac-1.0.4/eQTac/control_FDR.py
--rw-rw-rw-   0        0        0     4343 2023-04-17 11:42:17.000000 eQTac-1.0.4/eQTac/eQTac_correlation.py
--rw-rw-rw-   0        0        0     2260 2023-04-17 11:42:17.000000 eQTac-1.0.4/eQTac/eQTac_permutation.py
--rw-rw-rw-   0        0        0     2644 2023-04-17 11:42:17.000000 eQTac-1.0.4/eQTac/filter_bkg.py
--rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.4/eQTac/generate_PRE.py
--rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.4/eQTac/generate_mut_fa.py
--rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.4/eQTac/generate_snp_dict.py
--rw-rw-rw-   0        0        0     3832 2023-04-17 11:42:17.000000 eQTac-1.0.4/eQTac/geno2score.py
--rw-rw-rw-   0        0        0     2480 2023-04-17 11:42:17.000000 eQTac-1.0.4/eQTac/get_nullseq.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:10:21.204918 eQTac-1.0.4/eQTac.egg-info/
--rw-rw-rw-   0        0        0     3900 2023-04-19 08:10:20.000000 eQTac-1.0.4/eQTac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-04-19 08:10:20.000000 eQTac-1.0.4/eQTac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 08:10:20.000000 eQTac-1.0.4/eQTac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-19 08:10:20.000000 eQTac-1.0.4/eQTac.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 08:10:20.000000 eQTac-1.0.4/eQTac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 08:10:21.225863 eQTac-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-04-19 08:09:38.000000 eQTac-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:10:48.926388 eQTac-1.0.5/
+-rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3922 2023-04-19 09:10:48.923396 eQTac-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3451 2023-04-19 08:43:06.000000 eQTac-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 09:10:48.815409 eQTac-1.0.5/eQTac/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:08:46.000000 eQTac-1.0.5/eQTac/__init__.py
+-rw-rw-rw-   0        0        0     1860 2023-04-18 09:28:48.000000 eQTac-1.0.5/eQTac/control_FDR.py
+-rw-rw-rw-   0        0        0     4204 2023-04-19 08:46:12.000000 eQTac-1.0.5/eQTac/eQTac_correlation.py
+-rw-rw-rw-   0        0        0     2122 2023-04-19 08:47:10.000000 eQTac-1.0.5/eQTac/eQTac_permutation.py
+-rw-rw-rw-   0        0        0     2608 2023-04-19 08:48:46.000000 eQTac-1.0.5/eQTac/filter_bkg.py
+-rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.5/eQTac/generate_PRE.py
+-rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.5/eQTac/generate_mut_fa.py
+-rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.5/eQTac/generate_snp_dict.py
+-rw-rw-rw-   0        0        0     3646 2023-04-19 08:54:46.000000 eQTac-1.0.5/eQTac/geno2score.py
+-rw-rw-rw-   0        0        0     2457 2023-04-19 08:55:27.000000 eQTac-1.0.5/eQTac/get_nullseq.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:10:48.906446 eQTac-1.0.5/eQTac.egg-info/
+-rw-rw-rw-   0        0        0     3922 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 09:10:48.928382 eQTac-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-04-19 09:05:17.000000 eQTac-1.0.5/setup.py
```

### Comparing `eQTac-1.0.4/LICENSE` & `eQTac-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.4/PKG-INFO` & `eQTac-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: eQTac
-Version: 1.0.4
+Version: 1.0.5
 Summary: The eQTac method.
 Home-page: https://github.com/JFF1594032292/eQTac
 Author: Jiang Feng
 Author-email: 1594032292@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # eQTac
----
 EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
 ## Dependence
 ### Python packages
 ```
 numpy >= 1.22.4
 pandas >= 1.4.3
 pybedtools >= 0.8.2
 pysam >= 0.16.0.1
 rpy2 >= 3.4.2
 scipy >= 1.8.1
 ```
-### Other software
+### Other software (need manual installation)
 ```
 plink >= v1.90b6.24
 bedtools >= v2.30.0
 R >= 3.6.1
     r-gkmSVM >= 0.8.0
 ```
 ## Installation
```

### Comparing `eQTac-1.0.4/README.md` & `eQTac-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # eQTac
----
 EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
 ## Dependence
 ### Python packages
 ```
 numpy >= 1.22.4
 pandas >= 1.4.3
 pybedtools >= 0.8.2
 pysam >= 0.16.0.1
 rpy2 >= 3.4.2
 scipy >= 1.8.1
 ```
-### Other software
+### Other software (need manual installation)
 ```
 plink >= v1.90b6.24
 bedtools >= v2.30.0
 R >= 3.6.1
     r-gkmSVM >= 0.8.0
 ```
 ## Installation
```

### Comparing `eQTac-1.0.4/eQTac/control_FDR.py` & `eQTac-1.0.5/eQTac/control_FDR.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.4/eQTac/eQTac_correlation.py` & `eQTac-1.0.5/eQTac/eQTac_correlation.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,10 +88,10 @@
 def eQTac_correlation(PRE_scorefile, exp_file, result_file):
     score_data, exp_data, d_gene_info, d_cis, d_pre_info = extract_data(PRE_scorefile, exp_file)
     with open(result_file, 'w') as ff:
         calculate_correlation(score_data, exp_data, d_gene_info, d_cis, d_pre_info, ff)
 
 
 if __name__ == "__main__":
-    eQTac_correlation("../output_eQTac/OA_217.TOP.processed.chr1_22.QC.imputed.synovium_filter.vcf.gz.PRE_score",
-                      "../test_data/OA_synovium_v1.exp.chr1-22.expression.qtltools.covar_residual.gz",
-                      "../output_eQTac/OA_217.TOP.processed.chr1_22.QC.imputed.synovium_filter.vcf.gz.PRE_score.eQTac_result")
+    eQTac_correlation("../output_eQTac/test.geno.vcf.gz.PRE_score",
+                      "../test_data/test.exp_residual",
+                      "../output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result")
```

### Comparing `eQTac-1.0.4/eQTac/eQTac_permutation.py` & `eQTac-1.0.5/eQTac/eQTac_permutation.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,10 +45,10 @@
                     beta, se, p, intercept, r_value = st_linear_reg(exp, score)
                     ff.write("%.5g" % p + "\n")
             print("Permutation", seed + 1, "finished")
 
 
 if __name__ == "__main__":
     eQTac_permutation(
-        "../output_eQTac/OA_217.TOP.processed.chr1_22.QC.imputed.synovium_filter.vcf.gz.PRE_score",
-        "../test_data/OA_synovium_v1.exp.chr1-22.expression.qtltools.covar_residual.gz", 100,
-        "../output_eQTac/OA_217.TOP.processed.chr1_22.QC.imputed.synovium_filter.vcf.gz.PRE_score.eQTac_result.permutation_plist")
+        "../output_eQTac/test.geno.vcf.gz.PRE_scoree",
+        "../test_data/test.exp_residual", 100,
+        "../output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result.permutation_plist")
```

### Comparing `eQTac-1.0.4/eQTac/filter_bkg.py` & `eQTac-1.0.5/eQTac/filter_bkg.py`

 * *Files 15% similar despite different names*

```diff
@@ -66,9 +66,9 @@
                 if re.sub("^>", "", name) in name_set:
                     ff2.write(">" + name + "\n")
                     ff2.write(seq + "\n")
     return out_neg_fa, out_neg_bed
 
 
 if __name__ == '__main__':
-    filter_bkg("Merged_ATAC-all_summits.100bp.top500.negraw.bed", "Merged_ATAC-all_summits.100bp.top500.negraw.fa",
-               "../test_data/Merged_ATAC-all.p0.05_peaks.narrowPeak")
+    filter_bkg("../output_eQTac/test.positive.negraw.bed", "../output_eQTac/test.positive.negraw.fa",
+               "../test_data/test.exclude.bed")
```

### Comparing `eQTac-1.0.4/eQTac/generate_PRE.py` & `eQTac-1.0.5/eQTac/generate_PRE.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.4/eQTac/generate_mut_fa.py` & `eQTac-1.0.5/eQTac/generate_mut_fa.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.4/eQTac/generate_snp_dict.py` & `eQTac-1.0.5/eQTac/generate_snp_dict.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.4/eQTac/geno2score.py` & `eQTac-1.0.5/eQTac/geno2score.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,11 +77,11 @@
             snps = ",".join(snp_set)
             ff.write("\t".join([ch, start, end, enhancer, "%d" % snp_count, snps] + score_list) + "\n")
     return PRE_scorefile
 
 
 if __name__ == "__main__":
     geno2score(
-        "../output_eQTac/OA_217.TOP.processed.chr1_22.QC.imputed.synovium_filter.vcf.gz",
-        "../output_eQTac/OA_217.TOP.processed.chr1_22.QC.imputed.synovium_filter.snp.bed--Merged_ATAC-all_summits.100bp.top500.bed.pre_snplist.ld_info.snplist.bed.mutate.pred_out",
-        "../output_eQTac/OA_217.TOP.processed.chr1_22.QC.imputed.synovium_filter.snp.bed--Merged_ATAC-all_summits.100bp.top500.bed.pre_snplist.ld_info"
+        "../output_eQTac/test.geno.vcf.gz",
+        "../output_eQTac/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info.snplist.bed.mutate.pred_out",
+        "../output_eQTac/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info"
     )
```

### Comparing `eQTac-1.0.4/eQTac/get_nullseq.py` & `eQTac-1.0.5/eQTac/get_nullseq.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,8 +58,8 @@
     robjects.r(
         "library(gkmSVM);genNullSeqs('%(pos_bed_newpath)s',nMaxTrials=20,xfold=2.5,GC_match_tol=0.05,repeat_match_tol=0.05,length_match_tol=0.05,batchsize=500000,genomeVersion='hg19', outputPosFastaFN='%(pos_fa)s', outputBedFN='%(negraw_bed)s', outputNegFastaFN='%(negraw_fa)s')"
         % d)
     return pos_fa, pos_bed_newpath, negraw_fa, negraw_bed
 
 
 if __name__ == '__main__':
-    get_nullseq("../test_data/Merged_ATAC-all_summits.100bp.top500.bed", ".")
+    get_nullseq("../test_data/test.positive.bed", ".")
```

### Comparing `eQTac-1.0.4/eQTac.egg-info/PKG-INFO` & `eQTac-1.0.5/eQTac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: eQTac
-Version: 1.0.4
+Version: 1.0.5
 Summary: The eQTac method.
 Home-page: https://github.com/JFF1594032292/eQTac
 Author: Jiang Feng
 Author-email: 1594032292@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # eQTac
----
 EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
 ## Dependence
 ### Python packages
 ```
 numpy >= 1.22.4
 pandas >= 1.4.3
 pybedtools >= 0.8.2
 pysam >= 0.16.0.1
 rpy2 >= 3.4.2
 scipy >= 1.8.1
 ```
-### Other software
+### Other software (need manual installation)
 ```
 plink >= v1.90b6.24
 bedtools >= v2.30.0
 R >= 3.6.1
     r-gkmSVM >= 0.8.0
 ```
 ## Installation
```

### Comparing `eQTac-1.0.4/setup.py` & `eQTac-1.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f1:
     long_description = f1.read()
 
 setuptools.setup(
     name="eQTac",
-    version="1.0.4",
+    version="1.0.5",
     author="Jiang Feng",
     author_email="1594032292@qq.com",
     description="The eQTac method.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JFF1594032292/eQTac",
     packages=setuptools.find_packages(),
```

