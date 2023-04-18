# Comparing `tmp/chichitk-0.0.1.tar.gz` & `tmp/chichitk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chichitk-0.0.1.tar", last modified: Sat Apr 15 22:50:53 2023, max compression
+gzip compressed data, was "chichitk-0.0.2.tar", last modified: Tue Apr 18 22:04:38 2023, max compression
```

## Comparing `chichitk-0.0.1.tar` & `chichitk-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 22:50:53.167186 chichitk-0.0.1/
--rw-rw-rw-   0        0        0      783 2023-04-15 22:50:53.165192 chichitk-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-15 22:50:52.994510 chichitk-0.0.1/chichitk/
--rw-rw-rw-   0        0        0      573 2023-04-15 21:58:01.000000 chichitk-0.0.1/chichitk/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-03-23 15:31:05.000000 chichitk-0.0.1/chichitk/aspect_frame.py
--rw-rw-rw-   0        0        0    24750 2023-04-15 18:41:05.000000 chichitk-0.0.1/chichitk/buttons.py
--rw-rw-rw-   0        0        0    49848 2023-04-15 22:34:29.000000 chichitk-0.0.1/chichitk/canvas_items.py
--rw-rw-rw-   0        0        0    16147 2023-03-25 14:30:32.000000 chichitk-0.0.1/chichitk/dropdowns.py
--rw-rw-rw-   0        0        0     8815 2023-03-28 22:48:12.000000 chichitk-0.0.1/chichitk/entry_boxes.py
--rw-rw-rw-   0        0        0     6206 2023-04-14 23:14:31.000000 chichitk-0.0.1/chichitk/file_dialog.py
--rw-rw-rw-   0        0        0     4414 2023-04-14 23:15:29.000000 chichitk-0.0.1/chichitk/function_progress.py
--rw-rw-rw-   0        0        0    10705 2023-04-14 23:17:09.000000 chichitk-0.0.1/chichitk/labels.py
--rw-rw-rw-   0        0        0     8721 2023-04-14 23:18:49.000000 chichitk-0.0.1/chichitk/pdf_display.py
--rw-rw-rw-   0        0        0     7088 2023-04-15 18:29:00.000000 chichitk-0.0.1/chichitk/player.py
--rw-rw-rw-   0        0        0     5152 2023-03-24 16:40:10.000000 chichitk-0.0.1/chichitk/progress_bar.py
--rw-rw-rw-   0        0        0     3776 2023-03-28 23:26:56.000000 chichitk-0.0.1/chichitk/scrollable_frame.py
--rw-rw-rw-   0        0        0    66515 2023-04-15 22:36:25.000000 chichitk-0.0.1/chichitk/sliders.py
--rw-rw-rw-   0        0        0     4927 2023-03-24 17:01:52.000000 chichitk-0.0.1/chichitk/temp_menu.py
--rw-rw-rw-   0        0        0     9187 2023-04-04 22:46:09.000000 chichitk-0.0.1/chichitk/text_boxes.py
--rw-rw-rw-   0        0        0     9855 2023-04-15 18:26:04.000000 chichitk-0.0.1/chichitk/timer.py
--rw-rw-rw-   0        0        0     6880 2023-03-23 19:14:50.000000 chichitk-0.0.1/chichitk/tool_tip.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:50:53.142437 chichitk-0.0.1/chichitk.egg-info/
--rw-rw-rw-   0        0        0      783 2023-04-15 22:50:50.000000 chichitk-0.0.1/chichitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-04-15 22:50:52.000000 chichitk-0.0.1/chichitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 22:50:50.000000 chichitk-0.0.1/chichitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-15 22:50:50.000000 chichitk-0.0.1/chichitk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 22:50:50.000000 chichitk-0.0.1/chichitk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 22:50:53.168180 chichitk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1182 2023-04-15 22:45:46.000000 chichitk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:04:38.036381 chichitk-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-16 02:22:07.000000 chichitk-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3223 2023-04-18 22:04:38.036381 chichitk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2485 2023-04-18 21:24:18.000000 chichitk-0.0.2/Readme.md
+drwxrwxrwx   0        0        0        0 2023-04-18 22:04:38.006462 chichitk-0.0.2/chichitk/
+-rw-rw-rw-   0        0        0      656 2023-04-17 16:30:35.000000 chichitk-0.0.2/chichitk/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-04-17 00:34:05.000000 chichitk-0.0.2/chichitk/aspect_frame.py
+-rw-rw-rw-   0        0        0    26105 2023-04-16 23:33:38.000000 chichitk-0.0.2/chichitk/buttons.py
+-rw-rw-rw-   0        0        0    49997 2023-04-16 02:08:01.000000 chichitk-0.0.2/chichitk/canvas_items.py
+-rw-rw-rw-   0        0        0    16147 2023-03-25 14:30:32.000000 chichitk-0.0.2/chichitk/dropdowns.py
+-rw-rw-rw-   0        0        0     8815 2023-03-28 22:48:12.000000 chichitk-0.0.2/chichitk/entry_boxes.py
+-rw-rw-rw-   0        0        0     6098 2023-04-18 17:15:53.000000 chichitk-0.0.2/chichitk/file_dialog.py
+-rw-rw-rw-   0        0        0     4288 2023-04-16 21:18:55.000000 chichitk-0.0.2/chichitk/function_progress.py
+-rw-rw-rw-   0        0        0    34820 2023-04-18 17:09:52.000000 chichitk-0.0.2/chichitk/icons.py
+-rw-rw-rw-   0        0        0    10583 2023-04-16 21:19:48.000000 chichitk-0.0.2/chichitk/labels.py
+-rw-rw-rw-   0        0        0    10145 2023-04-18 17:35:06.000000 chichitk-0.0.2/chichitk/pdf_display.py
+-rw-rw-rw-   0        0        0     7301 2023-04-16 23:35:43.000000 chichitk-0.0.2/chichitk/player.py
+-rw-rw-rw-   0        0        0     5152 2023-03-24 16:40:10.000000 chichitk-0.0.2/chichitk/progress_bar.py
+-rw-rw-rw-   0        0        0     3776 2023-03-28 23:26:56.000000 chichitk-0.0.2/chichitk/scrollable_frame.py
+-rw-rw-rw-   0        0        0    66444 2023-04-17 23:52:20.000000 chichitk-0.0.2/chichitk/sliders.py
+-rw-rw-rw-   0        0        0     4927 2023-03-24 17:01:52.000000 chichitk-0.0.2/chichitk/temp_menu.py
+-rw-rw-rw-   0        0        0     9187 2023-04-04 22:46:09.000000 chichitk-0.0.2/chichitk/text_boxes.py
+-rw-rw-rw-   0        0        0     9855 2023-04-15 18:26:04.000000 chichitk-0.0.2/chichitk/timer.py
+-rw-rw-rw-   0        0        0     6880 2023-03-23 19:14:50.000000 chichitk-0.0.2/chichitk/tool_tip.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:04:38.034387 chichitk-0.0.2/chichitk.egg-info/
+-rw-rw-rw-   0        0        0     3223 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1196 2023-04-18 22:03:48.000000 chichitk-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 22:04:38.037377 chichitk-0.0.2/setup.cfg
```

### Comparing `chichitk-0.0.1/chichitk/__init__.py` & `chichitk-0.0.2/chichitk/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from .aspect_frame import *
 from .buttons import *
 from .dropdowns import *
 from .entry_boxes import *
 from .file_dialog import *
 from .function_progress import *
 from .labels import *
