# Comparing `tmp/herbiv-0.1a4.tar.gz` & `tmp/herbiv-0.1a5.tar.gz`

## Comparing `herbiv-0.1a4.tar` & `herbiv-0.1a5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 herbiv-0.1a4/setup.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/analysis.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/compute.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/get.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/output.py
--rw-r--r--   0        0        0 13073523 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_chemical_protein_links.csv
--rw-r--r--   0        0        0  1377866 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_chemicals.csv
--rw-r--r--   0        0        0  1978068 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_proteins.csv
--rw-r--r--   0        0        0  1227198 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_tcm.csv
--rw-r--r--   0        0        0  1029771 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_tcm_chemical_links.csv
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 herbiv-0.1a4/LICENSE
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 herbiv-0.1a4/README.md
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 herbiv-0.1a4/pyproject.toml
--rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 herbiv-0.1a4/PKG-INFO
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 herbiv-0.1a5/setup.py
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/analysis.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/compute.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/get.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/output.py
+-rw-r--r--   0        0        0 13073523 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_chemical_protein_links.csv
+-rw-r--r--   0        0        0  1377866 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_chemicals.csv
+-rw-r--r--   0        0        0  1978068 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_proteins.csv
+-rw-r--r--   0        0        0  1227198 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_tcm.csv
+-rw-r--r--   0        0        0  1029771 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_tcm_chemical_links.csv
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/result/Network.csv
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/result/Type.csv
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 herbiv-0.1a5/LICENSE
+-rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 herbiv-0.1a5/README.md
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 herbiv-0.1a5/pyproject.toml
+-rw-r--r--   0        0        0    12767 2020-02-02 00:00:00.000000 herbiv-0.1a5/PKG-INFO
```

### Comparing `herbiv-0.1a4/setup.py` & `herbiv-0.1a5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="herbiv",
-    version="0.1a4",
+    version="0.1a5",
     description="HerbiV是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。HerbiV is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology.",
     # Optional
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV",
     author="王皓阳",
     author_email="Wesady@qq.com",
```

### Comparing `herbiv-0.1a4/src/herbiv/compute.py` & `herbiv-0.1a5/src/herbiv/compute.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 import numpy as np
 
 
-def score(chem_protein_links, chem, tcm_chem_links, tcm):
+def score(tcm, tcm_chem_links, chem, chem_protein_links):
     """
     计算化合物和中药的Importance Score
-    :param chem_protein_links: pd.DataFrame类型，用于计算的的化合物-蛋白质（靶点）的连接信息
-    :param chem: pd.DataFrame类型，需要计算Importance Score的化合物信息
-    :param tcm_chem_links: pd.DataFrame类型，需要计算Importance Score的化合物的中药-成分信息
-    :param tcm: pd.DataFrame类型，需要计算Importance Score的中药信息
+    :param tcm: pd.DataFrame类型，中药信息
+    :param tcm_chem_links: pd.DataFrame类型，中药-化合物（中药成分）连接信息
+    :param chem: pd.DataFrame类型，化合物（中药成分）信息
+    :param chem_protein_links: pd.DataFrame类型，化合物（中药成分）-蛋白质（靶点）连接信息
     :return: chem: pd.DataFrame类型，化合物的Importance Score的计算结果
     :return: tcm: pd.DataFrame类型，中药的Importance Score的计算结果
     """
 
+    tcm_c = tcm.copy()
+    chem_c = chem.copy()
+
     # 计算化合物的Importance Score
