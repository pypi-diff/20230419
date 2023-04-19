# Comparing `tmp/popupsort-1.5.3.tar.gz` & `tmp/popupsort-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popupsort-1.5.3.tar", last modified: Wed Apr 12 15:22:34 2023, max compression
+gzip compressed data, was "popupsort-1.6.tar", last modified: Wed Apr 19 15:02:26 2023, max compression
```

## Comparing `popupsort-1.5.3.tar` & `popupsort-1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 15:22:34.349575 popupsort-1.5.3/
--rw-rw-rw-   0        0        0     1093 2023-03-18 09:14:08.000000 popupsort-1.5.3/LICENSE.md
--rw-rw-rw-   0        0        0     2552 2023-04-12 15:22:34.349575 popupsort-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1785 2023-04-09 15:41:22.000000 popupsort-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 15:22:34.330513 popupsort-1.5.3/popupsort/
--rw-rw-rw-   0        0        0       74 2023-04-12 15:13:39.000000 popupsort-1.5.3/popupsort/__init__.py
--rw-rw-rw-   0        0        0    15518 2023-04-12 15:22:19.000000 popupsort-1.5.3/popupsort/popupsort.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:22:34.347581 popupsort-1.5.3/popupsort.egg-info/
--rw-rw-rw-   0        0        0     2552 2023-04-12 15:22:34.000000 popupsort-1.5.3/popupsort.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-04-12 15:22:34.000000 popupsort-1.5.3/popupsort.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 15:22:34.000000 popupsort-1.5.3/popupsort.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-18 09:46:14.000000 popupsort-1.5.3/popupsort.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-04-12 15:22:34.000000 popupsort-1.5.3/popupsort.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 15:22:34.350573 popupsort-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      574 2023-04-12 15:22:28.000000 popupsort-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:26.726255 popupsort-1.6/
+-rw-rw-rw-   0        0        0     1093 2023-03-18 09:14:08.000000 popupsort-1.6/LICENSE.md
+-rw-rw-rw-   0        0        0     3214 2023-04-19 15:02:26.726255 popupsort-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2345 2023-04-12 15:32:31.000000 popupsort-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:26.710294 popupsort-1.6/popupsort/
+-rw-rw-rw-   0        0        0       73 2023-04-19 14:34:25.000000 popupsort-1.6/popupsort/__init__.py
+-rw-rw-rw-   0        0        0    15983 2023-04-19 14:57:27.000000 popupsort-1.6/popupsort/popupsort.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:26.724233 popupsort-1.6/popupsort.egg-info/
+-rw-rw-rw-   0        0        0     3214 2023-04-19 15:02:26.000000 popupsort-1.6/popupsort.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-04-19 15:02:26.000000 popupsort-1.6/popupsort.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:02:26.000000 popupsort-1.6/popupsort.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-18 09:46:14.000000 popupsort-1.6/popupsort.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-04-19 15:02:26.000000 popupsort-1.6/popupsort.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:02:26.727224 popupsort-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      568 2023-04-19 15:01:23.000000 popupsort-1.6/setup.py
```

### Comparing `popupsort-1.5.3/LICENSE.md` & `popupsort-1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `popupsort-1.5.3/PKG-INFO` & `popupsort-1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: popupsort
-Version: 1.5.3
+Version: 1.6
 Summary: A Python package for visualizing sorting algorithms
 Home-page: https://github.com/ZouheirN/PopUpSort
 Author: Zouheir Nakouzi
 Author-email: zouheir2002@gmail.com
 License: MIT
 Description: # PopUpSort
         
         <p align="center">
         <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FZouheirN%2FPopUpSort&count_bg=%23FFD43B&title_bg=%23306998&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
         </p>
         
         With the assistance of ChatGPT-3.5, I was able to create this sorting visualizer. 
         
-        The PopUpSort package is a Python package that visualizes the sorting algorithms: bubble sort, selection sort, and insertion sort. The package uses the Tkinter library for the graphical user interface.
+        The PopUpSort package is a Python package that visualizes multiple sorting algorithms. The package uses the Tkinter library for the graphical user interface.
         
         # Requirements
         - Python 3.x
         - tkinter library (included in most Python installations)
         
         # Installation
         
@@ -38,30 +38,43 @@
         ```
         
         ### Syntax
         ```python
         pus.sort(array, algorithm, speed) # Sorting an already defined array
         
         pus.sort_rand(size, min, max, algorithm, speed) # Auto generate an array and sort it
+        
+        pus.sort_compare(array, algorithms, speed) # Compare sorting algorithms
+        
+        pus.sort_compare_rand(size, min, max, algorithms, speed) # Auto generate an array and compare sorting algorithms
         ```
         
         ### Algorithms
         
         Replace 'algorithm' argument with any of these options:
         - 'Bubble Sort' or 'b'
         - 'Selection Sort' or 's'
         - 'Insertion Sort' or 'i'
         - 'Quick Sort' or 'q'
         - 'Merge Sort' or 'm'
         - 'Heap Sort' or 'h'
         - 'Shell Sort' or 'sh'
         
