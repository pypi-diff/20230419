# Comparing `tmp/notip-0.1.3.tar.gz` & `tmp/notip-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notip-0.1.3.tar", last modified: Mon Apr 17 22:24:28 2023, max compression
+gzip compressed data, was "notip-0.1.4.tar", last modified: Wed Apr 19 20:35:27 2023, max compression
```

## Comparing `notip-0.1.3.tar` & `notip-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 22:24:28.458430 notip-0.1.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-17 22:24:28.458430 notip-0.1.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      848 2023-04-17 09:55:41.000000 notip-0.1.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 22:24:28.454430 notip-0.1.3/notip/
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 12:46:44.000000 notip-0.1.3/notip/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    43762 2023-04-17 22:01:09.000000 notip-0.1.3/notip/posthoc_fmri.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 22:24:28.458430 notip-0.1.3/notip.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      108 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        6 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-04-17 22:24:28.458430 notip-0.1.3/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      976 2023-04-17 22:20:43.000000 notip-0.1.3/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 20:35:27.354179 notip-0.1.4/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-19 20:35:27.354179 notip-0.1.4/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      848 2023-04-17 09:55:41.000000 notip-0.1.4/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 20:35:27.354179 notip-0.1.4/notip/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 12:46:44.000000 notip-0.1.4/notip/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    37519 2023-04-19 20:34:39.000000 notip-0.1.4/notip/posthoc_fmri.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 20:35:27.354179 notip-0.1.4/notip.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      108 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        6 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-04-19 20:35:27.354179 notip-0.1.4/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      976 2023-04-19 20:35:13.000000 notip-0.1.4/setup.py
```

### Comparing `notip-0.1.3/PKG-INFO` & `notip-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notip
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nonparametric True Discovery Proportion control for brain imaging
 Home-page: https://github.com/alexblnn/Notip
 Download-URL: https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz
 Author: Alexandre Blain
 Author-email: alexandre.blain@inria.fr
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notip-0.1.3/README.md` & `notip-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `notip-0.1.3/notip/posthoc_fmri.py` & `notip-0.1.4/notip/posthoc_fmri.py`

 * *Files 8% similar despite different names*