-    chem['Importance Score'] = chem.loc[:, 'HVCID'].apply(
+    chem_c['Importance Score'] = chem_c.loc[:, 'HVCID'].apply(
         lambda x: 1 - (
                 1 - np.array([*chem_protein_links.loc[chem_protein_links['HVCID'] == x]['Combined_score']])).prod())
 
     # 计算中药的Importance Score
-    tcm['Importance Score'] = tcm.loc[:, 'HVMID'].apply(
-        lambda x: 1 - (1 - np.array([*chem.loc[
-            chem['HVCID'].isin(tcm_chem_links.loc[tcm_chem_links['HVMID'] == x]['HVCID'])][
+    tcm_c['Importance Score'] = tcm_c.loc[:, 'HVMID'].apply(
+        lambda x: 1 - (1 - np.array([*chem_c.loc[
+            chem_c['HVCID'].isin(tcm_chem_links.loc[tcm_chem_links['HVMID'] == x]['HVCID'])][
             'Importance Score']])).prod())
 
     # 根据Importance Score降序排序
-    tcm = tcm.sort_values(by='Importance Score', ascending=False)
+    tcm_c = tcm_c.sort_values(by='Importance Score', ascending=False)
 
     # 重新设置索引
-    tcm.index = range(tcm.shape[0])
+    tcm_c.index = range(tcm_c.shape[0])
+    chem_c.index = range(chem_c.shape[0])
 
-    return chem, tcm
+    return tcm_c, chem_c
 
 
 if __name__ == '__main__':
     import get
 
-    tcm_info1 = get.get_tcm('cn_name', ['柴胡'])
-    tcm_chem_links_info1 = get.get_tcm_chem_links('HVMID', tcm_info1['HVMID'])
-    chem_info1 = get.get_chemicals('HVCID', tcm_chem_links_info1['HVCID'])
-    chem_protein_links1 = get.get_chem_protein_links('HVCID', chem_info1['HVCID'])
-    chem_info1, tcm_info1 = score(chem_protein_links1, chem_info1, tcm_chem_links_info1, tcm_info1)
-
-    chem_protein_links2 = get.get_chem_protein_links('Ensembl_ID', ['ENSP0000026332', 'ENSP00000398698'], 0)
-    chem_info2 = get.get_chemicals('HVCID', chem_protein_links2['HVCID'])
-    tcm_chem_links_info2 = get.get_tcm_chem_links('HVCID', chem_info2['HVCID'])
-    tcm_info2 = get.get_tcm('HVMID', tcm_chem_links_info2['HVMID'])
-    chem_info2, tcm_info2 = score(chem_protein_links2, chem_info2, tcm_chem_links_info2, tcm_info2)
+    chem_protein_links_info = get.get_chem_protein_links('Ensembl_ID', ['ENSP0000026332', 'ENSP00000398698'])
+    chem_info = get.get_chemicals('HVCID', chem_protein_links_info['HVCID'])
+    tcm_chem_links_info = get.get_tcm_chem_links('HVCID', chem_info['HVCID'])
+    tcm_info = get.get_tcm('HVMID', tcm_chem_links_info['HVMID'])
+    tcm_info, chem_info = score(tcm_info, tcm_chem_links_info, chem_info, chem_protein_links_info)
```

### Comparing `herbiv-0.1a4/src/herbiv/get.py` & `herbiv-0.1a5/src/herbiv/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 
 
 def get_tcm(by, items):
     """
     读取HerbiV_tcm数据集，返回items中中药的信息
     :param by: str类型，数据集中与items相匹配的列的列名
-    :param items: pd.DataFrame或其他任何可以使用in判断一个元素是否在其中的组合数据类型，存放要查询的中药
+    :param items: 任何可以使用in判断一个元素是否在其中的组合数据类型，存放要查询的中药
     :return: pd.DataFrame类型，items中中药的信息
     """
 
     # 读取数据集
     current_directory = os.path.dirname(os.path.abspath(__file__))
     tcm_all = pd.read_csv(current_directory + r'/data/HerbiV_tcm.csv')
 
@@ -64,15 +64,15 @@
 
 
 def get_chem_protein_links(by, items, score=900):
     """
     读取HerbiV_chemicals数据集，返回items中化合物/蛋白质的combined_score大于等于score的化合物-蛋白质（靶点）连接信息
     :param by: str类型，数据集中与items相匹配的列的列名
     :param items: pd.DataFrame或其他任何可以使用in判断一个元素是否在其中的组合数据类型，存放要查询的化合物/蛋白质
-    :param score: int类型，仅combined_score大于等于score的记录会被筛选出
+    :param score: int类型，仅combined_score大于等于score的记录会被筛选出，默认为900
     :return: pd.DataFrame类型，items中化合物/蛋白质的combined_score大于等于score的化合物-蛋白质（靶点）连接信息
     """
     # 读取数据集
     current_directory = os.path.dirname(os.path.abspath(__file__))
     chem_protein_links_all = pd.read_csv(current_directory + r'/data/HerbiV_chemical_protein_links.csv')
 
     # 在HerbiV_chemical_protein_links中获取items中化合物/蛋白质的combined_score大于等于score的化合物-蛋白质（靶点）连接信息
@@ -109,18 +109,12 @@
     # 重置索引
     proteins.index = range(proteins.shape[0])
 
     return proteins
 
 
 if __name__ == '__main__':
-    tcm_info1 = get_tcm('cn_name', ['柴胡'])
-    tcm_chem_links_info1 = get_tcm_chem_links('HVMID', tcm_info1['HVMID'])
-    chem_info1 = get_chemicals('HVCID', tcm_chem_links_info1['HVCID'])
-    chem_protein_links1 = get_chem_protein_links('HVCID', chem_info1['HVCID'])
-    protein1 = get_proteins('Ensembl_ID', chem_protein_links1['Ensembl_ID'])
-
-    protein2 = get_proteins('Ensembl_ID', ['ENSP00000252519', 'ENSP00000381588'])
-    chem_protein_links2 = get_chem_protein_links('Ensembl_ID', protein2['Ensembl_ID'], 0)
-    chem_info2 = get_chemicals('HVCID', chem_protein_links2['HVCID'])
-    tcm_chem_links_info2 = get_tcm_chem_links('HVCID', chem_info2['HVCID'])
-    tcm_info2 = get_tcm('HVMID', tcm_chem_links_info2['HVMID'])
+    tcm_info = get_tcm('cn_name', ['柴胡', '黄芩'])
+    tcm_chem_links_info = get_tcm_chem_links('HVMID', tcm_info['HVMID'])
+    chem_info = get_chemicals('HVCID', tcm_chem_links_info['HVCID'])
+    chem_protein_links_info = get_chem_protein_links('HVCID', chem_info['HVCID'])
+    protein_info = get_proteins('Ensembl_ID', chem_protein_links_info['Ensembl_ID'])
```

### Comparing `herbiv-0.1a4/src/herbiv/output.py` & `herbiv-0.1a5/src/herbiv/output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 import os
 import pandas as pd
 
 
-def out_for_cyto(chem_protein_links, chem, genes, tcm_chem_links, tcm, path='result/'):
+def out_for_cyto(tcm, tcm_chem_links, chem, chem_protein_links, protein, path='result/'):
     r"""
     输出Cytoscape用于作图的网络文件和属性文件
-    :param chem_protein_links: pd.DataFrame类型，HerbiV_chemical_protein_links数据集数据集中包含目标基因且Combined_score大于等于score的记录
-    :param chem: pd.DataFrame类型，chem_protein_links中化合物的信息及其Importance Score
-    :param genes: pd.DataFrame类型，存储拟分析蛋白（基因）在STITCH中的ID与其名称的对应关系
-    :param tcm_chem_links: pd.DataFrame类型，包含filtered_chem中化合物的名称、STITCH数据库中的CID和HERB数据库中对应的中药
-    :param tcm: pd.DataFrame类型，tcm_chem_links中中药的信息及其Importance Score
+    :param tcm: pd.DataFrame类型，中药信息
+    :param tcm_chem_links: pd.DataFrame类型，中药-化合物（中药成分）连接信息
+    :param chem: pd.DataFrame类型，化合物（中药成分）信息
+    :param chem_protein_links: pd.DataFrame类型，化合物（中药成分）-蛋白质（靶点）连接信息
     :param path: 字符串类型，存放结果的目录
     """
-
-    chem_protein_links_c = chem_protein_links.copy()
-    chem_c = chem.copy()
-    genes_c = genes.copy()
-    tcm_chem_links_c = tcm_chem_links.copy()
     tcm_c = tcm.copy()
+    tcm_chem_links_c = tcm_chem_links.copy()
+    chem_c = chem.copy()
+    chem_protein_links_c = chem_protein_links.copy()
+    protein_c = protein.copy()
 
     # 若无path目录，先创建该目录
     if not os.path.exists(path):
         os.mkdir(path)
+
     out_chem_protein_links = chem_protein_links_c.iloc[:, 0:2]
     out_chem_protein_links.columns = ['SourceNode', 'TargetNode']
 
     out_chem_protein_links.loc[:, 'SourceNode'] = out_chem_protein_links.loc[:, 'SourceNode'].apply(
         lambda x: chem_c.loc[chem_c['HVCID'] == x]['Name'].iloc[0] if len(
             chem_c.loc[chem_c['HVCID'] == x]['Name']) > 0 else None)
 
     out_chem_protein_links.dropna(subset=['SourceNode'], inplace=True)
 
     out_chem_protein_links.loc[:, 'TargetNode'] = out_chem_protein_links.loc[:, 'TargetNode'].apply(
-        lambda x: genes_c.loc[genes_c['Ensembl_ID'] == x]['gene_name'].iloc[0] if len(
-            genes_c.loc[genes_c['Ensembl_ID'] == x]['gene_name']) > 0 else None)
+        lambda x: protein_c.loc[protein_c['Ensembl_ID'] == x]['gene_name'].iloc[0] if len(
+            protein_c.loc[protein_c['Ensembl_ID'] == x]['gene_name']) > 0 else None)
 
     out_chem_protein_links.dropna(subset=['TargetNode'], inplace=True)
 
     out_tcm_chem = tcm_chem_links_c.iloc[:, 0:2]
     out_tcm_chem.columns = ['SourceNode', 'TargetNode']
 
     out_tcm_chem.loc[:, 'SourceNode'] = out_tcm_chem.loc[:, 'SourceNode'].apply(
@@ -56,31 +55,28 @@
     out_chem.columns = ['Key']
     out_chem['Attribute'] = 'Chemicals'
 
     out_tcm = tcm_c.loc[:, ['cn_name']]
     out_tcm.columns = ['Key']
     out_tcm['Attribute'] = 'TCM'
 
-    out_gene = genes_c.loc[:, ['gene_name']]
+    out_gene = protein_c.loc[:, ['gene_name']]
     out_gene.columns = ['Key']
-    out_gene['Attribute'] = 'gene'
+    out_gene['Attribute'] = 'Proteins'
 
     # 输出Network文件
     pd.concat([out_chem_protein_links, out_tcm_chem]).to_csv(path + 'Network.csv', index=False)
 
     # 输出Type文件
     pd.concat([out_tcm, out_chem, out_gene]).to_csv(path + 'Type.csv', index=False)
 
 
 if __name__ == '__main__':
     import get
-    import compute
 
-    genes_info = ['ENSP0000026332', 'ENSP00000398698']
-    proteins = get.get_proteins('Ensembl_ID', genes_info)
-    chem_protein_links_info = get.get_chem_protein_links('Ensembl_ID', genes_info, 0)
+    protein_info = get.get_proteins('Ensembl_ID', ['ENSP0000026332', 'ENSP00000398698'])
+    chem_protein_links_info = get.get_chem_protein_links('Ensembl_ID', protein_info['Ensembl_ID'])
     chem_info = get.get_chemicals('HVCID', chem_protein_links_info['HVCID'])
     tcm_chem_links_info = get.get_tcm_chem_links('HVCID', chem_info['HVCID'])
     tcm_info = get.get_tcm('HVMID', tcm_chem_links_info['HVMID'])
-    chem_info, tcm_info = compute.score(chem_protein_links_info, chem_info, tcm_chem_links_info, tcm_info)
 
-    out_for_cyto(chem_protein_links_info, chem_info, genes_info, tcm_chem_links_info, tcm_info)
+    out_for_cyto(tcm_info, tcm_chem_links_info, chem_info, chem_protein_links_info, protein_info)
```

### Comparing `herbiv-0.1a4/src/herbiv/data/HerbiV_chemical_protein_links.csv` & `herbiv-0.1a5/src/herbiv/data/HerbiV_chemical_protein_links.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a4/src/herbiv/data/HerbiV_chemicals.csv` & `herbiv-0.1a5/src/herbiv/data/HerbiV_chemicals.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a4/src/herbiv/data/HerbiV_proteins.csv` & `herbiv-0.1a5/src/herbiv/data/HerbiV_proteins.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a4/src/herbiv/data/HerbiV_tcm.csv` & `herbiv-0.1a5/src/herbiv/data/HerbiV_tcm.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a4/src/herbiv/data/HerbiV_tcm_chemical_links.csv` & `herbiv-0.1a5/src/herbiv/data/HerbiV_tcm_chemical_links.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a4/LICENSE` & `herbiv-0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a4/pyproject.toml` & `herbiv-0.1a5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = [
     "hatchling",
+    "numpy",
     "pandas",
     "typing-extensions",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "herbiv"
-version = "0.1a4"
+version = "0.1a5"
 authors = [
   { name="王皓阳", email="Wesady@qq.com" },
 ]
-description = "药理大师是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。Pharmastar is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology."
+description = "HerbiV是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。HerbiV is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
```

