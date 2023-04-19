# Comparing `tmp/q2-dbbact-1.4.0.tar.gz` & `tmp/q2-dbbact-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2-dbbact-1.4.0.tar", last modified: Sun May 22 10:24:02 2022, max compression
+gzip compressed data, was "q2-dbbact-1.5.0.tar", last modified: Wed Apr 19 14:19:19 2023, max compression
```

## Comparing `q2-dbbact-1.4.0.tar` & `q2-dbbact-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 10:24:02.666727 q2-dbbact-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-05-22 10:23:52.000000 q2-dbbact-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6361 2022-05-22 10:24:02.666727 q2-dbbact-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5191 2022-05-22 10:23:52.000000 q2-dbbact-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 10:24:02.662727 q2-dbbact-1.4.0/q2_dbbact/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-22 10:23:52.000000 q2-dbbact-1.4.0/q2_dbbact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21213 2022-05-22 10:23:52.000000 q2-dbbact-1.4.0/q2_dbbact/methods.py
--rw-r--r--   0 runner    (1001) docker     (121)    21802 2022-05-22 10:23:52.000000 q2-dbbact-1.4.0/q2_dbbact/plugin_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    15912 2022-05-22 10:23:52.000000 q2-dbbact-1.4.0/q2_dbbact/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7762 2022-05-22 10:23:52.000000 q2-dbbact-1.4.0/q2_dbbact/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 10:24:02.666727 q2-dbbact-1.4.0/q2_dbbact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6361 2022-05-22 10:24:02.000000 q2-dbbact-1.4.0/q2_dbbact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-05-22 10:24:02.000000 q2-dbbact-1.4.0/q2_dbbact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-22 10:24:02.000000 q2-dbbact-1.4.0/q2_dbbact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-05-22 10:24:02.000000 q2-dbbact-1.4.0/q2_dbbact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-05-22 10:24:02.000000 q2-dbbact-1.4.0/q2_dbbact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-22 10:24:02.000000 q2-dbbact-1.4.0/q2_dbbact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-22 10:24:02.666727 q2-dbbact-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-05-22 10:23:52.000000 q2-dbbact-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:19:19.260610 q2-dbbact-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-19 14:19:02.000000 q2-dbbact-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-19 14:19:19.260610 q2-dbbact-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-19 14:19:02.000000 q2-dbbact-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:19:19.260610 q2-dbbact-1.5.0/q2_dbbact/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 14:19:02.000000 q2-dbbact-1.5.0/q2_dbbact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24745 2023-04-19 14:19:02.000000 q2-dbbact-1.5.0/q2_dbbact/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-04-19 14:19:02.000000 q2-dbbact-1.5.0/q2_dbbact/plugin_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-04-19 14:19:02.000000 q2-dbbact-1.5.0/q2_dbbact/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-19 14:19:02.000000 q2-dbbact-1.5.0/q2_dbbact/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:19:19.260610 q2-dbbact-1.5.0/q2_dbbact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-19 14:19:19.000000 q2-dbbact-1.5.0/q2_dbbact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-19 14:19:19.000000 q2-dbbact-1.5.0/q2_dbbact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:19:19.000000 q2-dbbact-1.5.0/q2_dbbact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 14:19:19.000000 q2-dbbact-1.5.0/q2_dbbact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-19 14:19:19.000000 q2-dbbact-1.5.0/q2_dbbact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 14:19:19.000000 q2-dbbact-1.5.0/q2_dbbact.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 14:19:19.260610 q2-dbbact-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-19 14:19:02.000000 q2-dbbact-1.5.0/setup.py
```

### Comparing `q2-dbbact-1.4.0/LICENSE` & `q2-dbbact-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `q2-dbbact-1.4.0/PKG-INFO` & `q2-dbbact-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: q2-dbbact
-Version: 1.4.0
+Version: 1.5.0
 Summary: A qiime2 (https://qiime2.org/) plugin for dbBact (http://dbbact.org) annotations of microbiome experiments
 Home-page: http://dbbact.org
 Author: dbBact team
 Author-email: info@dbbact.org
 License: BSD
 Keywords: microbiome qiime2 dbbact database analysis bioinformatics
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Plugins
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
@@ -97,9 +96,7 @@
 Input is the results of a differential abundance analysis (which provides two ASV groups - positive and negative effect size), and a dbBact term.
 
 The venn diagram shows how many of the ASVs in each group have the term, as well as how many total dbBact ASVs have the term associated.
 
 ```qiime dbbact venn --i-diff diff-cfs-dsfdr.qza --p-terms "small village" --p-source dsfdr --p-label1 Control --p-label2 CFS --o-visualization venn-cfs-human-village```
 
 ![venn](https://github.com/amnona/q2-dbbact/blob/main/pics/venn-cfs-village.png)
-
-
```