```diff
@@ -712,18 +712,19 @@
         df = pd.DataFrame(columns=cols)
     else:
         df = pd.DataFrame(columns=cols, data=rows)
 
     return df
 
 
-def get_clusters_table_all_methods(stat_img, fmri_input, stat_threshold=3,
-                             alpha=0.05,
-                             k_max=1000, B=1000, cluster_threshold=None,
-                             two_sided=False, min_distance=8., n_jobs=2, seed=None):
+def get_clusters_table_with_TDP(stat_img, fmri_input, stat_threshold=3,
+                                alpha=0.05,
+                                k_max=1000, n_permutations=1000, cluster_threshold=None,
+                                methods=['Notip'],
+                                two_sided=False, min_distance=8., n_jobs=2, seed=None):
     """Creates pandas dataframe with img cluster statistics.
     Parameters
     ----------
     stat_img : Niimg-like object,
        Statistical image (presumably in z- or p-scale).
     stat_threshold : `float`
         Cluster forming threshold in same scale as `stat_img` (either a
@@ -750,31 +751,29 @@
     df : `pandas.DataFrame`
         Table with peaks, subpeaks and estimated TDP using three methods
         from thresholded `stat_img`. For binary clusters
         (clusters with >1 voxel containing only one value), the table
         reports the center of mass of the cluster,
         rather than any peaks/subpeaks.
     """
-    cols = ['Cluster ID', 'X', 'Y', 'Z', 'Peak Stat', 'Cluster Size (mm3)',
-            'TDP (ARI)', 'TDP (Notip)']
     # Replace None with 0
     cluster_threshold = 0 if cluster_threshold is None else cluster_threshold
     # print(cluster_threshold)
     # check that stat_img is niimg-like object and 3D
     stat_img = check_niimg_3d(stat_img)
 
     stat_map_ = _safe_get_data(stat_img)
     # Perform calibration before thresholding
     stat_map_nonzero = stat_map_[stat_map_ != 0]
     hommel = _compute_hommel_value(stat_map_nonzero, alpha)
     ari_thr = sa.linear_template(alpha, hommel, hommel)
     pval0, simes_thr = calibrate_simes(fmri_input, alpha,
-                                       k_max=k_max, B=B, seed=seed)
+                                       k_max=k_max, B=n_permutations, seed=seed)
     learned_templates_ = sa.get_permuted_p_values_one_sample(fmri_input,
-                                                             B=B,
+                                                             B=n_permutations,
                                                              n_jobs=n_jobs,
                                                              seed=None)
     learned_templates = np.sort(learned_templates_, axis=0)
     learned_thr = sa.calibrate_jer(alpha, learned_templates, pval0, k_max)
 
     # Apply threshold(s) to image
     stat_img = threshold_img(
@@ -853,220 +852,55 @@
             ).tolist()
             subpeak_xyz = np.array(subpeak_xyz).T
 
             # Only report peak and, at most, top 3 subpeaks.
             n_subpeaks = np.min((len(subpeak_vals), 4))
             for subpeak in range(n_subpeaks):
                 if subpeak == 0:
-                    row = [
-                        c_id + 1,
-                        subpeak_xyz[subpeak, 0],
-                        subpeak_xyz[subpeak, 1],
-                        subpeak_xyz[subpeak, 2],
-                        "{0:.2f}".format(subpeak_vals[subpeak]),
-                        cluster_size_mm,
-                        "{0:.2f}".format(ari_tdp),
-                        "{0:.2f}".format(learned_tdp),
-                    ]
+                        if methods == ['ARI', 'Notip']:
+                            cols = ['Cluster ID', 'X', 'Y', 'Z', 'Peak Stat', 'Cluster Size (mm3)',
+                                    'TDP (ARI)', 'TDP (Notip)']
+                            row = [
+                                c_id + 1,
+                                subpeak_xyz[subpeak, 0],
+                                subpeak_xyz[subpeak, 1],
+                                subpeak_xyz[subpeak, 2],
+                                "{0:.2f}".format(subpeak_vals[subpeak]),
+                                cluster_size_mm,
+                                "{0:.2f}".format(ari_tdp),
+                                "{0:.2f}".format(learned_tdp)]
+                        else:
+                            cols = ['Cluster ID', 'X', 'Y', 'Z', 'Peak Stat', 'Cluster Size (mm3)',
+                                    'TDP (Notip)']
+                            row = [
+                                c_id + 1,
+                                subpeak_xyz[subpeak, 0],
+                                subpeak_xyz[subpeak, 1],
+                                subpeak_xyz[subpeak, 2],
+                                "{0:.2f}".format(subpeak_vals[subpeak]),
+                                cluster_size_mm,
+                                "{0:.2f}".format(learned_tdp)]                           
+                                    
                 else:
                     # Subpeak naming convention is cluster num+letter:
                     # 1a, 1b, etc
                     sp_id = '{0}{1}'.format(
                         c_id + 1,
                         ascii_lowercase[subpeak - 1],
                     )
                     row = [
                         sp_id,
                         subpeak_xyz[subpeak, 0],
                         subpeak_xyz[subpeak, 1],
                         subpeak_xyz[subpeak, 2],
                         "{0:.2f}".format(subpeak_vals[subpeak]),
-                        '',
-                        '',
-                        '',
-                    ]
-                rows += [row]
-
-        # If we reach this point, there are clusters in this sign
-        no_clusters_found = False
-
-    if no_clusters_found:
-        df = pd.DataFrame(columns=cols)
-    else:
-        df = pd.DataFrame(columns=cols, data=rows)
+                        '']
+                    
+                    row += [''] * len(methods)
 
-    return df
-
-
-def get_clusters_table_Notip(stat_img, fmri_input, stat_threshold=3,
-                             alpha=0.05,
-                             k_max=1000, B=1000, cluster_threshold=None,
-                             two_sided=False, min_distance=8., n_jobs=2, seed=None):
-    """Creates pandas dataframe with img cluster statistics.
-    Parameters
-    ----------
-    stat_img : Niimg-like object,
-       Statistical image (presumably in z- or p-scale).
-    stat_threshold : `float`
-        Cluster forming threshold in same scale as `stat_img` (either a
-        p-value or z-scale value).
-    fmri_input : array of shape (n_subjects, p)
-        Masked fMRI data
-    learned_templates : array of shape (B_train, p)
-        sorted quantile curves computed on training data
-    alpha : float
-        risk level
-    k_max : int
-        threshold families length
-    B : int
-        number of permutations at inference step
-    cluster_threshold : `int` or `None`, optional
-        Cluster size threshold, in voxels.
-    two_sided : `bool`, optional
-        Whether to employ two-sided thresholding or to evaluate positive values
-        only. Default=False.
-    min_distance : `float`, optional
-        Minimum distance between subpeaks in mm. Default=8mm.
-    Returns
-    -------
-    df : `pandas.DataFrame`
-        Table with peaks, subpeaks and estimated TDP using three methods
-        from thresholded `stat_img`. For binary clusters
-        (clusters with >1 voxel containing only one value), the table
-        reports the center of mass of the cluster,
-        rather than any peaks/subpeaks.
-    """
-    cols = ['Cluster ID', 'X', 'Y', 'Z', 'Peak Stat', 'Cluster Size (mm3)',
-            'Minimum TDP (Notip)']
-    # Replace None with 0
-    cluster_threshold = 0 if cluster_threshold is None else cluster_threshold
-    # print(cluster_threshold)
-    # check that stat_img is niimg-like object and 3D
-    stat_img = check_niimg_3d(stat_img)
-
-    stat_map_ = _safe_get_data(stat_img)
-    # Perform calibration before thresholding
-    stat_map_nonzero = stat_map_[stat_map_ != 0]
-    hommel = _compute_hommel_value(stat_map_nonzero, alpha)
-    ari_thr = sa.linear_template(alpha, hommel, hommel)
-    pval0, simes_thr = calibrate_simes(fmri_input, alpha,
-                                       k_max=k_max, B=B, seed=seed)
-    learned_templates_ = sa.get_permuted_p_values_one_sample(fmri_input,
-                                                             B=B,
-                                                             n_jobs=n_jobs,
-                                                             seed=None)
-    learned_templates = np.sort(learned_templates_, axis=0)
-    learned_thr = sa.calibrate_jer(alpha, learned_templates, pval0, k_max)
-
-    # Apply threshold(s) to image
-    stat_img = threshold_img(
-        img=stat_img,
-        threshold=stat_threshold,
-        cluster_threshold=cluster_threshold,
-        two_sided=two_sided,
-        mask_img=None,
-        copy=True,
-    )
-
-    # If cluster threshold is used, there is chance that stat_map will be
-    # modified, therefore copy is needed
-    stat_map = _safe_get_data(stat_img, ensure_finite=True,
-                              copy_data=(cluster_threshold is not None))
-    # Define array for 6-connectivity, aka NN1 or "faces"
-    conn_mat = np.zeros((3, 3, 3), int)
-    conn_mat[1, 1, :] = 1
-    conn_mat[1, :, 1] = 1
-    conn_mat[:, 1, 1] = 1
-    voxel_size = np.prod(stat_img.header.get_zooms())
-    signs = [1, -1] if two_sided else [1]
-    no_clusters_found = True
-    rows = []
-    for sign in signs:
-        # Flip map if necessary
-        temp_stat_map = stat_map * sign
-
-        # Binarize using CDT
-        binarized = temp_stat_map > stat_threshold
-        binarized = binarized.astype(int)
-
-        # If the stat threshold is too high simply return an empty dataframe
-        if np.sum(binarized) == 0:
-            warnings.warn(
-                'Attention: No clusters with stat {0} than {1}'.format(
-                    'higher' if sign == 1 else 'lower',
-                    stat_threshold * sign,
-                )
-            )
-            continue
-
-        # Now re-label and create table
-        label_map = ndimage.measurements.label(binarized, conn_mat)[0]
-        clust_ids = sorted(list(np.unique(label_map)[1:]))
-        peak_vals = np.array(
-            [np.max(temp_stat_map * (label_map == c)) for c in clust_ids])
-        # Sort by descending max value
-        clust_ids = [clust_ids[c] for c in (-peak_vals).argsort()]
-
-        for c_id, c_val in enumerate(clust_ids):
-            cluster_mask = label_map == c_val
-            masked_data = temp_stat_map * cluster_mask
-            masked_data_ = masked_data[masked_data != 0]
-            # Compute TDP bounds on cluster using our 3 methods
-            cluster_p_values = norm.sf(masked_data_)
-            ari_tdp = sa.min_tdp(cluster_p_values, ari_thr)
-            simes_tdp = sa.min_tdp(cluster_p_values, simes_thr)
-            learned_tdp = sa.min_tdp(cluster_p_values, learned_thr)
-            cluster_size_mm = int(np.sum(cluster_mask) * voxel_size)
-
-            # Get peaks, subpeaks and associated statistics
-            subpeak_ijk, subpeak_vals = _local_max(
-                masked_data,
-                stat_img.affine,
-                min_distance=min_distance,
-            )
-            subpeak_vals *= sign  # flip signs if necessary
-            subpeak_xyz = np.asarray(
-                coord_transform(
-                    subpeak_ijk[:, 0],
-                    subpeak_ijk[:, 1],
-                    subpeak_ijk[:, 2],
-                    stat_img.affine,
-                )
-            ).tolist()
-            subpeak_xyz = np.array(subpeak_xyz).T
-
-            # Only report peak and, at most, top 3 subpeaks.
-            n_subpeaks = np.min((len(subpeak_vals), 4))
-            for subpeak in range(n_subpeaks):
-                if subpeak == 0:
-                    row = [
-                        c_id + 1,
-                        subpeak_xyz[subpeak, 0],
-                        subpeak_xyz[subpeak, 1],
-                        subpeak_xyz[subpeak, 2],
-                        "{0:.2f}".format(subpeak_vals[subpeak]),
-                        cluster_size_mm,
-                        "{0:.2f}".format(learned_tdp),
-                    ]
-                else:
-                    # Subpeak naming convention is cluster num+letter:
-                    # 1a, 1b, etc
-                    sp_id = '{0}{1}'.format(
-                        c_id + 1,
-                        ascii_lowercase[subpeak - 1],
-                    )
-                    row = [
-                        sp_id,
-                        subpeak_xyz[subpeak, 0],
-                        subpeak_xyz[subpeak, 1],
-                        subpeak_xyz[subpeak, 2],
-                        "{0:.2f}".format(subpeak_vals[subpeak]),
-                        '',
-                        '',
-                    ]
                 rows += [row]
 
         # If we reach this point, there are clusters in this sign
         no_clusters_found = False
 
     if no_clusters_found:
         df = pd.DataFrame(columns=cols)
@@ -1074,15 +908,15 @@
         df = pd.DataFrame(columns=cols, data=rows)
 
     return df
 
 
 def get_tdp_bound_notip(stat_img, fmri_input, cluster_mask,
                         alpha=0.05,
-                        k_max=1000, B=1000, cluster_threshold=None,
+                        k_max=1000, n_permutations=1000, cluster_threshold=None,
                         two_sided=False, min_distance=8., n_jobs=2, seed=None):
     """Creates pandas dataframe with img cluster statistics.
     Parameters
     ----------
     stat_img : Niimg-like object,
        Statistical image (presumably in z- or p-scale).
     stat_threshold : `float`
@@ -1124,17 +958,17 @@
 
     stat_map_ = _safe_get_data(stat_img)
     # Perform calibration before thresholding
     stat_map_nonzero = stat_map_[stat_map_ != 0]
     hommel = _compute_hommel_value(stat_map_nonzero, alpha)
     ari_thr = sa.linear_template(alpha, hommel, hommel)
     pval0, simes_thr = calibrate_simes(fmri_input, alpha,
-                                       k_max=k_max, B=B, seed=seed)
+                                       k_max=k_max, B=n_permutations, seed=seed)
     learned_templates_ = sa.get_permuted_p_values_one_sample(fmri_input,
-                                                             B=B,
+                                                             B=n_permutations,
                                                              n_jobs=n_jobs,
                                                              seed=None)
     learned_templates = np.sort(learned_templates_, axis=0)
     learned_thr = sa.calibrate_jer(alpha, learned_templates, pval0, k_max)
 
     # If cluster threshold is used, there is chance that stat_map will be
     # modified, therefore copy is needed
```

### Comparing `notip-0.1.3/notip.egg-info/PKG-INFO` & `notip-0.1.4/notip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notip
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nonparametric True Discovery Proportion control for brain imaging
 Home-page: https://github.com/alexblnn/Notip
 Download-URL: https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz
 Author: Alexandre Blain
 Author-email: alexandre.blain@inria.fr
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notip-0.1.3/setup.py` & `notip-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 requirements = ["numpy>=1.15.0", "scipy>=1.0.0",
                 "joblib>=1.0.1", "scikit-learn>=0.22",
                 "nilearn","sanssouci","matplotlib",
                 "pandas", "joblib", "tqdm"]
 
 setup(
     name="notip",
-    version="0.1.3",
+    version="0.1.4",
     author="Alexandre Blain",
     author_email="alexandre.blain@inria.fr",
     description="Nonparametric True Discovery Proportion control for brain imaging",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/alexblnn/Notip",
     download_url="https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz",
```

