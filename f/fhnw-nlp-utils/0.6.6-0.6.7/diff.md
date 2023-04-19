# Comparing `tmp/fhnw_nlp_utils-0.6.6-py3-none-any.whl.zip` & `tmp/fhnw_nlp_utils-0.6.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 23312 bytes, number of entries: 18
+Zip file size: 23949 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 07:56 fhnw/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 07:56 fhnw/nlp/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 08:10 fhnw/nlp/utils/__init__.py
 -rw-r--r--  2.0 unx      144 b- defN 21-Sep-18 08:10 fhnw/nlp/utils/colab.py
 -rw-r--r--  2.0 unx     2254 b- defN 22-Aug-14 09:43 fhnw/nlp/utils/defaults.py
 -rw-r--r--  2.0 unx     6880 b- defN 22-Aug-14 09:42 fhnw/nlp/utils/normalize.py
 -rw-r--r--  2.0 unx    37887 b- defN 23-Mar-12 20:31 fhnw/nlp/utils/params.py
 -rw-r--r--  2.0 unx     9537 b- defN 22-Dec-12 20:18 fhnw/nlp/utils/ploting.py
 -rw-r--r--  2.0 unx     2262 b- defN 22-Aug-25 17:41 fhnw/nlp/utils/preprocess.py
 -rw-r--r--  2.0 unx    10048 b- defN 21-Nov-14 18:34 fhnw/nlp/utils/processing.py
 -rw-r--r--  2.0 unx     6838 b- defN 21-Nov-03 20:09 fhnw/nlp/utils/storage.py
 -rw-r--r--  2.0 unx     3346 b- defN 22-Oct-05 05:11 fhnw/nlp/utils/system.py
 -rw-r--r--  2.0 unx     3212 b- defN 22-Aug-10 15:41 fhnw/nlp/utils/text.py
--rw-r--r--  2.0 unx     4011 b- defN 23-Apr-15 14:21 fhnw/nlp/utils/transformers.py
--rw-r--r--  2.0 unx     1298 b- defN 23-Apr-15 14:21 fhnw_nlp_utils-0.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 14:21 fhnw_nlp_utils-0.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-15 14:21 fhnw_nlp_utils-0.6.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1459 b- defN 23-Apr-15 14:21 fhnw_nlp_utils-0.6.6.dist-info/RECORD
-18 files, 89273 bytes uncompressed, 20922 bytes compressed:  76.6%
+-rw-r--r--  2.0 unx     7656 b- defN 23-Apr-19 05:05 fhnw/nlp/utils/transformers.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-Apr-19 05:21 fhnw_nlp_utils-0.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 05:21 fhnw_nlp_utils-0.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-19 05:21 fhnw_nlp_utils-0.6.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1459 b- defN 23-Apr-19 05:21 fhnw_nlp_utils-0.6.7.dist-info/RECORD
+18 files, 92918 bytes uncompressed, 21559 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: fhnw/nlp/utils/text.py
 Comment: 
 
 Filename: fhnw/nlp/utils/transformers.py
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.6.dist-info/METADATA
+Filename: fhnw_nlp_utils-0.6.7.dist-info/METADATA
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.6.dist-info/WHEEL
+Filename: fhnw_nlp_utils-0.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.6.dist-info/top_level.txt
+Filename: fhnw_nlp_utils-0.6.7.dist-info/top_level.txt
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.6.dist-info/RECORD
+Filename: fhnw_nlp_utils-0.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fhnw/nlp/utils/transformers.py