-from .pdf_display import *
+from .pdf_display import PdfDisplay
 from .player import *
 from .progress_bar import *
 from .scrollable_frame import *
 from .sliders import *
 from .temp_menu import *
 from .text_boxes import *
 from .timer import *
 from .tool_tip import *
 
 # not importing from .canvas_items because these are not intended
-# to be used outside of chichitk
+# to be used outside of chichitk
+
+# not importing from .icons because this just contains icons as arrays
```

### Comparing `chichitk-0.0.1/chichitk/aspect_frame.py` & `chichitk-0.0.2/chichitk/aspect_frame.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,17 @@
         All content should be put in AspectFrame.frame NOT in AspectFrame
         directly
 
         For AspectFrame to work as intended, pack with fill='both' and
         expand=True, and grid with sticky='nsew'
 
         DO NOT use AspectFrame.place() because then AspectFrame will not work
+
+        AspectFrame should ALWAYS be packed with expand=True and grid with
+        sticky='nsew' and parent widget gridrowconfigure and gridcolumnconfigure
     '''
     def __init__(self, master, aspect_ratio:float, pad_bg:str='#ffffff',
                  frame_bg:str='#ffffff', config_callback:callable=None,
                  size_callback:callable=None):
         '''
         Parameters
         ----------
```

### Comparing `chichitk-0.0.1/chichitk/buttons.py` & `chichitk-0.0.2/chichitk/buttons.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import cv2, os
 import numpy as np
 from PIL import Image, ImageTk
 from tkinter import Frame, Button, Label
 
 from .tool_tip import ToolTip
+from .icons import icons
 
 
 def hex_to_rgb(hex_code:str):
     '''converts hex code to uint8 rgb'''
     return tuple([int(h, 16) for h in (hex_code[1:3], hex_code[3:5], hex_code[5:])])
 
 def image_replace_colors(img:np.array, colors_list:list):
@@ -172,33 +173,43 @@
         background color (set specifically for each hover/select status) can
         be changed with **kwargs passed to BaseButton
     '''
     def __init__(self, master, icon_path:str, command, label:str='', bar_height:int=3, **kwargs):
         '''
         Parameters
         ----------
-            master : frame in which to put button
-            icon_path : str - path to .png file
-            click_command : 0 argument function - function to be executed when button is clicked
-            bar_height : Int - height of bar at the bottom of button
+            :param master: frame in which to put button
+            :param icon_path: str or np.array - path to .png file or image array
+            :param click_command: 0 argument function - function to be executed when button is clicked
+            :param bar_height: Int - height of bar at the bottom of button
         '''
         BaseButton.__init__(self, master, command, bar_height=bar_height, **kwargs) # bar already packed buttom
         self.icon_frame = Frame(self)
         self.icon_frame.pack(side='top', padx=self.padx, pady=self.pady)
         self.icon = Button(self.icon_frame, borderwidth=0, command=self.click_button)
         self.icon.pack(side='left')
         self.label = Label(self.icon_frame, text=label, font=(self.font_name, self.font_size), bd=0)
         self.label.pack(side='right', fill='y')
 
         self.icon_frame.bind("<Button-1>", self.click_button)
         self.label.bind("<Button-1>", self.click_button)
         
+        # Load icon
+        if isinstance(icon_path, str): # path to image
+            assert len(icon_path) > 4, f'Invalid path: {icon_path}'
+            assert icon_path[-4:] == '.png', f'icon_path is not a .png file: {icon_path}'
+            assert os.path.exists(icon_path), f'Path to .png file does not exist: {icon_path}'
+            self.base_img = cv2.imread(icon_path)
+        elif isinstance(icon_path, np.ndarray): # 3d numpy array
+            self.base_img = icon_path
+        else:
+            raise TypeError(f'Invalid icon input to IconButton: {icon_path}')
+
         # Create Icons
         self.images = [[None, None], [None, None]]
-        self.base_img = cv2.imread(icon_path)
         for x, y in [[0, 0], [0, 1], [1, 0], [1, 1]]:
             temp_img = image_replace_colors(self.base_img.copy(), [('#ffffff', self.fg_colors[x][y]), ('#000000', self.bg_colors[x][y])])
             self.images[x][y] = ImageTk.PhotoImage(image=Image.fromarray(temp_img), master=self.icon_frame)
         off_img = image_replace_colors(self.base_img.copy(), [('#ffffff', self.off_fg), ('#000000', self.bg_colors[0][0])])
         self.off_icon = ImageTk.PhotoImage(image=Image.fromarray(off_img), master=self.icon_frame)
 
         self.config_colors()
@@ -360,18 +371,15 @@
             :param master: tk.Frame - parent widget
             :param command: 1 argument function (bool) called when button is clicked
             :param label: str - text to the left of button
             :param active_popup_label: str or None - hover popup text when button is selected
             :param inactive_popup_label: str or None - hover popup text when button is not selected
             :param active: bool - initial status of CheckButton
         '''