+        For sorting comparision, replace 'algorithms' argument with a list of algorithms:
+        ```python
+        algorithms = ['b', 's', 'i', 'q', 'm', 'h', 'sh'] # You can remove any algorithms you don't want to compare
+        ```
+        
         ### Examples
         ```python
         arr = [60,24,21,65,93,56,35,10,55,49,86,76] # Define an array
         pus.sort(arr, 'b', 0.02)                    # Visualize the bubble sort of this array with a speed of 0.02s
         
         pus.sort_rand(50, 1, 100, 'i') # Generate an array of size 50 with elements ranging from 1 to 100 and sort it using insertion sort, speed is 0.01 by default
+        
+        pus.sort_compare(arr, ['s','i']) # Compare selection and insertion algorithms
+        
+        pus.sort_compare_rand(100, 1, 20, ['q','h','m']) # Generate an array and compare quick sort, heap sort, and merge sort
         ```
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,26 +1,33 @@
-Metadata-Version: 2.1 Name: popupsort Version: 1.5.3 Summary: A Python package
+Metadata-Version: 2.1 Name: popupsort Version: 1.6 Summary: A Python package
 for visualizing sorting algorithms Home-page: https://github.com/ZouheirN/
 PopUpSort Author: Zouheir Nakouzi Author-email: zouheir2002@gmail.com License:
 MIT Description: # PopUpSort
                  [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FZouheirN%2FPopUpSort&count_bg=%23FFD43B&title_bg=%23306998&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 With the assistance of ChatGPT-3.5, I was able to create this sorting
-visualizer. The PopUpSort package is a Python package that visualizes the
-sorting algorithms: bubble sort, selection sort, and insertion sort. The
-package uses the Tkinter library for the graphical user interface. #
-Requirements - Python 3.x - tkinter library (included in most Python
-installations) # Installation ### Method 1: Using pip ```python pip install
-popupsort ``` ### Method 2: Download the source code, then open terminal in the
-downloaded folder (where setup.py is) and run ```python pip install . ``` #
-Usage ### First import the package ```python import popupsort as pus ``` ###
-Syntax ```python pus.sort(array, algorithm, speed) # Sorting an already defined
-array pus.sort_rand(size, min, max, algorithm, speed) # Auto generate an array
-and sort it ``` ### Algorithms Replace 'algorithm' argument with any of these
-options: - 'Bubble Sort' or 'b' - 'Selection Sort' or 's' - 'Insertion Sort' or
-'i' - 'Quick Sort' or 'q' - 'Merge Sort' or 'm' - 'Heap Sort' or 'h' - 'Shell
-Sort' or 'sh' ### Examples ```python arr =
+visualizer. The PopUpSort package is a Python package that visualizes multiple
+sorting algorithms. The package uses the Tkinter library for the graphical user
+interface. # Requirements - Python 3.x - tkinter library (included in most
+Python installations) # Installation ### Method 1: Using pip ```python pip
+install popupsort ``` ### Method 2: Download the source code, then open
+terminal in the downloaded folder (where setup.py is) and run ```python pip
+install . ``` # Usage ### First import the package ```python import popupsort
+as pus ``` ### Syntax ```python pus.sort(array, algorithm, speed) # Sorting an
+already defined array pus.sort_rand(size, min, max, algorithm, speed) # Auto
+generate an array and sort it pus.sort_compare(array, algorithms, speed) #
+Compare sorting algorithms pus.sort_compare_rand(size, min, max, algorithms,
+speed) # Auto generate an array and compare sorting algorithms ``` ###
+Algorithms Replace 'algorithm' argument with any of these options: - 'Bubble
+Sort' or 'b' - 'Selection Sort' or 's' - 'Insertion Sort' or 'i' - 'Quick Sort'
+or 'q' - 'Merge Sort' or 'm' - 'Heap Sort' or 'h' - 'Shell Sort' or 'sh' For
+sorting comparision, replace 'algorithms' argument with a list of algorithms:
+```python algorithms = ['b', 's', 'i', 'q', 'm', 'h', 'sh'] # You can remove
+any algorithms you don't want to compare ``` ### Examples ```python arr =
 [60,24,21,65,93,56,35,10,55,49,86,76] # Define an array pus.sort(arr, 'b',
 0.02) # Visualize the bubble sort of this array with a speed of 0.02s
 pus.sort_rand(50, 1, 100, 'i') # Generate an array of size 50 with elements
 ranging from 1 to 100 and sort it using insertion sort, speed is 0.01 by
