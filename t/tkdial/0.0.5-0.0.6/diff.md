# Comparing `tmp/tkdial-0.0.5.tar.gz` & `tmp/tkdial-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkdial-0.0.5.tar", last modified: Tue Apr 18 10:35:28 2023, max compression
+gzip compressed data, was "tkdial-0.0.6.tar", last modified: Wed Apr 19 12:03:37 2023, max compression
```

## Comparing `tkdial-0.0.5.tar` & `tkdial-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:35:28.326878 tkdial-0.0.5/
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 tkdial-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    16712 2023-04-18 10:35:28.326878 tkdial-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    16112 2023-04-18 10:34:41.000000 tkdial-0.0.5/README.md
--rw-rw-rw-   0        0        0      598 2023-04-18 10:35:28.342508 tkdial-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1133 2023-04-18 10:34:53.000000 tkdial-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:35:28.279989 tkdial-0.0.5/tkdial/
--rw-rw-rw-   0        0        0      381 2023-04-18 08:26:58.000000 tkdial-0.0.5/tkdial/__init__.py
--rw-rw-rw-   0        0        0    15120 2023-04-18 10:20:00.000000 tkdial-0.0.5/tkdial/jogwheel.py
--rw-rw-rw-   0        0        0    14988 2023-04-18 09:34:10.000000 tkdial-0.0.5/tkdial/meter.py
--rw-rw-rw-   0        0        0     9627 2023-04-18 09:33:53.000000 tkdial-0.0.5/tkdial/scrollknob.py
--rw-rw-rw-   0        0        0    17769 2023-04-18 09:34:03.000000 tkdial-0.0.5/tkdial/tkdial.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:35:28.311248 tkdial-0.0.5/tkdial.egg-info/
--rw-rw-rw-   0        0        0    16712 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       33 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 12:03:37.618637 tkdial-0.0.6/
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 tkdial-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    19517 2023-04-19 12:03:37.619217 tkdial-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    18917 2023-04-19 12:00:40.000000 tkdial-0.0.6/README.md
+-rw-rw-rw-   0        0        0      598 2023-04-19 12:03:37.620216 tkdial-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1179 2023-04-19 12:03:15.000000 tkdial-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:03:37.590552 tkdial-0.0.6/tkdial/
+-rw-rw-rw-   0        0        0      415 2023-04-19 08:59:42.000000 tkdial-0.0.6/tkdial/__init__.py
+-rw-rw-rw-   0        0        0     9266 2023-04-19 11:57:14.000000 tkdial-0.0.6/tkdial/imageknob.py
+-rw-rw-rw-   0        0        0    15120 2023-04-18 10:20:00.000000 tkdial-0.0.6/tkdial/jogwheel.py
+-rw-rw-rw-   0        0        0    14988 2023-04-18 09:34:10.000000 tkdial-0.0.6/tkdial/meter.py
+-rw-rw-rw-   0        0        0     9627 2023-04-18 09:33:53.000000 tkdial-0.0.6/tkdial/scrollknob.py
+-rw-rw-rw-   0        0        0    17769 2023-04-18 09:34:03.000000 tkdial-0.0.6/tkdial/tkdial.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:03:37.616793 tkdial-0.0.6/tkdial.egg-info/
+-rw-rw-rw-   0        0        0    19517 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       66 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/top_level.txt
```

### Comparing `tkdial-0.0.5/LICENSE` & `tkdial-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tkdial-0.0.5/PKG-INFO` & `tkdial-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tkdial
-Version: 0.0.5
-Summary: Rotatory dial-knob widgets for Tkinter.
-Home-page: https://github.com/Akascape/TkDial
-Author: Akascape
-License: Creative Commons Zero v1.0 Universal
-Keywords: tkinter,tkinter-dial,tkinter-widget,tkinter-knob,tkinter-meter,tkinter-dial-knob,dial-knob-widget,tkinter-gui
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # TkDial
 **This is a library containing some circular rotatory dial-knob widgets for Tkinter. It can be used in place of normal sliders and scale.**
 
 [![PyPI](https://img.shields.io/pypi/v/tkdial)](https://pypi.org/project/tkdial)
 ![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
 [![Downloads](https://static.pepy.tech/personalized-badge/tkdial?period=total&units=international_system&left_color=green&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tkdial)
 
@@ -119,15 +104,15 @@
   | _end_ |  The end point of the range |
   | _radius_ | Determines the distance of the unit lines between the center and the edge and also the length of the needle line |
   | _unit_length_ | Specify the length of the lines |
   | _unit_width_ | Specify the width of the lines |
   | _unit_color_ |  Specify the color of the unit lines |
   | _needle_color_ | Specify the color of the needle line |
   | _color_gradient_ | Specify which color gradient will be used for the units |
-  | _text_ | A string that will be displayed under the dial object |
+  | _text_ | A string that will be displayed under the dial object with value |
   | _text_color_ | Specify the color of the text that will be displayed under the dial object |
   | _text_font_ | Specify the font of the text that will be displayed under the dial object |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _scroll_ | A boolean (True/False), enables mouse scroll in dial (default=True) |
   | _scroll_steps_ | Number of steps per scroll |
   | _state_ | Specify the state of the needle |
   | _command_ | Call a function whenever the needle is rotated |
@@ -199,15 +184,15 @@
   | _width_ | Define width of the widget manually (optional) |
   | _height_ | Define height of the widget manually (optional) |
   | _start_ |  The start point of the range from where the bar will rotate |
   | _end_ |  The end point of the range |
   | _radius_ | Define the radius of the knob |
   | _border_width_ | Define the width of progress bar with respect to the outer and inner ring |
   | _start_angle_ | Determines the angle from where to rotate |
-  | _text_ | A string that will be displayed on the knob |
+  | _text_ | A string that will be displayed on the knob with value |
   | _text_color_ | Specify the color of the text that will be displayed on the knob |
   | _text_font_ | Specify the font of the text that will be displayed on the knob |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _fg_ | Specify the color of the inner circle |
   | _progress_color_ | Define the color of the progress bar |
   | _bar_color_ | Define the color of the progress bar's background |
   | _inner_width_ | Define the width of the inner ring |
@@ -293,15 +278,15 @@
   | _major_divisions_ | Determines the number of major lines in the scale |
   | _minor_divisions_ | Determines the number of minor lines in the scale |
   | _scale_color_ |  Specify the color of the meter scale |
   | _border_width_ | Define the width of the border case (default=1) |
   | _border_color_ |  Specify the color of the border case |
   | _needle_color_ | Specify the color of the needle line |
   | _axis_color_ | Specify which color of the axis wheel |
-  | _text_ | A string that will be displayed under the meter |
+  | _text_ | A string that will be displayed under the meter with value  |
   | _text_color_ | Specify the color of the text that will be displayed under the meter |
   | _text_font_ | Specify the font of the text that will be displayed under the meter |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _scroll_ | A boolean (True/False), enables mouse scroll in meter (default=True) |
   | _scroll_steps_ | Number of steps per scroll |
   | _state_ | Unbind/Bind the mouse movement with the needle |
   | _command_ | Call a function whenever the needle is rotated |
@@ -357,15 +342,15 @@
 ![Jogwheel styles](https://user-images.githubusercontent.com/89206401/232751129-72d29a4e-d0ea-49b4-9051-e65cabd5fb55.png)
 
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
-  | _bg_  | The default background color of the meter widget |
+  | _bg_  | The default background color of the widget |
   | _fg_ | Specify the color of the wheel face |
   | _width_ | Define width of the widget manually (optional) |
   | _height_ | Define height of the widget manually (optional) |
   | _start_ |  The start point of the range from where the knob will rotate |
   | _end_ |  The end point of the range |
   | _start_angle_ | Determines the starting angle of the arc |
   | _end_angle_ | Determines the final angle of the arc |
@@ -373,31 +358,102 @@
   | _divisions_ | Determines the number of scale lines in the scale |
   | _division_height_ | Determines the height of scale lines |
   | _scale_color_ |  Specify the color of the knob scale |
   | _border_width_ | Define the width of the border case (default=1) |
   | _border_color_ |  Specify the color of the border case |
   | _button_color_ | Specify the color of the knob |
   | _button_radius_ | Specify the radius the knob |
-  | _text_ | A string that will be displayed |
+  | _text_ | A string that will be displayed with value |
   | _text_color_ | Specify the color of the text that will be displayed |
   | _text_font_ | Specify the font of the text that will be displayed |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _scroll_ | A boolean (True/False), enables mouse scroll (default=True) |
   | _scroll_steps_ | Number of steps per scroll |
   | _state_ | Unbind/Bind the mouse movement with the widget |
   | _command_ | Call a function whenever the needle is rotated |
   
 ### Methods:
   | Methods   | Description |
   |-----------|-------------|
-  | _.get()_ | get the current value of the meter |
-  | _.set()_ | set the value of the meter |
-  | _.configure()_ | configure parameters of the meter| 
+  | _.get()_ | get the current value of the knob |
+  | _.set()_ | set the value of the knob |
+  | _.configure()_ | configure parameters of the knob | 
   | _.set_mark()_ | set markings for the scale. Eg: **meter.set_mark(from, to, color)** | 
   
-## Conclusion
-This library is focused to create some circular widgets that can be used with Tkinter easily.
-I hope it will be helpful for UI development in python.
+## ImageKnob
+### Usage
+```python
+import tkinter
+from tkdial import ImageKnob
+
+app = tkinter.Tk()
+
+customknob = ImageKnob(app, image="knob.png")
+customknob.grid()
 
-**Want to contribute?** See [this](https://github.com/Akascape/TkDial/discussions/1)
+app.mainloop()
+```
+
+![customknob](https://user-images.githubusercontent.com/89206401/233058156-007f967e-796c-40f1-9c91-419d990fb725.png)
+
+Styles:
+```python
+# Note: images are not provided, only for reference
+import customtkinter
+from tkdial import ImageKnob
+
+app = customtkinter.CTk()
+
+customknob = ImageKnob(app, image="knob.png", text_color="white", text="Volume ")
+customknob.grid(row=0, column=0)
+
+customknob2 = ImageKnob(app, image="knob2.png", scale_image="scale1.png",text="", scale_width=120)
+customknob2.grid(row=0, column=1, padx=20)
+
+customknob3 = ImageKnob(app, image="knob3.png", scale_image="scale2.png",text="",
+                        scale_width=50, start_angle=20, end_angle=-240,
+                        progress_color="cyan", progress=True)
+customknob3.grid(row=0, column=2)
+
+app.mainloop()
+```
+![customknob styles](https://user-images.githubusercontent.com/89206401/233058217-34888954-89dd-4e30-80ac-98f2d4bba6eb.png)
+
+
+## Arguments:
+  | Parameters  | Description |
+  | -------- | ----------- |
+  | _master_ | The master parameter is the parent widget |
+  | _bg_  | The default background color of the widget |
+  | _width_ | Define width of the widget manually (optional) |
+  | _height_ | Define height of the widget manually (optional) |
+  | _start_ |  The start point of the range from where the knob will rotate |
+  | _end_ |  The end point of the range |
+  | _image_ | pass the knob image |
+  | _scale_image_ | add a scale image (optional) |
+  | _scale_width_ | specify relative distance between scale and knob image |
+  | _start_angle_ | Determines the starting angle of the knob |
+  | _end_angle_ | Determines the final angle of the knob |
+  | _radius_ | Determines the radius for the widget |
+  | _text_ | A string that will be displayed with value |
+  | _text_color_ | Specify the color of the text that will be displayed |
+  | _text_font_ | Specify the font of the text that will be displayed |
+  | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
+  | _scroll_ | A boolean (True/False), enables mouse scroll (default=True) |
+  | _scroll_steps_ | Number of steps per scroll |
+  | _state_ | Unbind/Bind the mouse movement with the widget |
+  | _command_ | Call a function whenever the needle is rotated |
+  
+### Methods:
+  | Methods   | Description |
+  |-----------|-------------|
+  | _.get()_ | get the current value of the widget |
+  | _.set()_ | set the value of the widget |
+  | _.configure()_ | configure parameters of the widget | 
+
+Note: Images should be cropped in fixed ratio and saved with transparency(png).
+
+## Conclusion
+This library is focused to create some circular widgets that can be used with **Tkinter/Customtkinter** easily.
+I hope it will be helpful in UI development with python.
 
 [<img src="https://img.shields.io/badge/LICENSE-CC0_v0.1-informational?&color=blue&style=for-the-badge" width="200">](https://github.com/Akascape/TkDial/blob/main/LICENSE)
```

### Comparing `tkdial-0.0.5/README.md` & `tkdial-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: tkdial
+Version: 0.0.6
+Summary: Rotatory dial-knob widgets for Tkinter.
+Home-page: https://github.com/Akascape/TkDial
+Author: Akascape
+License: Creative Commons Zero v1.0 Universal
+Keywords: tkinter,tkinter-dial,tkinter-widget,tkinter-knob,tkinter-meter,tkinter-dial-knob,dial-knob-widget,tkinter-gui
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # TkDial
 **This is a library containing some circular rotatory dial-knob widgets for Tkinter. It can be used in place of normal sliders and scale.**
 
 [![PyPI](https://img.shields.io/pypi/v/tkdial)](https://pypi.org/project/tkdial)
 ![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
 [![Downloads](https://static.pepy.tech/personalized-badge/tkdial?period=total&units=international_system&left_color=green&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/tkdial)
 
@@ -104,15 +119,15 @@
   | _end_ |  The end point of the range |
   | _radius_ | Determines the distance of the unit lines between the center and the edge and also the length of the needle line |
   | _unit_length_ | Specify the length of the lines |
   | _unit_width_ | Specify the width of the lines |
   | _unit_color_ |  Specify the color of the unit lines |
   | _needle_color_ | Specify the color of the needle line |
   | _color_gradient_ | Specify which color gradient will be used for the units |
-  | _text_ | A string that will be displayed under the dial object |
+  | _text_ | A string that will be displayed under the dial object with value |
   | _text_color_ | Specify the color of the text that will be displayed under the dial object |
   | _text_font_ | Specify the font of the text that will be displayed under the dial object |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _scroll_ | A boolean (True/False), enables mouse scroll in dial (default=True) |
   | _scroll_steps_ | Number of steps per scroll |
   | _state_ | Specify the state of the needle |
   | _command_ | Call a function whenever the needle is rotated |
@@ -184,15 +199,15 @@
   | _width_ | Define width of the widget manually (optional) |
   | _height_ | Define height of the widget manually (optional) |
   | _start_ |  The start point of the range from where the bar will rotate |
   | _end_ |  The end point of the range |
   | _radius_ | Define the radius of the knob |
   | _border_width_ | Define the width of progress bar with respect to the outer and inner ring |
   | _start_angle_ | Determines the angle from where to rotate |
-  | _text_ | A string that will be displayed on the knob |
+  | _text_ | A string that will be displayed on the knob with value |
   | _text_color_ | Specify the color of the text that will be displayed on the knob |
   | _text_font_ | Specify the font of the text that will be displayed on the knob |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _fg_ | Specify the color of the inner circle |
   | _progress_color_ | Define the color of the progress bar |
   | _bar_color_ | Define the color of the progress bar's background |
   | _inner_width_ | Define the width of the inner ring |
@@ -278,15 +293,15 @@
   | _major_divisions_ | Determines the number of major lines in the scale |
   | _minor_divisions_ | Determines the number of minor lines in the scale |
   | _scale_color_ |  Specify the color of the meter scale |
   | _border_width_ | Define the width of the border case (default=1) |
   | _border_color_ |  Specify the color of the border case |
   | _needle_color_ | Specify the color of the needle line |
   | _axis_color_ | Specify which color of the axis wheel |
-  | _text_ | A string that will be displayed under the meter |
+  | _text_ | A string that will be displayed under the meter with value  |
   | _text_color_ | Specify the color of the text that will be displayed under the meter |
   | _text_font_ | Specify the font of the text that will be displayed under the meter |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _scroll_ | A boolean (True/False), enables mouse scroll in meter (default=True) |
   | _scroll_steps_ | Number of steps per scroll |
   | _state_ | Unbind/Bind the mouse movement with the needle |
   | _command_ | Call a function whenever the needle is rotated |
@@ -342,15 +357,15 @@
 ![Jogwheel styles](https://user-images.githubusercontent.com/89206401/232751129-72d29a4e-d0ea-49b4-9051-e65cabd5fb55.png)
 
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
-  | _bg_  | The default background color of the meter widget |
+  | _bg_  | The default background color of the widget |
   | _fg_ | Specify the color of the wheel face |
   | _width_ | Define width of the widget manually (optional) |
   | _height_ | Define height of the widget manually (optional) |
   | _start_ |  The start point of the range from where the knob will rotate |
   | _end_ |  The end point of the range |
   | _start_angle_ | Determines the starting angle of the arc |
   | _end_angle_ | Determines the final angle of the arc |
@@ -358,31 +373,102 @@
   | _divisions_ | Determines the number of scale lines in the scale |
   | _division_height_ | Determines the height of scale lines |
   | _scale_color_ |  Specify the color of the knob scale |
   | _border_width_ | Define the width of the border case (default=1) |
   | _border_color_ |  Specify the color of the border case |
   | _button_color_ | Specify the color of the knob |
   | _button_radius_ | Specify the radius the knob |
-  | _text_ | A string that will be displayed |
+  | _text_ | A string that will be displayed with value |
   | _text_color_ | Specify the color of the text that will be displayed |
   | _text_font_ | Specify the font of the text that will be displayed |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _scroll_ | A boolean (True/False), enables mouse scroll (default=True) |
   | _scroll_steps_ | Number of steps per scroll |
   | _state_ | Unbind/Bind the mouse movement with the widget |
   | _command_ | Call a function whenever the needle is rotated |
   
 ### Methods:
   | Methods   | Description |
   |-----------|-------------|
-  | _.get()_ | get the current value of the meter |
-  | _.set()_ | set the value of the meter |
-  | _.configure()_ | configure parameters of the meter| 
+  | _.get()_ | get the current value of the knob |
+  | _.set()_ | set the value of the knob |
+  | _.configure()_ | configure parameters of the knob | 
   | _.set_mark()_ | set markings for the scale. Eg: **meter.set_mark(from, to, color)** | 
   
-## Conclusion
-This library is focused to create some circular widgets that can be used with Tkinter easily.
-I hope it will be helpful for UI development in python.
+## ImageKnob
+### Usage
+```python
+import tkinter
+from tkdial import ImageKnob
+
+app = tkinter.Tk()
+
+customknob = ImageKnob(app, image="knob.png")
+customknob.grid()
 
-**Want to contribute?** See [this](https://github.com/Akascape/TkDial/discussions/1)
+app.mainloop()
+```
+
+![customknob](https://user-images.githubusercontent.com/89206401/233058156-007f967e-796c-40f1-9c91-419d990fb725.png)
+
+Styles:
+```python
+# Note: images are not provided, only for reference
+import customtkinter
+from tkdial import ImageKnob
+
+app = customtkinter.CTk()
+
+customknob = ImageKnob(app, image="knob.png", text_color="white", text="Volume ")
+customknob.grid(row=0, column=0)
+
+customknob2 = ImageKnob(app, image="knob2.png", scale_image="scale1.png",text="", scale_width=120)
+customknob2.grid(row=0, column=1, padx=20)
+
+customknob3 = ImageKnob(app, image="knob3.png", scale_image="scale2.png",text="",
+                        scale_width=50, start_angle=20, end_angle=-240,
+                        progress_color="cyan", progress=True)
+customknob3.grid(row=0, column=2)
+
+app.mainloop()
+```
+![customknob styles](https://user-images.githubusercontent.com/89206401/233058217-34888954-89dd-4e30-80ac-98f2d4bba6eb.png)
+
+
+## Arguments:
+  | Parameters  | Description |
+  | -------- | ----------- |
+  | _master_ | The master parameter is the parent widget |
+  | _bg_  | The default background color of the widget |
+  | _width_ | Define width of the widget manually (optional) |
+  | _height_ | Define height of the widget manually (optional) |
+  | _start_ |  The start point of the range from where the knob will rotate |
+  | _end_ |  The end point of the range |
+  | _image_ | pass the knob image |
+  | _scale_image_ | add a scale image (optional) |
+  | _scale_width_ | specify relative distance between scale and knob image |
+  | _start_angle_ | Determines the starting angle of the knob |
+  | _end_angle_ | Determines the final angle of the knob |
+  | _radius_ | Determines the radius for the widget |
+  | _text_ | A string that will be displayed with value |
+  | _text_color_ | Specify the color of the text that will be displayed |
+  | _text_font_ | Specify the font of the text that will be displayed |
+  | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
+  | _scroll_ | A boolean (True/False), enables mouse scroll (default=True) |
+  | _scroll_steps_ | Number of steps per scroll |
+  | _state_ | Unbind/Bind the mouse movement with the widget |
+  | _command_ | Call a function whenever the needle is rotated |
+  
+### Methods:
+  | Methods   | Description |
+  |-----------|-------------|
+  | _.get()_ | get the current value of the widget |
+  | _.set()_ | set the value of the widget |
+  | _.configure()_ | configure parameters of the widget | 
+
+Note: Images should be cropped in fixed ratio and saved with transparency(png).
+
+## Conclusion
+This library is focused to create some circular widgets that can be used with **Tkinter/Customtkinter** easily.
+I hope it will be helpful in UI development with python.
 
 [<img src="https://img.shields.io/badge/LICENSE-CC0_v0.1-informational?&color=blue&style=for-the-badge" width="200">](https://github.com/Akascape/TkDial/blob/main/LICENSE)
```

### Comparing `tkdial-0.0.5/setup.cfg` & `tkdial-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6b64 6961 6c0d 0a76 6572 7369   = tkdial..versi
-00000020: 6f6e 203d 2030 2e30 2e35 0d0a 6465 7363  on = 0.0.5..desc
+00000020: 6f6e 203d 2030 2e30 2e36 0d0a 6465 7363  on = 0.0.6..desc
 00000030: 7269 7074 696f 6e20 3d20 546b 696e 7465  ription = Tkinte
 00000040: 7220 4469 616c 2061 6e64 204b 6e6f 6220  r Dial and Knob 
 00000050: 5769 6467 6574 730d 0a6c 6f6e 675f 6465  Widgets..long_de
 00000060: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000070: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000080: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 00000090: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

### Comparing `tkdial-0.0.5/setup.py` & `tkdial-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'tkdial',
-    version = '0.0.5',
+    version = '0.0.6',
     description = "Rotatory dial-knob widgets for Tkinter.",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akascape',
     url = "https://github.com/Akascape/TkDial",
@@ -21,11 +21,11 @@
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     keywords = ['tkinter', 'tkinter-dial', 'tkinter-widget',
                 'tkinter-knob', 'tkinter-meter', 'tkinter-dial-knob',
                 'dial-knob-widget', 'tkinter-gui'],
     packages = ["tkdial"],
-    install_requires = ['colour'],
-    dependency_links = ['https://pypi.org/project/colour/'],
+    install_requires = ['colour', 'pillow'],
+    dependency_links = ['https://pypi.org/project/colour/', 'https://pypi.org/project/Pillow/'],
     python_requires = '>=3.6',
 )
```

### Comparing `tkdial-0.0.5/tkdial/jogwheel.py` & `tkdial-0.0.6/tkdial/jogwheel.py`

 * *Files identical despite different names*

### Comparing `tkdial-0.0.5/tkdial/meter.py` & `tkdial-0.0.6/tkdial/meter.py`

 * *Files identical despite different names*

### Comparing `tkdial-0.0.5/tkdial/scrollknob.py` & `tkdial-0.0.6/tkdial/scrollknob.py`

 * *Files identical despite different names*

### Comparing `tkdial-0.0.5/tkdial/tkdial.py` & `tkdial-0.0.6/tkdial/tkdial.py`

 * *Files identical despite different names*

### Comparing `tkdial-0.0.5/tkdial.egg-info/PKG-INFO` & `tkdial-0.0.6/tkdial.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkdial
-Version: 0.0.5
+Version: 0.0.6
 Summary: Rotatory dial-knob widgets for Tkinter.
 Home-page: https://github.com/Akascape/TkDial
 Author: Akascape
 License: Creative Commons Zero v1.0 Universal
 Keywords: tkinter,tkinter-dial,tkinter-widget,tkinter-knob,tkinter-meter,tkinter-dial-knob,dial-knob-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -119,15 +119,15 @@
   | _end_ |  The end point of the range |
   | _radius_ | Determines the distance of the unit lines between the center and the edge and also the length of the needle line |
   | _unit_length_ | Specify the length of the lines |
   | _unit_width_ | Specify the width of the lines |
   | _unit_color_ |  Specify the color of the unit lines |
   | _needle_color_ | Specify the color of the needle line |
   | _color_gradient_ | Specify which color gradient will be used for the units |
-  | _text_ | A string that will be displayed under the dial object |
+  | _text_ | A string that will be displayed under the dial object with value |
   | _text_color_ | Specify the color of the text that will be displayed under the dial object |
   | _text_font_ | Specify the font of the text that will be displayed under the dial object |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _scroll_ | A boolean (True/False), enables mouse scroll in dial (default=True) |
   | _scroll_steps_ | Number of steps per scroll |
   | _state_ | Specify the state of the needle |
   | _command_ | Call a function whenever the needle is rotated |
@@ -199,15 +199,15 @@
   | _width_ | Define width of the widget manually (optional) |
   | _height_ | Define height of the widget manually (optional) |
   | _start_ |  The start point of the range from where the bar will rotate |
   | _end_ |  The end point of the range |
   | _radius_ | Define the radius of the knob |
   | _border_width_ | Define the width of progress bar with respect to the outer and inner ring |
   | _start_angle_ | Determines the angle from where to rotate |
-  | _text_ | A string that will be displayed on the knob |
+  | _text_ | A string that will be displayed on the knob with value |
   | _text_color_ | Specify the color of the text that will be displayed on the knob |
   | _text_font_ | Specify the font of the text that will be displayed on the knob |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _fg_ | Specify the color of the inner circle |
   | _progress_color_ | Define the color of the progress bar |
   | _bar_color_ | Define the color of the progress bar's background |
   | _inner_width_ | Define the width of the inner ring |
@@ -293,15 +293,15 @@
   | _major_divisions_ | Determines the number of major lines in the scale |
   | _minor_divisions_ | Determines the number of minor lines in the scale |
   | _scale_color_ |  Specify the color of the meter scale |
   | _border_width_ | Define the width of the border case (default=1) |
   | _border_color_ |  Specify the color of the border case |
   | _needle_color_ | Specify the color of the needle line |
   | _axis_color_ | Specify which color of the axis wheel |
-  | _text_ | A string that will be displayed under the meter |
+  | _text_ | A string that will be displayed under the meter with value  |
   | _text_color_ | Specify the color of the text that will be displayed under the meter |
   | _text_font_ | Specify the font of the text that will be displayed under the meter |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _scroll_ | A boolean (True/False), enables mouse scroll in meter (default=True) |
   | _scroll_steps_ | Number of steps per scroll |
   | _state_ | Unbind/Bind the mouse movement with the needle |
   | _command_ | Call a function whenever the needle is rotated |
@@ -357,15 +357,15 @@
 ![Jogwheel styles](https://user-images.githubusercontent.com/89206401/232751129-72d29a4e-d0ea-49b4-9051-e65cabd5fb55.png)
 
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
-  | _bg_  | The default background color of the meter widget |
+  | _bg_  | The default background color of the widget |
   | _fg_ | Specify the color of the wheel face |
   | _width_ | Define width of the widget manually (optional) |
   | _height_ | Define height of the widget manually (optional) |
   | _start_ |  The start point of the range from where the knob will rotate |
   | _end_ |  The end point of the range |
   | _start_angle_ | Determines the starting angle of the arc |
   | _end_angle_ | Determines the final angle of the arc |
@@ -373,31 +373,102 @@
   | _divisions_ | Determines the number of scale lines in the scale |
   | _division_height_ | Determines the height of scale lines |
   | _scale_color_ |  Specify the color of the knob scale |
   | _border_width_ | Define the width of the border case (default=1) |
   | _border_color_ |  Specify the color of the border case |
   | _button_color_ | Specify the color of the knob |
   | _button_radius_ | Specify the radius the knob |
-  | _text_ | A string that will be displayed |
+  | _text_ | A string that will be displayed with value |
   | _text_color_ | Specify the color of the text that will be displayed |
   | _text_font_ | Specify the font of the text that will be displayed |
   | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
   | _scroll_ | A boolean (True/False), enables mouse scroll (default=True) |
   | _scroll_steps_ | Number of steps per scroll |
   | _state_ | Unbind/Bind the mouse movement with the widget |
   | _command_ | Call a function whenever the needle is rotated |
   
 ### Methods:
   | Methods   | Description |
   |-----------|-------------|
-  | _.get()_ | get the current value of the meter |
-  | _.set()_ | set the value of the meter |
-  | _.configure()_ | configure parameters of the meter| 
+  | _.get()_ | get the current value of the knob |
+  | _.set()_ | set the value of the knob |
+  | _.configure()_ | configure parameters of the knob | 
   | _.set_mark()_ | set markings for the scale. Eg: **meter.set_mark(from, to, color)** | 
   
-## Conclusion
-This library is focused to create some circular widgets that can be used with Tkinter easily.
-I hope it will be helpful for UI development in python.
+## ImageKnob
+### Usage
+```python
+import tkinter
+from tkdial import ImageKnob
+
+app = tkinter.Tk()
+
+customknob = ImageKnob(app, image="knob.png")
+customknob.grid()
+
+app.mainloop()
+```
+
+![customknob](https://user-images.githubusercontent.com/89206401/233058156-007f967e-796c-40f1-9c91-419d990fb725.png)
+
+Styles:
+```python
+# Note: images are not provided, only for reference
+import customtkinter
+from tkdial import ImageKnob
+
+app = customtkinter.CTk()
+
+customknob = ImageKnob(app, image="knob.png", text_color="white", text="Volume ")
+customknob.grid(row=0, column=0)
+
+customknob2 = ImageKnob(app, image="knob2.png", scale_image="scale1.png",text="", scale_width=120)
+customknob2.grid(row=0, column=1, padx=20)
+
+customknob3 = ImageKnob(app, image="knob3.png", scale_image="scale2.png",text="",
+                        scale_width=50, start_angle=20, end_angle=-240,
+                        progress_color="cyan", progress=True)
+customknob3.grid(row=0, column=2)
+
+app.mainloop()
+```
+![customknob styles](https://user-images.githubusercontent.com/89206401/233058217-34888954-89dd-4e30-80ac-98f2d4bba6eb.png)
+
+
+## Arguments:
+  | Parameters  | Description |
+  | -------- | ----------- |
+  | _master_ | The master parameter is the parent widget |
+  | _bg_  | The default background color of the widget |
+  | _width_ | Define width of the widget manually (optional) |
+  | _height_ | Define height of the widget manually (optional) |
+  | _start_ |  The start point of the range from where the knob will rotate |
+  | _end_ |  The end point of the range |
+  | _image_ | pass the knob image |
+  | _scale_image_ | add a scale image (optional) |
+  | _scale_width_ | specify relative distance between scale and knob image |
+  | _start_angle_ | Determines the starting angle of the knob |
+  | _end_angle_ | Determines the final angle of the knob |
+  | _radius_ | Determines the radius for the widget |
+  | _text_ | A string that will be displayed with value |
+  | _text_color_ | Specify the color of the text that will be displayed |
+  | _text_font_ | Specify the font of the text that will be displayed |
+  | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
+  | _scroll_ | A boolean (True/False), enables mouse scroll (default=True) |
+  | _scroll_steps_ | Number of steps per scroll |
+  | _state_ | Unbind/Bind the mouse movement with the widget |
+  | _command_ | Call a function whenever the needle is rotated |
+  
+### Methods:
+  | Methods   | Description |
+  |-----------|-------------|
+  | _.get()_ | get the current value of the widget |
+  | _.set()_ | set the value of the widget |
+  | _.configure()_ | configure parameters of the widget | 
+
+Note: Images should be cropped in fixed ratio and saved with transparency(png).
 
-**Want to contribute?** See [this](https://github.com/Akascape/TkDial/discussions/1)
+## Conclusion
+This library is focused to create some circular widgets that can be used with **Tkinter/Customtkinter** easily.
+I hope it will be helpful in UI development with python.
 
 [<img src="https://img.shields.io/badge/LICENSE-CC0_v0.1-informational?&color=blue&style=for-the-badge" width="200">](https://github.com/Akascape/TkDial/blob/main/LICENSE)
```