-        image_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "icons")
-        path1 = os.path.join(image_path, "box.png")
-        path2 = os.path.join(image_path, "checkbox.png")
-        DoubleIconButton.__init__(self, master, path1, path2,
+        DoubleIconButton.__init__(self, master, icons['box'], icons['checkbox'],
                                   lambda: command(True), lambda: command(False),
                                   label1=label, label2=label,
                                   popup_label1=inactive_popup_label,
                                   popup_label2=active_popup_label, **kwargs)
         if active:
             self.Button1.click_button()
 
@@ -380,14 +388,15 @@
         'bar_height' can be set to 0 to remove the bar.
         
         Background and foreground color can change based on select/hover status.
     '''
     def __init__(self, master, command, label:str='', **kwargs):
         '''just like IconButton but with no icon'''
         BaseButton.__init__(self, master, command, **kwargs)
+        self.label_text = label
         self.label = Label(self, text=label, font=(self.font_name, self.font_size), bd=0)
         self.label.pack(side='top', padx=self.padx, pady=self.pady)
         self.label.bind("<Button-1>", self.click_button)
 
         self.config_colors()
 
     def config_colors(self):
@@ -397,14 +406,18 @@
             bar_color = self.bar_colors[self.selected][self.hovering]
         else:
             bg, fg, bar_color = self.bg_colors[0][0], self.off_fg, self.bg_colors[0][0]
         self.config(bg=bg)
         self.bar.config(bg=bar_color)
         self.label.config(bg=bg, fg=fg)
 
+    def get_text(self):
+        '''returns label text'''
+        return self.label_text
+
 class ToggleLabelButton(LabelButton):
     ''' Extension of LabelButton that passes a boolean argument to callback
         command to indicate whether buttons is being selected or deselected.
     '''
     def __init__(self, master, command=None, label:str='', **kwargs):
         '''Toggle version of LabelButton
         
@@ -430,54 +443,66 @@
             play/pause - toggle button to start/stop playback
             skip_forward - go forward by a given increment
             next - go to next song or end of current song
             loop (toggle) - turn looping on or off
             '''
     def __init__(self, master, bg, play_function, stop_function, step_forward_function,
                  step_back_function, next_function, previous_function,
-                 active_icon_color='#ffffff', button_bar_height=0,
-                 button_padx=7, active=True):
-        '''buttons to control playback of MusicPlayer or VideoPlayer'''
+                 active_icon_color='#ffffff', hover_fg='#aaaaaa',
+                 button_padx=6, padx_weight=6, active=True):
+        '''
+        Parameters
+        ----------
+            :param master: tk.Frame - parent widget
+            :param bg: str (hex code) - background color
+            :param play_function: function () - called when play button is clicked
+            :param stop_function: function () - called when stop button is clicked
+            :param step_forward_function: function () - called when step_forward button is clicked
+            :param step_back_function: function () - called when step_back button is clicked
+            :param next_function: function () - called when next button is clicked
+            :param previous_function: function () - called when previous button is clicked
+            :param active_icon_color: str (hex code) - color of loop button when selected
+            :param hover_fg: str (hex code) - color of buttons when cursor is hovering
+            :param button_padx: int (pixels) - minimum distance between buttons
+            :param padx_weight: int - weight of x padding for button group
+            :param active: bool - if True, buttons are interactable by default
+        '''
         Frame.__init__(self, master, bg=bg)
         # for x padding so that buttons dont span full width of frame
-        self.grid_columnconfigure(0, weight=6)
-        self.grid_columnconfigure(7, weight=6)
+        self.grid_columnconfigure(0, weight=padx_weight)
+        self.grid_columnconfigure(7, weight=padx_weight)
         for i in range(6):
             self.grid_columnconfigure(i + 1, weight=1)
         
         # key-word arguments common to all buttons
-        bkwargs = {'bar_height':button_bar_height, 'inactive_bg':bg,
-                   'padx':button_padx}
+        bkwargs = {'bar_height':0, 'inactive_bg':bg,
+                   'inactive_hover_fg':hover_fg , 'padx':button_padx}
         
         # Create buttons
-        image_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "icons")
         self.buttons: list[IconButton] = []
-        previous_button = IconButton(self, os.path.join(image_path, "skip_back.png"),
-                                     previous_function, popup_label='Skip to Start',
+        previous_button = IconButton(self, icons['skip_back'], previous_function,
+                                     popup_label='Skip to Start',
                                      selectable=False, **bkwargs)
-        back_button = IconButton(self, os.path.join(image_path, "replay5.png"),
-                                 step_back_function, popup_label='Back 5 Seconds',
+        back_button = IconButton(self, icons['replay5'], step_back_function,
+                                 popup_label='Back 5 Seconds',
                                  selectable=False, **bkwargs)
-        self.play_button = DoubleIconButton(self, os.path.join(image_path, "play.png"),
-                                            os.path.join(image_path, "pause.png"),
+        self.play_button = DoubleIconButton(self, icons['play'], icons['pause'],
                                             play_function, stop_function,
                                             popup_label1='Play', popup_label2='Pause',
                                             **bkwargs)
-        forward_button = IconButton(self, os.path.join(image_path, "forward5.png"),
-                                    step_forward_function, popup_label='Forward 5 Seconds',
+        forward_button = IconButton(self, icons['forward5'], step_forward_function,
+                                    popup_label='Forward 5 Seconds',
                                     selectable=False, **bkwargs)
-        next_button = IconButton(self, os.path.join(image_path, "skip_forward.png"),
+        next_button = IconButton(self, icons['skip_forward'],
                                  next_function, popup_label='Skip to End',
                                  selectable=False, **bkwargs)
-        self.loop_button = ToggleIconButton(self, os.path.join(image_path, "loop.png"),
+        self.loop_button = ToggleIconButton(self, icons['loop'],
                                             popup_label='Toggle Loop',
-                                            bar_height=button_bar_height,
-                                            active_bg=bg, inactive_bg=bg,
-                                            active_fg=active_icon_color,
-                                            padx=button_padx)
+                                            active_bg=bg, active_fg=active_icon_color,
+                                            active_hover_fg=hover_fg, **bkwargs)
 
         # Grid buttons
         for i, button in enumerate([previous_button, back_button, self.play_button,
                                     forward_button, next_button, self.loop_button]):
             button.grid(row=0, column=i + 1)
             self.buttons.append(button)
 
@@ -493,14 +518,16 @@
         self.play_button.switch2()
 
     def to_play(self):
         '''switches stop button to play button without calling stop command'''
         self.play_button.switch1()
 
     def turn_on(self):
+        '''make buttons interactable by user'''
         for button in self.buttons:
             button.turn_on()
 
     def turn_off(self):
+        '''make buttons uninteractable by user'''
         for button in self.buttons:
             button.turn_off()
```

### Comparing `chichitk-0.0.1/chichitk/canvas_items.py` & `chichitk-0.0.2/chichitk/canvas_items.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     def __init__(self, canvas:Canvas, x:float, y0:float, height:int, width=4,
                  bg:str='#ffffff', drag_color:str='#e8ff00', hover_color=None,
                  select_color:str='#499de6', brighten_fact:float=-0.25,
                  select_brighten_fact:float=0.3, selectable:bool=True,
                  hoverable:bool=True, draggable:bool=True, show_drag_color=False,
                  drag_function=None, self_select_function=None, self_delete_function=None,
                  always_deselect:bool=False, menu_font_name='Segoe UI', menu_font_size=11,
-                 double_click_to_delete:bool=True, active=True, tag_name:str='tag',
-                 state:str='normal'):
+                 double_click_to_delete:bool=True, deletable=True, active=True,
+                 tag_name:str='tag', state:str='normal'):
         '''        
         Parameters
         ----------
             :param canvas: tk.Canvas - canvas in which to create rectangle
             :param x: float (pixels) - x coordinate of line
             :param y0: float (pixels) - line top in canvas
             :param height: float (pixels) - line height in canvas
@@ -54,14 +54,15 @@
             :param drag_function: 2-float input function (current_x, cursor_position_x) - returns 1 float (new_x)
             :param double_click_function: 1 argument function (event) or None - called when line is double clicked
             :param right_click_function: 1 argument function (event) or None - called when line is right clicked
             :param center_click_function: 1 argument function (event) or None - called when line is center clicked
             :param self_delete_function: 1 argument function (self) - called when item is self deleted (with popup menu)
             :param self_select_function: 1 argument function (self) - called when item is self selected (selected by clicking on Item)
             :param always_deselect: bool - if True, will deselect upon command even if cursor is hovering
+            :param deletable: bool - if True, line can be deleted from right-click popup menu
             :param active: bool - if False, CanvasEditFill will be unresponsive to user actions, regardless of other settings - for toggling
             :param tag_name: str - tag name given to all canvas items - should be general for items of guitar track, chords track, etc
             :param state: str - state in canvas when item is created - options: ['normal', 'hidden', 'disabled']
         '''
         self.active = active
         self.canvas = canvas
         self.brighten_fact = brighten_fact
@@ -84,18 +85,19 @@
         self.canvas.tag_bind(self.id, '<Leave>', self.__hover_leave)
         if self.draggable or self.selectable:
             self.canvas.tag_bind(self.id, '<Button-1>', self.click)
         if self.draggable:
             self.canvas.tag_bind(self.id, '<ButtonRelease-1>', self.release)
             self.canvas.tag_bind(self.id, '<B1-Motion>', self.drag)
 
-        self.menu = Menu(canvas, tearoff=False, bg='#000000', fg='#ffffff',
-                         activebackground='#222222', font=(menu_font_name, menu_font_size))
-        self.menu.add_command(label="Delete", command=self.self_delete)
-        self.canvas.tag_bind(self.id, "<Button-3>", self.right_click)
+        if deletable:
+            self.menu = Menu(canvas, tearoff=False, bg='#000000', fg='#ffffff',
+                            activebackground='#222222', font=(menu_font_name, menu_font_size))
+            self.menu.add_command(label="Delete", command=self.self_delete)
+            self.canvas.tag_bind(self.id, "<Button-3>", self.right_click)
         if double_click_to_delete:
             self.canvas.tag_bind(self.id, "<Double-Button-1>", self.self_delete)
 
     def set_active(self):
         '''sets state to active so that user interactions proceed as normal'''
         self.active = True
```

### Comparing `chichitk-0.0.1/chichitk/dropdowns.py` & `chichitk-0.0.2/chichitk/dropdowns.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.1/chichitk/entry_boxes.py` & `chichitk-0.0.2/chichitk/entry_boxes.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.1/chichitk/file_dialog.py` & `chichitk-0.0.2/chichitk/file_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from tkinter import Frame, Label, filedialog
 
 import os
 
 from .buttons import IconButton
+from .icons import icons
 
 
 class FileDialog(Frame):
     ''' Widget that allows user to load and store file names
 
         The currently loaded file can be retrieved using the .get() method
     '''
@@ -40,34 +41,31 @@
         self.__load_callback = load_callback
         self.__filename = None
         self.__target_filenames = target_filenames if target_filenames else []
         self.inactive_bg, self.loaded_bg = inactive_bg, loaded_bg
         self.file_active_fg, self.file_inactive_fg = file_active_fg, file_inactive_fg
         self.__filetypes = [(f'{t.upper()} Files', f'*.{t}') for t in file_types] + [('All Files', '*.*')]
 
-        image_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "icons")
-        icon_path = os.path.join(image_path, "file_upload.png")
-
         if row != None:
             file_label = Label(master, text=label, bg=bg, fg=fg,
                                font=(label_font_name, label_font_size))
             file_label.grid(row=row, column=start_col, padx=padx, pady=pady, sticky='nsew')
-            load_button = IconButton(master, icon_path, self.browse_file,
+            load_button = IconButton(master, icons['file_upload'], self.browse_file,
                                      popup_label='Upload File', selectable=False,
                                      bar_height=0, inactive_bg=bg)
             load_button.grid(row=row, column=start_col + 1, padx=padx, pady=pady, sticky='nsew')
             self.file_label = Label(master, text='No File Loaded', bg=inactive_bg,
                                     fg=self.file_inactive_fg,
                                     font=(file_font_name, file_font_size))
             self.file_label.grid(row=row, column=start_col + 2, padx=padx, pady=pady, sticky='nsew')
         else:
             file_label = Label(self, text=label, bg=bg, fg=fg,
                                font=(label_font_name, label_font_size))
             file_label.pack(side='left', fill='x', expand=True)
-            load_button = IconButton(self, icon_path, self.browse_file,
+            load_button = IconButton(self, icons['file_upload'], self.browse_file,
                                      popup_label='Upload File', selectable=False,
                                      bar_height=0, inactive_bg=bg)
             load_button.pack(side='right')
             self.file_label = Label(self, text='No File Loaded', bg=inactive_bg,
                                     fg=self.file_inactive_fg,
                                     font=(file_font_name, file_font_size))
             self.file_label.pack(side='left', fill='x', expand=True)
```

### Comparing `chichitk-0.0.1/chichitk/function_progress.py` & `chichitk-0.0.2/chichitk/function_progress.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from tkinter import Frame, Label
 
 from .progress_bar import ProgressBar
 from .buttons import IconButton
+from .icons import icons
 
 
 class FunctionProgress(Frame):
     ''' Widget to call a specific function and display the progress of that
         function's execution
         
         Uses IconButton to allow user to start the function
@@ -41,20 +42,17 @@
             :param inactive_color: str (hex code) or None - inactive part of progress bar
         '''
         Frame.__init__(self, master, bg=bg)
         self.inactive_bg, self.loaded_bg = inactive_bg, loaded_bg
         inactive_color = inactive_color if inactive_color else bg
         self.complete = False
 
-        image_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "icons")
-        icon_path = os.path.join(image_path, "file_upload.png")
-
         self.main_frame = Frame(self, bg=bg)
         self.main_frame.pack(side='top', fill='both', expand=True)
-        button = IconButton(self.main_frame, icon_path, command, label=label,
+        button = IconButton(self.main_frame, icons['edit'], command, label=label,
                             selectable=False, inactive_bg=bg, bar_height=2)
         button.pack(side='left', fill='both', expand=True)
         self.indicator = Label(self.main_frame, text=' ' * 3, bg=self.inactive_bg,
                                font=(font_name, font_size))
         self.indicator.pack(side='right', fill='y', pady=indicator_pady)
 
         self.Progress = ProgressBar(self, 100, bg, active_color=active_color,
```

### Comparing `chichitk-0.0.1/chichitk/labels.py` & `chichitk-0.0.2/chichitk/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import os
 from tkinter import Label, Frame
 
 from .entry_boxes import CheckEntry
 from .buttons import IconButton
+from .icons import icons
 
 
 class EditLabel(Frame):
     ''' Label that changes to an CheckEntry box when user double clicks to
         allow text to be edited
         
         Uses CheckEntry so that text can be checked as it is entered and
@@ -163,22 +163,20 @@
         self.min_function, self.max_function = min_val_function, max_val_function
         self.callback_function = callback_function
         Frame.__init__(self, master, bg=bg)
         self.grid_columnconfigure(0, weight=0)
         self.grid_columnconfigure(1, weight=1)
         self.grid_columnconfigure(2, weight=0)
 
-        image_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "icons")
-
-        minus_button = IconButton(self, os.path.join(image_path, "minus.png"),
+        minus_button = IconButton(self, icons['minus'],
                                   self.minus, selectable=False,
                                   bar_height=0, popup_label='-1', inactive_bg=bg,
                                   inactive_hover_fg=fg, inactive_fg=fg,
                                   inactive_hover_bg=hover_bg)
-        plus_button = IconButton(self, os.path.join(image_path, "plus.png"),
+        plus_button = IconButton(self, icons['plus'],
                                  self.plus, selectable=False,
                                  bar_height=0, popup_label='+1', inactive_bg=bg,
                                  inactive_hover_fg=fg, inactive_fg=fg,
                                  inactive_hover_bg=hover_bg)
         minus_button.grid(row=0, column=0)
         plus_button.grid(row=0, column=2)
```

### Comparing `chichitk-0.0.1/chichitk/pdf_display.py` & `chichitk-0.0.2/chichitk/pdf_display.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,128 @@
-from tkinter import Toplevel, Frame, Label, Text, Scrollbar, PhotoImage
+from tkinter import Toplevel, Frame, Label, Text, Scrollbar, PhotoImage, filedialog
 from threading import Thread
-import fitz
-import os
+import shutil # for copying files
+import fitz # fitz is PyMuPDF
 
 from .buttons import IconButton
+from .icons import icons
 
 
 class PdfDisplay(Frame):
     ''' Widget that displays pdf or 'No File Loaded' label when no pdf is loaded
     
         Contains a button that allows the user to open the pdf in a new window
     '''
     def __init__(self, master, bg, fg, font_name:str='Segoe UI', font_size:int=20,
                  button_pad:int=2, view_width=75, zoom_fact=1, height:int=600,
-                 new_window_option=True, zoom_options=True):
+                 buttons_side='left', buttons_bg='#ffffff',
+                 new_window_option=True, download_option=True, zoom_options=True):
         '''
         
         Parameters
         ----------
             :param master: tk.Frame - parent widget
             :param bg: str (hex code) - background color
             :param fg: str (hex code) - color of 'No File Loaded' label
             :param font_name: str - font name such as 'Segoe UI'
             :param font_size: int - font size
             :param button_pad: int - padding between button and top left corner
             :param view_width: int - width of view in pixels
             :param zoom_fact: float - factor by which to zoom pdf
+            :param buttons_side: str - Literal['left', 'right']
+            :param buttons_bg: str (hex code) - background color of buttons
             :param new_window_option: bool - if True, include button to open in new window
+            :param download_option: bool - if True, include button to download pdf
+            :param zoom_options: bool - if True, include buttons to zoom pdf
         '''
+        assert buttons_side in ['left', 'right'], f"Invalid buttons side: '{buttons_side}', must be 'left' or 'right'"
         Frame.__init__(self, master, bg=bg)
         self.button_pad = button_pad
         self.bg = bg # store for new window
         self.width, self.height = view_width, height
         self.zoom_fact = zoom_fact # never changes
         self.scale_fact = 1 # changes when zooming in and out
         self.img_object_list = []
+        self.buttons_side = buttons_side
         self.pdf_frame = None # tk.Frame once a pdf is loaded
         self.active = False # True when a pdf is loaded
 
         # Buttons Frame
         self.buttons_frame = Frame(self, bg='#ffffff')
 
-        image_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "icons")
+        bkwargs = {'bar_height':0, 'selectable':False, 'inactive_bg':buttons_bg,
+                   'inactive_hover_fg':None, 'popup_bg':self.bg}
 
         if new_window_option:
-            new_button = IconButton(self.buttons_frame,
-                                    os.path.join(image_path, "open_in_new.png"),
-                                    command=self.open_in_window, bar_height=0,
-                                    selectable=False, inactive_bg='#ffffff',
-                                    inactive_hover_fg=None, popup_bg=self.bg,
-                                    popup_label='Open In New Window')
-            new_button.pack(side='left')
+            new_button = IconButton(self.buttons_frame, icons['open_in_new'],
+                                    command=self.open_in_window,
+                                    popup_label='Open In New Window', **bkwargs)
+            new_button.pack(side=buttons_side)
+
+        if download_option:
+            down_button = IconButton(self.buttons_frame, icons['file_download'],
+                                     command=self.download_pdf,
+                                     popup_label='Download PDF', **bkwargs)
+            down_button.pack(side=buttons_side)
 
         if zoom_options:
-            out_button = IconButton(self.buttons_frame, os.path.join(image_path, "minus.png"),
-                                    command=self.zoom_out, bar_height=0,
-                                    selectable=False, inactive_bg='#ffffff',
-                                    inactive_hover_fg=None, popup_bg=self.bg,
-                                    popup_label='Zoom Out')
-            in_button = IconButton(self.buttons_frame, os.path.join(image_path, "plus.png"),
-                                   command=self.zoom_in, bar_height=0,
-                                   selectable=False, inactive_bg='#ffffff',
-                                   inactive_hover_fg=None, popup_bg=self.bg,
-                                   popup_label='Zoom In')
+            out_button = IconButton(self.buttons_frame, icons['minus'],
+                                    command=self.zoom_out,
+                                    popup_label='Zoom Out', **bkwargs)
+            in_button = IconButton(self.buttons_frame, icons['plus'],
+                                   command=self.zoom_in,
+                                   popup_label='Zoom In', **bkwargs)
             out_button.pack(side='left')
             in_button.pack(side='left')
         
         # Inactive Label
         self.label = Label(self, text='No File Loaded', bg=bg, fg=fg,
                            font=(font_name, font_size))
         self.label.pack(fill='both', expand=True)
 
     def position_buttons(self, event=None):
         '''repositions buttons - called when window is resized'''
         if self.active:
-            self.buttons_frame.place(x=self.pdf_frame.winfo_x() + self.button_pad,
-                                    y=self.pdf_frame.winfo_y() + self.button_pad,
-                                    anchor='nw')
+            if self.buttons_side == 'left':
+                x = self.pdf_frame.winfo_x() + self.button_pad
+                anchor = 'nw'
+            elif self.buttons_side == 'right':
+                right_edge = self.pdf_frame.winfo_x() + self.pdf_frame.winfo_width()
+                x = right_edge - self.scroll_y.winfo_width() - self.button_pad
+                anchor = 'ne'
+            else: # this should never happen
+                raise ValueError(f'PdfDisplay button side is invalid: {self.buttons_side}')
+            self.buttons_frame.place(x=x, y=self.pdf_frame.winfo_y() + self.button_pad,
+                                     anchor=anchor)
             self.buttons_frame.lift() # raise above pdf
 
     def remove_all(self):
         '''removes pdf, buttons, and label'''
         self.active = False
         self.label.pack_forget()
         self.buttons_frame.place_forget()
         if self.pdf_frame != None:
             self.pdf_frame.destroy()
 
     def show_pdf(self, filename:str):
-        '''loads pdf from the fiven filepath'''
+        '''loads pdf from the given filepath'''
         self.scale_fact = 1 # reset zoom
         self.filename = filename
         self.remove_all()
         self.active = True
         Thread(target=self.render_pdf()).start()
 
     def render_pdf(self):
         '''loads pdf from self.filename - MUST be called in Thread'''
         # Create image objects from pdf pages
         self.img_object_list = []
         for page in fitz.open(self.filename):
