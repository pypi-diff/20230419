# Comparing `tmp/vinset-3.0.5.tar.gz` & `tmp/vinset-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinset-3.0.5.tar", last modified: Sun Jul 10 23:51:55 2022, max compression
+gzip compressed data, was "vinset-4.0.0.tar", last modified: Wed Apr 19 03:12:48 2023, max compression
```

## Comparing `vinset-3.0.5.tar` & `vinset-4.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-07-10 23:51:55.872561 vinset-3.0.5/
--rw-rw-rw-   0        0        0    11558 2021-07-06 03:24:06.000000 vinset-3.0.5/LICENSE
--rw-rw-rw-   0        0        0      581 2022-07-10 23:51:55.871559 vinset-3.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6759 2022-07-08 10:54:31.000000 vinset-3.0.5/README.md
--rw-rw-rw-   0        0        0       42 2022-07-10 23:51:55.873554 vinset-3.0.5/setup.cfg
--rw-rw-rw-   0        0        0      983 2022-07-10 23:51:09.000000 vinset-3.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-10 23:51:55.847623 vinset-3.0.5/vinset/
--rw-rw-rw-   0        0        0        0 2021-07-05 23:17:38.000000 vinset-3.0.5/vinset/__init__.py
--rw-rw-rw-   0        0        0    42544 2022-07-10 23:51:09.000000 vinset-3.0.5/vinset/vin.py
-drwxrwxrwx   0        0        0        0 2022-07-10 23:51:55.869571 vinset-3.0.5/vinset.egg-info/
--rw-rw-rw-   0        0        0      581 2022-07-10 23:51:55.000000 vinset-3.0.5/vinset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2022-07-10 23:51:55.000000 vinset-3.0.5/vinset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-10 23:51:55.000000 vinset-3.0.5/vinset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-07-10 23:51:55.000000 vinset-3.0.5/vinset.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-08-03 04:08:55.000000 vinset-3.0.5/vinset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2022-07-10 23:51:55.000000 vinset-3.0.5/vinset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-07-10 23:51:55.000000 vinset-3.0.5/vinset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 03:12:48.343947 vinset-4.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-03-26 20:05:51.000000 vinset-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0      560 2023-04-19 03:12:48.343947 vinset-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6863 2023-03-26 20:05:51.000000 vinset-4.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 03:12:48.343947 vinset-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-04-17 21:29:38.000000 vinset-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 03:12:48.329933 vinset-4.0.0/vinset/
+-rw-rw-rw-   0        0        0        0 2023-03-26 20:05:52.000000 vinset-4.0.0/vinset/__init__.py
+-rw-rw-rw-   0        0        0    54148 2023-04-19 03:09:32.000000 vinset-4.0.0/vinset/vin.py
+drwxrwxrwx   0        0        0        0 2023-04-19 03:12:48.329933 vinset-4.0.0/vinset.egg-info/
+-rw-rw-rw-   0        0        0      560 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-19 03:11:11.000000 vinset-4.0.0/vinset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/top_level.txt
```

### Comparing `vinset-3.0.5/LICENSE` & `vinset-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vinset-3.0.5/PKG-INFO` & `vinset-4.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 3.0.5
+Version: 4.0.0
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Command line program to draw the graph from video and csv files.
-
```

### Comparing `vinset-3.0.5/README.md` & `vinset-4.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -87,99 +87,92 @@
 5, 10.4, 2.321, 0.2442
 5, 10.5, 2.324, 0.679
 ```
 DataID column is optional but it can be filter by given config file.
 
 
 ## Example configuration file
-
+### pim_video_middle.json
 ```
