# Comparing `tmp/cellmap-1.0.1.dev202304181101-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304190155-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1389906 bytes, number of entries: 6
+Zip file size: 1390321 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    60956 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304181101.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304181101.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304181101.dist-info/RECORD
-6 files, 4510320 bytes uncompressed, 1389020 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    62699 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304190155.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304190155.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304190155.dist-info/RECORD
+6 files, 4512063 bytes uncompressed, 1389435 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304181101.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304190155.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304181101.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304190155.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304181101.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304190155.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -5,14 +5,16 @@
 import matplotlib.pyplot as plt
 from matplotlib import patheffects as PathEffects
 import matplotlib.cm
 import networkx as nx
 import scipy
 import sklearn.preprocessing
 import sklearn.neighbors
+from sklearn.linear_model import LinearRegression
+from sklearn.preprocessing import PolynomialFeatures
 import matplotlib.colors
 import pandas as pd
 import logging
 import scanpy
 import scvelo as scv
 import plotly.graph_objects as go
 from plotly.offline import plot
@@ -1264,19 +1266,19 @@
     target_clusters,
     n_cells = 50,
     register = 10,
     basis = 'umap',
     potential_key = 'potential',
     cluster_key = 'clusters',
     graph_method = 'Delauney',
+    path_key = 'path',
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
-    return_path = False
 ):
 
     # kwargs_arg = check_arguments(adata, verbose = True, exp_key=exp_key, vkey = vkey, basis=basis, graph_method=graph_method)
     # exp_key,vkey,basis = kwargs_arg['exp_key'],kwargs_arg['vkey'],kwargs_arg['basis']
 
     basis_key = 'X_%s' % basis
     data_pos = adata.obsm[basis_key]
@@ -1308,18 +1310,18 @@
     
     cmap_ = plt.get_cmap("tab10")
     figsize = (10,8)
     fig,ax = plt.subplots(figsize=figsize)
     ax.triplot(tri_,color='gray',zorder=0,alpha=0.2,lw=1)
     clusters_ = adata.obs[cluster_key]
     idx_ = clusters_ == source_cluster
-    ax.scatter(data_pos[idx_,0],data_pos[idx_,1],color=cmap_(0),zorder=10,marker='o',alpha=0.2,s=5,label=source_cluster+' (source)')
+    ax.scatter(data_pos[idx_,0],data_pos[idx_,1],color='gray',zorder=10,marker='D',alpha=0.2,s=5,label=source_cluster+' (source)')
     for i_trg_ in range(len(target_clusters)):
         idx_ = clusters_ == target_clusters[i_trg_]
-        ax.scatter(data_pos[idx_,0],data_pos[idx_,1],color=cmap_(i_trg_+1),zorder=10,marker='o',alpha=0.2,s=5,label=target_clusters[i_trg_]+' (target)')
+        ax.scatter(data_pos[idx_,0],data_pos[idx_,1],color=cmap_(i_trg_),zorder=10,marker='o',alpha=0.2,s=5,label=target_clusters[i_trg_]+' (target)')
     leg = ax.legend(bbox_to_anchor=(1.05, 0.5), loc='center left', borderaxespad=0, fontsize=12,markerscale=3)
     for lh in leg.legendHandles: lh.set_alpha(1)
 
     data_src_ = data_pos[adata.obs[cluster_key].values == source_cluster]
     center_src_ = np.mean(data_src_,axis=0)
     centrality_src_ = np.linalg.norm(data_src_-center_src_,axis=1)
     src_set_all_ = np.arange(adata.shape[0])[adata.obs[cluster_key].values == source_cluster][np.argsort(centrality_src_)]
@@ -1341,15 +1343,55 @@
         for src_,trg_ in np.vstack((src_set_,trg_set_)).T:
             path = nx.dijkstra_path(G, source=src_, target=trg_, weight='weight')
             pathes.append(path)
             edges.append(np.array([[path[i], path[i+1]] for i in range(len(path)-1)]))
             weights.append((sum([G[path[i]][path[i+1]]['weight'] for i in range(len(path)-1)]))/sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
             dists.append(sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
         path_all.append(pathes)
-        ax.scatter(data_pos[src_set_,0],data_pos[src_set_,1],color=cmap_(0),zorder=20,marker='o',s=20)
-        ax.scatter(data_pos[trg_set_,0],data_pos[trg_set_,1],color=cmap_(i_trg_+1),zorder=20,marker='o',s=20)
+        ax.scatter(data_pos[trg_set_,0],data_pos[trg_set_,1],color=cmap_(i_trg_),zorder=20,marker='o',s=20)
         for i in range(n_cells_):
-            src_,trg_ = src_set_[i],trg_set_[i]
-            for s,t in edges[i]:
-                ax.plot([data_pos[s,0],data_pos[t,0]],[data_pos[s,1],data_pos[t,1]],color=cmap_(i_trg_+1),zorder=10)
+            ax.plot(data_pos[pathes[i],0],data_pos[pathes[i],1],color=cmap_(i_trg_),zorder=10,ls=':')
+    ax.scatter(data_pos[src_set_,0],data_pos[src_set_,1],color='gray',zorder=20,marker='D',s=30)
     ax.axis('off')
-    if return_path: return path_all
+    adata.uns[path_key] = path_all
+
+def path_gene_profile(
+    adata,
+    source_cluster,
+    target_clusters,
+    genes,
+    path_key = 'path',
+    exp_key = None,
+    fontsize_title = 16,
+    fontsize_label = 14,
+    fontsize_legend = 12,
+):
+    if exp_key == None:
+        if scipy.sparse.issparse(adata.X): data_exp = adata.X.toarray()
+        else: data_exp = adata.X
+    else:
+        data_exp = adata.layers[exp_key]
+    path = adata.uns[path_key]
+    cmap_ = plt.get_cmap("tab10")
+
+    for gene in genes:
+        if gene in adata.var.index:
+            fig = plt.figure(figsize=(10,6))
+            for i in range(len(path)):
+                x_data,y_data = np.empty(0,dtype=float),np.empty(0,dtype=float)
+                for pi in path[i]:
+                    x_data = np.append(x_data,np.linspace(0,1,len(pi)))
+                    y_data = np.append(y_data,data_exp[:,adata.var.index==gene][pi])
+                X = x_data[:, np.newaxis]
+                poly = PolynomialFeatures(degree=10)
+                X_poly = poly.fit_transform(X)
+                model = LinearRegression()
+                model.fit(X_poly, y_data)
+                plt.scatter(x_data, y_data,color=cmap_(i),alpha=0.05)
+                plot_x = np.linspace(0,1,100)
+                plt.plot(plot_x, model.predict(poly.fit_transform(plot_x[:, np.newaxis])),color=cmap_(i),lw=5,label=target_clusters[i])
+            plt.legend(bbox_to_anchor=(1.05, 0.5), loc='center left', borderaxespad=0,title='Target', fontsize=fontsize_legend, title_fontsize=fontsize_legend)
+            plt.xticks([0,1],['Source\n(%s)' % source_cluster,'Target'],fontsize=fontsize_label)
+            plt.title(gene,fontsize=fontsize_title)
+            plt.show()
+        else:
+            print('Gene \"%s\" was not found' % gene)
```

## Comparing `cellmap-1.0.1.dev202304181101.dist-info/METADATA` & `cellmap-1.0.1.dev202304190155.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304181101
+Version: 1.0.1.dev202304190155
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