-            pix = page.getPixmap(dpi=int(72 * self.zoom_fact * self.scale_fact))
+            pix = page.get_pixmap(dpi=int(72 * self.zoom_fact * self.scale_fact))
             pix1 = fitz.Pixmap(pix, 0) if pix.alpha else pix
-            image = pix1.getImageData("ppm")
+            image = pix1.tobytes("ppm")
             self.img_object_list.append(PhotoImage(data=image))
 
         # Create new pdf frame
         width = int(self.width * self.scale_fact)
         height = int(self.height * self.scale_fact)
         self.pdf_frame = Frame(self, height=height, width=width, bg=self.bg)
         self.scroll_y = Scrollbar(self.pdf_frame, orient="vertical")
@@ -118,14 +134,15 @@
                              xscrollcommand=self.scroll_x.set, #font=('Segoe UI', 2),
                              height=height, width=width)
         self.pdf_text.pack(side="left")
         self.scroll_x.config(command=self.pdf_text.xview)
         self.scroll_y.config(command=self.pdf_text.yview)
         self.pdf_frame.pack()
         self.pdf_frame.bind('<Configure>', self.position_buttons)
+        self.update() # render so that buttons are positioned properly
         self.position_buttons() # place buttons and raise above pdf
 
         # Add pages to text box
         for i, img in enumerate(self.img_object_list):
             if i > 0: # add space before next page
                 self.pdf_text.insert('end', '\n\n')
             self.pdf_text.image_create('end', image=img)
@@ -153,14 +170,23 @@
 
     def to_loading(self, text='Loading...'):
         '''removes current pdf and displays loading text'''
         self.remove_all()
         self.label.config(text=text)
         self.label.pack(fill='both', expand=True)
 
