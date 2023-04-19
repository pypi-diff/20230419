# Comparing `tmp/radarplt-1.1.0.tar.gz` & `tmp/radarplt-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radarplt-1.1.0.tar", max compression
+gzip compressed data, was "radarplt-2.0.0.tar", max compression
```

## Comparing `radarplt-1.1.0.tar` & `radarplt-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-04-18 18:40:56.926019 radarplt-1.1.0/LICENSE
--rw-r--r--   0        0        0     4749 2023-04-18 18:40:56.926223 radarplt-1.1.0/README.md
--rw-r--r--   0        0        0      504 2023-04-19 12:16:25.884076 radarplt-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    10356 2023-04-19 12:13:41.656876 radarplt-1.1.0/radarplt/__init__.py
--rw-r--r--   0        0        0     3782 2023-04-18 18:40:56.937136 radarplt-1.1.0/radarplt/factory.py
--rw-r--r--   0        0        0      327 2023-04-18 18:40:56.937259 radarplt-1.1.0/radarplt/helpers.py
--rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 radarplt-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-18 18:40:56.926019 radarplt-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4749 2023-04-18 18:40:56.926223 radarplt-2.0.0/README.md
+-rw-r--r--   0        0        0      504 2023-04-19 13:29:43.550605 radarplt-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11134 2023-04-19 13:30:27.196312 radarplt-2.0.0/radarplt/__init__.py
+-rw-r--r--   0        0        0     3782 2023-04-18 18:40:56.937136 radarplt-2.0.0/radarplt/factory.py
+-rw-r--r--   0        0        0      327 2023-04-18 18:40:56.937259 radarplt-2.0.0/radarplt/helpers.py
+-rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 radarplt-2.0.0/PKG-INFO
```

### Comparing `radarplt-1.1.0/LICENSE` & `radarplt-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radarplt-1.1.0/README.md` & `radarplt-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `radarplt-1.1.0/radarplt/__init__.py` & `radarplt-2.0.0/radarplt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
     def plot(self) -> Tuple[Figure, Union[List[Axes], Axes]]:
         fig, ax = plt.subplots(
             subplot_kw=dict(projection="radar"), dpi=300, figsize=self.figsize
         )
         self._plot_target_ranges(ax)
         self._plot_df(ax)
-        self._add_tick_labels(ax)
+        self._add_tick_labels(fig, ax)
 
         return (fig, ax)
 
     def _plot_target_ranges(self, ax):
         if len(self.target_ranges) == 0:
             return
         first = True  # only want to plot label with first target
@@ -219,38 +219,55 @@
                     r.append(val)
             r += [r[0]]
             theta += [theta[0]]
             ax.plot(theta, r, c=self.colors[curr_color], marker="o", label=hue)
             ax.fill(theta, r, facecolor=self.colors[curr_color], alpha=0.25)
             curr_color += 1
 
-    def _add_tick_labels(self, ax):
+    def _add_tick_labels(self, fig, ax):
         ax.set_rmax(1)
         ax.set_rticks(ticks=[0.25, 0.5, 0.75], labels=[])
         ax.grid(True)
         labels = [self.plot_labels[label] for label in self.ordered_labels]
         label_angles = [
             self.angles[label] * 180 / np.pi for label in self.ordered_labels
         ]
+
+        # rotation reset to 0 for polar coordinates, so we'll remove all xticks and
+        # just use the coordinates we get when we run thetagrids
         lines, labels = plt.thetagrids(label_angles, labels)
-        angle = np.deg2rad(67.5)
+        ax.set_xticks([])
+        n_labels = []
+        for i in range(len(labels)):
+            label = labels[i]
+            x, y = label.get_position()
+            lab = ax.text(x, y, label.get_text(), transform=label.get_transform(),
+                     ha=label.get_ha(), va=label.get_va())
+            lab.set_rotation(label_angles[i])
+            n_labels.append(lab)
+        labels = n_labels
+            
         # plot ranges for values
         for i in range(len(self.ordered_labels)):
-            offset = 0
-            theta = label_angles[i] * np.pi / 180 + offset
+            label = labels[i]
+            theta = label_angles[i] * np.pi / 180
 
             r = 0.25
             lower, upper = self.value_ranges[self.ordered_labels[i]]
             text = round(r * (upper - lower) + lower, 2)
-            plt.text(theta, r, text, fontsize=8)
+            t = ax.text(theta + 0.2, r, text, fontsize=8, 
+                        ha=label.get_ha(), va=label.get_va())
+            t.set_rotation(label_angles[i] + 90)
 
             r = 0.75
             lower, upper = self.value_ranges[self.ordered_labels[i]]
             text = round(r * (upper - lower) + lower, 2)
-            plt.text(theta, r, text, fontsize=8)
+            t = ax.text(theta + 0.07, r, text, fontsize=8,
+                    ha=label.get_ha(), va=label.get_va())
+            t.set_rotation(label_angles[i] + 90)
 
 
 def plot(
     df: pd.DataFrame,
     label_column: str,
     value_column: str,
     hue_column: Optional[str] = None,
```

### Comparing `radarplt-1.1.0/radarplt/factory.py` & `radarplt-2.0.0/radarplt/factory.py`

 * *Files identical despite different names*

### Comparing `radarplt-1.1.0/PKG-INFO` & `radarplt-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radarplt
-Version: 1.1.0
+Version: 2.0.0
 Summary: 
 Home-page: https://github.com/jdkern11/radar_plot.git
 Author: jdkern11
 Author-email: josephdanielkern@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