-default ``` Platform: UNKNOWN Description-Content-Type: text/markdown
+default pus.sort_compare(arr, ['s','i']) # Compare selection and insertion
+algorithms pus.sort_compare_rand(100, 1, 20, ['q','h','m']) # Generate an array
+and compare quick sort, heap sort, and merge sort ``` Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `popupsort-1.5.3/README.md` & `popupsort-1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FZouheirN%2FPopUpSort&count_bg=%23FFD43B&title_bg=%23306998&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 </p>
 
 With the assistance of ChatGPT-3.5, I was able to create this sorting visualizer. 
 
-The PopUpSort package is a Python package that visualizes the sorting algorithms: bubble sort, selection sort, and insertion sort. The package uses the Tkinter library for the graphical user interface.
+The PopUpSort package is a Python package that visualizes multiple sorting algorithms. The package uses the Tkinter library for the graphical user interface.
 
 # Requirements
 - Python 3.x
 - tkinter library (included in most Python installations)
 
 # Installation
 
@@ -30,27 +30,40 @@
 ```
 
 ### Syntax
 ```python
 pus.sort(array, algorithm, speed) # Sorting an already defined array
 
 pus.sort_rand(size, min, max, algorithm, speed) # Auto generate an array and sort it
+
+pus.sort_compare(array, algorithms, speed) # Compare sorting algorithms
+
+pus.sort_compare_rand(size, min, max, algorithms, speed) # Auto generate an array and compare sorting algorithms
 ```
 
 ### Algorithms
 
 Replace 'algorithm' argument with any of these options:
 - 'Bubble Sort' or 'b'
 - 'Selection Sort' or 's'
 - 'Insertion Sort' or 'i'
 - 'Quick Sort' or 'q'
 - 'Merge Sort' or 'm'
 - 'Heap Sort' or 'h'
 - 'Shell Sort' or 'sh'
 
+For sorting comparision, replace 'algorithms' argument with a list of algorithms:
+```python
+algorithms = ['b', 's', 'i', 'q', 'm', 'h', 'sh'] # You can remove any algorithms you don't want to compare
+```
+
 ### Examples
 ```python
 arr = [60,24,21,65,93,56,35,10,55,49,86,76] # Define an array
 pus.sort(arr, 'b', 0.02)                    # Visualize the bubble sort of this array with a speed of 0.02s
 
 pus.sort_rand(50, 1, 100, 'i') # Generate an array of size 50 with elements ranging from 1 to 100 and sort it using insertion sort, speed is 0.01 by default
+
+pus.sort_compare(arr, ['s','i']) # Compare selection and insertion algorithms
+
+pus.sort_compare_rand(100, 1, 20, ['q','h','m']) # Generate an array and compare quick sort, heap sort, and merge sort
 ```