+    def download_pdf(self):
+        '''opens dialog to download the current pdf file
+        this can only ever be called when a pdf is being viewed'''
+        destination = filedialog.asksaveasfilename(initialdir='/', title='Select destination file',
+                                                    filetypes=(('PDF File', '*.pdf'), ('All Files', '*.*')))
+        if destination[-4:] != '.pdf':
+            destination += '.pdf'
+        shutil.copy2(self.filename, destination)
+
     def open_in_window(self):
         '''opens PDF in new window - can only ever be called when a PDF is being viewed'''
         PdfWindow(self.filename, self.bg)
 
 class PdfWindow(Toplevel):
     ''' Window to view a single PDF File
```

### Comparing `chichitk-0.0.1/chichitk/player.py` & `chichitk-0.0.2/chichitk/player.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         
         An example use case could be playing frames from a video
     '''
     def __init__(self, master:Frame, callback, delay:float, bg:str='#000000',
                  slider_type:str='single', frame_num=1000, frame_rate=29.97,
                  step_increment:int=150, end_callback=None, start_callback=None,
                  stop_callback=None, skip_callback=None, buttons_on_top=False,
-                 value_display_fact=1):
+                 buttons_padx_weight=6, value_display_fact=1):
         ''' Only keeps track of the current frame using Timer
 
         Parameters
         ----------
             :param master: tk.Frame - parent widget
             :param callback: function (step) - called with each iteration
             :param delay: float - seconds between each iteration
@@ -34,14 +34,15 @@
                                          - back when step buttons are clicked
             :param end_callback: function () - called when final step is reached
                                              - not called if looping is on
             :param start_callback: function (current_step) - called when timer is started
             :param stop_callback: function () - called when timer is stopped
             :param skip_callback: function (current_step) - called when step is incremented
             :param buttons_on_top: bool - True to put buttons on top, or False for bottom
+            :param buttons_padx_weight: int - weight of padding for PlayerButtons
             :param value_display_fact: int - pushed only to SimpleScrollBar
         '''
         self.__callback = callback
         self.__end_callback = end_callback
         self.__frame_rate = frame_rate
         self.__step_increment = step_increment
         super().__init__(master, bg=bg)
@@ -68,15 +69,16 @@
             self.__Slider = DoubleScrollBar(self, self.__slider_update, None, frame_num,
                                             min_frame=0, start_frame=0, frame_rate=self.__frame_rate,
                                             bg=bg)
         self.__Slider.pack(side=slider_side, fill='x')
 
         self.__Buttons = PlayerButtons(self, bg, self.__Timer.start, self.__Timer.stop,
                                        self.step_forward, self.step_back,
-                                       self.__Timer.to_end, self.__Timer.reset)
+                                       self.__Timer.to_end, self.__Timer.reset,
+                                       padx_weight=buttons_padx_weight)
         self.__Buttons.pack(side=buttons_side, fill='x')
 
     def start(self):
         '''starts player - called externally - not from buttons'''
         self.__Timer.start()
         self.__Buttons.to_stop()
 
@@ -149,10 +151,11 @@
 
     def __end(self):
         '''called when player reaches the end (max step)'''
         if self.__Buttons.is_looped():
             self.__Timer.reset()
             self.__Timer.start()
         else: # no loop - actually stopping
+            self.__Buttons.to_play()
             if self.__end_callback is not None:
                 self.__end_callback()
-        
+
```

### Comparing `chichitk-0.0.1/chichitk/progress_bar.py` & `chichitk-0.0.2/chichitk/progress_bar.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.1/chichitk/scrollable_frame.py` & `chichitk-0.0.2/chichitk/scrollable_frame.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.1/chichitk/sliders.py` & `chichitk-0.0.2/chichitk/sliders.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,39 +746,41 @@
         self.command = command # function acception 1 numeric argument
         self.active_fill_callback = active_fill_callback
         self.label = label # can be none to display no label
         self.mouse_wheel_steps = mouse_wheel_steps
         self.height, self.padx = height, padx
         self.active_color, self.inactive_color, self.hover_color = active_color, inactive_color, hover_color
         self.font_name, self.label_font_size, self.tick_font_size = font_name, label_font_size, tick_font_size
-        self.label_line_id, self.x_label_id, self.width = [None] * 3
-        self.ticks, self.labels = [], []
         self.show_fill, self.active_fill = show_fill, active_fill
         self.confine_to_active_region = confine_to_active_region
         self.hovering, self.dragging = False, False
         self.frame_rate = frame_rate
         self.active_x0, self.active_x1 = active_x0, active_x1 # frames
         self.current_frame, self.min_frame, self.max_frame = start_frame, min_frame, frames
         self.min_seconds, self.max_seconds = self.min_frame / frame_rate, self.max_frame / frame_rate
+        self.width = None
         if self.label:
             self.label_line_height, self.tick_height = height * 0.5, height * 0.59
         else:
             self.label_line_height, self.tick_height = height * 0.65, height * 0.76
         self.divisions = np.array([1/2**i for i in range(4, 0, -1)] + [1, 2, 5, 10, 25, 50, 100]) # smallest is 0.0625 (1/16)
 
         if self.show_fill:
             self.Fill = CanvasEditFill(self, 'sb_fill', 0, 0, 0, self.label_line_height, line_width=2, bg=active_fill_color,
                                        main_text_hover_justify='center', main_text=fill_text, selectable=False, hoverable=True,
                                        box_draggable='horizontal', left_draggable=active_fill, right_draggable=active_fill,
                                        left_drag_function=self.active_drag0, right_drag_function=self.active_drag1,
                                        box_drag_function=self.active_drag, brighten_fact=0, raise_on_click=False,
                                        active=active and self.active_fill)
-        self.Line = CanvasEditLine(self, 0, 0, self.label_line_height, width=6, bg=self.inactive_color, drag_color=self.active_color,
-                                   hover_color=self.hover_color, selectable=False, hoverable=True, draggable=True, show_drag_color=True,
-                                   drag_function=self.main_drag, active=active)
+        self.Line = CanvasEditLine(self, 0, 0, self.label_line_height, width=6,
+                                   bg=self.inactive_color, drag_color=self.active_color,
+                                   hover_color=self.hover_color, selectable=False,
+                                   hoverable=True, draggable=True, deletable=False,
+                                   show_drag_color=True, drag_function=self.main_drag,
+                                   active=active)
 
         self.bind('<Configure>', self.frame_width)
         self.bind('<MouseWheel>', self.mouse_wheel_scroll)
         self.event_generate('<Configure>', when='tail')
 
     def frame_width(self, event):
         '''called whenever window is resized'''