### Comparing `q2-dbbact-1.4.0/README.md` & `q2-dbbact-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `q2-dbbact-1.4.0/q2_dbbact/methods.py` & `q2-dbbact-1.5.0/q2_dbbact/methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         raise ValueError('Table seems to contain untrimmed sequences. Please run qiime dbbact trim-primers on the table prior to running enrichment.')
     else:
         print('Identified region %s' % region)
 
     # do the dbbact term enrichment test (using 2 feature groups or feature effect size rank correlation)
     if method == 'groups':
         print('%d ASVs' % len(exp.feature_metadata))
-        exp = exp.filter_by_metadata('reject', ['1'], axis='f')
+        exp = exp.filter_by_metadata('reject', ['1', 1], axis='f')
         print('%d significant ASVs' % len(exp.feature_metadata))
         pos_features = ndata[ndata['effect'] > 0].index.values
         res = db.enrichment(exp, features=pos_features, term_type=term_type, max_id=maxid, random_seed=random_seed)
         df = res[0]
     elif method == 'correlation':
         print('searching for dbbact term enrichment for %d ASVs' % len(exp.feature_metadata))
         dd = db.rank_enrichment(exp, 'effect', max_id=maxid, random_seed=random_seed)
@@ -59,14 +59,88 @@
     # need to rename the index to "id"
     # and cannot contain non-numeric columns
     df.drop('term', axis='columns', inplace=True)
     df.index.rename('id', inplace=True)
     return df
 
 
