# Comparing `tmp/drep-3.4.2.tar.gz` & `tmp/drep-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drep-3.4.2.tar", last modified: Mon Feb  6 19:04:43 2023, max compression
+gzip compressed data, was "drep-3.4.3.tar", last modified: Wed Apr 19 00:06:26 2023, max compression
```

## Comparing `drep-3.4.2.tar` & `drep-3.4.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-06 19:04:43.446421 drep-3.4.2/
--rw-r--r--   0 mattolm    (501) staff       (20)      270 2023-02-06 19:04:43.446251 drep-3.4.2/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)     1925 2023-01-11 23:09:49.000000 drep-3.4.2/README.md
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-06 19:04:43.441233 drep-3.4.2/bin/
--rwxr-xr-x   0 mattolm    (501) staff       (20)      849 2023-01-11 23:09:49.000000 drep-3.4.2/bin/dRep
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-06 19:04:43.443400 drep-3.4.2/drep/
--rw-r--r--   0 mattolm    (501) staff       (20)        6 2023-02-06 19:02:22.000000 drep-3.4.2/drep/VERSION
--rw-r--r--   0 mattolm    (501) staff       (20)    11616 2021-01-25 21:20:07.000000 drep-3.4.2/drep/WorkDirectory.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     2844 2021-01-28 01:16:56.000000 drep-3.4.2/drep/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)    14201 2023-01-11 23:12:10.000000 drep-3.4.2/drep/argumentParser.py
--rw-r--r--   0 mattolm    (501) staff       (20)     3334 2021-01-28 01:17:39.000000 drep-3.4.2/drep/controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9432 2021-01-28 01:23:27.000000 drep-3.4.2/drep/d_adjust.py
--rw-r--r--   0 mattolm    (501) staff       (20)    48935 2022-07-31 23:11:17.000000 drep-3.4.2/drep/d_analyze.py
--rw-r--r--   0 mattolm    (501) staff       (20)    13663 2021-01-28 01:19:36.000000 drep-3.4.2/drep/d_bonus.py
--rw-r--r--   0 mattolm    (501) staff       (20)    11304 2023-02-06 19:02:36.000000 drep-3.4.2/drep/d_choose.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-06 19:04:43.445769 drep-3.4.2/drep/d_cluster/
--rw-r--r--   0 mattolm    (501) staff       (20)        0 2021-01-25 21:20:07.000000 drep-3.4.2/drep/d_cluster/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)     3775 2021-01-25 21:20:07.000000 drep-3.4.2/drep/d_cluster/cluster_utils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    15921 2021-06-14 16:36:17.000000 drep-3.4.2/drep/d_cluster/compare_utils.py
--rw-r--r--   0 mattolm    (501) staff       (20)     6695 2021-06-14 16:51:41.000000 drep-3.4.2/drep/d_cluster/controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)    18489 2022-07-31 22:32:06.000000 drep-3.4.2/drep/d_cluster/external.py
--rw-r--r--   0 mattolm    (501) staff       (20)     5910 2021-01-25 21:20:07.000000 drep-3.4.2/drep/d_cluster/greedy_clustering.py
--rw-r--r--   0 mattolm    (501) staff       (20)        0 2021-01-25 21:20:07.000000 drep-3.4.2/drep/d_cluster/parsers.py
--rw-r--r--   0 mattolm    (501) staff       (20)    22198 2021-06-22 22:41:52.000000 drep-3.4.2/drep/d_cluster/utils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    13182 2022-07-31 23:24:47.000000 drep-3.4.2/drep/d_evaluate.py
--rw-r--r--   0 mattolm    (501) staff       (20)    23044 2023-01-11 23:09:49.000000 drep-3.4.2/drep/d_filter.py
--rw-r--r--   0 mattolm    (501) staff       (20)     4161 2022-07-31 23:24:37.000000 drep-3.4.2/drep/d_workflows.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-06 19:04:43.444411 drep-3.4.2/drep.egg-info/
--rw-r--r--   0 mattolm    (501) staff       (20)      270 2023-02-06 19:04:43.000000 drep-3.4.2/drep.egg-info/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)      709 2023-02-06 19:04:43.000000 drep-3.4.2/drep.egg-info/SOURCES.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-02-06 19:04:43.000000 drep-3.4.2/drep.egg-info/dependency_links.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2021-01-28 02:34:03.000000 drep-3.4.2/drep.egg-info/not-zip-safe
--rw-r--r--   0 mattolm    (501) staff       (20)       67 2023-02-06 19:04:43.000000 drep-3.4.2/drep.egg-info/requires.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        5 2023-02-06 19:04:43.000000 drep-3.4.2/drep.egg-info/top_level.txt
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-06 19:04:43.446060 drep-3.4.2/helper_scripts/
--rwxr-xr-x   0 mattolm    (501) staff       (20)    32249 2021-01-26 18:20:18.000000 drep-3.4.2/helper_scripts/ScaffoldLevel_dRep.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     4265 2022-07-15 17:06:17.000000 drep-3.4.2/helper_scripts/parse_stb.py
--rw-r--r--   0 mattolm    (501) staff       (20)       38 2023-02-06 19:04:43.446468 drep-3.4.2/setup.cfg
--rw-r--r--   0 mattolm    (501) staff       (20)      898 2021-01-25 21:20:07.000000 drep-3.4.2/setup.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-04-19 00:06:26.047199 drep-3.4.3/
+-rw-r--r--   0 mattolm    (501) staff       (20)      231 2023-04-19 00:06:26.047061 drep-3.4.3/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)     1925 2023-01-11 23:09:49.000000 drep-3.4.3/README.md
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-04-19 00:06:26.041611 drep-3.4.3/bin/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)      849 2023-01-11 23:09:49.000000 drep-3.4.3/bin/dRep
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-04-19 00:06:26.044381 drep-3.4.3/drep/
+-rw-r--r--   0 mattolm    (501) staff       (20)        6 2023-04-18 21:39:08.000000 drep-3.4.3/drep/VERSION
+-rw-r--r--   0 mattolm    (501) staff       (20)    11616 2021-01-25 21:20:07.000000 drep-3.4.3/drep/WorkDirectory.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     2844 2021-01-28 01:16:56.000000 drep-3.4.3/drep/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    14201 2023-01-11 23:12:10.000000 drep-3.4.3/drep/argumentParser.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     3334 2021-01-28 01:17:39.000000 drep-3.4.3/drep/controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9455 2023-04-18 22:14:22.000000 drep-3.4.3/drep/d_adjust.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    49046 2023-04-18 22:14:22.000000 drep-3.4.3/drep/d_analyze.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    13663 2021-01-28 01:19:36.000000 drep-3.4.3/drep/d_bonus.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    11304 2023-02-06 19:02:36.000000 drep-3.4.3/drep/d_choose.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-04-19 00:06:26.046643 drep-3.4.3/drep/d_cluster/
+-rw-r--r--   0 mattolm    (501) staff       (20)        0 2021-01-25 21:20:07.000000 drep-3.4.3/drep/d_cluster/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     3775 2021-01-25 21:20:07.000000 drep-3.4.3/drep/d_cluster/cluster_utils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    15989 2023-04-18 22:17:20.000000 drep-3.4.3/drep/d_cluster/compare_utils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     6695 2021-06-14 16:51:41.000000 drep-3.4.3/drep/d_cluster/controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    18510 2023-04-18 22:14:22.000000 drep-3.4.3/drep/d_cluster/external.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     5910 2021-01-25 21:20:07.000000 drep-3.4.3/drep/d_cluster/greedy_clustering.py
+-rw-r--r--   0 mattolm    (501) staff       (20)        0 2021-01-25 21:20:07.000000 drep-3.4.3/drep/d_cluster/parsers.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    22219 2023-04-18 22:14:22.000000 drep-3.4.3/drep/d_cluster/utils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    13182 2022-07-31 23:24:47.000000 drep-3.4.3/drep/d_evaluate.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    23044 2023-01-11 23:09:49.000000 drep-3.4.3/drep/d_filter.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     4161 2022-07-31 23:24:37.000000 drep-3.4.3/drep/d_workflows.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-04-19 00:06:26.045431 drep-3.4.3/drep.egg-info/
+-rw-r--r--   0 mattolm    (501) staff       (20)      231 2023-04-19 00:06:26.000000 drep-3.4.3/drep.egg-info/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)      709 2023-04-19 00:06:26.000000 drep-3.4.3/drep.egg-info/SOURCES.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-04-19 00:06:26.000000 drep-3.4.3/drep.egg-info/dependency_links.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2021-01-28 02:34:03.000000 drep-3.4.3/drep.egg-info/not-zip-safe
+-rw-r--r--   0 mattolm    (501) staff       (20)       67 2023-04-19 00:06:26.000000 drep-3.4.3/drep.egg-info/requires.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        5 2023-04-19 00:06:26.000000 drep-3.4.3/drep.egg-info/top_level.txt
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-04-19 00:06:26.046905 drep-3.4.3/helper_scripts/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    32325 2023-04-18 22:38:18.000000 drep-3.4.3/helper_scripts/ScaffoldLevel_dRep.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     4265 2022-07-15 17:06:17.000000 drep-3.4.3/helper_scripts/parse_stb.py
+-rw-r--r--   0 mattolm    (501) staff       (20)       38 2023-04-19 00:06:26.047238 drep-3.4.3/setup.cfg
+-rw-r--r--   0 mattolm    (501) staff       (20)      898 2021-01-25 21:20:07.000000 drep-3.4.3/setup.py
```

### Comparing `drep-3.4.2/README.md` & `drep-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/bin/dRep` & `drep-3.4.3/bin/dRep`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/WorkDirectory.py` & `drep-3.4.3/drep/WorkDirectory.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/__init__.py` & `drep-3.4.3/drep/__init__.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/argumentParser.py` & `drep-3.4.3/drep/argumentParser.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/controller.py` & `drep-3.4.3/drep/controller.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/d_adjust.py` & `drep-3.4.3/drep/d_adjust.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     # Remove values without enough coverage
     Xdb.loc[Xdb['alignment_coverage'] <= cov_thresh, 'ani'] = 0
 
     # Make it symmetrical
     Xdb['av_ani'] = Xdb.apply(lambda row: dClust.average_ani (row,Xdb),axis=1)
     Xdb['dist'] = 1 - Xdb['av_ani']
-    db = Xdb.pivot("reference","querry","dist")
+    db = Xdb.pivot(index="reference", columns="querry", values="dist")
 
     # Cluster it
     if threshold == None:
         threshold = float(0)
     cdb, linkage = drep.d_cluster.cluster_utils.cluster_hierarchical(db, linkage_method = clust_method, \
                                                                      linkage_cutoff = threshold)
```