```

#### html2text {}

```diff
@@ -1,23 +1,29 @@
 # PopUpSort
                  [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FZouheirN%2FPopUpSort&count_bg=%23FFD43B&title_bg=%23306998&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 With the assistance of ChatGPT-3.5, I was able to create this sorting
-visualizer. The PopUpSort package is a Python package that visualizes the
-sorting algorithms: bubble sort, selection sort, and insertion sort. The
-package uses the Tkinter library for the graphical user interface. #
-Requirements - Python 3.x - tkinter library (included in most Python
-installations) # Installation ### Method 1: Using pip ```python pip install
-popupsort ``` ### Method 2: Download the source code, then open terminal in the
-downloaded folder (where setup.py is) and run ```python pip install . ``` #
-Usage ### First import the package ```python import popupsort as pus ``` ###
-Syntax ```python pus.sort(array, algorithm, speed) # Sorting an already defined
-array pus.sort_rand(size, min, max, algorithm, speed) # Auto generate an array
-and sort it ``` ### Algorithms Replace 'algorithm' argument with any of these
-options: - 'Bubble Sort' or 'b' - 'Selection Sort' or 's' - 'Insertion Sort' or
-'i' - 'Quick Sort' or 'q' - 'Merge Sort' or 'm' - 'Heap Sort' or 'h' - 'Shell
-Sort' or 'sh' ### Examples ```python arr =
+visualizer. The PopUpSort package is a Python package that visualizes multiple
+sorting algorithms. The package uses the Tkinter library for the graphical user
+interface. # Requirements - Python 3.x - tkinter library (included in most
+Python installations) # Installation ### Method 1: Using pip ```python pip
+install popupsort ``` ### Method 2: Download the source code, then open
+terminal in the downloaded folder (where setup.py is) and run ```python pip
+install . ``` # Usage ### First import the package ```python import popupsort
+as pus ``` ### Syntax ```python pus.sort(array, algorithm, speed) # Sorting an
+already defined array pus.sort_rand(size, min, max, algorithm, speed) # Auto
+generate an array and sort it pus.sort_compare(array, algorithms, speed) #
+Compare sorting algorithms pus.sort_compare_rand(size, min, max, algorithms,
+speed) # Auto generate an array and compare sorting algorithms ``` ###
+Algorithms Replace 'algorithm' argument with any of these options: - 'Bubble
+Sort' or 'b' - 'Selection Sort' or 's' - 'Insertion Sort' or 'i' - 'Quick Sort'
+or 'q' - 'Merge Sort' or 'm' - 'Heap Sort' or 'h' - 'Shell Sort' or 'sh' For
+sorting comparision, replace 'algorithms' argument with a list of algorithms:
+```python algorithms = ['b', 's', 'i', 'q', 'm', 'h', 'sh'] # You can remove
+any algorithms you don't want to compare ``` ### Examples ```python arr =
 [60,24,21,65,93,56,35,10,55,49,86,76] # Define an array pus.sort(arr, 'b',
 0.02) # Visualize the bubble sort of this array with a speed of 0.02s
 pus.sort_rand(50, 1, 100, 'i') # Generate an array of size 50 with elements
 ranging from 1 to 100 and sort it using insertion sort, speed is 0.01 by
-default ```
+default pus.sort_compare(arr, ['s','i']) # Compare selection and insertion
+algorithms pus.sort_compare_rand(100, 1, 20, ['q','h','m']) # Generate an array
+and compare quick sort, heap sort, and merge sort ```
```

### Comparing `popupsort-1.5.3/popupsort/popupsort.py` & `popupsort-1.6/popupsort/popupsort.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import re
 import time
 from tkinter import *
 
 
 class SortingVisualizer:
     def __init__(self, arr, speed):
-
         if not isinstance(arr, list):
             raise TypeError("Input array must be a list")
 
         if speed < 0:
             raise ValueError("Speed must be a non-negative value")
 
         self.arr = arr
@@ -36,14 +35,16 @@
 
         self.time_label = Label(self.window, text="Elapsed Time: 0.000s", fg="black", font=("Helvetica", 16))
         self.time_label.pack(side=BOTTOM)
 
         if self.n == 0:
             raise ValueError("Cannot visualize an empty array")
 
+        self.isCompare = False
+
         self.draw_array(self.arr, color='blue')
         self.speed = speed
 
         self.start_time = time.time()
         self.timer_stopped = False
         self.update_timer()
 
@@ -211,39 +212,44 @@
                 merge(arr, l, m, r)
                 self.draw_array(self.arr, color='blue', highlight=list(range(l, r + 1)))
                 time.sleep(self.speed)
 
         merge_sort_helper(self.arr, 0, self.n - 1)
         self.completed()
 