+def continuous_enrichment(table: biom.Table,
+                   metadata: pd.DataFrame,
+                   field: str,
+                   val1: List[str] = None,
+                   val2: List[str] = None,
+                   repseqs: DNAFASTAFormat = None,
+                   freq_weight: str = 'rank',
+                   random_seed: int = 0,
+                   fdr_method: str = 'dsfdr',
+                   term_type: str = 'term',
+                   alpha: float = 0.1,
+                   maxid: int = None) -> pd.DataFrame:
+
+    ca.set_log_level('INFO')
+    db = dbbact_calour.dbbact.DBBact()
+    db.set_log_level('INFO')
+
+    # set random seed to None (i.e. random every time) if 0 is provided
+    if random_seed == 0:
+        random_seed = None
+
+    metadata = metadata.to_dataframe()
+
+    # check and prepare the metadata columns for the testing
+    md_fields = metadata.columns
+    if field not in md_fields:
+        raise ValueError('Field %s not found in metadata file' % field)
+    labels = metadata[field].unique()
+    n = len(labels)
+    if n == 1:
+        raise ValueError('Only one category in metadata column "%s". Aborting' % field)
+    if val1 is None and val2 is None:
+        if n == 2:
+            val1 = [labels[0]]
+            val2 = [labels[1]]
+            print('No values supplied for field %s, assigning from the two values present (%s, %s)' % (field, val1, val2))
+        else:
+            raise ValueError('Cannot perform %s test on more than two categories in metadata and val1 and val2 not supplied. Aborting' % statistical_test)
+
+    if val1 is not None:
+        if len([x for x in metadata[field] if x in val1]) == 0:
+            raise ValueError('No values matching val1 (%s) found in metadata field %s' % (val1, field))
+    if val2 is not None:
+        if len([x for x in metadata[field] if x in val2]) == 0:
+            raise ValueError('No values matching val2 (%s) found in metadata field %s' % (val2, field))
+
+    # create the calour.AmpliconExperiment from the table and metadata
+    samples = table.ids(axis='sample')
+    features = table.ids(axis='observation')
+    feature_metadata = pd.DataFrame(index=features, columns={'_feature_id': features})
+    # use repseqs if supplied
+    if repseqs is not None:
+        print('converting hashes to sequences using repseqs file')
+        feature_metadata = _seqs_from_repseqs(feature_metadata, repseqs)
+    metadata = metadata.filter(items=samples, axis='index')
+    exp = ca.AmpliconExperiment(data=table.transpose().matrix_data, sample_metadata=metadata, feature_metadata=feature_metadata, sparse=False)
+    print('created experiment %r' % exp)
+
+    # do the continuous enrichment test ( using dbbact.sample_enrichment() )
+    res = db.sample_enrichment(exp, field, value1=val1, value2=val2, term_type=term_type, fdr_method=fdr_method, alpha=alpha, freq_weight=freq_weight, max_id=maxid, random_seed=random_seed)
+    df = res.feature_metadata
+    print('found %d enriched terms' % len(df))
+
+    # qiime2 plugin stuff:
+    # need to rename the index to "id"
+    # and cannot contain non-numeric columns so need to create a new column with the direction as number
+    df.drop('term', axis='columns', inplace=True)
+    df.rename({'_calour_stat': 'odif'}, axis='columns', inplace=True)
+    df['dir(1=%s,-1=%s)' % (val1, val2)] = df['_calour_direction'].apply(lambda x: 1 if x == val1 else -1)
+    df.drop('_calour_direction', axis='columns', inplace=True)
+    df.index.rename('id', inplace=True)
+    return df
+
+
 def single_enrichment(bg_table: biom.Table = None, test_table: biom.Table = None, bg_seqs: DNAFASTAFormat = None, test_seqs: DNAFASTAFormat = None,
                       repseqs: DNAFASTAFormat = None) -> pd.DataFrame:
     # test we have the correct inputs
     if bg_table is None and bg_seqs is None:
         raise ValueError('Must supply either bg_table or bg_seqs')
     if test_table is None and test_seqs is None:
         raise ValueError('Must supply either test_table or test_seqs')
@@ -208,22 +282,22 @@
         raise ValueError('Field %s not found in metadata file' % field)
     if pair_field is not None:
         if pair_field not in md_fields:
             raise ValueError('Pair field %s not found in metadata file' % field)
     labels = metadata[field].unique()
     n = len(labels)
     if n == 1:
-        raise ValueError('Only one category in metadata column. Aborting')
+        raise ValueError('Only one category in metadata column "%s". Aborting' % field)
     if val1 is None and val2 is None:
         if n == 2:
             val1 = [labels[0]]
             val2 = [labels[1]]
             print('No values supplied for field, assigning from the two values present (%s, %s)' % (val1, val2))
         else:
-            raise ValueError('Cannot perform %s test on more than two categories in metadata and val1 and val2 not supplied. Aborting' % statistical_test)
+            raise ValueError('Cannot perform %s test on more than two categories in metadata field "%s", and val1 and val2 not supplied. Aborting' % (field, statistical_test))
 
     if val1 is not None:
         if len([x for x in metadata[field] if x in val1]) == 0:
             raise ValueError('No values matching val1 (%s) found in metadata field %s' % (val1, field))
     if val2 is not None:
         if len([x for x in metadata[field] if x in val2]) == 0:
             raise ValueError('No values matching val2 (%s) found in metadata field %s' % (val2, field))
```

### Comparing `q2-dbbact-1.4.0/q2_dbbact/plugin_setup.py` & `q2-dbbact-1.5.0/q2_dbbact/plugin_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from qiime2.plugin import (SemanticType, Str, Int, Float, Choices, List,
                            MetadataColumn, Categorical, Numeric, Metadata, Bool, Visualization)
 from q2_types.feature_table import (
     FeatureTable, Frequency)
 from q2_types.feature_data import (FeatureData, Differential, Sequence, Taxonomy, )
 
 from . import __version__
