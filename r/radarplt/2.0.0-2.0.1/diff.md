# Comparing `tmp/radarplt-2.0.0.tar.gz` & `tmp/radarplt-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radarplt-2.0.0.tar", max compression
+gzip compressed data, was "radarplt-2.0.1.tar", max compression
```

## Comparing `radarplt-2.0.0.tar` & `radarplt-2.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-04-18 18:40:56.926019 radarplt-2.0.0/LICENSE
--rw-r--r--   0        0        0     4749 2023-04-18 18:40:56.926223 radarplt-2.0.0/README.md
--rw-r--r--   0        0        0      504 2023-04-19 13:29:43.550605 radarplt-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    11134 2023-04-19 13:30:27.196312 radarplt-2.0.0/radarplt/__init__.py
--rw-r--r--   0        0        0     3782 2023-04-18 18:40:56.937136 radarplt-2.0.0/radarplt/factory.py
--rw-r--r--   0        0        0      327 2023-04-18 18:40:56.937259 radarplt-2.0.0/radarplt/helpers.py
--rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 radarplt-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-18 18:40:56.926019 radarplt-2.0.1/LICENSE
+-rw-r--r--   0        0        0     4749 2023-04-18 18:40:56.926223 radarplt-2.0.1/README.md
+-rw-r--r--   0        0        0      504 2023-04-19 13:36:23.912964 radarplt-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11318 2023-04-19 13:36:14.573663 radarplt-2.0.1/radarplt/__init__.py
+-rw-r--r--   0        0        0     3782 2023-04-18 18:40:56.937136 radarplt-2.0.1/radarplt/factory.py
+-rw-r--r--   0        0        0      327 2023-04-18 18:40:56.937259 radarplt-2.0.1/radarplt/helpers.py
+-rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 radarplt-2.0.1/PKG-INFO
```

### Comparing `radarplt-2.0.0/LICENSE` & `radarplt-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radarplt-2.0.0/README.md` & `radarplt-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `radarplt-2.0.0/radarplt/__init__.py` & `radarplt-2.0.1/radarplt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -231,58 +231,67 @@
         label_angles = [
             self.angles[label] * 180 / np.pi for label in self.ordered_labels
         ]
 
         # rotation reset to 0 for polar coordinates, so we'll remove all xticks and
         # just use the coordinates we get when we run thetagrids
         lines, labels = plt.thetagrids(label_angles, labels)
-        ax.set_xticks([])
         n_labels = []
         for i in range(len(labels)):
             label = labels[i]
             x, y = label.get_position()
-            lab = ax.text(x, y, label.get_text(), transform=label.get_transform(),
-                     ha=label.get_ha(), va=label.get_va())
+            lab = ax.text(
+                x,
+                y,
+                label.get_text(),
+                transform=label.get_transform(),
+                ha=label.get_ha(),
+                va=label.get_va(),
+            )
             lab.set_rotation(label_angles[i])
             n_labels.append(lab)
+        # don't want to remove the ticks, just the label text
+        ax.set_xticklabels(["" for label in labels])
         labels = n_labels
-            
+
         # plot ranges for values
         for i in range(len(self.ordered_labels)):
             label = labels[i]
             theta = label_angles[i] * np.pi / 180
 
             r = 0.25
             lower, upper = self.value_ranges[self.ordered_labels[i]]
             text = round(r * (upper - lower) + lower, 2)
-            t = ax.text(theta + 0.2, r, text, fontsize=8, 
-                        ha=label.get_ha(), va=label.get_va())
+            t = ax.text(
+                theta + 0.2, r, text, fontsize=8, ha=label.get_ha(), va=label.get_va()
+            )
             t.set_rotation(label_angles[i] + 90)
 
             r = 0.75
             lower, upper = self.value_ranges[self.ordered_labels[i]]
             text = round(r * (upper - lower) + lower, 2)
-            t = ax.text(theta + 0.07, r, text, fontsize=8,
-                    ha=label.get_ha(), va=label.get_va())
+            t = ax.text(
+                theta + 0.07, r, text, fontsize=8, ha=label.get_ha(), va=label.get_va()
+            )
             t.set_rotation(label_angles[i] + 90)
 
 
 def plot(
     df: pd.DataFrame,
     label_column: str,
     value_column: str,
     hue_column: Optional[str] = None,
     value_ranges: Optional[Dict[str, List[float]]] = {},
     plot_labels: Optional[Dict[str, str]] = {},
     target_ranges: Optional[Dict[str, List[float]]] = {},
-    figsize: Optional[Tuple[float]] = (6.4, 4.8)
+    figsize: Optional[Tuple[float]] = (6.4, 4.8),
 ) -> Tuple[Figure, Union[List[Axes], Axes]]:
     return RadarPlot(
         df,
         label_column,
         value_column,
         hue_column,
         value_ranges,
         plot_labels,
         target_ranges,
-        figsize=figsize
+        figsize=figsize,
     ).plot()
```

### Comparing `radarplt-2.0.0/radarplt/factory.py` & `radarplt-2.0.1/radarplt/factory.py`

 * *Files identical despite different names*

### Comparing `radarplt-2.0.0/PKG-INFO` & `radarplt-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radarplt
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Home-page: https://github.com/jdkern11/radar_plot.git
 Author: jdkern11
 Author-email: josephdanielkern@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