@@ -1020,51 +1022,45 @@
         if self.confine_to_active_region: # do not allow user to move scrollbar outside of active region
             frame = min(self.active_x1 - 1, max(self.active_x0 + 1, frame))
         self.set_frame(frame)
         self.command(self.current_frame - 1)
 
     def remove(self):
         '''removes all labels and ticks from the x axis'''
-        if self.label_line_id:
-            self.delete(self.label_line_id)
-            self.label_line_id = None
-        if self.x_label_id:
-            self.delete(self.x_label_id)
-            self.x_label_id = None
-        for id in self.ticks:
-            self.delete(id)
-        self.ticks = []
-        for id in self.labels:
-            self.delete(id)
-        self.labels = []
+        # deletes everything except line and active fill
+        for i in self.find_all():
+            if i != self.Line.id and (not self.show_fill or i != self.Fill.box_id):
+                self.delete(i)
 
     def draw(self, max_ticks=15, tick_x_buffer=0.01):
         '''draws label line and ticks/labels on canvas
         updates position of main scroll line and active region fill'''
         if not self.width:
             # width will not be set for sliders on subsequent pages that have not be loaded yet
             return None
         self.remove()
         self.update_line_x()
         self.update_fill_x(callback=False)
-        self.label_line_id = self.create_line(self.xmin, self.label_line_height, self.xmax,
-                                                self.label_line_height, fill='#ffffff', width=1)
+        self.create_line(self.xmin, self.label_line_height, self.xmax,
+                         self.label_line_height, fill='#ffffff', width=1)
         if self.label != None:
-            self.x_label_id = self.create_text(self.width / 2, self.height, text=self.label, fill='#ffffff',
-                                                font=(self.font_name, self.label_font_size), anchor='s')
+            self.create_text(self.width / 2, self.height, text=self.label,
+                             fill='#ffffff', font=(self.font_name, self.label_font_size),
+                             anchor='s')
         
         # draw ticks and labels
         increment = self.divisions[self.divisions > (self.max_seconds - self.min_seconds) / max_ticks].min()
         ticks = np.arange(int(self.min_seconds / increment), int(self.max_seconds / increment) + 1) * increment # in seconds
         for sec, label in zip(ticks, [seconds_text(t) for t in ticks]):
             x = self.xmin + (self.xmax - self.xmin) * (sec - self.min_seconds) / (self.max_seconds - self.min_seconds)
             if x + (self.xmax - self.xmin) * tick_x_buffer >= self.xmin and x - (self.xmax - self.xmin) * tick_x_buffer <= self.xmax:
-                self.ticks.append(self.create_line(x, self.label_line_height, x, self.tick_height, fill='#ffffff', width=1))
-                self.labels.append(self.create_text(x, self.tick_height, text=label, fill='#ffffff',
-                                                    font=(self.font_name, self.tick_font_size), anchor='n'))
+                self.create_line(x, self.label_line_height, x, self.tick_height,
+                                 fill='#ffffff', width=1)
+                self.create_text(x, self.tick_height, text=label, fill='#ffffff',
+                                 font=(self.font_name, self.tick_font_size), anchor='n')
 
 class DoubleScrollBar(Frame):
     ''' Extension of PlotScrollBar that combines to PlotScrollBars to give user
         more precise control
         
         The top scrollbar displays an adjustable active region, which defines
         the bounds of the bottom scrollbar. User can use the bottom scrollbar
@@ -1114,26 +1110,28 @@
                                            active_fill_color=active_fill_color,
                                            bg=bg, show_fill=True, active_fill=active_fill,
                                            fill_text=fill_text, active_x0=active_x0,
                                            active_x1=active_x1, mouse_wheel_steps=mouse_wheel_steps,
                                            font_name=font_name, label_font_size=label_font_size,
                                            tick_font_size=tick_font_size, active=active,
                                            confine_to_active_region=confine_to_active_region,
-                                           active_fill_callback=fill_callback)
+                                           active_fill_callback=fill_callback,
+                                           frame_rate=self.frame_rate)
         self.SecondaryScrollBar = PlotScrollBar(self, self.__secondary_command,
                                                 label, frames=self.MainScrollBar.active_x1,
                                                 min_frame=self.MainScrollBar.active_x0,
                                                 start_frame=start_frame,
                                                 height=secondary_height, padx=padx,
                                                 active_color=active_color, inactive_color=inactive_color,
                                                 hover_color=hover_color, active_fill_color=active_fill_color, bg=bg,
                                                 show_fill=False, active_fill=False,
                                                 mouse_wheel_steps=mouse_wheel_steps,
                                                 font_name=font_name, label_font_size=label_font_size,
-                                                tick_font_size=tick_font_size, active=active)
+                                                tick_font_size=tick_font_size, active=active,
+                                                frame_rate=self.frame_rate)
         self.MainScrollBar.pack(side='top', fill='x')
         self.SecondaryScrollBar.pack(side='top', fill='x')
 
     def get_active_bounds(self, start_frame:int, min_frame:int, max_frame:int, width_perc:float):
         '''returns bounds of active region based
         
         Parameters
```

### Comparing `chichitk-0.0.1/chichitk/temp_menu.py` & `chichitk-0.0.2/chichitk/temp_menu.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.1/chichitk/text_boxes.py` & `chichitk-0.0.2/chichitk/text_boxes.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.1/chichitk/timer.py` & `chichitk-0.0.2/chichitk/timer.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.1/chichitk/tool_tip.py` & `chichitk-0.0.2/chichitk/tool_tip.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.1/chichitk.egg-info/SOURCES.txt` & `chichitk-0.0.2/chichitk.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-setup.py
+LICENSE
+Readme.md
+pyproject.toml
 chichitk/__init__.py
 chichitk/aspect_frame.py
 chichitk/buttons.py
 chichitk/canvas_items.py
 chichitk/dropdowns.py
 chichitk/entry_boxes.py
 chichitk/file_dialog.py
 chichitk/function_progress.py
+chichitk/icons.py
 chichitk/labels.py
 chichitk/pdf_display.py
 chichitk/player.py
 chichitk/progress_bar.py
 chichitk/scrollable_frame.py
 chichitk/sliders.py
 chichitk/temp_menu.py
```