-from .methods import single_enrichment, enrichment, embed_seqs, bg_term_enrichment, diff_abundance, enrich_pipeline, trim_primers
+from .methods import single_enrichment, enrichment, embed_seqs, bg_term_enrichment, diff_abundance, enrich_pipeline, trim_primers, continuous_enrichment
 from .visualizations import draw_wordcloud_vis, plot_enrichment, heatmap, venn
 
 
 _citation = ('manuscript in preparation')
 
 _short_description = "A Qiime2 plugin for the dbBact bacterial knowledge-base (dbbact.org)"
 
@@ -147,14 +147,56 @@
     output_descriptions={'enriched': 'the enriched dbBact terms'},
     name='dbBact term enrichment for differential abundance results',
     description=("Identify dbBact terms enriched in results of differential abundance (terms significantly more represented in either of the differential abundance groups or correlated with effect size)")
 )
 
 
 plugin.methods.register_function(
+    function=continuous_enrichment,
+    inputs={'table': FeatureTable[Frequency],
+            'repseqs': FeatureData[Sequence]
+            },
+    outputs=[('enriched', FeatureData[Differential])],
+    parameters={
+        'metadata': Metadata,
+        'field': Str,
+        'val1': List[Str],
+        'val2': List[Str],
+        'random_seed': Int,
+        'fdr_method': Str % Choices(_fdr_method),
+        'freq_weight': Str % Choices(['log2', 'rank', 'linear', 'binary']),
+        'term_type': Str % Choices(['term', 'annotation']),
+        'random_seed': Int,
+        'maxid': Int,
+        'alpha': Float,
+        'random_seed': Int
+    },
+    input_descriptions={
+        'table': 'The biom table with hashed ASV IDs',
+        'repseqs': 'The corresponding repseqs file with hashed ASV IDs',
+    },
+    parameter_descriptions={
+        'metadata': 'Metadata (mapping) file for the table',
+        'field': 'The metadata field on which to perform the differential abundance test',
+        'val1': 'Metadata values (in field) for samples in group1. Can supply multiple values',
+        'val2': 'Metadata values (in field) for samples in group2. Can supply multiple values. If not provided, take all samples not in group1',
+        'freq_weight': 'The method to use for weighting the frequency of each ASV in the table. "rank" - rank of the feature frequency across samples, "log2" - log2 of the frequency, "linear" - linear frequency, "binary" - binary frequency (1 if >0, 0 otherwise)',
+        'term_type': '"term" to get enriched dbBact terms, "annotation" to get list of enriched dbBact annotations in one group compared to the other',
+        'random_seed': 'If provided, use as the random seed for the enrichment permutation test (to ensure complete replication)',
+        'maxid': 'The maximal dbBact annotation id to use (to enable replication of results after new annotations are added to dbBact',
+        'alpha': 'The FDR threshold to use for enriched term significance',
+        'random_seed': 'If provided, use as the random seed for the enrichment permutation test (to ensure complete replication)'
+    },
+    output_descriptions={'enriched': 'the enriched dbBact terms'},
+    name='dbBact term enrichment using continuous frequency weights',
+    description=("Identify dbBact terms enriched between two sample groups using continuous frequency weights")
+)
+
+
+plugin.methods.register_function(
     function=embed_seqs,
     inputs={'repseqs': FeatureData[Sequence],
             'table': FeatureTable[Frequency]},
     outputs=[('merged', FeatureTable[Frequency])],
     parameters={},
     input_descriptions={
         'table': 'The biom table with hashed ASV IDs',
```

### Comparing `q2-dbbact-1.4.0/q2_dbbact/utils.py` & `q2-dbbact-1.5.0/q2_dbbact/utils.py`

 * *Files identical despite different names*

### Comparing `q2-dbbact-1.4.0/q2_dbbact/visualizations.py` & `q2-dbbact-1.5.0/q2_dbbact/visualizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
 
 
 def plot_enrichment(output_dir: str, enriched: pd.DataFrame, max_show: int = 10, max_len: int = 40, colors: List[str] = ['green', 'red'],
                     labels: List[str] = ['group1', 'group2'], enriched_exp_color: str = 'white'):
     '''Plot the enriched terms bar plot
     '''
     enriched['term'] = enriched.index.values
-    ax = ca.plotting.plot_enrichment(None, enriched, max_show=max_show, max_len=max_len, colors=colors, labels=labels, enriched_exp_color=enriched_exp_color)
+    numbers_kwargs = {'color': enriched_exp_color, 'weight': 'bold'}
+    ax = ca.plotting.plot_enrichment(None, enriched, max_show=max_show, max_len=max_len, colors=colors, labels=labels, numbers_kwargs=numbers_kwargs)
     ax.figure.tight_layout()
     ax.figure.savefig(os.path.join(output_dir, 'enriched_terms.svg'), bbox_inches='tight')
     ax.figure.savefig(os.path.join(output_dir, 'enriched_terms.pdf'), bbox_inches='tight')
     enriched.to_csv(os.path.join(output_dir, 'enriched_terms.tsv'), sep='\t')
     with open(os.path.join(output_dir, 'index.html'), 'w') as fl:
         fl.write('<html><body>\n')
         fl.write('<h1>dbBact enriched terms</h1>\n')
```

#### html2text {}

```diff
@@ -38,17 +38,18 @@
 ' % focus_terms) fl.write('
 [wordcloud]\n') fl.write('Download_as_PDF
 \n') fl.write('Download_scores_as_tsv
 \n') fl.write('
 ') def plot_enrichment(output_dir: str, enriched: pd.DataFrame, max_show: int =
 10, max_len: int = 40, colors: List[str] = ['green', 'red'], labels: List[str]
 = ['group1', 'group2'], enriched_exp_color: str = 'white'): '''Plot the
-enriched terms bar plot ''' enriched['term'] = enriched.index.values ax =
+enriched terms bar plot ''' enriched['term'] = enriched.index.values
+numbers_kwargs = {'color': enriched_exp_color, 'weight': 'bold'} ax =
 ca.plotting.plot_enrichment(None, enriched, max_show=max_show, max_len=max_len,
-colors=colors, labels=labels, enriched_exp_color=enriched_exp_color)
+colors=colors, labels=labels, numbers_kwargs=numbers_kwargs)
 ax.figure.tight_layout() ax.figure.savefig(os.path.join(output_dir,
 'enriched_terms.svg'), bbox_inches='tight') ax.figure.savefig(os.path.join
 (output_dir, 'enriched_terms.pdf'), bbox_inches='tight') enriched.to_csv
 (os.path.join(output_dir, 'enriched_terms.tsv'), sep='\t') with open
 (os.path.join(output_dir, 'index.html'), 'w') as fl: fl.write('
 \n') fl.write('
 ****** dbBact enriched terms ******
```

### Comparing `q2-dbbact-1.4.0/q2_dbbact.egg-info/PKG-INFO` & `q2-dbbact-1.5.0/q2_dbbact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: q2-dbbact
-Version: 1.4.0
+Version: 1.5.0
 Summary: A qiime2 (https://qiime2.org/) plugin for dbBact (http://dbbact.org) annotations of microbiome experiments
 Home-page: http://dbbact.org
 Author: dbBact team
 Author-email: info@dbbact.org
 License: BSD
 Keywords: microbiome qiime2 dbbact database analysis bioinformatics
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Plugins
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
@@ -97,9 +96,7 @@
 Input is the results of a differential abundance analysis (which provides two ASV groups - positive and negative effect size), and a dbBact term.
 
 The venn diagram shows how many of the ASVs in each group have the term, as well as how many total dbBact ASVs have the term associated.
 
 ```qiime dbbact venn --i-diff diff-cfs-dsfdr.qza --p-terms "small village" --p-source dsfdr --p-label1 Control --p-label2 CFS --o-visualization venn-cfs-human-village```
 
 ![venn](https://github.com/amnona/q2-dbbact/blob/main/pics/venn-cfs-village.png)
-
-
```

### Comparing `q2-dbbact-1.4.0/setup.py` & `q2-dbbact-1.5.0/setup.py`

 * *Files identical despite different names*