```diff
@@ -36,14 +36,15 @@
     params: dict
         The dictionary containing the parameters
     data: dataframe
         The data
     predict_func: callable
         The function that computes the prediction
     """
+    
     import os
     from datetime import datetime
     
     from fhnw.nlp.utils.storage import save_dataframe
     from fhnw.nlp.utils.storage import load_dataframe
     
     verbose = params.get("verbose", False)
@@ -104,7 +105,109 @@
     if verbose:
         print(datetime.now().time(), "Prediction done. Batches:", str(data.shape[0] // batch_size), ", processed elements:", str(data.shape[0]), ", total predictions:", len(predictions))
     
     pred_data = pd.DataFrame(predictions)
     save_dataframe(pred_data, store_path)
     
     return pred_data
+    
+
+def dataframe_to_dataset(params, data):
+    """Converts a dataframe into a Huggingface dataset
+
+    Parameters
+    ----------
+    params: dict
+        The dictionary containing the parameters
+    data: dataframe
+        The data
+        
+    Returns
+    -------
+    dataset
+        The Huggingface dataset
+    """
+    
+    import pandas as pd
+    from fhnw.nlp.utils.params import compute_binarized_labels
+    from fhnw.nlp.utils.params import create_label_binarizer_and_set
+    
+    from datasets import ClassLabel
+    from datasets import Dataset
+    
+    X_column_name = params.get("X_column_name", "text")
+    y_column_name = params.get("y_column_name", "label")
+    computed_objects_column_name = params.get("computed_objects_column_name", "computed_objects")
+    
+    data = data.drop(labels=data.columns.difference([X_column_name, y_column_name]), axis=1)
+    
+    label_binarizer = params.setdefault(computed_objects_column_name, {}).get("label_binarizer", None)
+    if label_binarizer is None:
+        create_label_binarizer_and_set(params, data)
+        label_binarizer = params[computed_objects_column_name]["label_binarizer"]
+    num_classes = len(label_binarizer.classes_)
+    class_names = list(label_binarizer.classes_)
+    
+    data[y_column_name] = compute_binarized_labels(params, data)
+    
+    data.index.name = "idx"
+    
+    dataset = Dataset.from_pandas(data)
+    
+    dataset.features["label"] = ClassLabel(num_classes=num_classes, names=class_names)
+    
+    return dataset
+
+
+def dataframe_to_datasets(params, data, data_test=None):
+    """Converts a dataframe into a Huggingface dataset dictionary with a train, val and test split
+
+    Parameters
+    ----------
+    params: dict
+        The dictionary containing the parameters
+    data: dataframe
+        The data
+    data_test: dataframe
+        The user defined test split (use None to automatically generate a test split)  
+        
+    Returns
+    -------
+    dataset
+        The Huggingface dataset dictionary
+    """
+    
+    import pandas as pd
+    from fhnw.nlp.utils.params import compute_binarized_labels
+    from fhnw.nlp.utils.params import create_label_binarizer_and_set
+    from fhnw.nlp.utils.params import get_train_test_split
+    
+    from datasets import ClassLabel
+    from datasets import Dataset
+    from datasets import DatasetDict
+    
+    X_column_name = params.get("X_column_name", "text")
+    y_column_name = params.get("y_column_name", "label")
+    computed_objects_column_name = params.get("computed_objects_column_name", "computed_objects")
+    
+    data = data.drop(labels=data.columns.difference([X_column_name, y_column_name]), axis=1)
+
+    # ensure label_binarizer builds on all data (function dataframe_to_dataset will use the existing)
+    label_binarizer = params.setdefault(computed_objects_column_name, {}).get("label_binarizer", None)
+    if label_binarizer is None:
+        create_label_binarizer_and_set(params, data)
+        label_binarizer = params[computed_objects_column_name]["label_binarizer"]
+    
+    # do the split
+    if data_test is None:
+        data, data_test = get_train_test_split(params, data)
+    data_train, data_val = get_train_test_split(params, data)
+
+    dataset_train = dataframe_to_dataset(params, data_train)
+    dataset_test = dataframe_to_dataset(params, data_test)
+    dataset_val = dataframe_to_dataset(params, data_val)
+    
+    transformers_datasets = DatasetDict({"train":dataset_train, "validation":dataset_val, "test":dataset_test})
+    
+    params.setdefault(computed_objects_column_name, {})["transformers_datasets"] = transformers_datasets
+    
+    return transformers_datasets
```

## Comparing `fhnw_nlp_utils-0.6.6.dist-info/METADATA` & `fhnw_nlp_utils-0.6.7.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhnw-nlp-utils
-Version: 0.6.6
+Version: 0.6.7
 Summary: Utilities for NLP courses taught at FHNW.
 Home-page: http://github.com/markif/fhnw-nlp-utils
 Author: Fabian
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

## Comparing `fhnw_nlp_utils-0.6.6.dist-info/RECORD` & `fhnw_nlp_utils-0.6.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 fhnw/nlp/utils/params.py,sha256=xavHoG_CMmygKGp3lwHqPbZUpfnrjdLjZPII2fiZPjE,37887
 fhnw/nlp/utils/ploting.py,sha256=8ya50BauVgWfRh7X7V9urU5SCvd7RSF7INhCgKHdzzc,9537
 fhnw/nlp/utils/preprocess.py,sha256=FDy6HAYS3OjKue9kVigh7Cg84gc3rju5Zu0WuOLVoq0,2262
 fhnw/nlp/utils/processing.py,sha256=73R2Vy4tMzXpbjSbck7xZFDigaA3cjuLxbe-ZXxs_uc,10048
 fhnw/nlp/utils/storage.py,sha256=F3C19qp9x2cGHnE0mdLVQxLLqBzgtFUCWZSGtzmk_yw,6838
 fhnw/nlp/utils/system.py,sha256=yRphzlhw34C8qyl-sgUSbz56_Ckr8G-tsRJkko-pv-U,3346
 fhnw/nlp/utils/text.py,sha256=ElaWYdl_7YkHc_IHJyEUZPvKgcADTcbEBEL1FO5emME,3212
-fhnw/nlp/utils/transformers.py,sha256=DnSQhF00EMDF_-8616BRI9X_iPHvGidP4AZkfoq0mis,4011
-fhnw_nlp_utils-0.6.6.dist-info/METADATA,sha256=McOy4MXZ6NLlCP-aEQ9GREJxMevyYbMXidyJaZJhArc,1298
-fhnw_nlp_utils-0.6.6.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
-fhnw_nlp_utils-0.6.6.dist-info/top_level.txt,sha256=G3JGQX_1iq_fMxU1-sbRHKR8vesyWdKRcLPkdbd66MA,5
-fhnw_nlp_utils-0.6.6.dist-info/RECORD,,
+fhnw/nlp/utils/transformers.py,sha256=Jge66cuppFN3llTo38FSKvjuuqbHtAZXnfgeGj6qWe4,7656
+fhnw_nlp_utils-0.6.7.dist-info/METADATA,sha256=Qd31vHy-smo76PieXLtyJ2rbTCYeS1OlOHwcOYvIPBo,1298
+fhnw_nlp_utils-0.6.7.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
+fhnw_nlp_utils-0.6.7.dist-info/top_level.txt,sha256=G3JGQX_1iq_fMxU1-sbRHKR8vesyWdKRcLPkdbd66MA,5
+fhnw_nlp_utils-0.6.7.dist-info/RECORD,,
```