-    def heapify(self, arr, n, i, highlight):
+    def heapify(self, n, i):
         largest = i
         left = 2 * i + 1
         right = 2 * i + 2
 
-        if left < n and arr[i] < arr[left]:
+        if left < n and self.arr[left] > self.arr[largest]:
             largest = left
 
-        if right < n and arr[largest] < arr[right]:
+        if right < n and self.arr[right] > self.arr[largest]:
             largest = right
 
         if largest != i:
-            arr[i], arr[largest] = arr[largest], arr[i]
-            self.heapify(arr, n, largest, highlight)
-            self.draw_array(arr, color='blue', highlight=highlight)
-
-    def heap_sort(self, arr):
-        n = len(arr)
-
-        for i in range(n, -1, -1):
-            self.heapify(arr, n, i, [])
-
-        for i in range(n - 1, 0, -1):
-            arr[0], arr[i] = arr[i], arr[0]
-            self.heapify(arr, i, 0, [i, 0])
+            self.arr[i], self.arr[largest] = self.arr[largest], self.arr[i]
+            self.draw_array(self.arr, color='blue', highlight=[i, largest])
+            time.sleep(self.speed)
+
+            self.heapify(n, largest)
+
+    def heap_sort(self):
+        for i in range(self.n // 2 - 1, -1, -1):
+            self.heapify(self.n, i)
+
+        for i in range(self.n - 1, 0, -1):
+            self.arr[0], self.arr[i] = self.arr[i], self.arr[0]
+            self.draw_array(self.arr, color='blue', highlight=[0, i])
+            time.sleep(self.speed)
+
+            self.heapify(i, 0)
+
+        self.completed()
 
     def shell_sort(self):
         gap = self.n // 2
 
         while gap > 0:
             for i in range(gap, self.n):
                 temp = self.arr[i]
@@ -258,19 +264,27 @@
             gap //= 2
 
         self.completed()
 
     def completed(self):
         self.timer_stopped = True
         self.draw_array(self.arr, color='green2')
-        self.window.mainloop()
+        if not self.isCompare:
+            self.window.mainloop()
+        else:
+            self.window.destroy()
+
+
+isCompare = False
 
 
 def sort(arr, algorithm, speed=0.01):
+    global isCompare
     sv = SortingVisualizer(arr, speed)
+    sv.isCompare = isCompare
 
     if algorithm.lower() == 'bubble sort' or algorithm.lower() == 'b':
         sv.label.config(text="Bubble Sort")
         sv.bubble_sort()
     elif algorithm.lower() == 'selection sort' or algorithm.lower() == 's':
         sv.label.config(text="Selection Sort")
         sv.selection_sort()
@@ -281,16 +295,15 @@
         sv.label.config(text="Quick Sort")
         sv.quick_sort()
     elif algorithm.lower() == 'merge sort' or algorithm.lower() == 'm':
         sv.label.config(text="Merge Sort")
         sv.merge_sort()
     elif algorithm.lower() == 'heap sort' or algorithm.lower() == 'h':
         sv.label.config(text="Heap Sort")
-        sv.heap_sort(arr)
-        sv.completed()
+        sv.heap_sort()
     elif algorithm.lower() == 'shell sort' or algorithm.lower() == 'sh':
         sv.label.config(text="Shell Sort")
         sv.shell_sort()
 
     return '%.3f' % sv.total_time + 's'
 
 
@@ -314,24 +327,25 @@
         sv.label.config(text="Quick Sort")
         sv.quick_sort()
     elif algorithm.lower() == 'merge sort' or algorithm.lower() == 'm':
         sv.label.config(text="Merge Sort")
         sv.merge_sort()
     elif algorithm.lower() == 'heap sort' or algorithm.lower() == 'h':
         sv.label.config(text="Heap Sort")
-        sv.heap_sort(arr)
-        sv.completed()
+        sv.heap_sort()
     elif algorithm.lower() == 'shell sort' or algorithm.lower() == 'sh':
         sv.label.config(text="Shell Sort")
         sv.shell_sort()
 
     return '%.3f' % sv.total_time + 's'
 
 
 def sort_compare(arr, algorithms, speed=0.01):
+    global isCompare
+    isCompare = True
     arr_copy = []
 
     for i in range(len(algorithms)):
         arr_copy.append(arr.copy())
 
     sv = []
 
@@ -376,17 +390,20 @@
         text = Label(frame, text=sv[i], font=("Helvetica", 12))
         text.pack(side="bottom")
 
         frame2 = Frame(frame, width=100, height=100)
         frame2.pack()
 
     window.mainloop()
+    isCompare = False
 
 
 def sort_compare_rand(size, min, max, algorithms, speed=0.01):
+    global isCompare
+    isCompare = True
     arr = []
     for i in range(size):
         arr.append(random.randint(min, max))
 
     arr_copy = []
 
     for i in range(len(algorithms)):
@@ -434,8 +451,9 @@
 
         text = Label(frame, text=sv[i], font=("Helvetica", 12))
         text.pack(side="bottom")
 
         frame2 = Frame(frame, width=100, height=100)
         frame2.pack()
 
-    window.mainloop()
+    window.mainloop()
+    isCompare = False
```

### Comparing `popupsort-1.5.3/popupsort.egg-info/PKG-INFO` & `popupsort-1.6/popupsort.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: popupsort
-Version: 1.5.3
+Version: 1.6
 Summary: A Python package for visualizing sorting algorithms
 Home-page: https://github.com/ZouheirN/PopUpSort
 Author: Zouheir Nakouzi
 Author-email: zouheir2002@gmail.com
 License: MIT
 Description: # PopUpSort
         
         <p align="center">
         <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FZouheirN%2FPopUpSort&count_bg=%23FFD43B&title_bg=%23306998&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
         </p>
         
         With the assistance of ChatGPT-3.5, I was able to create this sorting visualizer. 
         
-        The PopUpSort package is a Python package that visualizes the sorting algorithms: bubble sort, selection sort, and insertion sort. The package uses the Tkinter library for the graphical user interface.
+        The PopUpSort package is a Python package that visualizes multiple sorting algorithms. The package uses the Tkinter library for the graphical user interface.
         
         # Requirements
         - Python 3.x
         - tkinter library (included in most Python installations)
         
         # Installation
         
@@ -38,30 +38,43 @@
         ```
         
         ### Syntax
         ```python
         pus.sort(array, algorithm, speed) # Sorting an already defined array
         
         pus.sort_rand(size, min, max, algorithm, speed) # Auto generate an array and sort it
+        
+        pus.sort_compare(array, algorithms, speed) # Compare sorting algorithms
+        
+        pus.sort_compare_rand(size, min, max, algorithms, speed) # Auto generate an array and compare sorting algorithms
         ```
         
         ### Algorithms
         
         Replace 'algorithm' argument with any of these options:
         - 'Bubble Sort' or 'b'
         - 'Selection Sort' or 's'
         - 'Insertion Sort' or 'i'
         - 'Quick Sort' or 'q'
         - 'Merge Sort' or 'm'
         - 'Heap Sort' or 'h'
         - 'Shell Sort' or 'sh'
         
+        For sorting comparision, replace 'algorithms' argument with a list of algorithms:
+        ```python
+        algorithms = ['b', 's', 'i', 'q', 'm', 'h', 'sh'] # You can remove any algorithms you don't want to compare
+        ```
+        
         ### Examples
         ```python
         arr = [60,24,21,65,93,56,35,10,55,49,86,76] # Define an array
         pus.sort(arr, 'b', 0.02)                    # Visualize the bubble sort of this array with a speed of 0.02s
         
         pus.sort_rand(50, 1, 100, 'i') # Generate an array of size 50 with elements ranging from 1 to 100 and sort it using insertion sort, speed is 0.01 by default
+        
+        pus.sort_compare(arr, ['s','i']) # Compare selection and insertion algorithms
+        
+        pus.sort_compare_rand(100, 1, 20, ['q','h','m']) # Generate an array and compare quick sort, heap sort, and merge sort
         ```
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,26 +1,33 @@
-Metadata-Version: 2.1 Name: popupsort Version: 1.5.3 Summary: A Python package
+Metadata-Version: 2.1 Name: popupsort Version: 1.6 Summary: A Python package
 for visualizing sorting algorithms Home-page: https://github.com/ZouheirN/
 PopUpSort Author: Zouheir Nakouzi Author-email: zouheir2002@gmail.com License:
 MIT Description: # PopUpSort
                  [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FZouheirN%2FPopUpSort&count_bg=%23FFD43B&title_bg=%23306998&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 With the assistance of ChatGPT-3.5, I was able to create this sorting
-visualizer. The PopUpSort package is a Python package that visualizes the
-sorting algorithms: bubble sort, selection sort, and insertion sort. The
-package uses the Tkinter library for the graphical user interface. #
-Requirements - Python 3.x - tkinter library (included in most Python
-installations) # Installation ### Method 1: Using pip ```python pip install
-popupsort ``` ### Method 2: Download the source code, then open terminal in the
-downloaded folder (where setup.py is) and run ```python pip install . ``` #
-Usage ### First import the package ```python import popupsort as pus ``` ###
-Syntax ```python pus.sort(array, algorithm, speed) # Sorting an already defined
-array pus.sort_rand(size, min, max, algorithm, speed) # Auto generate an array
-and sort it ``` ### Algorithms Replace 'algorithm' argument with any of these
-options: - 'Bubble Sort' or 'b' - 'Selection Sort' or 's' - 'Insertion Sort' or
-'i' - 'Quick Sort' or 'q' - 'Merge Sort' or 'm' - 'Heap Sort' or 'h' - 'Shell
-Sort' or 'sh' ### Examples ```python arr =
+visualizer. The PopUpSort package is a Python package that visualizes multiple
+sorting algorithms. The package uses the Tkinter library for the graphical user
+interface. # Requirements - Python 3.x - tkinter library (included in most
+Python installations) # Installation ### Method 1: Using pip ```python pip
+install popupsort ``` ### Method 2: Download the source code, then open
+terminal in the downloaded folder (where setup.py is) and run ```python pip
+install . ``` # Usage ### First import the package ```python import popupsort
+as pus ``` ### Syntax ```python pus.sort(array, algorithm, speed) # Sorting an
+already defined array pus.sort_rand(size, min, max, algorithm, speed) # Auto
+generate an array and sort it pus.sort_compare(array, algorithms, speed) #
+Compare sorting algorithms pus.sort_compare_rand(size, min, max, algorithms,
+speed) # Auto generate an array and compare sorting algorithms ``` ###
+Algorithms Replace 'algorithm' argument with any of these options: - 'Bubble
+Sort' or 'b' - 'Selection Sort' or 's' - 'Insertion Sort' or 'i' - 'Quick Sort'
+or 'q' - 'Merge Sort' or 'm' - 'Heap Sort' or 'h' - 'Shell Sort' or 'sh' For
+sorting comparision, replace 'algorithms' argument with a list of algorithms:
+```python algorithms = ['b', 's', 'i', 'q', 'm', 'h', 'sh'] # You can remove
+any algorithms you don't want to compare ``` ### Examples ```python arr =
 [60,24,21,65,93,56,35,10,55,49,86,76] # Define an array pus.sort(arr, 'b',
 0.02) # Visualize the bubble sort of this array with a speed of 0.02s
 pus.sort_rand(50, 1, 100, 'i') # Generate an array of size 50 with elements
 ranging from 1 to 100 and sort it using insertion sort, speed is 0.01 by
-default ``` Platform: UNKNOWN Description-Content-Type: text/markdown
+default pus.sort_compare(arr, ['s','i']) # Compare selection and insertion
+algorithms pus.sort_compare_rand(100, 1, 20, ['q','h','m']) # Generate an array
+and compare quick sort, heap sort, and merge sort ``` Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `popupsort-1.5.3/setup.py` & `popupsort-1.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name='popupsort',
-    version='1.5.3',
+    version='1.6',
     description='A Python package for visualizing sorting algorithms',
-    long_description = README,
+    long_description=README,
     long_description_content_type="text/markdown",
     author='Zouheir Nakouzi',
     author_email='zouheir2002@gmail.com',
     url='https://github.com/ZouheirN/PopUpSort',
     packages=['popupsort'],
     license='MIT',
-    license_files = ('LICENSE.md',),
+    license_files=('LICENSE.md',),
     zip_safe=False
 )
```

