# Comparing `tmp/MLandPattern-0.1.6-py3-none-any.whl.zip` & `tmp/MLandPattern-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5388 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8099 b- defN 23-Apr-18 18:54 MLandPattern/MLandPattern.py
+Zip file size: 5369 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     8056 b- defN 23-Apr-18 22:18 MLandPattern/MLandPattern.py
 -rw-r--r--  2.0 unx       27 b- defN 23-Mar-29 18:22 MLandPattern/__init__.py
 -rw-r--r--  2.0 unx     5071 b- defN 23-Mar-29 09:34 MLandPattern/general_methods.py
--rw-r--r--  2.0 unx      225 b- defN 23-Apr-18 18:57 MLandPattern-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 18:57 MLandPattern-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-18 18:57 MLandPattern-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      569 b- defN 23-Apr-18 18:57 MLandPattern-0.1.6.dist-info/RECORD
-7 files, 14096 bytes uncompressed, 4372 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx      225 b- defN 23-Apr-18 22:18 MLandPattern-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 22:18 MLandPattern-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-18 22:18 MLandPattern-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      569 b- defN 23-Apr-18 22:18 MLandPattern-0.1.7.dist-info/RECORD
+7 files, 14053 bytes uncompressed, 4353 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: MLandPattern/__init__.py
 Comment: 
 
 Filename: MLandPattern/general_methods.py
 Comment: 
 
-Filename: MLandPattern-0.1.6.dist-info/METADATA
+Filename: MLandPattern-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: MLandPattern-0.1.6.dist-info/WHEEL
+Filename: MLandPattern-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: MLandPattern-0.1.6.dist-info/top_level.txt
+Filename: MLandPattern-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: MLandPattern-0.1.6.dist-info/RECORD
+Filename: MLandPattern-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## MLandPattern/MLandPattern.py

```diff
@@ -229,9 +229,8 @@
     :param mu: row vector with the mean associated to each dimension
     :param c: Covariance matrix
     :return: the logarithm of the likelihood of the datapoints, and the associated gaussian density
     """
     M = c.shape[1]
     logN = logpdf_GAU_ND(X, mu, c)
     print(logN.shape)
-    acum = logN.sum(1) if M != 1 else logN.sum()
-    return acum
+    return logN.sum()
```

