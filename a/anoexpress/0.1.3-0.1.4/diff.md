# Comparing `tmp/anoexpress-0.1.3.tar.gz` & `tmp/anoexpress-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoexpress-0.1.3.tar", max compression
+gzip compressed data, was "anoexpress-0.1.4.tar", max compression
```

## Comparing `anoexpress-0.1.3.tar` & `anoexpress-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1075 2022-11-12 23:31:02.745561 anoexpress-0.1.3/LICENSE
--rw-r--r--   0        0        0       66 2023-03-06 23:08:43.188006 anoexpress-0.1.3/anoexpress/__init__.py
--rw-r--r--   0        0        0    25133 2023-04-05 12:34:58.715685 anoexpress-0.1.3/anoexpress/anoexpress.py
--rw-r--r--   0        0        0      750 2023-04-17 13:36:20.788753 anoexpress-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 anoexpress-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-11-12 23:31:02.745561 anoexpress-0.1.4/LICENSE
+-rw-r--r--   0        0        0       66 2023-03-06 23:08:43.188006 anoexpress-0.1.4/anoexpress/__init__.py
+-rw-r--r--   0        0        0    27217 2023-04-19 14:11:43.044076 anoexpress-0.1.4/anoexpress/anoexpress.py
+-rw-r--r--   0        0        0      750 2023-04-19 14:11:31.544075 anoexpress-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 anoexpress-0.1.4/PKG-INFO
```

### Comparing `anoexpress-0.1.3/LICENSE` & `anoexpress-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anoexpress-0.1.3/anoexpress/anoexpress.py` & `anoexpress-0.1.4/anoexpress/anoexpress.py`

 * *Files 2% similar despite different names*

```diff
@@ -473,14 +473,60 @@
         column_name='pfam', 
         target_gene_list=top_geneIDs,
         N=N,
         k=k)
         
     return(hyper_geo)
 
+def kegg_hypergeometric(analysis, name, func, percentile=0.05):
+    """
+    Perform a hypergeometric test on GO terms of the the top % percentile genes ranked by user input function.
+
+    Parameters
+    ----------
+    analysis: {"gamb_colu", "gamb_colu_arab", "gamb_colu_arab_fun", "fun"}
+      which analysis to load gene expression data for. analyses with more species will have less genes
+      present, due to the process of finding orthologs.
+    name: str
+      name of the function to rank genes by
+    func: function
+      function to rank genes by (such as np.nanmedian, np.nanmean)
+    percentile: float, optional
+      percentile of genes to use for the enriched set in hypergeometric test. Defaults to 0.05
+
+    Returns
+    -------
+    go_hypergeo_results: pd.DataFrame
+    """
+
+    fc_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/ano-express/main/results/fcs.{analysis}.tsv", sep="\t")
+    fc_genes = fc_data.reset_index()['GeneID'].to_list()
+
+    # get top % percentile genes ranked by func
+    fc_ranked = load_candidates(analysis=analysis, name=name, func=func)
+    percentile_idx = fc_ranked.reset_index()['GeneID'].unique().shape[0] * percentile
+    top_geneIDs = fc_ranked.reset_index().loc[:, 'GeneID'][:int(percentile_idx)] 
+
+    # load gene annotation file 
+    kegg_df = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/ano-express/main/resources/AgamP4.kegg", sep="\t")
+    kegg_annotations = kegg_df[['kegg_pathway', 'description']].rename(columns={'kegg_pathway':'annotation'}).drop_duplicates()
+    kegg_df = kegg_df[['GeneID', 'kegg_pathway']].drop_duplicates()
+    kegg_df = kegg_df.query("GeneID in @fc_genes")
+    N = kegg_df.GeneID.unique().shape[0] #Total number of genes with some annotation 
+    k = np.isin(kegg_df.loc[:, 'GeneID'].unique(), top_geneIDs).sum() 
+
+    hyper_geo = _hypergeometric(
+        annotation_df=kegg_df, 
+        column_name='kegg_pathway', 
+        target_gene_list=top_geneIDs,
+        N=N,
+        k=k)    
+    hyper_geo = hyper_geo.merge(kegg_annotations, how='left')
+    return(hyper_geo)
+
 def _hypergeometric(annotation_df, column_name, target_gene_list, N, k):
     """
     This function performs a hypergeometric test on a given annotation column
     """
     from scipy.stats import hypergeom
     from tqdm import tqdm
     from statsmodels.stats.multitest import fdrcorrection
```

### Comparing `anoexpress-0.1.3/pyproject.toml` & `anoexpress-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anoexpress"
-version = "0.1.3"
+version = "0.1.4"
 description = "A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "anoexpress" }
 ]
```

### Comparing `anoexpress-0.1.3/PKG-INFO` & `anoexpress-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anoexpress
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
 Requires-Python: >=3.7.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