-{"csv_data" : "data.csv",
-  "display": "True",
+{ "display": "True",
   "axes" : [ {  "name" : "main",
-                "box_title": "Left",
-                "box_title_font_scale": 0.8,
+                "box_title": "Pupil movement",
+                "box_title_x_position": 70,
+                "box_title_y_position": 20,
+                "box_title_color": "red",
+                "box_title_font_scale": 0.4,
                 "box_color": "red",
-                "box_thickness": "2",
-                "background" : { "fill":"black", "opacity" : 0.1 },
-                "position" :  { "x" : 100, "y" : 100, "width" : 500, "height" : 250 } } ],
-  "series" : [ { "name"  : "displacement",
+                "box_thickness": "1",
+                "background" : { "fill":"black", "opacity" : 0.3 },
+                "position" :  { "x" : 65, "y" : 56, "width" : 250, "height" : 80 } }],
+  "series" : [ { "name"  : "x_nom_graph_line",
                 "parent_axes" : "main",
                 "line_color": "green",
-                "line_thickness": 2,
-                "zero_line_display": "True",
+                "line_thickness": 1,
+                "zero_line_display": "False",
                 "zero_line_thickness": 1,
-                "display_type": "pen",
-                "t_label"     : "CurrentTime",
-                "y_label"     : "D / V",
+                "display_type": "static",
+                "t_label"     : "time",
+                "t_label_x_position"     : 112,
+                "t_label_y_position"     : 100,
+                "time_offset": -0.09578,
+                "y_label"     : "x_nom",
+                "y_label_x_position"     : 15,
+                "y_label_y_position"     : 125,
                 "label_thickness": 1,
-                "label_font_scale": 0.6,
-                "t_data": "record_timestamp",
-                "y_data": "y_nom",
-                "filter": "FaLSE",
-                "filterBy" : "DataID=2",
-                "pointer_value": {"Enabled": "True", "Color": "red", "Radius": 4},
-                "y-limit" : { "type" : "fixed", "limits" : { "lower" : -1, "upper" : 2 } },
-                "t-limit" : { "type" : "time",  "width" : 10 }},
-                { "name"  : "velocity",
-                "parent_axes" : "main",
-                  "line_color": "magenta",
-                  "line_thickness": 1,
-                  "zero_line_display": "True",
-                "zero_line_thickness": 1,
-                "display_type": "refresh",
-                "t_label"     : "CurrentTime",
-                "y_label"     : "D / V",
-                  "label_thickness": 1,
-                  "label_font_scale": 0.6,
-                  "t_data": "record_timestamp",
-                "y_data": "y_value",
-                  "filter": "False",
-                "filterBy" : "DataID=5",
-                  "pointer_value": {"Enabled": "True", "Color": "red", "Radius": 4},
-                "y-limit" : { "type" : "fixed", "limits" : { "lower" : -100, "upper" : 100 } },
+                "label_font_scale": 0.4,
+                "t_data": "local_time",
+                "y_data": "x_nom",
+                "filter": "False",
+                "filterBy" : "None",
+                "pointer_value": {"Enabled": "True", "Color": "red", "Radius": 3},
+                "y-limit" : { "type" : "fixed", "limits" : { "lower" : 0.3, "upper" : 0.6 } },
                 "t-limit" : { "type" : "time",  "width" : 10 }}]}
 ```
 ## Configuration format explanation
-### csv_data = input csv file.
 
 ### display = video will be displayed during producing video if it is true.
 
 ### axes = the information of graph boxes.
 
 1.  name = the name of the axes that will be checked from series information.
-2.  box_title = the name of the graph box.
-3.  box_title_font_scale = the font scale of tile
-4.  box_color = the color of the box.
-5.  box_thickess = the thickness of line of box.
-6.  background = the color and opacity of background rectangle box.
-7.  position = x, y coordinates, width and height information of the box.
+2.  box_title = the title of the graph box.
+3.  box_title_x_position = the x position of title
+4.  box_title_y_position = the y position of title
+5.  box_title_color = the color of tile
+6.  box_title_font_scale = the font scale of tile
+7.  box_color = the color of the box.
+8.  box_thickess = the thickness of line of box.
+9.  background = the color and opacity of background rectangle box.
+10.  position = x cordinate, y coordinate, width and height of the box.
 
 ### series = the information of labels and lines.
 
 1.  name = the name or type of line.
 2.  parent_axes = the name of parent axes to be called.
 3.  line_color = the color of data line.
 4.  line_thickness = the color of data line thickess.
 5.  zero_line_display = the zero level line will be displayed if it is true and it is actually within lower and upper limit.
 6.  zero_line_thickess = the thickess of zero line
 7.  display_type = the display type of line. It can be "pen" or "static". If it is "pen", it will be drawn with time. If it is "static", the whole line will be displayed within time scale.
 8.  t_label = the label name for time/x axis.
-9.  y_label = the label name of y axis.
-10.  y_label_x = the x axis offset position of "y_label".
-11.  y_label_y = the y axis offset position of "y_label".
-12.  label_thickess = the thickess of label.
-13.  label_font_scale = the font scale of label.
-14.  t_data = the column name of csv file for time/ x axis data.
-15.  y_data = the column name of csv file for y axis data
-16.  filter = it will filter "DataID" column if it is true.
-17.  filterBy = the column name of csv file and the value to be used to filter. eg. "DataID=4"
-18.  pointer_value = the color and radius information of pointer whether it is enabled or not.
-19.  y-limit = type and limits of y axis
-20.  t-limit = type and width of time/x axis
+9.  t_label_x_position = x position of the time label. The bigger the number, the closer to the right of the graph box.
+10. t_label_y_position = y position of the time label. The bigger the number, the closer to the bottom of the the graph box.
+11. time_offset = time difference in milliseconds between start time of gaze.csv and left_right_combined.video. (This `time_offset` is optional and if it is not included, it will be zero.)
+12.  y_label_x_position = x position of the y label. The bigger the number, the closer to the left of the graph box.
+13. y_label_y_position = y position of the y label. The bigger the number, the closer to the top of the the graph box.
+14.  label_thickess = the thickess of label.
+15.  label_font_scale = the font scale of label.
+16.  t_data = the column name of csv file for time/ x axis data.
+17.  y_data = the column name of csv file for y axis data
+18.  filter = it will filter "DataID" column if it is true.
+19.  filterBy = the column name of csv file and the value to be used to filter. eg. "DataID=4"
+20.  pointer_value = the color and radius information of pointer whether it is enabled or not.
+21.  y-limit = type and limits of y axis
+22.  t-limit = type and width of time/x axis
 
 ### Note: 
 1.  Color information can be tuple string eg. "(0,0,255)" or 6 hex color code eg. "#ffffff" or basic color strings which are "red", "green", "blue", "yellow", "black", "white" and "magenta".
 2.  Zero line will be displayed if it is enabled and it is actually can be drawn according to the lower limit and upper limit. eg. If lower limit is 1 and upper limit is 2, zero line cannot be drawn.
 
 _________________________________
 # Version upgrade guide
```

### Comparing `vinset-3.0.5/setup.py` & `vinset-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw the graph from video and csv files.'
 
 setup(
     name='vinset',
-    version='3.0.5',
+    version='4.0.0',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/vinset',
     description='gaze visualisation program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

### Comparing `vinset-3.0.5/vinset/vin.py` & `vinset-4.0.0/vinset/vin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import json
+import os.path
+
 import cv2
 import csv
 import time
 import numpy as np
 import sys
 import math
 import argparse
@@ -254,67 +256,21 @@
             total_value += d[1]
         avg_time = total_time / length_array
         avg_value = total_value / length_array
         val = [avg_time, avg_value]
         return val
 
 
-def main():
-    parser = argparse.ArgumentParser(prog='vinset', description='VINSET package.')
-    parser.add_argument('--version', action='version', version='3.0.5'),
-    parser.add_argument("-i", dest="input_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
-                        help="input mp4 file", metavar="filename.mp4")
-    parser.add_argument("-d", dest="input_data_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
-                        help="input csv data file", metavar="filename.csv")
-    parser.add_argument("-o", dest="output_filename", required=True, type=argparse.FileType('w'), default=sys.stdout,
-                        help="output mp4 file", metavar="filename.mp4")
-    parser.add_argument("-c", dest="config_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
-                        help="config json file", metavar="filename.json")
-
-    # get all input name in string
-    args = parser.parse_args()
-    input_file = args.input_filename.name
-    csv_data = args.input_data_filename.name
-    output_file = args.output_filename.name
-    config_file = args.config_filename.name
-
-    # start whether the inputs are in correct types or not
-    if str(input_file).endswith(".mp4"):
-        print("Input file name:", input_file)
-    else:
-        print("Input file must be mp4.")
-    if str(csv_data).endswith(".csv"):
-        print("Input data file name:", csv_data)
-    else:
-        print("Input data file must be csv.")
-    if str(output_file).endswith(".mp4"):
-        print("Output file name:", output_file)
-    else:
-        print("Output file must be mp4.")
-    if str(config_file).endswith(".json"):
-        print("Config file name:", config_file)
-    else:
-        print("Config file must be json.")
-
-    data = None
-    draw_able = True
-    try:
-        f = open(config_file)
-        data = json.load(f)
-        print(f"{config_file} is loaded successfully by json.")
-    except ValueError:
-        draw_able = False
-        print(f"{config_file} cannot be loaded by json.")
-
-    if draw_able and data:
-        axes_array = data["axes"]
-        series_array = data["series"]
-        display_able = str_to_bool(str(data["display"]))
+def overlay_graph(draw_able_input, config_info_input, input_video_file, csv_data_to_be_used, output_video_file):
+    if draw_able_input and config_info_input:
+        axes_array = config_info_input["axes"]
+        series_array = config_info_input["series"]
+        display_able = str_to_bool(str(config_info_input["display"]))
 
-        input_video = cv2.VideoCapture(input_file)
+        input_video = cv2.VideoCapture(input_video_file)
         frame_width = input_video.get(cv2.CAP_PROP_FRAME_WIDTH)
         print("Frame width:", frame_width)
         frame_height = input_video.get(cv2.CAP_PROP_FRAME_HEIGHT)
         print("Frame height:", frame_height)
         frame_rate = input_video.get(cv2.CAP_PROP_FPS)
         print("Frame rate:", frame_rate)
         frame_count = input_video.get(cv2.CAP_PROP_FRAME_COUNT)
@@ -350,17 +306,17 @@
                 info_filter = str_to_bool(str(info["filter"]))
                 filter_by = None
                 if info_filter:
                     filter_by = info["filterBy"]
                 if str(display_type).lower() == "pen":
                     # getting data from csv with or without filter
                     if info_filter:
-                        data_arr = get_data_array(csv_data, t_data, y_data, t_offset, info_filter, filter_by)
+                        data_arr = get_data_array(csv_data_to_be_used, t_data, y_data, t_offset, info_filter, filter_by)
                     else:
-                        data_arr = get_data_array(csv_data, t_data, y_data, t_offset)
+                        data_arr = get_data_array(csv_data_to_be_used, t_data, y_data, t_offset)
                     series_data_array = []
                     # calculate the max duration of time can be displayed in one pixel
                     time_interval_for_data = round(1000 / (axes_pos_w / t_w), 4)
                     # calculate how many display for the whole video
                     number_of_time_interval = math.ceil(max_video_length / time_interval_for_data)
                     # lower range starts with 0 and upper range starts with milliseconds
                     # calculated from time interval for data
@@ -392,17 +348,17 @@
                         upper_range = round((upper_range + time_interval_for_data), 2)
                     draw_data_array.append({"series_name": series_name, "display_type": display_type,
                                             "series_data_array": series_data_array})
 
                 elif str(display_type).lower() == "static":
                     # getting data from csv with or without filter
                     if info_filter:
-                        data_arr = get_data_array(csv_data, t_data, y_data, t_offset, info_filter, filter_by)
+                        data_arr = get_data_array(csv_data_to_be_used, t_data, y_data, t_offset, info_filter, filter_by)
                     else:
-                        data_arr = get_data_array(csv_data, t_data, y_data, t_offset)
+                        data_arr = get_data_array(csv_data_to_be_used, t_data, y_data, t_offset)
                     series_data_array = []
                     # calculate the max duration of time can be displayed in one pixel
                     time_interval_for_data = round(1000 / (axes_pos_w / t_w), 4)
                     # calculate how many display for the whole video
                     number_of_time_interval = math.ceil(max_video_length / time_interval_for_data)
                     # lower range starts with 0 and upper range starts with milliseconds
                     # calculated from time interval for data
@@ -511,15 +467,15 @@
                              (axes_pos_x + space_value,
                               axes_pos_h + axes_pos_y - height_of_scale),
                              box_color, box_thickness)
                 # after this points, the raw black image is filled with
                 # all graphs and labels
 
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
-        v_writer = cv2.VideoWriter(output_file, fourcc, int(frame_rate), (int(frame_width), int(frame_height)))
+        v_writer = cv2.VideoWriter(output_video_file, fourcc, int(frame_rate), (int(frame_width), int(frame_height)))
         whole_t = time.time()
         count = 0
         drawing_graph = True
 
         while drawing_graph:
 
             # start_tt = time.time()
@@ -800,14 +756,301 @@
                 count += 1
                 if cv2.waitKey(1) & 0xFF == ord('q'):
                     break
             else:
                 end_whole_t = time.time()
                 print("\r")
                 print(f"The whole process took {round((end_whole_t - whole_t), 4)} seconds.")
-                print(f"{output_file} is successfully produced.")
+                print(f"{output_video_file} is successfully produced.")
                 print("Thank you for using VINSET")
                 break
 
         input_video.release()
         v_writer.release()
         cv2.destroyAllWindows()
+
+
+def overlay_text(draw_able_input, config_info_input, input_video_file, output_video_file):
+    text_info = config_info_input["text_info"]
+    text_font_size = text_info["text_font_size"]
+    text_color = text_info["text_color"]
+    text_color_tuple = change_string_to_color_tuple(text_color)
+    text_thickness = text_info["text_thickness"]
+    timeline_file_name = config_info_input["timeline_file_name"]
+    timeline_file = str(input_video_file).replace(os.path.basename(input_video_file), timeline_file_name)
+    timeline_info = None
+    stimulus_text_display_location = config_info_input["stimulus_text_display_location"]
+    va_text_display_location = config_info_input["va_text_display_location"]
+    sti_x_position = stimulus_text_display_location["x"]
+    sti_y_position = stimulus_text_display_location["y"]
+    va_x_position = va_text_display_location["x"]
+    va_y_position = va_text_display_location["y"]
+    minimum_va_decimal = text_info["minimum_va_decimal"]
+
+    try:
+        f = open(timeline_file)
+        timeline_info = json.load(f)
+        print(f"{timeline_file} is loaded successfully by json.")
+        # print(timeline_info)
+    except ValueError:
+        draw_able_input = False
+        print(f"{timeline_file} cannot be loaded by json.")
+
+    if draw_able_input and config_info_input:
+        display_able = str_to_bool(str(config_info_input["display"]))
+
+        input_video = cv2.VideoCapture(input_video_file)
+        frame_width = input_video.get(cv2.CAP_PROP_FRAME_WIDTH)
+        print("Frame width:", frame_width)
+        frame_height = input_video.get(cv2.CAP_PROP_FRAME_HEIGHT)
+        print("Frame height:", frame_height)
+        frame_rate = input_video.get(cv2.CAP_PROP_FPS)
+        print("Frame rate:", frame_rate)
+        frame_count = input_video.get(cv2.CAP_PROP_FRAME_COUNT)
+        print("Frame count:", frame_count)
+
+        stimulus_level_array = get_logmar_level_array(timeline_info, text_info)
+
+        final_stimulus_level_array = add_logmar_interval(stimulus_level_array, text_info)
+
+        # for d in final_stimulus_level_array:
+        #     print(d)
+        # return
+
+        max_video_length = math.ceil(frame_count_to_time(frame_count, frame_rate))
+        print(f"Video length:{max_video_length / 1000} sec")
+
+        fourcc = cv2.VideoWriter_fourcc(*'mp4v')
+        v_writer = cv2.VideoWriter(output_video_file, fourcc, int(frame_rate), (int(frame_width), int(frame_height)))
+        whole_t = time.time()
+        count = 0
+        drawing_graph = True
+        start_drawing = False
+        stimulus_display_text = None
+        sweep_order = None
+        final_stimulus_level_array_length = len(final_stimulus_level_array)
+        stimulus_index = 0
+
+        while drawing_graph:
+
+            # start_tt = time.time()
+            ret, frame = input_video.read()
+            # end_tt = time.time()
+            print_percent_done(count, frame_count)
+            check_timer = frame_count_to_time(count, frame_rate)
+
+            if ret:
+                if stimulus_index < final_stimulus_level_array_length:
+                    stimulus_timestamp_to_check = final_stimulus_level_array[stimulus_index]["timestamp"] * 1000
+                    if check_timer >= stimulus_timestamp_to_check:
+                        start_drawing = True
+                        stimulus_display_text = str(final_stimulus_level_array[stimulus_index]["logmar"])
+                        sweep_order = final_stimulus_level_array[stimulus_index]["sweep_order"]
+                        stimulus_index += 1
+
+                if start_drawing:
+                    nearest_stimulus_text = get_nearest_stimulus(stimulus_display_text)
+                    cv2.putText(frame, f"Stimulus Level:{str(nearest_stimulus_text)}", (sti_x_position, sti_y_position),
+                                cv2.FONT_HERSHEY_SIMPLEX, text_font_size,
+                                text_color_tuple, text_thickness)
+                    va_display_text = get_va_from_stimulus(str(stimulus_display_text), sweep_order, minimum_va_decimal)
+                    cv2.putText(frame, f"VA       Level:{str(va_display_text)}", (va_x_position, va_y_position),
+                                cv2.FONT_HERSHEY_SIMPLEX, text_font_size,
+                                text_color_tuple, text_thickness)
+                    if sweep_order == "resting":
+                        start_drawing = False
+
+                if display_able:
+                    cv2.imshow("Frame", frame)
+                    # cv2.imshow("F", clone_frame)
+                    # vsr_t = time.time()
+                    v_writer.write(frame)
+                    # vso_t = time.time()
+                    count += 1
+                    if cv2.waitKey(1) & 0xFF == ord('q'):
+                        break
+            else:
+                end_whole_t = time.time()
+                print("\r")
+                print(f"The whole process took {round((end_whole_t - whole_t), 4)} seconds.")
+                print(f"{output_video_file} is successfully produced.")
+                print("Thank you for using VINSET")
+                break
+
+        input_video.release()
+        v_writer.release()
+        cv2.destroyAllWindows()
+
+
+def get_logmar_level_array(timeline_info_info, text_info_input):
+    draw_data = []
+    text_indicator = text_info_input["text_marker_location"]
+    time_indicator = text_info_input["time_marker_location"]
+    first_text_indicator, second_text_indicator, third_text_indicator = str(text_indicator).split("->")
+    first_time_indicator, second_time_indicator, third_time_indicator = str(time_indicator).split("->")
+    minimum_va_decimal = text_info_input["minimum_va_decimal"]
+    for event in timeline_info_info:
+        first_attribute = str(list(event.keys())[0])
+        if first_attribute == first_text_indicator:
+            event_info = event[first_attribute]
+            time_value = event_info[second_time_indicator][third_time_indicator]
+            text_value = str(round((float(event_info[second_text_indicator][third_text_indicator])), 2))
+            text_value = check_and_add_decimal(text_value, minimum_va_decimal)
+            data = {"timestamp": time_value, "logmar": text_value}
+            draw_data.append(data)
+    # for data in draw_data:
+    #     print(data)
+
+    return draw_data
+
+
+def add_logmar_interval(draw_data_array_input, text_info_input):
+    va_logmar_interval = text_info_input["va_logmar_interval"]
+    draw_data_array_length = len(draw_data_array_input)
+    last_index = draw_data_array_length - 1
+    minimum_va_decimal = text_info_input["minimum_va_decimal"]
+
+    final_data_array = []
+    for index in range(draw_data_array_length):
+        if index is not last_index:
+            first_value = draw_data_array_input[index]
+            second_value = draw_data_array_input[index + 1]
+            first_logmar = float(first_value["logmar"])
+            second_logmar = float(second_value["logmar"])
+            first_timestamp = first_value["timestamp"]
+            second_timestamp = second_value["timestamp"]
+
+            logmar_diff = first_logmar - second_logmar
+            sweep_order = "descending" if logmar_diff >= 0 else "ascending"
+            number_of_intervals = int(round(abs(logmar_diff), 1) / va_logmar_interval)
+            first_value["sweep_order"] = sweep_order
+            second_value["sweep_order"] = sweep_order
+
+            if logmar_diff == 0:
+                first_value["sweep_order"] = "resting"
+                second_value["sweep_order"] = "resting"
+                final_data_array.append(first_value)
+                final_data_array.append(second_value)
+            else:
+                extra_data = number_of_intervals - 1
+                each_time_interval_duration = (second_timestamp - first_timestamp) / number_of_intervals
+                final_data_array.append(first_value)
+                for ind in range(extra_data):
+                    time_value = first_timestamp + ((ind + 1) * each_time_interval_duration)
+                    if sweep_order == "descending":
+                        text_value = str(round((first_logmar - ((ind + 1) * va_logmar_interval)), 2))
+                    else:
+                        text_value = str(round(first_logmar + ((ind + 1) * va_logmar_interval), 2))
+                    data = {"timestamp": time_value, "logmar": text_value, "sweep_order":sweep_order}
+                    final_data_array.append(data)
+                final_data_array.append(second_value)
+    last_data = final_data_array[-1]
+    last_data["sweep_order"] = "resting"
+    final_data_array = list({dictionary['timestamp']: dictionary for dictionary in final_data_array}.values())
+
+    return final_data_array
+
+
+def check_and_add_decimal(string_input, min_decimal_input):
+    decimal_count = str(string_input)[::-1].find('.')
+    if 0 < decimal_count < min_decimal_input:
+        num_of_zero_to_add = min_decimal_input - decimal_count
+        string_input = string_input + "0" * num_of_zero_to_add
+    return string_input
+
+
+def get_va_from_stimulus(string_input, sweep_order_input, min_decimal_input):
+    if sweep_order_input == "descending" or sweep_order_input == "resting":
+        output = str(round((float(string_input) + 0.1), 2))
+        output_string = check_and_add_decimal(output, min_decimal_input)
+    else:
+        output = string_input
+        output_string = check_and_add_decimal(output, min_decimal_input)
+    return output_string
+
+
+def get_nearest_stimulus(string_input):
+    point_index = str(string_input).find(".") + 2
+    if point_index > -1:
+        string_input = string_input[:point_index]
+        if float(string_input) == 0:
+            string_input = "0.0"
+    return string_input
+
+
+def main():
+    parser = argparse.ArgumentParser(prog='vinset', description='VINSET package.')
+    parser.add_argument('--version', action='version', version='4.0.0'),
+    parser.add_argument("-i", dest="input_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
+                        help="input mp4 file", metavar="filename.mp4")
+    parser.add_argument("-d", dest="input_data_filename", required=False, type=argparse.FileType('r'),
+                        default=sys.stdin,
+                        help="input csv data file", metavar="filename.csv")
+    parser.add_argument("-o", dest="output_filename", required=True, type=argparse.FileType('w'), default=sys.stdout,
+                        help="output mp4 file", metavar="filename.mp4")
+    parser.add_argument("-c", dest="config_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
+                        help="config json file", metavar="filename.json")
+    parser.add_argument("-t", dest="overlay_type", required=False, default=sys.stdin,
+                        help="overlay type", metavar="graph or text")
+
+    # get all input name in string
+    args = parser.parse_args()
+    input_file = args.input_filename.name
+    csv_data = args.input_data_filename.name
+    output_file = args.output_filename.name
+    config_file = args.config_filename.name
+    overlay_type = args.overlay_type
+    csv_data_input = False if str(csv_data) == "<stdin>" else True
+    overlay_type_input = False if "_io.TextIOWrapper" in str(overlay_type) else True
+
+    # start whether the inputs are in correct types or not
+    if str(input_file).endswith(".mp4"):
+        print("Input file name:", input_file)
+    else:
+        print("Input file must be mp4.")
+    if csv_data_input:
+        if str(csv_data).endswith(".csv"):
+            print("Input data file name:", csv_data)
+        else:
+            print("Input data file must be csv.")
+    else:
+        print("There is no csv data input")
+    if str(csv_data).endswith(".csv"):
+        print("Input data file name:", csv_data)
+    else:
+        print("Input data file must be csv.")
+    if str(output_file).endswith(".mp4"):
+        print("Output file name:", output_file)
+    else:
+        print("Output file must be mp4.")
+    if str(config_file).endswith(".json"):
+        print("Config file name:", config_file)
+    else:
+        print("Config file must be json.")
+    if overlay_type_input:
+        if str(overlay_type) == "graph" or str(overlay_type) == "text":
+            print("Overlay type:", overlay_type)
+        else:
+            print("Overlay type must be graph or text.")
+    else:
+        print("There is no overlay type input")
+
+    config_info = None
+    draw_able = True
+    try:
+        f = open(config_file)
+        config_info = json.load(f)
+        print(f"{config_file} is loaded successfully by json.")
+    except ValueError:
+        draw_able = False
+        print(f"{config_file} cannot be loaded by json.")
+
+    if not overlay_type_input or str(overlay_type) == "graph":
+        if csv_data_input:
+            overlay_graph(draw_able, config_info, input_file, csv_data, output_file)
+        else:
+            print("There is no csv data input -d in commandline.")
+            print("Please add -d argument in commandline in order to proceed.")
+    elif str(overlay_type) == "text":
+        overlay_text(draw_able, config_info, input_file, output_file)
+    else:
+        print("Invalid overlay type input. It must be graph or text.")
```

### Comparing `vinset-3.0.5/vinset.egg-info/PKG-INFO` & `vinset-4.0.0/vinset.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 3.0.5
+Version: 4.0.0
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Command line program to draw the graph from video and csv files.
-
```