### Comparing `drep-3.4.2/drep/d_analyze.py` & `drep-3.4.3/drep/d_analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,15 +629,15 @@
         Makes and shows plot
     '''
     sns.set_style('white',{'axes.grid': False})
 
     if Mdb['genome1'].dtype.name == 'category':
         logging.error("WARNING: Primary dendrogram labels may be shuffled! Load as csv to prevent this")
 
-    db = Mdb.pivot("genome1","genome2","similarity")
+    db = Mdb.pivot(index="genome1", columns="genome2", values="similarity")
     names = list(db.columns)
     name2cluster = Cdb.set_index('genome')['primary_cluster'].to_dict()
     name2color = gen_color_dictionary(names, name2cluster)
 
     # Make the dendrogram
     g = fancy_dendrogram(linkage,names,name2color,threshold=threshold)
     plt.title('MASH clustering')
@@ -847,15 +847,15 @@
     plt.show()
     plt.close(fig)
 
     if Wmdb is not None:
         # Make a MASH linkage for the dendrogram
         db = Wmdb.copy()
         db['dist'] = 1 - db['similarity']
-        linkage_db = db.pivot("genome1","genome2","dist")
+        linkage_db = db.pivot(index="genome1", columns="genome2", values="dist")
         names = list(linkage_db.columns)
         Cdb, linkage = drep.d_cluster.cluster_utils.cluster_hierarchical(linkage_db, linkage_method='average', \
                                                                          linkage_cutoff= 0)
 
         # Make the MASH dendrogram
         _make_dendrogram(linkage,names)
         plt.title('MASH dendrogram')
@@ -869,15 +869,15 @@
 
     if Wndb is not None:
         # Make a ANIn linkage for the dendrogram
         d = Wndb.copy()
         drep.d_cluster.add_avani(d)
         #d['av_ani'] = d.apply(lambda row: drep.d_cluster.average_ani (row,d),axis=1)
         d['dist'] = 1 - d['av_ani']
-        db = d.pivot("reference", "querry", "dist")
+        db = d.pivot(index="reference", columns="querry", values="dist")
         names = list(db.columns)
         Cdb, linkage = drep.d_cluster.cluster_utils.cluster_hierarchical(db, linkage_method='average', \
                                                                          linkage_cutoff= 0)
 
         # Make the ANIn dendrogram
         _make_dendrogram(linkage,names)
         plt.title('ANIn dendrogram (NOT filtered for alignment length)')
@@ -891,15 +891,15 @@
 
         # Make a ANIn linkage for the filtered dendrogram
         d = Wndb.copy()
         d.loc[d['alignment_coverage'] <= 0.1, 'ani'] = 0
         drep.d_cluster.add_avani(d)
         #d['av_ani'] = d.apply(lambda row: drep.d_cluster.average_ani (row,d),axis=1)
         d['dist'] = 1 - d['av_ani']
-        db = d.pivot("reference", "querry", "dist")
+        db = d.pivot(index="reference", columns="querry", values="dist")
         names = list(db.columns)
         Cdb, linkage = drep.d_cluster.cluster_utils.cluster_hierarchical(db, linkage_method='average', \
                                                                          linkage_cutoff= 0)
 
         # Make the ANIn dendrogram
         _make_dendrogram(linkage,names)
         plt.title('ANIn dendrogram (filtered for 10% alignment)')
@@ -1534,15 +1534,15 @@
     if comp_method == 'ANIn':
         Xdb.loc[Xdb['alignment_coverage'] <= cov_thresh, 'ani'] = 0
 
     # Make it symmetrical
     drep.d_cluster.add_avani(Xdb)
     #Xdb['av_ani'] = Xdb.apply(lambda row: drep.d_cluster.average_ani (row,Xdb),axis=1)
     Xdb['dist'] = 1 - Xdb['av_ani']
-    db = Xdb.pivot("reference","querry","dist")
+    db = Xdb.pivot(index="reference", columns="querry", values="dist")
 
     # Cluster it
     if threshold == None:
         threshold = float(0)
     cdb, linkage = drep.d_cluster.cluster_utils.cluster_hierarchical(db, linkage_method = clust_method, \
                                                                      linkage_cutoff = threshold)
```

### Comparing `drep-3.4.2/drep/d_bonus.py` & `drep-3.4.3/drep/d_bonus.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/d_choose.py` & `drep-3.4.3/drep/d_choose.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/d_cluster/cluster_utils.py` & `drep-3.4.3/drep/d_cluster/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/d_cluster/compare_utils.py` & `drep-3.4.3/drep/d_cluster/compare_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 
     # Load key words
     P_Lmethod = kwargs.get('clusterAlg','single')
     P_Lcutoff = 1 - kwargs.get('P_ani',.9)
 
     # Do the actual clustering
     db['dist'] = 1 - db['similarity']
-    linkage_db = db.pivot("genome1","genome2","dist")
+    linkage_db = db.pivot(index="genome1", columns="genome2", values="dist")
     Cdb, linkage = drep.d_cluster.cluster_utils.cluster_hierarchical(linkage_db, linkage_method= P_Lmethod, \
                                                                      linkage_cutoff= P_Lcutoff)
     Cdb = Cdb.rename(columns={'cluster':'primary_cluster'})
     Cdb['primary_cluster'] = Cdb['primary_cluster'].astype(int)
 
     # Preparing clustering for return
     arguments = {'linkage_method':P_Lmethod,'linkage_cutoff':P_Lcutoff,\
@@ -299,15 +299,16 @@
 
             if len(ndb) == 0:
                 logging.error("CRITICAL ERROR WITH PRIMARY CLUSTER {0}; TRYING AGAIN".format(name))
                 ndb = compare_genomes(bdb, algorithm, data_folder, **kwargs)
 
             if len(ndb) > 0:
                 ndb['primary_cluster'] = name
-                Ndb = Ndb.append(ndb)
+                Ndb = pd.concat([Ndb, ndb])
+                #Ndb = Ndb.append(ndb)
             else:
                 logging.error("DOUBLE CRITICAL ERROR AGAIN WITH PRIMARY CLUSTER {0}; SKIPPING".format(name))
 
         # Run clustering on Ndb
         Cdb, c2ret = drep.d_cluster.utils._cluster_Ndb(Ndb, comp_method=algorithm, **kwargs)
 
         return Ndb, Cdb, c2ret
```

### Comparing `drep-3.4.2/drep/d_cluster/controller.py` & `drep-3.4.3/drep/d_cluster/controller.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/d_cluster/external.py` & `drep-3.4.3/drep/d_cluster/external.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     fdb['ani'] = [x/100 for x in fdb['ani']]
 
     return fdb
 
 
 def _fix_fastani(odb):
     # Add back missing genomes
-    fdb = odb.pivot('reference', 'querry', 'ani')
+    fdb = odb.pivot(index="reference", columns="querry", values="ani")
     fdb.reset_index(level=0, inplace=True)
     fdb.fillna(0, inplace=True)
     fdb = fdb.melt(id_vars=['reference']).rename(
             columns={'value':'ani'})
 
     # Add back alignment coverage
     fdb = pd.merge(fdb, odb[['reference', 'querry', 'alignment_coverage']], on=['reference', 'querry'], how='outer')
```

### Comparing `drep-3.4.2/drep/d_cluster/greedy_clustering.py` & `drep-3.4.3/drep/d_cluster/greedy_clustering.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/d_cluster/utils.py` & `drep-3.4.3/drep/d_cluster/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     # Remove values without enough coverage
     d.loc[d['alignment_coverage'] <= cov_thresh, 'ani'] = 0
 
     # Make a linkagedb by averaging values and setting self-compare to 1
     drep.d_cluster.external.add_avani(d)
     d['dist'] = 1 - d['av_ani']
-    db = d.pivot("reference", "querry", "dist")
+    db = d.pivot(index="reference", columns="querry", values="dist")
 
     return db
 
 
 def estimate_time(comps, alg):
     '''
     Estimate time, in minutes, based on comparison algorithm and number of comparisons
```

### Comparing `drep-3.4.2/drep/d_evaluate.py` & `drep-3.4.3/drep/d_evaluate.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/d_filter.py` & `drep-3.4.3/drep/d_filter.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep/d_workflows.py` & `drep-3.4.3/drep/d_workflows.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/drep.egg-info/SOURCES.txt` & `drep-3.4.3/drep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/helper_scripts/ScaffoldLevel_dRep.py` & `drep-3.4.3/helper_scripts/ScaffoldLevel_dRep.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,16 @@
     '''
     Sdb = pd.DataFrame()
     for i, fasta in enumerate(fastas):
         db = load_scaffold2length(fasta)
         db['loc'] = fasta
         db['priority'] = i
         db['sort_name'] = os.path.basename(fasta)
-        Sdb = Sdb.append(db)
+        Sdb = pd.concat([Sdb, db])
+        #Sdb = Sdb.append(db)
 
     Sdb['loc'] = Sdb['loc'].astype('category')
     Sdb['sort_name'] = Sdb['sort_name'].astype('category')
     Sdb['priority'] = Sdb['priority'].astype(int)
     Sdb['length'] = Sdb['length'].astype(int)
 
     return Sdb
@@ -597,15 +598,16 @@
             print('De-replicating scaffolds')
 
         # Make a new file where scaffolds that were in new and current are removed from new
         newfile = os.path.join(temp_folder, "deReplication_v{0}.fasta".format(i))
         rmdb = reconsile(Sdb, current, new, newfile, temp_folder, **kwargs)
 
         # Keep track of what was removed
-        RMdb = RMdb.append(rmdb)
+        #RMdb = RMdb.append(rmdb)
+        RMdb = pd.concat([RMdb, rmdb])
 
         current = newfile
 
     return current, RMdb, Sdb
 
 def gen_report(output_folder, final_file, RMdb, Sdb, scaffDb, verbose=False, selfCompairson=False):
     '''
```

### Comparing `drep-3.4.2/helper_scripts/parse_stb.py` & `drep-3.4.3/helper_scripts/parse_stb.py`

 * *Files identical despite different names*

### Comparing `drep-3.4.2/setup.py` & `drep-3.4.3/setup.py`

 * *Files identical despite different names*

