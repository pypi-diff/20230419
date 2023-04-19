# Comparing `tmp/epkernel-1.1.7-py3-none-win_amd64.whl.zip` & `tmp/epkernel-1.1.8-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 47382 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat     7130 b- defN 23-Feb-03 06:14 epkernel/Application.py
--rw-rw-rw-  2.0 fat   148519 b- defN 23-Feb-07 03:40 epkernel/BASE.py
--rw-rw-rw-  2.0 fat      597 b- defN 23-Feb-07 07:29 epkernel/Configuration.py
+Zip file size: 55042 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat       64 b- defN 23-Apr-18 03:13 epkernel/Analysis.py
+-rw-rw-rw-  2.0 fat     9662 b- defN 23-Apr-18 03:13 epkernel/Application.py
+-rw-rw-rw-  2.0 fat   161283 b- defN 23-Apr-18 03:07 epkernel/BASE.py
+-rw-rw-rw-  2.0 fat     1421 b- defN 23-Apr-18 05:53 epkernel/Configuration.py
 -rw-rw-rw-  2.0 fat      666 b- defN 23-Feb-14 06:00 epkernel/GUI.py
--rw-rw-rw-  2.0 fat     1849 b- defN 22-Dec-14 06:01 epkernel/Input.py
--rw-rw-rw-  2.0 fat    10667 b- defN 23-Feb-07 06:03 epkernel/Output.py
+-rw-rw-rw-  2.0 fat     5625 b- defN 23-Apr-18 03:11 epkernel/Guide.py
+-rw-rw-rw-  2.0 fat     1897 b- defN 23-Apr-18 03:11 epkernel/Input.py
+-rw-rw-rw-  2.0 fat       58 b- defN 22-Nov-16 03:34 epkernel/Optimization.py
+-rw-rw-rw-  2.0 fat    12016 b- defN 23-Apr-18 03:09 epkernel/Output.py
 -rw-rw-rw-  2.0 fat      118 b- defN 22-Nov-16 01:58 epkernel/__init__.py
--rw-rw-rw-  2.0 fat       56 b- defN 22-Nov-16 03:34 epkernel/analysis.py
--rw-rw-rw-  2.0 fat     2738 b- defN 22-Dec-01 07:35 epkernel/epcam.py
--rw-rw-rw-  2.0 fat       58 b- defN 22-Nov-16 03:34 epkernel/optimization.py
--rw-rw-rw-  2.0 fat    37677 b- defN 23-Feb-07 03:33 epkernel/Action/Information.py
--rw-rw-rw-  2.0 fat    12051 b- defN 23-Feb-14 04:03 epkernel/Action/Selection.py
--rw-rw-rw-  2.0 fat     1922 b- defN 22-Nov-16 05:57 epkernel/Edition/Job.py
--rw-rw-rw-  2.0 fat    30022 b- defN 23-Feb-14 03:18 epkernel/Edition/Layers.py
--rw-rw-rw-  2.0 fat     6296 b- defN 23-Feb-07 07:55 epkernel/Edition/Matrix.py
+-rw-rw-rw-  2.0 fat     4760 b- defN 23-Mar-23 05:54 epkernel/epcam.py
+-rw-rw-rw-  2.0 fat    42198 b- defN 23-Apr-18 03:22 epkernel/Action/Information.py
+-rw-rw-rw-  2.0 fat    15089 b- defN 23-Apr-18 03:30 epkernel/Action/Selection.py
+-rw-rw-rw-  2.0 fat     2509 b- defN 23-Apr-18 03:14 epkernel/Edition/Job.py
+-rw-rw-rw-  2.0 fat    35969 b- defN 23-Apr-18 03:21 epkernel/Edition/Layers.py
+-rw-rw-rw-  2.0 fat     9598 b- defN 23-Apr-18 03:21 epkernel/Edition/Matrix.py
 -rw-rw-rw-  2.0 fat     4708 b- defN 22-Nov-29 02:38 epkernel/MI/stackup.py
--rw-rw-rw-  2.0 fat      251 b- defN 23-Feb-14 06:07 epkernel-1.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-Feb-14 06:07 epkernel-1.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Feb-14 06:07 epkernel-1.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1561 b- defN 23-Feb-14 06:07 epkernel-1.1.7.dist-info/RECORD
-20 files, 266993 bytes uncompressed, 44876 bytes compressed:  83.2%
+-rw-rw-rw-  2.0 fat      251 b- defN 23-Apr-18 05:53 epkernel-1.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Apr-18 05:53 epkernel-1.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-18 05:53 epkernel-1.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1636 b- defN 23-Apr-18 05:53 epkernel-1.1.8.dist-info/RECORD
+21 files, 309635 bytes uncompressed, 52426 bytes compressed:  83.1%
```

## zipnote {}

```diff
@@ -1,35 +1,38 @@
+Filename: epkernel/Analysis.py
+Comment: 
+
 Filename: epkernel/Application.py
 Comment: 
 
 Filename: epkernel/BASE.py
 Comment: 
 
 Filename: epkernel/Configuration.py
 Comment: 
 
 Filename: epkernel/GUI.py
 Comment: 
 
-Filename: epkernel/Input.py
+Filename: epkernel/Guide.py
 Comment: 
 
-Filename: epkernel/Output.py
+Filename: epkernel/Input.py
 Comment: 
 
-Filename: epkernel/__init__.py
+Filename: epkernel/Optimization.py
 Comment: 
 
-Filename: epkernel/analysis.py
+Filename: epkernel/Output.py
 Comment: 
 
-Filename: epkernel/epcam.py
+Filename: epkernel/__init__.py
 Comment: 
 
-Filename: epkernel/optimization.py
+Filename: epkernel/epcam.py
 Comment: 
 
 Filename: epkernel/Action/Information.py
 Comment: 
 
 Filename: epkernel/Action/Selection.py
 Comment: 
@@ -42,20 +45,20 @@
 
 Filename: epkernel/Edition/Matrix.py
 Comment: 
 
 Filename: epkernel/MI/stackup.py
 Comment: 
 
-Filename: epkernel-1.1.7.dist-info/METADATA
+Filename: epkernel-1.1.8.dist-info/METADATA
 Comment: 
 
-Filename: epkernel-1.1.7.dist-info/WHEEL
+Filename: epkernel-1.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: epkernel-1.1.7.dist-info/top_level.txt
+Filename: epkernel-1.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: epkernel-1.1.7.dist-info/RECORD
+Filename: epkernel-1.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## epkernel/Application.py

```diff
@@ -1,13 +1,14 @@
 import os, json, tarfile
 from epkernel import Configuration,  GUI, Input, Output, BASE
 from epkernel.Action import Information, Selection
 from epkernel.Edition import Layers, Matrix, Job
 from epkernel.MI import stackup
 import shutil
+import numpy as np
 
 #指定step创建矩形profile
 def create_rect_profile_jwApp(job:str, step:str, xmin:int, ymin:int, xmax:int, ymax:int):
     try:
         Matrix.create_layer(job,'profile__fz')
         Layers.add_line(job, step, ['profile__fz'], 'r1', xmin, ymin, xmin, ymax, True, [])
         Layers.add_line(job, step, ['profile__fz'], 'r1', xmax, ymin, xmax, ymax, True, [])
@@ -98,20 +99,20 @@
         for i in attributes:
             new.append({i: attributes[i]})
         Layers.add_round_surface(job, step, layers, polarity, new,center_x,center_y,radius)
     except Exception as e:
         print(e)
     return 0
 
-def add_text_jwApp(job:str, step:str, layers:list, symbol:str, fontname:str, text:str, xsize:int, ysize:int, linewidth:int, location_x:int, location_y:int,polarity:bool,orient:int,attributes:dict,special_angle:float=0):
+def add_text_jwApp(job:str, step:str, layers:list, fontname:str, text:str, xsize:int, ysize:int, linewidth:int, location_x:int, location_y:int,polarity:bool,orient:int,attributes:dict,special_angle:float=0):
     try:
         new = list()
         for i in attributes:
             new.append({i: attributes[i]})
-        Layers.add_text(job,step,layers,symbol,fontname,text,xsize,ysize,linewidth,location_x,location_y,polarity,orient,new,special_angle)
+        Layers.add_text(job,step,layers,fontname,text,xsize,ysize,linewidth,location_x,location_y,polarity,orient,new,special_angle)
     except Exception as e:
         print(e)
     return 0
 
 def add_line_jwApp(job:str, step:str, layers:list, symbol:str, start_x:int, start_y:int, end_x:int, end_y:int, polarity:bool, attributes:dict):
     try:
         new = list()
@@ -142,59 +143,127 @@
         return matrix_dict
     except Exception as e:
         print(e)
     return {} 
 
 def get_selected_feature_infos_jwApp(job:str, step:str, layer:str)->list:
     try:
-        select = Information.is_selected(job,step,layer)
+        select = Information.has_selected_features(job,step,layer)
         if select == True:
             ret = Information.get_selected_features_infos(job,step,layer)
         else:
             ret = Information.get_all_features_info(job,step,layer)
         return ret
     except Exception as e:
         print(e)
     return []
 
 def get_selected_symbol_info_jwApp(job:str, step:str, layer:str)->dict:
     try:
-        select = Information.is_selected(job, step, layer)
+        select = Information.has_selected_features(job, step, layer)
         if select == True:
             ret = Information.get_selected_symbol_info(job, step, layer)
         else:
             ret = Information.get_all_symbol_info(job, step, layer)
         return ret
     except Exception as e:
         print(e)
     return {}
-     
-def add_pad_jwApp(job:str, step:str, layers:list, symbol:str, location_x:int, location_y:int, polarity:bool, orient:int, attributes:dict,nx=1,ny=1,dx=0,dy=0,special_angle = 0):
+
+#增加了自动更新symbol的功能     
+def add_pad_jwApp(job:str, step:str, layers:list, symbol:str, location_x:int, location_y:int, polarity:bool, orient:int, attributes:dict,nx:int=1,ny:int=1,dx:int=0,dy:int=0,special_angle:float = 0):
     try:
         new = list()
         for i in attributes:
             new.append({i: attributes[i]})
         for m in range(0,nx):
             for n in range(0,ny):
                 location_x1 = location_x + dx*m
                 location_y1 = location_y + dy*n
                 Layers.add_pad(job, step, layers, symbol, location_x1, location_y1, polarity, orient, new,special_angle)
     except Exception as e:
         print(e)
     return 0
 
-def sr_tab_add(job:str, step:str, child_steps:list):
+#操作拼版
+def sr_tab_add_jwApp(job:str, step:str, child_steps:list):
     try:
-        info = Information.get_step_info(job, step)
+        info = Information.get_sr_step_info(job, step)
         info.append(child_steps)
         Layers.step_repeat(job, step, info)
     except Exception as e:
         print(e)
     return 0
 
+def rename_layer_jwApp(job:str,old_name:str,new_name:str):
+    try:
+        info = Information.get_layer_information(job)
+        for i in info:
+            if i['name'] == old_name:
+                context = i['context']
+                type = i['type']
+                polarity = i['polarity']
+                if polarity == 'positive':
+                    polarity = True
+                else:
+                    polarity = False
+                Matrix.change_matrix_row(job,old_name,context,type,new_name,polarity)
+    except Exception as e:
+        print(e)
 
+def has_usersymbol_jwApp(job:str,symbolname:str)->bool:
+    try:
+        usersymbol_list = Information.get_usersymbol_list(job)
+        for usersymbol in usersymbol_list:
+            if usersymbol  == symbolname:
+                return True
+    except Exception as e:
+        print(e)
+    return False
 
-
-
+def get_selected_features_box_jwApp(job:str, step:str, layers:list)->dict:
+    try:
+        has_selected = False
+        for layer in layers:
+            selected = Information.has_selected_features(job,step,layer)
+            if selected == True:
+                has_selected = True
+        if has_selected == True:
+            box = Information.get_selected_features_box(job,step,layers)
+        else:
+            box = BASE.layer_box(job,step,layers)
+            box = json.loads(box)['paras']
+        return box
+    except Exception as e:
+        print(e)
+        return {}
+
+def save_partial_steps_jwApp(job:str,steps:list,path:str)->bool:
+    try:
+        jobname = job+'backup'
+        Job.create_job(jobname)
+        Job.copy_job(job,jobname)
+        Job.rename_job(job,'jobtest')
+        stepnames = Information.get_steps(jobname)
+        for stepname in stepnames:
+            if stepname not in steps:
+                Matrix.delete_step(jobname,stepname)
+        Job.rename_job(jobname,job)
+        save = Output.save_job(job,path)
+        Job.close_job(job)
+        Job.rename_job('jobtest',job)
+        return save
+    except Exception as e:
+        print(e)
+        return False
+
+def sr_tab_delete_jwApp(job:str,step:str,indexes:list):
+    try:
+        index = (np.array(indexes)-1).tolist()
+        info = Information.get_sr_step_info(job, step)
+        infos = np.delete(info,index).tolist()
+        Layers.step_repeat(job, step, infos)
+    except Exception as e:
+        print(e)
```

## epkernel/BASE.py

```diff
@@ -97,33 +97,36 @@
     data = {
         'func': 'GET_SELECT_PARAM',
         'paras': {}
     }
     return epcam.process(json.dumps(data))
 
 #设置新的筛选条件    profile_value//0: all 1: in  2: out
-def set_select_param(featuretypes, has_symbols, symbols, minline, maxline, dcode, attributes_flag, attributes_value, 
-                        profile_value, use_selection,use_symbol_range=False,symbol_range={},use_attr_range=False,attr_range={}):
+def set_select_param(featuretypes, has_symbols, symbols,  dcode, attributes_flag, attributes_value, 
+                        profile_value, use_selection,use_symbol_range=False,symbol_range={},use_attr_range=False,attr_range=[],
+                        exclude_attributes_value=[],exclude_attr_ranges=[]):
     data = {
         'func': 'SET_SELECT_PARAM',
         'paras': {'param':{
                   'featuretypes': featuretypes, 
                   'has_symbols': has_symbols, 
                   'symbols': symbols, 
-                  'minline': minline,
-                  'maxline': maxline,
+                #   'minline': minline,
+                #   'maxline': maxline,
                   'dcode': dcode,
                   'attributes_flag': attributes_flag,
                   'attributes_value': attributes_value,
                   'profile_value': profile_value,
                   'use_selection': use_selection,
                   'use_symbol_range':use_symbol_range,
                   'symbol_range':symbol_range,
                   'use_attr_range':use_attr_range,
-                  'attr_range':attr_range
+                  'attr_range':attr_range,
+                  'exclude_attributes_value':exclude_attributes_value,
+                  'exclude_attr_ranges':exclude_attr_ranges
                   }
                   }
     }
     #print(json.dumps(data))
     epcam.process(json.dumps(data))
 
 #创建新层
@@ -236,16 +239,16 @@
                   'step': step, 
                   'layer': layer}
     }
     ret = epcam.process(json.dumps(data))
     return ret
 
 def filter_by_mode(jobname, step, layer, reference_layers, mode, feature_type_ref, symbolflag , symbolnames, 
-                    use_symbol_range=False,symbol_range={},use_attr_range=False,attr_range={},attrflag = -1,
-                    attrlogic = 0, attributes = []):
+                    attrflag = -1,attrlogic = 0, attributes = [],use_symbol_range=False,symbol_range={},
+                    use_attr_range=False,attr_range={}):
     data = {
         'func': 'FILTER_BY_MODE',
         'paras': {'jobname': jobname, 
                   'step': step, 
                   'layer': layer,
                   'reference_layers': reference_layers, 
                   'mode': mode, 
@@ -2177,35 +2180,65 @@
                         'step': step
                         }                    
             } 
     js = json.dumps(data)
     #print(js)
     return epcam.process(json.dumps(data))
 
-def fill_profile(job,step,layer,profile_resize,child_profile_resize,avoid_drill_size,fill_by_pattern,symbolname,dx,dy,avoid_drill=True):
+# def fill_profile(job,step,layer,profile_resize,child_profile_resize,avoid_drill_size,fill_by_pattern,symbolname,dx,dy,avoid_drill=True):
+#     data = {
+#             'func': 'FILL_PROFILE',
+#             'paras': {
+#                         'job': job,
+#                         'step': step,
+#                         'layer':layer,
+#                         'profile_resize':profile_resize,
+#                         'child_profile_resize':child_profile_resize,
+#                         'avoid_drill_size':avoid_drill_size,
+#                         'fill_by_pattern':fill_by_pattern,  #是否选择自己的symbol填充profile true or false
+#                         'symbolname':symbolname,            #fill_by_pattern为false，symbolname填空
+#                         'dx':dx,
+#                         'dy':dy,
+#                         'avoid_drill':avoid_drill
+#                         }                    
+#             } 
+#     js = json.dumps(data)
+#     #print(js)
+#     return epcam.process(json.dumps(data))
+
+def fill_profile(job,step,layers,step_repeat_nesting,nesting_child_steps,step_margin_x,step_margin_y,max_distance_x,
+                 max_distance_y,SR_step_margin_x,SR_step_margin_y,SR_max_distance_x,SR_max_distance_y,avoid_drill,
+                 avoid_rout,avoid_feature,polarity):
     data = {
             'func': 'FILL_PROFILE',
             'paras': {
                         'job': job,
                         'step': step,
-                        'layer':layer,
-                        'profile_resize':profile_resize,
-                        'child_profile_resize':child_profile_resize,
-                        'avoid_drill_size':avoid_drill_size,
-                        'fill_by_pattern':fill_by_pattern,  #是否选择自己的symbol填充profile true or false
-                        'symbolname':symbolname,            #fill_by_pattern为false，symbolname填空
-                        'dx':dx,
-                        'dy':dy,
-                        'avoid_drill':avoid_drill
+                        'layers':layers,
+                        'step_repeat_nesting':step_repeat_nesting,
+                        'nesting_child_steps':nesting_child_steps,
+                        'step_margin_x':step_margin_x,
+                        'step_margin_y':step_margin_y,  
+                        'max_distance_x':max_distance_x,           
+                        'max_distance_y':max_distance_y,
+                        'SR_step_margin_x':SR_step_margin_x,
+                        'SR_step_margin_y':SR_step_margin_y,
+                        'SR_max_distance_x':SR_max_distance_x,
+                        'SR_max_distance_y':SR_max_distance_y,
+                        'avoid_drill':avoid_drill,
+                        'avoid_rout':avoid_rout,
+                        'avoid_feature':avoid_feature,
+                        'polarity':polarity
                         }                    
             } 
     js = json.dumps(data)
     #print(js)
     return epcam.process(json.dumps(data))
 
+
 def use_pattern_fill_contours(jobname,stepname,layername,symbolname,dx,dy,break_partial,cut_primitive,origin_point,outline,outlinewidth,outline_invert,odd_offset = 0,even_offset = 0):
     data = {
             'func': 'USE_PATTERN_FILL_CONTOURS',
             'paras': {
                         'jobname': jobname,
                         'stepname': stepname,
                         'layername':layername,
@@ -2637,15 +2670,15 @@
 
 def use_solid_fill_contours(jobname, stepname, layernames, solid_type, min_brush, use_arcs):
     data = {      
             "func": "USE_SOLID_FILL_CONTOURS",
             "paras":{
                         "jobname":jobname,
                         "stepname":stepname,
-                        "layernames":layernames,
+                        "_layernames":layernames,
                         "solid_type":solid_type,
                         "min_brush":min_brush,
                         "use_arcs":use_arcs
                         }
             }
     js = json.dumps(data)
     print(js)
@@ -3401,34 +3434,39 @@
             "disLayer":disLayer,
             "mode":mode            
         }
     }
     return epcam.process(json.dumps(data))
 
 # 绕pointx,pointy顺时针旋转
-def Srotate(angle:float, valuex:float, valuey:float, pointx:float, pointy:float):
+def Srotate(angle:int, valuex:int, valuey:int, pointx:int, pointy:int):
     if angle %180 != 0:
         sin = math.sin(math.radians(angle))
         cos = math.sqrt(1-sin**2)
     else:
         cos = math.cos(math.radians(angle))
         sin = math.sqrt(1-cos**2)
     sRotatex = (valuex-pointx)*cos + (valuey-pointy)*sin + pointx
     sRotatey = (valuey-pointy)*cos - (valuex-pointx)*sin + pointy
     return sRotatex,sRotatey
 # 坐标平移
-def Move(x:float, y:float, delta_x:float, delta_y:float):
+def Move(x:int, y:int, delta_x:int, delta_y:int):
     end_x = delta_x+x
     end_y = delta_y+y
     return (end_x, end_y)
 # 水平镜像
-def mirror_y(point_x:float, point_y:float):
-    end_x = -point_x
-    end_y = point_y
-    return (end_x, end_y)
+def mirror_y(point_x:int, point_y:int,datum_x:int):
+    dx = point_x-datum_x
+    if dx>0:
+        end_x = datum_x-dx
+    elif dx<0:
+        end_x = datum_x-dx
+    elif dx == 0:
+        end_x = datum_x
+    return (end_x, point_y)
 # 坐标缩放(sx、sy为缩放系数0-1表示缩小，大于1表示扩大)(px、py为基准点坐标)
 def scale(x:float, y:float, sx:float, sy:float, px:float, py:float):
     # x = inch2nm(x)
     # y = inch2nm(y)
     end_x = x*sx + px*(1-sx)
     end_y = y*sy + py*(1-sy)
     # end_x = nm2inch(end_x)
@@ -3474,60 +3512,54 @@
     if zeroes == 0:
         pass
     else:
         if c < number_format_r:
             d2 = d2.ljust(number_format_r, '0')
     return (d1,d2)
 # 槽孔数据
-def slotLenth(job:str, step:str, layer:str, location:dict, unit:bool, angle:float, mirror:bool, number_format_l:int, number_format_r:int, zeroes:int, pointx:float, pointy:float, delta_x:float, delta_y:float, x_scale:float, y_scale:float):
-    location_x = location['X']
-    location_y = location['Y']
-    selectpolygon=[]
-    min = 1 #nm
-    selectpolygon.append([location_x-min,location_y-min])
-    selectpolygon.append([location_x+min,location_y-min])
-    selectpolygon.append([location_x+min,location_y+min])
-    selectpolygon.append([location_x-min,location_y+min])
-    selectpolygon.append([location_x-min,location_y-min])
-    select_feature(job, step, layer, selectpolygon,{},0,True)
-    ret = get_selected_feature_infos(job, step, layer)
-    info = json.loads(ret)['paras']
-    # info = Information.get_selected_features_infos(job, step, layer)
-    for n in info:
-        xs,ys,xe,ye = n['XS'],n['YS'],n['XE'],n['YE']
-        if unit == False:
-            xs = inch2mm(xs)
-            ys = inch2mm(ys)
-            xe = inch2mm(xe)
-            ye = inch2mm(ye)
-        if angle !=0:
-            xs,ys = Srotate(angle,xs,ys,pointx,pointy)
-            xe,ye = Srotate(angle,xe,ye,pointx,pointy)
-            xs = round(xs,number_format_r)
-            ys = round(ys,number_format_r)
-            xe = round(xe,number_format_r)
-            ye = round(ye,number_format_r)
-        if mirror ==True:
-            xs,ys = mirror_y(xs,ys)
-            xe,ye = mirror_y(xe,ye)  
-        if delta_x != 0 or delta_y != 0:
-            xs,ys = Move(xs,ys,delta_x,delta_y)
-            xe,ye = Move(xe,ye,delta_x,delta_y)
-        if x_scale != 1 or y_scale != 1:
-            xs,ys = scale(xs,ys,x_scale,y_scale,pointx,pointy)
-            xe,ye = scale(xe,ye,x_scale,y_scale,pointx,pointy)
-        xs = data_processing(xs,number_format_l,number_format_r,zeroes)
-        ys = data_processing(ys,number_format_l,number_format_r,zeroes)
-        xe = data_processing(xe,number_format_l,number_format_r,zeroes)
-        ye = data_processing(ye,number_format_l,number_format_r,zeroes)
-        xs = 'X'+xs[0]+xs[1]
-        ys = 'Y'+ys[0]+ys[1]
-        xe = 'X'+xe[0]+xe[1]
-        ye = 'Y'+ye[0]+ye[1]
-        digital = xs+ys+'G85'+xe+ye
+def slotLenth( location:dict, unit:bool, angle:float, mirror:bool, number_format_l:int, number_format_r:int, zeroes:int, pointx:float, pointy:float, delta_x:float, delta_y:float, x_scale:float, y_scale:float):
+    xs = location['X1']
+    xe = location['X2']
+    ys = location['Y1']
+    ye = location['Y2']
+    if unit == False:
+        xs = nm2mm(xs)
+        ys = nm2mm(ys)
+        xe = nm2mm(xe)
+        ye = nm2mm(ye)
+    elif unit == True:
+        xs = nm2inch(xs)
+        ys = nm2inch(ys)
+        xe = nm2inch(xe)
+        ye = nm2inch(ye)
+    if angle !=0:
+        xs,ys = Srotate(angle,xs,ys,pointx,pointy)
+        xe,ye = Srotate(angle,xe,ye,pointx,pointy)
+        xs = round(xs,number_format_r)
+        ys = round(ys,number_format_r)
+        xe = round(xe,number_format_r)
+        ye = round(ye,number_format_r)
+    if mirror ==True:
+        xs,ys = mirror_y(xs,ys,xs)
+        xe,ye = mirror_y(xe,ye,xs)          #根据实际情况修改
+    if delta_x != 0 or delta_y != 0:
+        xs,ys = Move(xs,ys,delta_x,delta_y)
+        xe,ye = Move(xe,ye,delta_x,delta_y)
+    if x_scale != 1 or y_scale != 1:
+        xs,ys = scale(xs,ys,x_scale,y_scale,pointx,pointy)
+        xe,ye = scale(xe,ye,x_scale,y_scale,pointx,pointy)
+    xs = data_processing(xs,number_format_l,number_format_r,zeroes)
+    ys = data_processing(ys,number_format_l,number_format_r,zeroes)
+    xe = data_processing(xe,number_format_l,number_format_r,zeroes)
+    ye = data_processing(ye,number_format_l,number_format_r,zeroes)
+    xs = 'X'+xs[0]+xs[1]
+    ys = 'Y'+ys[0]+ys[1]
+    xe = 'X'+xe[0]+xe[1]
+    ye = 'Y'+ye[0]+ye[1]
+    digital = xs+ys+'G85'+xe+ye
     return digital
 # 圆孔
 def isPad(location:dict, unit:bool, angle:float, mirror:bool, number_format_l:int, number_format_r:int, zeroes:int, pointx:float,pointy:float, delta_x:float, delta_y:float, x_scale:float, y_scale:float):
     x,y = location['X'],location['Y']
     if unit == True:
         x = nm2inch(x)
         y = nm2inch(y)
@@ -3535,74 +3567,26 @@
         x = nm2mm(x)
         y = nm2mm(y)
     if angle != 0:
         x,y = Srotate(angle,x,y,pointx,pointy)
         x = round(x,number_format_r)
         y = round(y,number_format_r)
     if mirror ==True:
-        x,y = mirror_y(x,y)
+        x,y = mirror_y(x,y,x)                 #根据实际情况修改
     if delta_x != 0 or delta_y != 0:
         x,y = Move(x,y,delta_x,delta_y)
     if x_scale != 1 or y_scale != 1:
         x,y = scale(x,y,x_scale,y_scale,pointx,pointy)
     x = data_processing(x,number_format_l,number_format_r,zeroes)
     y = data_processing(y,number_format_l,number_format_r,zeroes)
     x = 'X'+x[0]+x[1]
     y = 'Y'+y[0]+y[1]
     xy = x+y
     return xy
 
-def Deduplication(data):
-    Toc = []        
-    ab = []
-    THolesize = []
-    TSlotLenth = []
-    for b in data:
-        THolesize.append(b['iHoleSize'])
-        TSlotLenth.append(b['iSlotLenth'])
-    for e in range(0,len(data)):
-        if e in ab:
-            pass
-        else:
-            hole = data[e]['iHoleSize']
-            tool = data[e]['iToolIdx']
-            location = data[e]['vLocations']
-            slotlenth = data[e]['iSlotLenth']
-            to_dict = {}
-            # Toc = []
-            if THolesize.count(hole) == 1 or TSlotLenth.count(slotlenth) == 1:
-                to_dict['iToolIdx'] =tool
-                to_dict['iHoleSize'] = hole
-                to_dict['iSlotLenth'] = slotlenth
-                to_dict['vLocations'] = location
-                Toc.append(to_dict)
-                ab.append(e)
-            else:
-                for t in range(e+1,len(data)):
-                    iholesize = data[t]['iHoleSize']
-                    lenth = data[t]['iSlotLenth']
-                    locat = data[t]['vLocations']
-                    if hole == iholesize and t != e and slotlenth == lenth:
-                        location.extend(locat)
-                        location = [dict(t) for t in set([tuple(d.items()) for d in location])]
-                        to_dict = {}
-                        to_dict['iToolIdx'] =tool
-                        to_dict['iHoleSize'] = hole
-                        to_dict['iSlotLenth'] = slotlenth
-                        to_dict['vLocations'] = location
-                        Toc.append(to_dict)
-                        ab.append(t)
-                if to_dict == {}:
-                    to_dict['iToolIdx'] =tool
-                    to_dict['iHoleSize'] = hole
-                    to_dict['iSlotLenth'] = slotlenth
-                    to_dict['vLocations'] = location
-                    Toc.append(to_dict)
-    return Toc
-
 #arc2line
 def arc2lines(job, step, layers,radius,sel_type):
     data = {
         'func': 'ARC2LINES',
         'paras': [
                     {'job': job},
                     {'step': step},
@@ -4438,8 +4422,461 @@
     data = {
         'func': 'NEAR_HOLE_SPLITTER',
         'paras': {'holeSize': holeSize,
                   'holeSpacing': holeSpacing,
                   'inPoints':inPoints
         }
     }
-    return epcam.process(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def _init():
+    global _global_dict
+    _global_dict={}
+
+def set_value(key,value):
+    _global_dict[key]=value
+
+def get_value(key):
+    try:
+        return _global_dict[key]
+    except:
+        print('读取'+key+'失败\r\n')
+
+
+def refresh_joblist(jobname, stepname):
+    data = {
+        'func': 'REFRESH_JOBLIST',
+        'paras': {
+                'jobname': jobname,
+                'stepname':stepname
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.uiprocess(json.dumps(data))
+
+    
+def close_all_layer(jobname, stepname):
+    data = {
+        'func': 'CLOSE_ALL_LAYER',
+        'paras': {
+                'jobname': jobname,
+                'stepname':stepname
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.uiprocess(json.dumps(data))
+
+def display_layers(job, step, clayer = '', snaplayer = '', displaylayers = [], affectedlayers = []):
+    data = {
+        'func': 'DISPLAY_LAYERS',
+        'paras': {
+                'jobname': job,
+                'stepname':step,
+                'clayer':clayer,
+                'snaplayer':snaplayer,
+                'displaylayers':displaylayers,
+                'affectedlayers':affectedlayers
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.uiprocess(json.dumps(data))
+
+def set_layer_infos(job,layerInfo,oldAndNewlayerParams):
+    data = {
+        'func': 'SET_LAYER_INFOS',
+        'paras': {
+                'job': job,
+                'layerInfo':layerInfo,
+                'oldAndNewlayerParams': oldAndNewlayerParams
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+
+def get_fill_param():
+    data = {
+        'func': 'GET_FILL_PARAM',
+        'paras': {
+                
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def set_fill_param(fillType,gridParams,patternParams,solidParams):
+    data = {
+        'func': 'SET_FILL_PARAM',
+        'paras': {
+                'fillType': fillType,
+                'gridParams':gridParams,
+                'patternParams': patternParams,
+                'solidParams': solidParams
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+
+
+def step_flip(job,step):
+    data = {
+        'func': 'STEP_FLIP',
+        'paras': {
+                'job': job,
+                'step':step
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def pcsAnalysis(job, step, path):
+    data = {
+        'cmd': 'pcsAnalysis',
+        'job': job,
+        'step': step,
+        'path': path
+    }  
+    return epcam.pcsAnalysis(json.dumps(data))
+
+def read_auto_matrix_rule(path):
+    data = {
+        'cmd': 'readPathFactoryJson',
+        'path': path
+    }  
+    return epcam.readPathFactoryJson(json.dumps(data))
+
+def read_auto_matrix_template(path):
+    data = {
+        'cmd': 'readPathTemplateConfigJson',
+        'path': path
+    }  
+    return epcam.readPathTemplateConfigJson(json.dumps(data))
+
+def auto_matrix(nameList):
+    data = {
+        'cmd': 'getMatchedLayers',
+        'NameList': nameList
+    }  
+    return epcam.getMatchedLayers(json.dumps(data))
+
+def saveNewMatchRule(matchRule, path, ruleName):
+    data = {
+        'cmd': 'saveNewMatchRule',
+        'MatchRule': matchRule,
+        'path': path,
+        'RuleName': ruleName
+    }  
+    return epcam.saveNewMatchRule(json.dumps(data))
+
+def getSignalLayers(layerInfos):
+    signalLayers = []
+    for v in layerInfos:
+        if v["type"] == "signal":
+            signalLayers.append(v['name'])
+    return signalLayers
+
+def typeMatchLayer2LayerInfo(matchLayers, layerInfos, oldList, newList, signalNames = []):
+    for vv in matchLayers:
+        layerInfo = {}
+        layerInfo['type'] = vv['attr']['type']
+        layerInfo['name'] = vv['newname']
+        layerInfo['context'] = vv['attr']['context']
+        layerInfo['polarity'] = vv['attr']['polarity']
+        layerInfo['start_name'] = ""
+        layerInfo['end_name'] = ""
+        layerInfo['old_name'] = vv['oldname']
+        layerInfo['row'] = len(layerInfos) + 1
+        if vv["LayerType"] == "drill":
+            start_index = vv['attr']['startindex']
+            end_index = vv['attr']['endindex']
+            if (start_index < len(signalNames)) and (end_index < len(signalNames)):
+                layerInfo['start_name'] = signalNames[start_index]
+                layerInfo['end_name'] = signalNames[end_index]
+        #nameMap.append({vv['oldname'] : vv['newname']})
+        oldList.append(vv['oldname'])
+        newList.append(vv['newname'])
+        layerInfos.append(layerInfo)
+
+def matchLayers2LayerInfos(matchLayers):
+    layerInfos = []
+    oldList = []
+    newList = []
+    solderPasteTop = []
+    silkScreenTop = []
+    solderMaskTop = []
+    signalTop = []
+    signalInner = []
+    signalBot = []
+    solderMaskBot = []
+    silkScreenBot = []
+    solderPasteBot = []
+    drill = []
+    for v in matchLayers:
+        if v["LayerType"] == "solder-paste-top":
+            solderPasteTop = v['MatchedLayer']
+        if v["LayerType"] == "silk-screen-top":
+            silkScreenTop = v['MatchedLayer']
+        if v["LayerType"] == "solder-mask-top":
+            solderMaskTop = v['MatchedLayer']
+        if v["LayerType"] == "signal-top":
+            signalTop = v['MatchedLayer']
+        if v["LayerType"] == "signal-inner":
+            signalInner = v['MatchedLayer']
+        if v["LayerType"] == "signal-bot":
+            signalBot = v['MatchedLayer']
+        if v["LayerType"] == "solder-mask-bot":
+            solderMaskBot = v['MatchedLayer']
+        if v["LayerType"] == "silk-screen-bot":
+            silkScreenBot = v['MatchedLayer']
+        if v["LayerType"] == "solder-paste-bot":
+            solderPasteBot = v['MatchedLayer']
+        if v["LayerType"] == "drill":
+            drill = v['MatchedLayer']
+    typeMatchLayer2LayerInfo(solderPasteTop, layerInfos, oldList, newList)
+    typeMatchLayer2LayerInfo(silkScreenTop, layerInfos, oldList, newList)
+    typeMatchLayer2LayerInfo(solderMaskTop, layerInfos, oldList, newList)
+    typeMatchLayer2LayerInfo(signalTop, layerInfos, oldList, newList)
+    typeMatchLayer2LayerInfo(signalInner, layerInfos, oldList, newList)
+    typeMatchLayer2LayerInfo(signalBot, layerInfos, oldList, newList)
+    typeMatchLayer2LayerInfo(solderMaskBot, layerInfos, oldList, newList)
+    typeMatchLayer2LayerInfo(silkScreenBot, layerInfos, oldList, newList)
+    typeMatchLayer2LayerInfo(solderPasteBot, layerInfos, oldList, newList)
+    signalNames = getSignalLayers(layerInfos)
+    typeMatchLayer2LayerInfo(drill, layerInfos, oldList, newList, signalNames)
+    return (layerInfos, oldList, newList)
+
+def get_layer_attributes(job,step,layer):
+    data = {
+        'func': 'GET_LAYER_ATTRIBUTES',
+        'paras': {
+            'job': job, #string
+            'step': step, #string
+            'layer': layer #string
+        }
+    }
+    return epcam.process(json.dumps(data))
+
+def edit_layer_attributes(job,step,layer,edit_mode,edit_attr_name,edit_attr_value):
+    data = {
+        'func': 'EDIT_LAYER_ATTRIBUTES',
+        'paras': {
+            'job': job, #string
+            'step': step, #string
+            'layer': layer, #string
+            'editMode': edit_mode, #int
+            'editAttrName': edit_attr_name,#string
+            'editAttrValue': edit_attr_value #string
+        }
+    }
+    return epcam.process(json.dumps(data))
+
+def get_step_attributes(job,step):
+    data = {
+        'func': 'GET_STEP_ATTRIBUTES',
+        'paras': {
+            'job': job, #string
+            'step': step #string
+        }
+    }
+    return epcam.process(json.dumps(data))
+
+def edit_step_attributes(job,step,edit_mode,edit_attr_name,edit_attr_value):
+    data = {
+        'func': 'EDIT_STEP_ATTRIBUTES',
+        'paras': {
+            'job': job, #string
+            'step': step, #string
+            'editMode': edit_mode, #int
+            'editAttrName': edit_attr_name,#string
+            'editAttrValue': edit_attr_value #string
+        }
+    }
+    return epcam.process(json.dumps(data))
+
+
+def change_to_guide_tool(jobname, stepname, type):
+    data = {
+        'func': 'CHANGE_TO_GUIDE_TOOL',
+        'paras': {
+                'jobname': jobname,
+                'stepname':stepname,
+                'type':type
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.uiprocess(json.dumps(data))
+
+def change_to_last_tool(jobname, stepname):
+    data = {
+        'func': 'CHANGE_TO_LAST_TOOL',
+        'paras': {
+                'jobname': jobname,
+                'stepname':stepname
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.uiprocess(json.dumps(data))
+
+def get_clicked_point(jobname, stepname):
+    data = {
+        'func': 'GET_CLICKED_POINT',
+        'paras': {
+                'jobname': jobname,
+                'stepname':stepname
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.uiprocess(json.dumps(data))
+
+def get_clicked_box(jobname, stepname):
+    data = {
+        'func': 'GET_CLICKED_BOX',
+        'paras': {
+                'jobname': jobname,
+                'stepname':stepname
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.uiprocess(json.dumps(data))
+
+def layer_box(job,step,layers):
+    data = {
+        'func': 'LAYER_BOX',
+        'paras': {
+            'job': job, 
+            'step': step, 
+            'layers': layers
+        }
+    }
+    return epcam.process(json.dumps(data))
+
+def check_rout_output(job,step,layer):
+    data = {
+        'func': 'CHECK_ROUT_OUTPUT',
+        'paras': {
+            'job': job, 
+            'step': step, 
+            'sourceLayer': layer
+        }
+    }
+    # print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def edit_selected_features_attributes(job,step,layer,mode,attributes):
+    data = {
+        'func': 'EDIT_SELECTED_FEATURES_ATTRIBUTES',
+        'paras': {
+            'job': job, 
+            'step': step, 
+            'layer': layer,
+            'mode': mode, 
+            'attributes': attributes
+        }
+    }
+    # print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def get_actived_step_info(job):
+    data = {
+        'func': 'GET_ACTIVED_STEP_INFO',
+        'paras': {
+            'jobname': job    
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.uiprocess(json.dumps(data))
+
+
+def add_chain(job,step,layer,chain_number,first_index,comp,is_CCW,add_plunge,toolsize,rout_flag=0,feed=0,speed=0):
+    data = {
+        'func': 'ADDCHAIN',
+        'paras': {
+            'job': job, 
+            'step': step, 
+            'layer': layer,
+            'chainNumber': chain_number, 
+            'firstIndex': first_index,
+            'comp': comp, 
+            'isCCW': is_CCW, 
+            'addPlunge': add_plunge,
+            'toolSize': toolsize,
+            'routflag': rout_flag, 
+            'feed': feed,
+            'speed': speed
+        }
+    }
+    # print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def get_all_features_report_flattern(job,step,layer):
+    data = {
+        'func': 'GET_ALL_FEATURES_REPORT_FLATTERN',
+        'paras': {
+            'job': job, 
+            'step': step, 
+            'layer': layer       
+        }
+    }
+    # print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+
+def select_features_by_net(job,step,layer,vec_dest_layername,use_select_info,selectpolygon):
+    data = {
+        'func': 'SELECT_FEATURES_BY_NET',
+        'paras': {
+            'jobname': job, 
+            'stepname': step, 
+            'layername': layer,  
+            'vec_dest_layername': vec_dest_layername, 
+            'use_select_info': use_select_info, 
+            'selectpolygon': selectpolygon
+        }
+    }
+    # print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def usersymbol_is_used(job,symbolname):
+    data = {
+        'func': 'USERSYMBOL_IS_USED',
+        'paras': {
+            'job': job, 
+            'symbolName': symbolname
+        }
+    }
+    # print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def delete_usersymbol(job,symbolname):
+    data = {
+        'func': 'DELETE_USERSYMBOL',
+        'paras': {
+            'job': job, 
+            'symbolName': symbolname
+        }
+    }
+    # print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def rename_usersymbol(job,oldname,newname):
+    data = {
+        'func': 'RENAME_USERSYMBOL',
+        'paras': {
+            'job': job, 
+            'oldName': oldname,
+            'newName': newname
+        }
+    }
+    # print(json.dumps(data))
+    return epcam.process(json.dumps(data))
+
+def set_symbol_ui_data(oldstr, unit):
+    data = {
+        'func': 'SET_SYMBOL_UI_DATA',
+        'paras': {
+                'oldstr': oldstr,
+                'unit':unit
+                }   
+    }
+    #print(json.dumps(data))
+    return epcam.uiprocess(json.dumps(data))
```

## epkernel/Configuration.py

```diff
@@ -1,24 +1,57 @@
-import os, sys, json
-from epkernel import epcam, BASE
+import os, sys, json,requests,time
+from epkernel import Input,epcam,BASE
+from epkernel.Action import Information
+
 
 def init(path:str): 
     epcam.init(path)
     BASE.set_config_path(path)
     v = epcam.getVersion()
     version = v['ep_version'] + v['sub_version']
-    if not version == '1.01':
+    if not version == '1.1.3.19':
         print("Epkernel与bin包版本不匹配，请谨慎使用")
 
 def set_sysattr_path(path:str):
     try:
         BASE.set_sysAttr_path(path)
     except Exception as e:
         print(e)
     return 
 
 def set_userattr_path(path:str):
     try:
         BASE.set_userAttr_path(path)
     except Exception as e:
         print(e)
-    return  
+    return    
+    
+def read_auto_matrix_rule(path:str)->dict:
+    try:
+        ccc = BASE.read_auto_matrix_rule(path)
+        return json.loads(ccc)
+    except Exception as e:
+        print(e)
+        return None
+
+def read_auto_matrix_template(path:str)->dict:
+    try:
+        ccc = BASE.read_auto_matrix_template(path)
+        return json.loads(ccc)
+    except Exception as e:
+        print(e)
+        return None
+
+def add_new_match_rule(layer_infos:list, path:str)->dict:
+    try:
+        ruleName=time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(time.time()))
+        ret = BASE.saveNewMatchRule(layer_infos,path,ruleName)
+        ret = json.loads(ret)
+        return ret
+    except Exception as e:
+        print(e)
+    return {}
+
+
+
+
+
```

## epkernel/Input.py

```diff
@@ -1,22 +1,23 @@
 import os, sys, json
 from epkernel import BASE
 from epkernel.Action import Information
 from epkernel.Edition import Job
 
 #打开料号
-def open_job(job:str, path:str):
+def open_job(job:str, path:str)->bool:
     try:
        ret= json.loads(BASE.open_job(path, job))['paras']['status']
        return ret   
     except Exception as e:
         print(e)
         return False
 
-def open_eps(job:str, path:str):
+
+def open_eps(job:str, path:str)->bool:
     try:
         open_jobs = Information.get_opened_jobs()
         if job in open_jobs: #存在
             return False
         else:
             ret = BASE.open_eps(job, path)
             ret_= json.loads(ret)
@@ -30,28 +31,30 @@
                         return False
                     else:
                         return False
     except Exception as e:
         print(e)
     return False
 
+
+
 def file_identify(path:str)->dict:
     try:
         ret = BASE.file_identify(path)
         data = json.loads(ret)
         if 'paras' in data:
             return data['paras']
         return None
     except Exception as e:
         return None
 
 def file_translate(path:str, job:str, step:str, layer:str, param:dict)->bool:
     try:
         file_format = param['format']
-        if file_format == 'Gerber274x' or file_format == 'Excellon2' or file_format == 'DXF':
+        if file_format == 'Gerber274x' or file_format == 'Excellon2' or file_format == 'DXF' or file_format == 'Excellon1':
             ret = BASE.file_translate(path, job, step, layer, param, '', '', '', [])    
             data = json.loads(ret)
             if 'paras' in data:
                 if 'result' in data['paras']:
                     return data['paras']['result']
     except Exception as e:
         return False
```

## epkernel/Output.py

```diff
@@ -1,33 +1,43 @@
 import os, sys, json
 from epkernel import epcam, BASE
 from epkernel.Action import Information,Selection
 
-def save_eps(job:str, path:str):
+def save_eps(job:str, path:str)->bool:
     try:
         filename = os.path.basename(path)
         suffix = os.path.splitext(filename)[1]
         if suffix == '.eps':
             BASE.setJobParameter(job,job)
             BASE.save_eps(job,path)
             return True
         else:
             pass
     except Exception as e:
         print(e)
     return False
 
-def save_gerber( job:str, step:str, layer:str, filename:str,  resize:int, angle:float, scalingX:float, scalingY:float, mirror:bool, rotate:bool, scale:bool, cw:bool,  mirrorpointX:int, mirrorpointY:int, rotatepointX:int, rotatepointY:int, scalepointX:int, scalepointY:int, mirrorX:bool, mirrorY:bool, numberFormatL=2, numberFormatR=6, zeros=2, unit=0):
+
+def save_gerber( job:str, step:str, layer:str, filename:str,  resize:int=0, angle:float=0, 
+                scalingX:float=1, scalingY:float=1, mirror:bool=False, rotate:bool=False, 
+                scale:bool=False, cw:bool=False,  mirrorpointX:int=0, mirrorpointY:int=0, 
+                rotatepointX:int=0, rotatepointY:int=0, scalepointX:int=0, scalepointY:int=0, 
+                mirrorX:bool = False, mirrorY:bool = False, numberFormatL:int=2, 
+                numberFormatR:int=6, zeros:int=0, unit:int=0)->bool:
     try:
         _type = 0
         gdsdbu = 0.01
         profiletop = False
         cutprofile = True
         isReverse = False
         cut_polygon = []
+        if scalingX == 0:
+            scalingX == 1
+        if scalingY == 0:
+            scalingY == 1
         if mirrorX == True and mirrorY ==True:
             mirrordirection = 'XY'
         elif mirrorX==True and mirrorY ==False:
             mirrordirection = 'Y'
         elif mirrorX==False and mirrorY ==True:
             mirrordirection = 'X'
         else:
@@ -42,80 +52,114 @@
         else:
             ret = False
         return ret
     except Exception as e:
         print(e)
     return False
 
-def save_excellon2(job:str, step:str, layer:str, path:str, isMetric:bool, number_format_l=2, number_format_r=6, zeroes=2, unit=0, tool_unit=1, x_scale=1, y_scale=1, x_anchor=0, y_anchor=0):
+def save_excellon2(job:str, step:str, layer:str, path:str, number_format_l:int=2, 
+                   number_format_r:int=6, zeroes:int=2, unit:int=0, tool_unit:int=1, 
+                   x_scale:float=1, y_scale:float=1, x_anchor:int=0, y_anchor:int=0)->bool:
     try:
+        isMetric = unit
         layer_info = Information.get_layer_information(job)
         for i in range(0,len(layer_info)):
             if layer_info[i]['name']==layer and layer_info[i]['context'] == 'board' and layer_info[i]['type'] =='drill':
                 BASE.drill2file(job, step, layer,path,isMetric,number_format_l,number_format_r,
                     zeroes,unit,tool_unit,x_scale,y_scale,x_anchor,y_anchor, manufacator = '', tools_order = [])
                 return True
     except Exception as e:
         print(e)
     return False
 
-def save_rout(job:str, step:str, layer:str, path:str, number_format_l=2,number_format_r=6,zeroes=2,unit=0,tool_unit=1,x_scale=1,y_scale=1,x_anchor=0,y_anchor=0, break_arcs = False):
+
+
+def save_rout(job:str, step:str, layer:str, path:str, number_format_l:int=2,
+              number_format_r:int=6,zeroes:int=2,unit:int=0,tool_unit:int=1,x_scale:float=1,
+              y_scale:float=1,x_anchor:int=0,y_anchor:int=0, break_arcs:bool = False)->dict:
     try:
-        layer_info = Information.get_layer_information(job)
-        for i in range(0,len(layer_info)):
-            if layer_info[i]['name'] == layer and layer_info[i]['context'] == 'board' and layer_info[i]['type'] == 'rout':
-                repeat = BASE.get_all_step_repeat_steps(job,step)
-                data = json.loads(repeat)
-                step_repeat = []
-                if  not data['steps'] == None:
-                    for _step in data['steps']:
-                        step_repeat.append(_step)
-                step_repeat.append(step)
-                can_back = True
-                for j in range(0,len(step_repeat)):
-                    _step = step_repeat[j]
-                    Selection.reverse_select(job, _step, layer)
-                    ret = Information.get_selected_features_infos(job,_step,layer)
-                    if ret == None:
-                        can_back=False
-                        return False
-                    Selection.clear_select(job, _step, layer)
-                    if len(ret) == 0:
-                        can_back=False
-                        return False
-                    for k in range(0,len(ret)):
-                        attribute = ret[k]['attributes']
-                        has_chain = False
-                        for m in range(0,len(attribute)):
-                            if  '.rout_chain' in attribute[m]:
-                                has_chain = True
-                        if  has_chain == False:
-                                can_back=False
-                                return False
-                if can_back==True:
-                    BASE.rout2file(job, step, layer,path,number_format_l,number_format_r,zeroes,unit,tool_unit,x_scale,y_scale,x_anchor,y_anchor, 0, 0, 0, 0, 0, break_arcs)
-                return True
+        check = BASE.check_rout_output(job,step,layer)
+        info = json.loads(check)['paras']
+        errorResult1 = info['checkResult1']['errorResult']
+        errorResult2 = info['checkResult2']['errorResult']
+        errorResult3 = info['checkResult3']['errorResult']
+        error = {}
+        for i in errorResult1:
+            featureinfo = i['featureInfo']
+            if featureinfo != []:
+                infos = featureinfo[:3]
+                infor = []
+                for m in infos:
+                    infor.append(m['feature_index'])
+                error['featureInfo'] = infor
+                error['step'] = i['step']
+                error['errorType'] = 0
+                error['result'] = False
+                break
+        if error == {}:
+            for j in errorResult2:
+                featureinfo = j['featureInfo']
+                if featureinfo != []:
+                    infos = featureinfo[:3]
+                    infor = []
+                    for m in infos:
+                        infor.append(m['feature_index'])
+                    error['featureInfo'] = infor
+                    error['step'] = j['step']
+                    error['errorType'] = 1
+                    error['result'] = False
+                    break
+        if error == {}:
+            for n in errorResult3:
+                featureinfo = n['featureInfo']
+                if featureinfo != []:
+                    infos = featureinfo[:3]
+                    infor = []
+                    for m in infos:
+                        infor.append(m['feature_index'])
+                    error['featureInfo'] = infor
+                    error['step'] = n['step']
+                    error['errorType'] = 2
+                    error['result'] = False
+                    break
+        if error == {}:
+            ret = BASE.rout2file(job, step, layer,path,number_format_l,number_format_r,zeroes,unit,tool_unit,x_scale,y_scale,x_anchor,y_anchor, 0, 0, 0, 0, 0, break_arcs)
+            if 'status' in ret:
+                ret = {'result':False,'errorType':3}
+            else:
+                ret = json.loads(ret)['paras']
+                if ret == True:
+                    ret = {'result':True}
+                else:
+                    ret = {'result':False,'errorType':3}
+            return ret
+        else:
+            return error
     except Exception as e:
         print(e)
-    return False
+    return {}
+
+
+
 
 def save_job(job:str,path:str)->bool:
     try:
         layers = Information.get_layers(job)
         steps = Information.get_steps(job)
         for step in steps:
             for layer in layers:
                 BASE.load_layer(job,step,layer)
         BASE.save_job_as(job,path)
         return True
     except Exception as e:
         print(e)
     return False
 
-def save_dxf(job:str,step:str,layers:list,savePath:str):
+
+def save_dxf(job:str,step:str,layers:list,savePath:str)->bool:
     try:
         _ret = BASE.dxf2file(job,step,layers,savePath)
         ret = json.loads(_ret)['paras']['result']
         return ret
     except Exception as e:
         print(e)
     return False
@@ -142,56 +186,48 @@
             else:
                 ret = False
             return ret
     except Exception as e:
         print(e)
     return False
 
-def save_gds(job:str, step:str, layer:str, filename:str, gdsdbu:float):
+def save_png(job:str, step:str, layers:list, xmin:int, ymin:int, xmax:int, ymax:int, picpath:str, backcolor:list, layercolors:list)->bool:
     try:
-        _type = 1
-        resize = 0
-        angle = 0
-        scalingX = 1
-        scalingY = 1
-        isReverse = False
-        mirror = False
-        rotate = False
-        scale = False
-        profiletop =False
-        cw = False
-        cutprofile =   True
-        mirrorpointX = 0
-        mirrorpointY = 0
-        rotatepointX = 0
-        rotatepointY = 0
-        scalepointX = 0
-        scalepointY = 0
-        mirrordirection = 'X'
-        cut_polygon = []
-        numberFormatL = 2
-        numberFormatR = 6
-        zeros = 0
-        unit = 0
-        _ret = BASE.layer_export(job, step, layer, _type, filename, gdsdbu, resize, angle, scalingX, scalingY, isReverse,
-                    mirror, rotate, scale, profiletop, cw, cutprofile, mirrorpointX, mirrorpointY, rotatepointX,
-                    rotatepointY, scalepointX, scalepointY, mirrordirection, cut_polygon,numberFormatL,numberFormatR,
-                    zeros,unit)
-        ret = json.loads(_ret)['status']
-        if ret == 'true':
-            ret = True
+        (picpath,picname) = os.path.split(picpath)
+        layer_sum = len(layers)
+        color_sum = len(layercolors)
+        back_sum = len(backcolor)
+        b = True
+        if  back_sum != 4:
+            b = False
         else:
-            ret = False
-        return ret
+            if layer_sum != color_sum:
+                b = False
+            else:
+                for i in range(0,color_sum):
+                    color = layercolors[i]
+                    if len(color) != 4:
+                        b = False
+                        break
+        if b == True:
+            _ret = BASE.save_png(job,step,layers,xmin,ymin,xmax,ymax,picpath,picname,backcolor,layercolors)
+            ret = json.loads(_ret)['status']
+            if ret == 'true':
+                ret = True
+            else:
+                ret = False
+            return ret
     except Exception as e:
         print(e)
     return False
 
 # 输出文件
-def save_drill(job:str, step:str,data:list,filename:str, unit:bool, tool_unit:bool, number_format_l:int, number_format_r:int, zeroes:int, x_scale:float, y_scale:float, x_anchor:int, y_anchor:int):
+def save_drill(data:list,filename:str, unit:bool=True, tool_unit:bool=False, 
+               number_format_l:int=2, number_format_r:int=6, zeroes:int=2, 
+               x_scale:float=1, y_scale:float=1, x_anchor:int=0, y_anchor:int=0)->bool:
   try:
     file = open(filename, 'w', encoding = 'utf-8')
     file.write('M48'+'\n')
     if unit == True:
         file.write('INCH')
     else:
         file.write('METRIC')
@@ -221,60 +257,78 @@
         x_anchor = BASE.nm2mm(x_anchor)
         y_anchor = BASE.nm2mm(y_anchor)
     for i in data:
         toolIdx = i['iToolIdx']
         to = str(toolIdx).rjust(2,'0')
         part = 'T'+to
         file.write(part+'\n')
-        iSlotLenth = i['iSlotLenth']
         location = i['vLocations']
-        if iSlotLenth!=0:
-            for j in location:
-                digital = BASE.slotLenth(job, step, 'drill.backup', j, unit, 0, False, number_format_l, number_format_r, zeroes, x_anchor, y_anchor, 0, 0, x_scale, y_scale)
+        vLocations_slots = i['vLocations_slots']
+        if vLocations_slots!=[]:
+            for j in vLocations_slots:
+                digital = BASE.slotLenth(j, unit, 0, False, number_format_l, number_format_r, zeroes, x_anchor, y_anchor, 0, 0, x_scale, y_scale)
                 file.write(digital+'\n')
         else:
             for pad in location:
                 xy = BASE.isPad(pad, unit, 0, False, number_format_l, number_format_r, zeroes, x_anchor, y_anchor, 0, 0, x_scale, y_scale)
                 file.write(xy+'\n')
     file.write('M30')
     file.close()
     print("保存文件成功")
     return True
   except Exception as e:
     print(e)
   return False
 
 
-
-
-def save_png(job:str, step:str, layers:list, xmin:int, ymin:int, xmax:int, ymax:int, picpath:str, backcolor:list, layercolors:list)->bool:
+def save_gds(job:str, step:str, layer:str, filename:str, gdsdbu:float)->bool:
     try:
-        (picpath,picname) = os.path.split(picpath)
-        layer_sum = len(layers)
-        color_sum = len(layercolors)
-        back_sum = len(backcolor)
-        b = True
-        if  back_sum != 4:
-            b = False
+        _type = 1
+        resize = 0
+        angle = 0
+        scalingX = 1
+        scalingY = 1
+        isReverse = False
+        mirror = False
+        rotate = False
+        scale = False
+        profiletop =False
+        cw = False
+        cutprofile =   True
+        mirrorpointX = 0
+        mirrorpointY = 0
+        rotatepointX = 0
+        rotatepointY = 0
+        scalepointX = 0
+        scalepointY = 0
+        mirrordirection = 'X'
+        cut_polygon = []
+        numberFormatL = 2
+        numberFormatR = 6
+        zeros = 0
+        unit = 0
+        _ret = BASE.layer_export(job, step, layer, _type, filename, gdsdbu, resize, angle, scalingX, scalingY, isReverse,
+                    mirror, rotate, scale, profiletop, cw, cutprofile, mirrorpointX, mirrorpointY, rotatepointX,
+                    rotatepointY, scalepointX, scalepointY, mirrordirection, cut_polygon,numberFormatL,numberFormatR,
+                    zeros,unit)
+        ret = json.loads(_ret)['status']
+        if ret == 'true':
+            ret = True
         else:
-            if layer_sum != color_sum:
-                b = False
-            else:
-                for i in range(0,color_sum):
-                    color = layercolors[i]
-                    if len(color) != 4:
-                        b = False
-                        break
-        if b == True:
-            _ret = BASE.save_png(job,step,layers,xmin,ymin,xmax,ymax,picpath,picname,backcolor,layercolors)
-            ret = json.loads(_ret)['status']
-            if ret == 'true':
-                ret = True
-            else:
-                ret = False
-            return ret
+            ret = False
+        return ret
+    except Exception as e:
+        print(e)
+    return False
+
+def save_svg(job:str, step:str, layersinfo:dict, savepath:str)->bool:
+    try:
+        layersinfo = [layersinfo]
+        BASE.save_svg(job, step, layersinfo,savepath)
+        return True
     except Exception as e:
         print(e)
     return False
 
 
 
+
```

## epkernel/epcam.py

```diff
@@ -12,35 +12,51 @@
 #dll = ctypes.cdll.LoadLibrary(pp)
 
 #epbin_path = os.getcwd() + r'py\bin"
 
 dll = None
 dmsdll = None
 vdll = None
+uidll = None
+# dfmdll = None
+matrixdll = None
+bin_path = None
 
 isInit = False
 
 def init(path):
-    bin_path = path
-    os.environ['path'] += (r";" + bin_path)
 
     global dll
     global dmsdll
     global vdll
+    global uidll
+    # global dfmdll
+    global matrixdll
+    global bin_path
+
+    bin_path = path
+    os.environ['path'] += (r";" + bin_path)
 
     dll = ctypes.CDLL(bin_path + r"\EPCAM_CTYPE.dll")
+    uidll = ctypes.CDLL(bin_path + r"\EPCAM_UITYPE.dll")
     dmsdll = ctypes.CDLL(bin_path + r"\DMS_CTYPE.dll")
     vdll = ctypes.CDLL(bin_path + r"\Form_View.dll")
+    # dfmdll = ctypes.CDLL(bin_path + r"\dfmDataAnalysis.dll")
+    matrixdll = ctypes.CDLL(bin_path + r"\AutoMatrix.dll")
 
     dll.process.restype =  ctypes.c_char_p
     dll.init_func_map.restype =  ctypes.c_char_p
     dll.init_orig_func_map.restype =  ctypes.c_char_p
     dll.getVersion.restype =  ctypes.c_char_p
     # dll.getVersion.restype =  ctypes.c_char_p
     dll.process.argtypes = [ctypes.c_char_p]
+    uidll.process.restype =  ctypes.c_char_p
+    uidll.init_ui_func_map.restype =  ctypes.c_char_p
+    # uidll.init_orig_func_map.restype =  ctypes.c_char_p
+    uidll.process.argtypes = [ctypes.c_char_p]
     vdll.init.argtypes = [ctypes.c_char_p]
     vdll.view_cmd.argtypes = [ctypes.c_char_p]
     dmsdll.init.restype = ctypes.c_char_p
     dmsdll.uploadmongo.restype = ctypes.c_char_p
     dmsdll.getParam.restype = ctypes.c_char_p
     dmsdll.downloadjob.restype = ctypes.c_char_p
 
@@ -52,16 +68,24 @@
 
     dmsdll.getOrderInfoByJobName.restype = ctypes.c_char_p
     dmsdll.set_robot_status.restype = ctypes.c_int
     dmsdll.epdms_order_status_update.restype = ctypes.c_char_p
     dmsdll.epdms_flow_status_update.restype = ctypes.c_char_p
     dmsdll.get_mongo_fsname.restype = ctypes.c_char_p
 
+    # dfmdll.pcsAnalysis.restype = ctypes.c_char_p
+
+    matrixdll.readPathFactoryJson.restype = ctypes.c_char_p
+    matrixdll.readPathTemplateConfigJson.restype = ctypes.c_char_p
+    matrixdll.getMatchedLayers.restype = ctypes.c_char_p
+    matrixdll.saveNewMatchRule.restype = ctypes.c_char_p
+
     ret = dll.init_func_map()
     ret = dll.init_orig_func_map()
+    ret = uidll.init_ui_func_map()
     vstring_path = bytes(bin_path, encoding='utf-8')
     vdll.init(vstring_path)
 
     global isInit
     isInit = True
 
     return ret.decode('utf-8')
@@ -90,7 +114,44 @@
     string_vjson = bytes(vjson, encoding='utf-8')
     vdll.view_cmd(string_vjson)
 
 def getVersion():
     ret = dll.getVersion()
     ret = ret.decode('utf-8')
     return json.loads(ret)
+
+def uiprocess(json):
+    json.encode('utf-8')
+    #print(type(json))
+    string_buff = bytes(json, encoding='utf-8')
+    #print(type(string_buff), string_buff)
+    ret = uidll.process(string_buff)
+    #print(ret)
+    return ret.decode('utf-8')
+
+# def pcsAnalysis(vjson):
+#     string_vjson = bytes(vjson, encoding='utf-8')
+#     ret = dfmdll.pcsAnalysis(string_vjson)
+#     return ret.decode('gbk')
+
+def readPathFactoryJson(vjson):
+    string_vjson = bytes(vjson, encoding='utf-8')
+    ret = matrixdll.readPathFactoryJson(string_vjson)
+    return ret.decode('gbk')
+
+def readPathTemplateConfigJson(vjson):
+    string_vjson = bytes(vjson, encoding='utf-8')
+    ret = matrixdll.readPathTemplateConfigJson(string_vjson)
+    return ret.decode('gbk')
+
+def getMatchedLayers(vjson):
+    string_vjson = bytes(vjson, encoding='utf-8')
+    ret = matrixdll.getMatchedLayers(string_vjson)
+    return ret.decode('gbk')
+
+def saveNewMatchRule(vjson):
+    string_vjson = bytes(vjson, encoding='utf-8')
+    ret = matrixdll.saveNewMatchRule(string_vjson)
+    return ret.decode('gbk')
+
+def get_config_path():
+    return bin_path
```

## epkernel/Action/Information.py

```diff
@@ -1,11 +1,11 @@
 import os, sys, json, math
 from epkernel import epcam, BASE
 
-def check_matrix_info(job:str, step='', layers=[])->bool:
+def check_matrix_info(job:str, step:str='', layers:list=[])->bool:
     try:
         if isinstance(job, str) and isinstance(step, str) and isinstance(layers, list):
             open_jobs = get_opened_jobs()
             if job in open_jobs: 
                 if step == '' and layers == []:
                     return False
                 step_lst= get_steps(job)
@@ -26,22 +26,26 @@
             print("请检查填写的参数类型!")
             return False
     except Exception as e:
         return False
         print(e)
     return True
 
-def is_selected(job:str,step:str,layer:str)->bool:
-    ret = BASE.is_selected(job,step,layer)
-    ret = json.loads(ret)
-    if 'result' in ret:
-        return ret['result']
+def has_selected_features(job:str,step:str,layer:str)->bool:
+    try:
+        ret = BASE.is_selected(job,step,layer)
+        ret = json.loads(ret)
+        if 'result' in ret:
+            return ret['result']
+        return False
+    except Exception as e:
+        print(e)
     return False
 
-def get_drill_layer_name(job:str)->list:
+def get_drill_layers(job:str)->list:
     """
     #获取孔层layer名
     :param     job:
     :param     step:
     :return    drill_list:孔层名列表
     :raises    error:
     """
@@ -202,18 +206,22 @@
         ret = json.loads(_ret)['points']
         return ret
     except Exception as e:
         print(e)
     return []
 
 def get_layer_feature_count(job:str, step:str, layer:str)->int:
-    ret = BASE.get_layer_feature_count(job, step, layer)
-    ret = json.loads(ret)
-    if 'featureNum' in ret:
-        return int(ret['featureNum'])
+    try:
+        ret = BASE.get_layer_feature_count(job, step, layer)
+        ret = json.loads(ret)
+        if 'featureNum' in ret:
+            return int(ret['featureNum'])
+        return -1
+    except Exception as e:
+        print(e)
     return -1
 
 def get_steps(job:str)->list:
     try:
         ret = BASE.get_matrix(job)
         data = json.loads(ret)
         steps = data['paras']['steps']
@@ -253,15 +261,20 @@
         info= check_matrix_info(job, step)
         if info:
             ret_= BASE.has_profile(job,step)
             data_= json.loads(ret_)['result']
             if data_:
                 ret = BASE.get_profile_box(job, step)
                 data = json.loads(ret)
-                profile_box = data['paras']
+                box = data['paras']
+                profile_box = {}
+                profile_box['xmax'] = box['Xmax']
+                profile_box['xmin'] = box['Xmin']
+                profile_box['ymax'] = box['Ymax']
+                profile_box['ymin'] = box['Ymin']
                 return profile_box
             print('没有profile!')
             return {}
         return None
     except Exception as e:
         print(e)
     return None
@@ -275,33 +288,32 @@
         xminlist=[]
         yminlist=[]
         xmaxlist=[]
         ymaxlist=[]
         for repeat_info in repeat_infos:
             repeat_infox=repeat_info['X']
             repeat_infoy=repeat_info['Y']
-            set_box=BASE.get_profile_box(job, repeat_info['NAME'])
-            set_box=json.loads(set_box)['paras']
+            set_box=get_profile_box(job, repeat_info['NAME'])
             datum_x=json.loads(BASE.get_step_header_infos(job, repeat_info['NAME']))['x_datum']
             datum_y=json.loads(BASE.get_step_header_infos(job, repeat_info['NAME']))['y_datum']
             x_offset = repeat_infox - datum_x
             y_offset = repeat_infoy - datum_y
             pts=[]
-            pts.append([set_box['Xmin']+x_offset,set_box['Ymin']+y_offset])
-            pts.append([set_box['Xmin']+x_offset,set_box['Ymax']+y_offset])
-            pts.append([set_box['Xmax']+x_offset,set_box['Ymax']+y_offset])
-            pts.append([set_box['Xmax']+x_offset,set_box['Ymin']+y_offset])
-            width=set_box['Xmax']-set_box['Xmin']
-            height=set_box['Ymax']-set_box['Ymin']
+            pts.append([set_box['xmin']+x_offset,set_box['ymin']+y_offset])
+            pts.append([set_box['xmin']+x_offset,set_box['ymax']+y_offset])
+            pts.append([set_box['xmax']+x_offset,set_box['ymax']+y_offset])
+            pts.append([set_box['xmax']+x_offset,set_box['ymin']+y_offset])
+            width=set_box['xmax']-set_box['xmin']
+            height=set_box['ymax']-set_box['ymin']
             if repeat_info['MIRROR']:
                 pts.clear()
-                pts.append([set_box['Xmin']+x_offset-width,set_box['Ymin']+y_offset])
-                pts.append([set_box['Xmin']+x_offset-width,set_box['Ymax']+y_offset])
-                pts.append([set_box['Xmin']+x_offset,set_box['Ymax']+y_offset])
-                pts.append([set_box['Xmin']+x_offset,set_box['Ymin']+y_offset])
+                pts.append([set_box['xmin']+x_offset-width,set_box['ymin']+y_offset])
+                pts.append([set_box['xmin']+x_offset-width,set_box['ymax']+y_offset])
+                pts.append([set_box['xmin']+x_offset,set_box['ymax']+y_offset])
+                pts.append([set_box['xmin']+x_offset,set_box['ymin']+y_offset])
 
             if repeat_info['ANGLE']!=0:
                 value = math.acos(-1) / 180
                 ratio = -1 * repeat_info['ANGLE'] * value
                 if repeat_info['MIRROR']:
                     ratio = -1 * (360-repeat_info['ANGLE']) * value
                 for pt in pts:
@@ -335,20 +347,20 @@
         gSRxmin=xminlist[0]
         gSRymin=yminlist[0]
         gSRxmax=xmaxlist[0]
         gSRymax=ymaxlist[0]
         gSRxcenter = (gSRxmax-gSRxmin)/2
         gSRycenter = (gSRymax-gSRymin)/2
         infos={}
-        infos['gSRxmin']=gSRxmin
-        infos['gSRymin']=gSRymin
-        infos['gSRxmax']=gSRxmax
-        infos['gSRymax']=gSRymax
-        infos['gSRxcenter'] = gSRxcenter
-        infos['gSRycenter'] = gSRycenter
+        infos['xmin']=gSRxmin
+        infos['ymin']=gSRymin
+        infos['xmax']=gSRxmax
+        infos['ymax']=gSRymax
+        infos['xcenter'] = gSRxcenter
+        infos['ycenter'] = gSRycenter
         return infos
     except Exception as e:
         print(e)
     return {}
 
 def get_selected_features_box(job:str, step:str, layers:list)->dict:
     try:
@@ -405,15 +417,15 @@
         featureinfos = []
         if data['paras'] != False:
             return data['paras']
     except Exception as e:
         print(e)
     return None
 
-def get_selected_features_count(job:str, step:str, layer = '')->int:
+def get_selected_features_count(job:str, step:str, layer:str = '')->int:
     try:
         if layer != '':
             count_sum=0
             features_count = get_selected_features_infos(job,step,layer)
             if features_count!=None:
                 count_sum = len(features_count)
             else:
@@ -519,32 +531,72 @@
                     layer_dict['polarity'] = layer_infos[i]['polarity']
                     layer_list.append(layer_dict)
         return layer_list
     except Exception as e:
         print(e)
     return []
 
-def get_step_info(job:str,step:str)->list:
+def get_sr_step_info(job:str,step:str)->list:
     try:
         ret = BASE.get_step_repeat(job,step)
         data = json.loads(ret)
         step_info = data['result']
         step_list = []
         for i in range(0,len(step_info)):
             step_dict = {}
-            step_dict['NAME'] = step_info[i]['NAME']
+            name= step_info[i]['NAME'].lower()
+            step_dict['NAME'] = name
             step_dict['X'] = step_info[i]['X']
             step_dict['Y'] = step_info[i]['Y']
             step_dict['DX'] = step_info[i]['DX']
             step_dict['DY'] = step_info[i]['DY']
             step_dict['NX'] = step_info[i]['NX']
             step_dict['NY'] = step_info[i]['NY']
             step_dict['ANGLE'] = step_info[i]['ANGLE']
             step_dict['MIRROR'] = step_info[i]['MIRROR']
             step_list.append(step_dict)
+        for n in step_list:
+            stepname = n['NAME']
+            angle = n['ANGLE']
+            mirror = n['MIRROR']
+            dx = n['DX']
+            dy = n['DY']
+            nx = n['NX']
+            ny = n['NY']
+            sx = n['X']
+            sy = n['Y']
+            point = get_datum_point(job,stepname)
+            box = get_profile_box(job,stepname)
+            x_datum = point['x_datum']
+            y_datum = point['y_datum']   
+            xMax = box['xmax']
+            xMin = box['xmin']
+            yMax = box['ymax']
+            yMin = box['ymin']          
+            delta_x = sx - x_datum
+            delta_y = sy - y_datum          #子step在panel中的相对位置
+            Minx,Miny = BASE.Srotate(angle,xMin,yMin,x_datum,y_datum)
+            Maxx,Maxy = BASE.Srotate(angle,xMax,yMax,x_datum,y_datum)
+            maxx = Maxx+delta_x
+            maxy = Maxy+delta_y
+            minx = Minx+delta_x
+            miny = Miny+delta_y             
+            if mirror == True:
+                minx,miny = BASE.mirror_y(minx,miny,sx)
+                maxx,maxy = BASE.mirror_y(maxx,maxy,sx)       #子step的box坐标先旋转后平移镜像
+            Max_x = max([maxx,minx])
+            Max_y = max([maxy,miny])
+            Min_x = min([maxx,minx])
+            Min_y = min([maxy,miny])
+            max_x = Max_x+dx*(nx-1)
+            max_y = Max_y+dy*(ny-1)         #根据nx、ny阵列获得整体box坐标
+            n['xmin'] = Min_x
+            n['ymin'] = Min_y
+            n['xmax'] = max_x
+            n['ymax'] = max_y
         return step_list
     except Exception as e:
         print(e)
     return []
 
 def get_sub_steps_name(job:str,step:str)->list:
     try:
@@ -556,77 +608,85 @@
         print(e)
     return []        
 
 def get_layer_information(job:str)->list:
     try:
         _ret = BASE.get_matrix(job)
         data = json.loads(_ret)
-        ret =[]
+        ret = []
         ret = data['paras']['info']
         signal_list = []
-        solder_list = []
-        silk_list = []
-        paste_list = []
-        j = 0
         for j in range(0,len(ret)):
-            if ret[j]['context'] =='board'and ret[j]['type'] == 'signal':
-                signal_list.append(ret[j]['row'])
-            elif ret[j]['context'] =='board'and ret[j]['type'] == 'solder_mask':
-                solder_list.append(ret[j]['row'])
-            elif ret[j]['context'] =='board'and ret[j]['type'] == 'silk_screen':
-                silk_list.append(ret[j]['row'])
-            elif ret[j]['context'] == 'board' and ret[j]['type'] == 'solder_paste':
-                paste_list.append(ret[j]['row'])
+            if ret[j]['context'] == 'board' and ret[j]['type'] == 'signal' or ret[j]['type'] == 'power_ground':
+                signal_list.append(j)  
         b = len(signal_list)
-        b_list = signal_list[1:(b-1)]
-        for i in ret:
-                index = i['row']
-                if index == signal_list[0]:
-                    i['orientation'] = "top_signal"
-                elif index == signal_list[-1]:
-                    i['orientation'] = "bottom_signal"
-                elif (index in b_list):
-                    i['orientation'] = 'inner'
-                elif (index in solder_list):
-                    l1 = abs(signal_list[0]-index) 
-                    l2 = abs(signal_list[-1]-index) 
-                    if l1<l2:
-                        i['orientation'] = 'top_solder_mask'
-                    elif l1>l2:
-                        i['orientation'] = 'bottom_solder_mask'
-                elif (index in silk_list):
-                    l1 = abs(signal_list[0]-index)
-                    l2 = abs(signal_list[-1]-index)
-                    if l1<l2:
-                        i['orientation'] = 'top_silk_screen'
-                    elif l1>l2:
-                        i['orientation'] = 'bottom_silk_screen'
-                elif (index in paste_list):
-                    l1 = abs(signal_list[0]-index)
-                    l2 = abs(signal_list[-1]-index)
-                    if l1<l2:
-                        i['orientation'] = 'top_solder_paste'
-                    elif l1>l2:
-                        i['orientation'] = 'bottom_solder_paste'
+        if signal_list != []:
+            if b == 2:
+                begin = min(signal_list)
+                end = max(signal_list)
+                b_list = []
+            else:
+                b_list = signal_list[1:(b-1)]
+                begin = min(b_list)
+                end = max(b_list)
+            for i in range(0,len(ret)):
+                if ret[i]['context'] == 'misc':
+                    ret[i]['side'] = 'none'
+                    ret[i]['foil_side'] = 'none'
+                elif ret[i]['context'] == 'board' and ret[i]['type'] != 'signal' and ret[i]['type'] != 'power_ground':
+                    if i < begin:
+                        if ret[i]['type'] == 'silk_screen' or ret[i]['type'] == 'solder_mask' or ret[i]['type'] == 'solder_paste':
+                            ret[i]['side'] = 'top'
+                        else:
+                            ret[i]['side'] = 'none'
+                    elif i > end:
+                        if ret[i]['type'] == 'silk_screen' or ret[i]['type'] == 'solder_mask' or ret[i]['type'] == 'solder_paste':
+                            ret[i]['side'] = 'bottom'
+                        else:
+                            ret[i]['side'] = 'none' 
+                    ret[i]['foil_side'] = 'none'
+            ret[signal_list[0]]['side'] = 'top'
+            ret[signal_list[0]]['foil_side'] = 'top'
+            ret[signal_list[-1]]['side'] = 'bottom'
+            ret[signal_list[-1]]['foil_side'] = 'bottom'
+            if b_list != []:
+                if len(b_list) % 2  == 0:
+                    for m in range(begin,end,2):
+                        ret[m]['side'] = 'inner'
+                        ret[m]['foil_side'] = 'top'
+                        m += 1
+                        ret[m]['side'] = 'inner'
+                        ret[m]['foil_side'] = 'bottom'
                 else:
-                    i['orientation'] = ''
+                    for n in range(begin,end,2):
+                        ret[n]['side'] = 'inner'
+                        ret[n]['foil_side'] = 'top'
+                        n += 1
+                        ret[n]['side'] = 'inner'
+                        ret[n]['foil_side'] = 'bottom'  
+                    ret[end]['side'] = 'inner'
+                    ret[end]['foil_side'] = 'top'
+        else:
+            for t in ret:
+                t['side'] = 'none'
+                t['foil_side'] = 'none'
         return ret
     except Exception as e:
         print(e)
     return []
 
 def get_all_selected_features_count(job:str, step:str)->int:
     try:
         sum = 0
         layers = get_layers(job)
         feature_list = []
         feature_dict = {}
         for i in layers:
             layer = i
-            ret = is_selected(job,step,layer)
+            ret = has_selected_features(job,step,layer)
             if ret ==True:
                 count = get_selected_features_count(job,step,layer)
                 sum = sum+count
             else:
                 count = 0
             # feature_dict = {}
             feature_dict[layer] = count
@@ -640,36 +700,41 @@
 def get_drill_info(job:str, step:str, layer:str)->list:
     try:
         layer_info = get_layer_information(job)
         for i in range(0,len(layer_info)):
             if layer_info[i]['name']==layer and layer_info[i]['context'] == 'board' and layer_info[i]['type'] =='drill':
                 data = BASE.get_drill_info(job, step, layer)
                 data = json.loads(data)['paras']['vecDrillTools']
-                BASE.set_drill_info(job,step,layer,data)
-                _ret = BASE.auto_get_drill_info(job,step,layer)
-                ret = json.loads(_ret)['result']['data']['drills']
+                info = json.loads(BASE.set_drill_info(job,step,layer,data))['status']
+                if info == 'true':
+                    _ret = BASE.auto_get_drill_info(job,step,layer)
+                    ret = json.loads(_ret)['result']['data']['drills']
         return ret
     except Exception as e:
         print(e)
     return []
 
 def has_profile(job:str, step:str)->bool:
     try:
         _ret = BASE.has_profile(job, step)
         ret = json.loads(_ret)['result']
         return ret
     except Exception as e:
         print(e)
     return False
 
-def get_all_symbol_info(job:str, step:str, layer:str)->dict:
+def get_all_symbol_info(job:str, step:str, layer:str,sr:bool = False)->dict:
     try:
         BASE.load_layer(job, step, layer)
-        _ret = BASE.get_all_features_report(job,step,layer)
-        ret = json.loads(_ret)['paras']
+        if sr == False:
+            _ret = BASE.get_all_features_report(job,step,layer)
+            ret = json.loads(_ret)['paras']
+        else:
+            _ret = BASE.get_all_features_report_flattern(job,step,layer)
+            ret = json.loads(_ret)['paras']
         return ret
     except Exception as e:
         print(e)
     return {}
 
 def get_layer_report(job:str, layer:str)->dict:
     try:
@@ -688,14 +753,16 @@
                 silk_list.append(ret[j]['row'])
         b = len(signal_list)
         b_list = signal_list[1:(b-1)]
         for i in range(0,len(ret)):
             if ret[i]['name'] == layer:
                 index = ret[i]['row']
                 layer_dict = {}
+                layer_dict['context'] = ret[i]['context']
+                layer_dict['type'] = ret[i]['type']
                 if index == signal_list[0]:
                     layer_dict['location'] = "outer_top"
                 elif index == signal_list[-1]:
                     layer_dict['location'] = "outer_bottom"
                 elif (index in b_list):
                     layer_dict['location'] = 'inner'
                 elif (index in solder_list):
@@ -708,16 +775,16 @@
                 elif (index in silk_list):
                     l1 = abs(signal_list[0]-index)
                     l2 = abs(signal_list[-1]-index)
                     if l1<l2:
                         layer_dict['location'] = 'top'
                     elif l1>l2:
                         layer_dict['location'] = 'bottom'
-                layer_dict['context'] = ret[i]['context']
-                layer_dict['type'] = ret[i]['type']
+                else:
+                    layer_dict['location'] = 'none'
         return layer_dict
     except Exception as e:
         print(e)
     return {}
 
 def get_outerlayer_closest_soldermask(job:str, layer:str)->str:
     try:
@@ -793,19 +860,20 @@
                 break
         for n in range(0,len(ret)):
             if ret[n]['name'] == start or ret[n]['name'] == end:
                 drill_list.append(ret[n]['row'])
                 name_list = list(range(math.ceil(drill_list[0]), math.floor(drill_list[-1]) + 1))
         for m in range(0,len(ret)):
             b = ret[m]['row']
-            if (b in name_list):
-                layer_dict = {}
-                layer_dict['name'] = ret[m]['name']
-                layer_dict['index'] = ret[m]['row']
-                layer_list.append(layer_dict)
+            if b in name_list:
+                if ret[m]['type'] == 'signal' or ret[m]['type'] == 'power_ground':
+                    layer_dict = {}
+                    layer_dict['name'] = ret[m]['name']
+                    layer_dict['index'] = ret[m]['row']
+                    layer_list.append(layer_dict)
         return layer_list
     except Exception as e:
         print(e)
     return []
 
 def get_rout_cross(job:str, layer:str)->list:
     try:
@@ -817,42 +885,47 @@
             if ret[i]['name'] ==layer and ret[i]['context'] == 'board' and ret[i]['type'] == 'rout':
                 start = ret[i]['start_name']
                 end = ret[i]['end_name']
                 break
         for n in range(0,len(ret)):
             if ret[n]['name'] == start or ret[n]['name'] == end:
                 rout_list.append(ret[n]['row'])
-        name_list = list(range(math.ceil(rout_list[0]), math.floor(rout_list[-1]) + 1))
+                name_list = list(range(math.ceil(rout_list[0]), math.floor(rout_list[-1]) + 1))
         for m in range(0,len(ret)):
             b = ret[m]['row']
-            if (b in name_list):
-                layer_dict = {}
-                layer_dict['name'] = ret[m]['name']
-                layer_dict['index'] = ret[m]['row']
-                layer_list.append(layer_dict)
+            if b in name_list:
+                if ret[m]['type'] == 'signal' or ret[m]['type'] == 'power_ground':
+                    layer_dict = {}
+                    layer_dict['name'] = ret[m]['name']
+                    layer_dict['index'] = ret[m]['row']
+                    layer_list.append(layer_dict)
         return layer_list
     except Exception as e:
         print(e)
     return []
 
 def get_datum_point(job:str, step:str)->dict:
     try:
-        _ret = BASE.get_step_header_infos(job,step)
-        ret = json.loads(_ret)
-        point_dict = {}
-        point_dict['x_datum'] = ret['x_datum']
-        point_dict['y_datum'] = ret['y_datum']
-        return point_dict
+        ret = check_matrix_info(job,step,[])
+        if ret == True:
+            data = BASE.get_step_header_infos(job,step)
+            data = json.loads(data)
+            point_dict = {}
+            point_dict['x_datum'] = data['x_datum']
+            point_dict['y_datum'] = data['y_datum']
+            return point_dict
+        else:
+            return None
     except Exception as e:
         print(e)
-    return {}
+    return None
 
 def get_sub_step_info(job:str, step:str)->list:
     try:
-        data = get_step_info(job,step)
+        data = get_sr_step_info(job,step)
         datum_point = []
         # 获取panel中所有pcs、set的基准点坐标，旋转角度、是否镜像
         for s in data:
             nx = s['NX']
             ny = s['NY']
             dx = s['DX']
             dy = s['DY']
@@ -869,15 +942,15 @@
                     point['angle'] = angle
                     point['name'] = step1
                     point['mirror'] = mirror
                     datum_point.append(point)
                     sy = sy+dy
                 sx = sx+dx
                 sy = sy-(dy*ny)
-            info1 = get_step_info(job,step1)
+            info1 = get_sr_step_info(job,step1)
             if info1 != []:
                 for b in info1:
                     for i in range(0,1):
                         step2 = b['NAME']
                         nx1 = b['NX']
                         ny1 = b['NY']
                         sx1 = b['X']
@@ -957,33 +1030,33 @@
             px = t['X']
             py = t['Y']     #edit在panel中基准点的坐标
             an = t['angle']    #edit在panel中的旋转角度
             datum = get_datum_point(job,stepname)             
             p_x = datum['x_datum']
             p_y = datum['y_datum']                 #edit本身的基准点坐标
             set_box = get_profile_box(job,stepname)
-            set_minx = set_box['Xmin']
-            set_miny = set_box['Ymin']
-            set_maxx = set_box['Xmax']
-            set_maxy = set_box['Ymax']               #edit的profile_box
+            set_minx = set_box['xmin']
+            set_miny = set_box['ymin']
+            set_maxx = set_box['xmax']
+            set_maxy = set_box['ymax']               #edit的profile_box
             delta_x = px-p_x
             delta_y = py-p_y
             minx = set_minx
             miny = set_miny
             maxx = set_maxx
             maxy = set_maxy
             if an != 0:
                 minx,miny = BASE.Srotate(an,set_minx,set_miny,p_x,p_y)
                 maxx,maxy = BASE.Srotate(an,set_maxx,set_maxy,p_x,p_y)
             if delta_x != 0 or delta_y != 0:
                 minx,miny = BASE.Move(minx,miny,delta_x,delta_y)
                 maxx,maxy = BASE.Move(maxx,maxy,delta_x,delta_y)
             if mir == True:
-                minx,miny = BASE.mirror_y(minx,miny)
-                maxx,maxy = BASE.mirror_y(maxx,maxy)
+                minx,miny = BASE.mirror_y(minx,miny,px)
+                maxx,maxy = BASE.mirror_y(maxx,maxy,px)
             x_list = [minx,maxx]
             y_list = [miny,maxy]
             xmin = min(x_list)
             ymin = min(y_list)
             xmax = max(x_list)
             ymax = max(y_list)
             # px = BASE.nm2inch(px)
@@ -1031,14 +1104,60 @@
         ret = BASE.get_user_symbol_box(job,userSymbolName)
         ret = json.loads(ret)['paras']
         return ret
     except Exception as e:
         print(e)
     return []
 
+def get_fill_param()->dict:
+    try:
+        _ret = BASE.get_fill_param()
+        ret = json.loads(_ret)['paras']
+        return ret
+    except Exception as e:
+        print(e)
+        return {}
 
+def get_layer_attributes(job:str, step:str,layer:str)->dict:
+    try:
+        _ret = BASE.get_layer_attributes(job,step,layer)
+        ret = json.loads(_ret)['paras']
+        return ret
+    except Exception as e:
+        print(e)
+        return []
+
+def get_step_attributes(job:str, step:str)->dict:
+    try:
+        _ret = BASE.get_step_attributes(job,step)
+        ret = json.loads(_ret)['paras']
+        return ret
+    except Exception as e:
+        print(e)
+        return {}
+
+def check_rout_output(job:str, step:str, layer:str)->dict:
+    try:
+        layersinfo = get_layer_information(job)
+        for info in layersinfo:
+            if info['name'] == layer and info['type'] == 'rout' and info['context'] == 'board':
+                _ret = BASE.check_rout_output(job,step,layer)
+                ret = json.loads(_ret)['paras']
+                return ret
+    except Exception as e:
+        print(e)
+    return {}
+
+def identify_symbol(symbolname:str)->bool:
+    try:
+        _ret = BASE.identify_symbol(symbolname)
+        ret = json.loads(_ret)['result']
+        return ret
+    except Exception as e:
+        print(e)
+    return False
```

## epkernel/Action/Selection.py

```diff
@@ -1,12 +1,13 @@
 import os, sys, json
 import math
 from epkernel import BASE
 from epkernel.Action import Information
 
+
 def set_attribute_filter(logic:int, attribute_list:list):
     """
     #设置属性筛选
     :param     logic:0 ：全部满足  1:有其一
     :param     attribute_list:要设置的属性列表
     :returns   :
     :raise    error:
@@ -30,20 +31,20 @@
         BASE.select_features_by_filter(job, step, layers)
     except Exception as e:
         print(e)
     return 0
 
 def reset_select_filter():
     try:
-        BASE.set_select_param(0x7F, False, [], 0, 0, -1, -1, [], 0, True)
+        BASE.set_select_param(0x7F, False, [], -1, -1, [], 0, True)
     except Exception as e:
         print(e)
     return 0
 
-def clear_select(job:str, step:str, layer = ''):
+def clear_select(job:str, step:str, layer:str = ''):
     try:
         layers = Information.get_layers(job)
         if layer == '':
             for layer in layers:
                 BASE.clear_selected_features(job, step, layer)
         else:
             BASE.clear_selected_features(job, step, layer)
@@ -63,28 +64,26 @@
         select_param = data['paras']['param']
         #print(data)  
         flag = select_param['attributes_flag']
         value = select_param['attributes_value']   
         symbols = select_param['symbols']
         pr_value = select_param['profile_value']
         sele = select_param['use_selection']
-        minline = select_param['minline']
-        maxline = select_param['maxline']
         dcode = select_param['dcode']
         has_symbol = select_param['has_symbols']
         featuretype_list= [positive,negative,text,surface,arc,line,pad]
         for index in range(len(featuretype_list)):
             if featuretype_list[index]==True:
                 featuretype_list[index]=len(featuretype_list)-index-1
             else:
                 featuretype_list[index]=None
         for type_ in featuretype_list:
             if type_!=None:
                 featuretype_sum += math.pow(2,type_)
-        BASE.set_select_param(featuretype_sum, has_symbol, symbols,minline, maxline,dcode, flag,value, pr_value,sele)
+        BASE.set_select_param(featuretype_sum, has_symbol, symbols,dcode, flag,value, pr_value,sele)
     except Exception as e:
         print(e)
         return None
 
 def set_include_symbol_filter(symbol_list:list):
     """
     #设置include symbol筛选
@@ -97,51 +96,16 @@
         data = json.loads(ret)
         select_param = data['paras']['param']
         featuretype = select_param['featuretypes']
         flag = select_param['attributes_flag']
         value = select_param['attributes_value']   
         pr_value = select_param['profile_value']
         sele = select_param['use_selection']
-        minline = select_param['minline']
-        maxline = select_param['maxline']
         dcode = select_param['dcode']
-        symbols = []
-        for j in symbol_list:
-            ss = []
-            s = ''
-            n = ''
-            for i in range(len(j)):
-                if j[i].isdigit() or j[i] == '.':
-                    if not s == '':
-                        ss.append(s)
-                        s = ''
-                    n += j[i]
-                    if i == len(j) - 1:
-                        ss.append(n)
-                        n = ''  
-                else:
-                    s += j[i]
-                    if not n == '':
-                        ss.append(n)
-                        n = ''
-                    if i == len(j) - 1:
-                        ss.append(s)
-                        s = ''
-            cc = ''
-            for d in ss:
-                if d.isdigit() or '.' in d:
-                    if '.' in d:
-                        e1 = d.split('.')[0]
-                        e2 = d.split('.')[1]
-                        if len(e2) < 3:
-                            e2 = e2.ljust(3, '0')
-                        d = e1 + '.' + e2    
-                cc += d
-            symbols.append(cc)
-        BASE.set_select_param(featuretype, True, symbols,minline, maxline,dcode, flag,value, pr_value,sele)
+        BASE.set_select_param(featuretype, True, symbol_list,dcode, flag,value, pr_value,sele)
     except Exception as e:
         print(e)
     return 0
 
 def reverse_select(job:str, step:str, layer:str):
     """
     #反选
@@ -182,19 +146,14 @@
 def select_feature_by_polygon(job:str, step:str, layer:str, selectpolygon:list):
     try:
         BASE.select_feature(job, step, layer, selectpolygon, {}, 1, True) # 1：框选 
     except Exception as e:
         print(e)
     return 0
     
-def create_job(job:str):
-    try:
-        BASE.job_create(job)
-    except Exception as e:
-        print(e)
 
 def select_feature_by_point(job:str, step:str, layer:str, location_x:int,location_y:int):
     try:
         selectpolygon=[]
         min = 1 #nm
         selectpolygon.append([location_x-min,location_y-min])
         selectpolygon.append([location_x+min,location_y-min])
@@ -209,15 +168,14 @@
 #0:all 1:in 2:out
 def set_inprofile_filter(mode:int):
     try:
         ret = BASE.get_select_param()
         data = json.loads(ret)
         select_param = data['paras']['param']
         BASE.set_select_param(select_param['featuretypes'], select_param['has_symbols'], select_param['symbols'], 
-                                select_param['minline'], select_param['maxline'],
                                 select_param['dcode'], select_param['attributes_flag'],
                                 select_param['attributes_value'], mode,
                                 select_param['use_selection'])
     except Exception as e:
         print(e)
     return 0
 
@@ -231,115 +189,197 @@
 def unselect_features_by_filter(job:str, step:str, layers:list):
     try:
         BASE.unselect_features_by_filter(job, step, layers)
     except Exception as e:
         print(e)
     return 
 
-def filter_by_mode(job:str, step:str, layer:str, reference_layers:list, mode:int, positive:bool,negative:bool,text:bool,surface:bool,
-        arc:bool,line:bool,pad:bool, symbolflag:int , symbolnames:list,use_symbol_range=False,symbol_range={},
-        use_attr_range=False,attr_range={}, attrflag = -1,attrlogic = 0, attributes = []):
+def filter_by_mode(job:str, step:str, layer:str, reference_layers:list, mode:int, positive:bool,
+                   negative:bool,text:bool,surface:bool,arc:bool,line:bool,pad:bool, 
+                   symbolflag:int , symbolnames:list, attrflag:int = -1,attrlogic:int = 0, 
+                   attributes:list = [],use_symbol_range:bool=False,symboltype:str='',
+                   symbolrange:list=[],use_attr_range:bool=False,attrtype:str='',
+                   attrrange:list=[]):
     try:
         feature_type_ref=0
         featuretype_list= [positive,negative,text,surface,arc,line,pad]
         for index in range(len(featuretype_list)):
             if featuretype_list[index]==True:
                 featuretype_list[index]=len(featuretype_list)-index-1
             else:
                 featuretype_list[index]=None
         for type_ in featuretype_list:
             if type_!=None:
                 feature_type_ref += math.pow(2,type_)
+
+        dict_new = dict(symbolrange)
+        keys = list(dict_new.keys())
+        key_list = [str(i) for i in keys]
+        value_list = list(dict_new.values())
+        ranges = dict(zip(key_list,value_list))
+        new_list = []
+        for key,value in ranges.items():
+            dict_new = {}
+            dict_new[key] = value
+            new_list.append(dict_new)
+        symbol_range = {}
+        symbol_range['range'] = new_list
+        symbol_range['symbol_type'] = symboltype  
+
+        dict_new1 = dict(attrrange)
+        keys1 = list(dict_new1.keys())
+        key_list1 = [str(i) for i in keys1]
+        value_list1 = list(dict_new1.values())
+        ranges1 = dict(zip(key_list1,value_list1))
+        new_list1 = []
+        for key,value in ranges1.items():
+            dict_new1 = {}
+            dict_new1[key] = value
+            new_list1.append(dict_new1)
+        attr_range = {}
+        attr_range['attr_value_range'] = new_list1
+        attr_range['attr_name'] = attrtype
         BASE.filter_by_mode(job, step, layer, reference_layers, mode, feature_type_ref, symbolflag , symbolnames, 
-                    use_symbol_range,symbol_range,use_attr_range,attr_range,attrflag,attrlogic, attributes)
+                    attrflag ,attrlogic, attributes,use_symbol_range,symbol_range,
+                    use_attr_range,attr_range)
     except Exception as e:
         print(e)
         return None
 
 def set_symbol_filter(has_symbols:bool, symbol_list:list):
     try:
         ret = BASE.get_select_param()
         data = json.loads(ret)
         select_param = data['paras']['param']
         featuretype = select_param['featuretypes']
         flag = select_param['attributes_flag']
         value = select_param['attributes_value']   
         pr_value = select_param['profile_value']
         sele = select_param['use_selection']
-        minline = select_param['minline']
-        maxline = select_param['maxline']
         dcode = select_param['dcode']
-        symbols = []
-        for j in symbol_list:
-            ss = []
-            s = ''
-            n = ''
-            for i in range(len(j)):
-                if j[i].isdigit() or j[i] == '.':
-                    if not s == '':
-                        ss.append(s)
-                        s = ''
-                    n += j[i]
-                    if i == len(j) - 1:
-                        ss.append(n)
-                        n = ''  
-                else:
-                    s += j[i]
-                    if not n == '':
-                        ss.append(n)
-                        n = ''
-                    if i == len(j) - 1:
-                        ss.append(s)
-                        s = ''
-            cc = ''
-            for d in ss:
-                if d.isdigit() or '.' in d:
-                    if '.' in d:
-                        e1 = d.split('.')[0]
-                        e2 = d.split('.')[1]
-                        if len(e2) < 3:
-                            e2 = e2.ljust(3, '0')
-                        d = e1 + '.' + e2    
-                cc += d
-            symbols.append(cc)
-        BASE.set_select_param(featuretype, has_symbols, symbols, minline, maxline, dcode, flag, value, pr_value, sele)
+        BASE.set_select_param(featuretype, has_symbols, symbol_list, dcode, flag, value, pr_value, sele)
     except Exception as e:
         print(e)
     return 0
 
-def set_symbol_range_filter(symbol_range:dict):
-    try:
-        featuretypes=127
-        has_symbols=False
-        symbols=[]
-        minline=0.0
-        maxline=0.0
-        dcode=-1
-        attributes_flag=-1
-        attributes_value=[]
-        profile_value=0
-        use_selection=True
-        BASE.set_select_param(featuretypes,has_symbols,symbols,minline,maxline,dcode,attributes_flag,attributes_value,profile_value,use_selection,True,symbol_range,False,{})
+def set_symbol_range_filter(type:str, range:list):
+    try:
+        ret = BASE.get_select_param()
+        data = json.loads(ret)
+        select_param = data['paras']['param']
+        featuretypes = select_param['featuretypes']
+        attributes_flag = select_param['attributes_flag']
+        attributes_value = select_param['attributes_value']   
+        profile_value = select_param['profile_value']
+        use_selection = select_param['use_selection']
+        dcode = select_param['dcode']
+        has_symbols=select_param['has_symbols']
+        symbols=select_param['symbols']
+        use_attr_range = select_param['use_attr_range']
+        attr_range = select_param['attr_range']
+        exclude_attributes_value = select_param['exclude_attributes_value']
+        exclude_attr_range = select_param['exclude_attr_range']
+        # 合并参数
+        dict_new = dict(range)
+        keys = list(dict_new.keys())
+        key_list = [str(i) for i in keys]
+        value_list = list(dict_new.values())
+        ranges = dict(zip(key_list,value_list))
+        new_list = []
+        for k,v in ranges.items():
+            dict_new = {}
+            dict_new[k] = v
+            new_list.append(dict_new)
+        symbol_range = {}
+        symbol_range['range'] = new_list
+        symbol_range['symbol_type'] = type
+        BASE.set_select_param(featuretypes,has_symbols,symbols,dcode,
+                              attributes_flag,attributes_value,profile_value,use_selection,
+                              True,symbol_range,use_attr_range,attr_range,exclude_attributes_value,exclude_attr_range)
     except Exception as e:
         print(e)
     return None
 
-def set_attr_range_filter(attr_range:dict):
+def set_attr_range_filter(logic:int,attr_range:list):
     try:
-        featuretypes=127
-        has_symbols=False
-        symbols=[]
-        minline=0.0
-        maxline=0.0
-        dcode=-1
-        attributes_flag=-1
-        attributes_value=[]
-        profile_value=0
-        use_selection=True
-        BASE.set_select_param(featuretypes,has_symbols,symbols,minline,maxline,dcode,attributes_flag,attributes_value,profile_value,use_selection,False,{},True,attr_range)
+        ret = BASE.get_select_param()
+        data = json.loads(ret)
+        select_param = data['paras']['param']
+        featuretypes = select_param['featuretypes']
+        attributes_value = select_param['attributes_value']   
+        profile_value = select_param['profile_value']
+        use_selection = select_param['use_selection']
+        dcode = select_param['dcode']
+        has_symbols=select_param['has_symbols']
+        symbols=select_param['symbols']
+        use_symbol_range = select_param['use_symbol_range']
+        symbol_range = select_param['symbol_range']
+        exclude_attributes_value = select_param['exclude_attributes_value']
+        exclude_attr_range = select_param['exclude_attr_range']
+        BASE.set_select_param(featuretypes,has_symbols,symbols,dcode,
+                              logic,attributes_value,profile_value,use_selection,
+                              use_symbol_range,symbol_range,True,attr_range,exclude_attributes_value,exclude_attr_range)
     except Exception as e:
         print(e)
     return None
+
+def set_exclude_attr_filter(attr:list):
+    try:
+        ret = BASE.get_select_param()
+        data = json.loads(ret)
+        select_param = data['paras']['param']
+        featuretypes = select_param['featuretypes']
+        attributes_value = select_param['attributes_value']   
+        profile_value = select_param['profile_value']
+        use_selection = select_param['use_selection']
+        dcode = select_param['dcode']
+        has_symbols=select_param['has_symbols']
+        symbols=select_param['symbols']
+        symbol_range = select_param['symbol_range']
+        attr_range = select_param['attr_range']
+        exclude_attr_range = select_param['exclude_attr_range']
+        use_symbol_range = select_param['use_symbol_range']
+        BASE.set_select_param(featuretypes,has_symbols,symbols,dcode,0,
+                            attributes_value,profile_value,use_selection,use_symbol_range,
+                            symbol_range,True,attr_range,attr,exclude_attr_range)
+    except Exception as e:
+        print(e)
+
+def set_exclude_attr_range_filter(attr_range:list):
+    try:
+        ret = BASE.get_select_param()
+        data = json.loads(ret)
+        select_param = data['paras']['param']
+        featuretypes = select_param['featuretypes']
+        attributes_value = select_param['attributes_value']   
+        profile_value = select_param['profile_value']
+        use_selection = select_param['use_selection']
+        dcode = select_param['dcode']
+        has_symbols=select_param['has_symbols']
+        symbols=select_param['symbols']
+        symbol_range = select_param['symbol_range']
+        include_attr_range = select_param['attr_range']
+        exclude_attributes_value = select_param['exclude_attributes_value']
+        use_symbol_range = select_param['use_symbol_range']
+        BASE.set_select_param(featuretypes, has_symbols, symbols,  dcode, 0, attributes_value, 
+                        profile_value, use_selection,use_symbol_range,symbol_range,True,include_attr_range,
+                        exclude_attributes_value,attr_range)
+    except Exception as e:
+        print(e)
+
+def select_features_by_net(job:str,step:str,layer:str,use_select_info:bool,location_x:int,location_y:int,tolerance:int):
+    try:
+        selectpolygon=[]
+        selectpolygon.append({'ix':location_x-tolerance,'iy':location_y-tolerance})
+        selectpolygon.append({'ix':location_x+tolerance,'iy':location_y-tolerance})
+        selectpolygon.append({'ix':location_x+tolerance,'iy':location_y+tolerance})
+        selectpolygon.append({'ix':location_x-tolerance,'iy':location_y+tolerance})
+        selectpolygon.append({'ix':location_x-tolerance,'iy':location_y-tolerance})
+        BASE.select_features_by_net(job,step,layer,[],use_select_info,selectpolygon)
+    except Exception as e:
+        print(e)
+
+
```

## epkernel/Edition/Job.py

```diff
@@ -1,50 +1,65 @@
 import os, sys, json, re
 from epkernel import BASE
 from epkernel.Action import Information
 
-def delete_job(job:str):
+
+def delete_job(job:str)->None:
     try:
         BASE.job_delete(job)
     except Exception as e:
         print(e)
 
 def create_job(job:str)->bool:
     try:
+        openedjob = Information.get_opened_jobs()
+        if job in openedjob:
+            return False
+        for ch in job:
+            if u'\u4e00' <= ch <= u'\u9fff':
+                return False
         if re.search('((?=[\x20-\x7e]+)[^A-Za-z0-9\_\+\-])',job)!=None or job=='eplib':
             return False
         else:
             ret = json.loads(BASE.job_create(job))['status']
             return bool(ret)
     except Exception as e:
         print(e)
         return False
         
 def rename_job(src_jobname:str, dst_jobname:str)->bool:
     try:
+        openedjob = Information.get_opened_jobs()
+        if dst_jobname in openedjob:
+            return False
         if json.loads(BASE.is_job_open(src_jobname))['paras']['status']== True:
+            # 判断料名中是否有中文
+            for ch in dst_jobname:
+                if u'\u4e00' <= ch <=u'\u9fff':
+                    return False
+            # 判断料号中是否有特殊符号
             if re.search('((?=[\x20-\x7e]+)[^A-Za-z0-9\_\+\-])',dst_jobname)!=None or dst_jobname=='eplib':
                 return False
             else:
                 BASE.job_rename(src_jobname, dst_jobname)
                 return True
     except Exception as e:
         print(e)
         return False
-
+#判断指定料号是否打开       
 def is_job_open(job:str)->bool:
     try:
         _ret= BASE.is_job_open(job)
         ret =json.loads(_ret)['paras']['status']
         return ret
     except Exception as e:
         print(e)
         return False 
 
-#关闭指定料号(job)并清空内存，若不存在该料号名则不执行返回False值
+#关闭指定料号(job)并清空内存,若不存在该料号名则不执行返回False值
 def close_job(job:str)->bool:
     try:
         data= is_job_open(job)
         if data:
             ret_ =BASE.close_job(job)
             ret= json.loads(ret_)['status']
             return ret
@@ -60,7 +75,9 @@
         ret= BASE.copy_job(src_job,dst_job)
         data = json.loads(ret)['paras'][0]
         return data
     except Exception as e:
         print(repr(e))
     return None
 
+
+
```

## epkernel/Edition/Layers.py

```diff
@@ -1,30 +1,32 @@
 import os, sys, json
 from epkernel import BASE
 import math
 from epkernel.Edition import Layers,Matrix
 from epkernel.Action import Selection, Information
 
+
 #将指定层中选中的feature拷贝至目标层，若无选中feature则将指定层资料整层拷贝
-def copy_other(src_job:str, src_step:str, src_layer:str, dst_layer:str, invert:bool, offset_x:int, offset_y:int, mirror:int, resize:float, rotation:float, x_anchor:float, y_anchor:float):
+def copy2other_layer(src_job:str, src_step:str, src_layer:str, dst_layer:str, invert:bool, offset_x:int, 
+                     offset_y:int, mirror:int, resize:float, rotation:float, x_anchor:float, y_anchor:float):
     try:
         BASE.sel_copy_other(src_job, src_step, [src_layer], [dst_layer], invert, offset_x, offset_y, 
                     mirror, resize, rotation, x_anchor, y_anchor)
     except Exception as e:
         print(e)
     return None
 
-def delete_feature(job, step, layers):
+def delete_feature(job:str, step:str, layers:list):
     try:
         BASE.sel_delete(job, step, layers)
     except Exception as e:
         print(e)
     return 0
 
-def change_text(job:str, step:str, layers:list, text:str, font:str, x_size:int, y_size:int, width:int, polarity:bool, mirror:int,angle=0)->None:
+def change_text(job:str, step:str, layers:list, text:str, font:str, x_size:int, y_size:int, width:int, polarity:bool, mirror:int,angle:int=0)->None:
     try:
         if polarity==True:
             polarity=1
         else:
             polarity=-1
         BASE.change_text(job, step, layers, text, font, x_size, y_size, width, polarity, mirror,angle)
     except Exception as e:
@@ -42,15 +44,15 @@
     try:
         layer = ''
         if len(layers) > 0:
             layer = layers[0]
         if polarity==True:
             polarity=1
         else:
-            polarity=0
+            polarity=-1
         BASE.add_line(job, step, layers, layer, symbol, start_x, start_y, end_x, end_y, polarity, 0, attributes)
     except Exception as e:
         print(e)
     return 0
     
 def hierarchy_edit(job:str, step:str, layers:list, mode:int):
     try:
@@ -63,29 +65,29 @@
     try:
         layer = ''
         if len(layers)> 0:
             layer = layers[0]
         if polarity==True:
             polarity=1
         else:
-            polarity=0
+            polarity=-1
         BASE.add_surface(job, step, layers, layer, polarity, 0, False, attributes, points_location)
     except Exception as e:
         print(e)
     return ''
 
 def add_round_surface(job:str, step:str, layers:list, polarity:bool, attributes:list,center_x:int,center_y:int,radius:int)->None:
     try:
         layer = ''
         if len(layers)> 0:
             layer = layers[0]
         if polarity==True:
             polarity=1
         else:
-            polarity=0
+            polarity=-1
         point2_x = center_x + radius
         point2_y = center_y
         points_location = [[point2_x, point2_y],[center_x, center_y]]
         BASE.add_surface(job, step, layers, layer, polarity, 0, True, attributes, points_location)
     except Exception as e:
         print(e)
     return '' 
@@ -100,45 +102,37 @@
 def resize_polyline(job:str, step:str, layers:list, size:float, sel_type:bool):
     try:
         BASE.resize_polyline(job, step, layers, size, sel_type)
     except Exception as e:
         print(e)
     return ''
 
-#将指定料号指定层中选中的feature移动至目标料号下的目标层中，
-def move2other_layer(src_job:str, src_step:str, src_layers:list, dst_job:str, dst_step:str, dst_layer:str, invert:bool, offset_x:int, offset_y:int, mirror:int, resize:float, rotation:float, x_anchor:float, y_anchor:float)->None:
-    try:
-        BASE.sel_move_other(src_job, src_step, src_layers, dst_job, dst_step, dst_layer, invert, offset_x, offset_y, 
-                    mirror, resize, rotation, x_anchor, y_anchor)
-    except Exception as e:
-        print(e)
-    return None
-
 def contourize(job:str, step:str, layers:list, accuracy:int, separate_to_islands:bool, size:int, mode:int):
     try:
+        mode = mode+1
         BASE.contourize(job, step, layers, accuracy, separate_to_islands, size, mode)
     except Exception as e:
         print(e)
     return ''
 
-def add_pad(job:str, step:str, layers:list, symbol:str, location_x:int, location_y:int, polarity:bool, orient:int, attributes:list,special_angle=0)->None:
+def add_pad(job:str, step:str, layers:list, symbol:str, location_x:int, location_y:int, polarity:bool, orient:int, attributes:list,special_angle:float=0)->None:
     try:
         layer=''
         if len(layers)>0:
             layer=layers[0]
         if polarity==True:
             polarity=1
         else:
-            polarity=0
+            polarity=-1
         BASE.add_pad(job, step, layers, layer, symbol, location_x, location_y, polarity, 0, orient,attributes,special_angle)
     except Exception as e:
         print(e)
     return ''
 
-def change_feature_symbols(job:str, step:str, layers:list, symbol:str,pad_angle = False):
+def change_feature_symbols(job:str, step:str, layers:list, symbol:str,pad_angle:bool = False):
     try:
         BASE.change_feature_symbols(job, step, layers, symbol, pad_angle)
     except Exception as e:
         print(e)
     return 0
 
 #将指定料号的step下的指定层的所有feature信息拷贝至目标料号的step下的对应层中
@@ -189,65 +183,59 @@
         BASE.line2pad_new(job, step, layers)
     except Exception as e:
         print(e)
     return 
 
 def modify_attributes(job:str, step:str, layers:list, mode:int, attributes:list):
     try:
-        BASE.modify_attributes(job, step, layers, mode, attributes)
-    except Exception as e:
-        print(e)
-    return 
-
-def use_solid_fill_contours(job:str, step:str, layers:list, solid_type:bool, min_brush=0, use_arcs=False):
-    try:
-        BASE.use_solid_fill_contours(job, step, layers, solid_type, min_brush, use_arcs)
+        for layer in layers:
+            BASE.edit_selected_features_attributes(job, step, layer, mode, attributes)
     except Exception as e:
         print(e)
     return 
 
-def use_pattern_fill_contours(job:str,step:str,layer:str,symbolname:str,dx:float,dy:float,break_partial:bool,cut_primitive:bool,origin_point:bool,outline:bool,outlinewidth = 0,outline_invert = False,odd_offset = 0,even_offset = 0):
+def use_pattern_fill_contours(job:str,step:str,layer:str,symbolname:str,dx:int,dy:int,break_partial:bool,cut_primitive:bool,origin_point:bool,outline:bool,outlinewidth:float = 0,outline_invert:bool = False,odd_offset:int = 0,even_offset:int = 0):
     try:
         BASE.use_pattern_fill_contours(job,step,layer,symbolname,dx,dy,break_partial,cut_primitive,origin_point,outline,outlinewidth,outline_invert,odd_offset,even_offset)
     except Exception as e:
         print(e)
     return 
 
 def add_arc(job:str, step:str, layers:list, symbol:str, start_x:int, start_y:int, end_x:int, end_y:int, center_x:int, center_y:int,cw:bool,polarity:int, attributes:list)->None:
     try:
         layer=''
         if len(layers)>0:
             layer=layers[0]
         if polarity==True:
             polarity=1
         else:
-            polarity=0
+            polarity=-1
         dcode = 0
         BASE.add_arc(job, step, layers, layer, symbol, start_x, start_y, end_x, end_y, center_x, center_y,cw,polarity, dcode, attributes)
     except Exception as e:
         print(e)
     return None
 
 def layer_compare(job1:str, step1:str, layer1:str, job2:str, step2:str, layer2:str, tol:int, isGlobal:bool, consider_SR:bool, comparison_map_layername:str, map_layer_resolution:int)->None:
     try:
         BASE.layer_compare(job1, step1, layer1, job2, step2, layer2, tol, isGlobal, consider_SR, comparison_map_layername, map_layer_resolution)
     except Exception as e:
         print(e)
     return None
 
-def add_text(job:str, step:str, layers:list, symbol:str, fontname:str, text:str, xsize:int, ysize:int, linewidth:int, location_x:int, location_y:int,polarity:bool,orient:int,  attributes:list,special_angle=0)->None:
+def add_text(job:str, step:str, layers:list, fontname:str, text:str, xsize:int, ysize:int, linewidth:int, location_x:int, location_y:int,polarity:bool,orient:int,  attributes:list,special_angle:float=0)->None:
     try:
         layer = ''
         if len(layers)>0:
             layer = layers[0]
         if polarity == True:
             polarity = 1
         else:
-            polarity = 0
-        BASE.add_text(job, step, layer, symbol, fontname, text, xsize, ysize, linewidth, location_x, location_y, polarity,orient, 0, layers, attributes,special_angle)
+            polarity = -1
+        BASE.add_text(job, step, layer, '',fontname, text, xsize, ysize, linewidth, location_x, location_y, polarity,orient, 0, layers, attributes,special_angle)
     except Exception as e:
         print(e)
     return ''     
 
 def change_polarity(job:str,step:str,layers:list,polarity:int,type:int)->bool:
     try:
         sel_type = type
@@ -258,19 +246,33 @@
         else:
             ret = False
         return ret
     except Exception as e:
         print(e)
         return False
 
-def fill_profile(job:str,step:str,layer:str,profile_resize:int,child_profile_resize:int,avoid_drill_size:int,fill_by_pattern:bool,symbolname:str,dx:int,dy:int,avoid_drill=True)->bool:
-    try:
-        _ret = BASE.fill_profile(job,step,layer,profile_resize,child_profile_resize,avoid_drill_size,fill_by_pattern,symbolname,dx,dy,avoid_drill)
-        ret = json.loads(_ret)['result']
-        return ret
+def fill_profile(job:str, step:str, layers:list, fill_type:int=0 ,step_repeat_nesting:bool=True, nesting_child_steps:list=[], step_margin_x:int=0,
+                 step_margin_y:int=0, max_distance_x:int=0, max_distance_y:int=0,SR_step_margin_x:int=0,SR_step_margin_y:int=0,
+                 SR_max_distance_x:int=0,SR_max_distance_y:int=0,avoid_drill:int=0,avoid_rout:int=0,avoid_feature:int=0,
+                 polarity:bool=True)->bool:
+    try:
+        info = Information.get_fill_param()
+        patternParams = info['patternParams']
+        solidParams = info['solidParams']
+        gridParams = info['gridParams']
+        BASE.set_fill_param(fill_type,gridParams,patternParams,solidParams)
+        if  solidParams['minBrush'] == 0 :
+            if fill_type == 1 or solidParams['solidType'] == False:
+                return False
+        else:
+            _ret = BASE.fill_profile(job,step,layers,step_repeat_nesting,nesting_child_steps,step_margin_x,step_margin_y,
+                                    max_distance_x,max_distance_y,SR_step_margin_x,SR_step_margin_y,SR_max_distance_x,
+                                    SR_max_distance_y,avoid_drill,avoid_rout,avoid_feature,polarity)
+            ret = json.loads(_ret)['result']
+            return ret
     except Exception as e:
         print(e)
         return False
 
 def resize_global(job:str, step:str, layers:list, type:int, size:int):
     try:
         sel_type = type
@@ -333,15 +335,15 @@
                 featuretype_list[index]=None
         for type_ in featuretype_list:
             if type_!=None:
                 featuretype_sum += math.pow(2,type_)
         for i in layers:
             layer = i
             BASE.load_layer(job,step,layer)
-            BASE.clip_area_use_manual(jobname, stepname, layers, points, margin, clipcontour,clipinside, featuretype_sum)
+        BASE.clip_area_use_manual(jobname, stepname, layers, points, margin, clipcontour,clipinside, featuretype_sum)
     except Exception as e:
         print(e)
     return None
 
 def clip_area_use_profile(job:str, step:str, layers:list,  clipinside:bool, clipcontour:bool, margin:float, text:bool, surface:bool, arc:bool, line:bool, pad:bool):
     try:
         positive = True
@@ -355,15 +357,15 @@
                 featuretype_list[index]=None
         for type_ in featuretype_list:
             if type_!=None:
                 featuretype_sum += math.pow(2,type_)
         for i in layers:
             layer = i
             BASE.load_layer(job,step,layer)
-            BASE.clip_area_use_profile(job, step, layers, clipinside, clipcontour, margin, featuretype_sum)
+        BASE.clip_area_use_profile(job, step, layers, clipinside, clipcontour, margin, featuretype_sum)
     except Exception as e:
         print(e)
     return None
 
 def transform_features(job:str,step:str,layer:str,mode:int,rotate:bool,scale:bool,mirror_X:bool,mirror_Y:bool,duplicate:bool,datumPoint:dict,angle:float,xscale:float,yscale:float,xoffset:int,yoffset:int):
     try:
         jobname = job
@@ -377,15 +379,14 @@
 def rounding_line_corner(job:str, step:str, layers:list, radius:int):
     try:
         BASE.rounding_line_corner(job,step,layers,radius)
     except Exception as e:
         print(e)
     return 
 
-
 def flatten_step(job:str, step:str ,flatten_layer:str, dst_layer:str)->bool:
     try:
         layers = Information.get_layers(job)
         ret = BASE.get_all_step_repeat_steps(job,step)
         steps = json.loads(ret)['steps']
         if steps != None:
             for i in range(0,len(layers)):
@@ -399,16 +400,16 @@
                             ret = False
                         return ret
         else:
             pass
     except Exception as e:
         print(e)
     return False
-    
-def layer_compare_point(job1:str, step1:str, layer1:str, job2:str, step2:str, layer2:str, tol = 22860,isGlobal = True,consider_SR = True, map_layer_resolution = 5080000)->list:
+
+def layer_compare_point(job1:str, step1:str, layer1:str, job2:str, step2:str, layer2:str, tol:int = 22860,isGlobal:bool = True,consider_SR:bool = True, map_layer_resolution:int = 5080000)->list:
     try:
         tolerance = tol
         mode = isGlobal
         point = BASE.layer_compare_point(job1, step1, layer1, job2, step2, layer2, tolerance, mode, consider_SR, map_layer_resolution)
         points = json.loads(point)['result']
         return points
     except Exception as e:
@@ -439,46 +440,46 @@
             return False
         Matrix.create_layer(job,'line_back')
         Matrix.create_layer(job,'slotpad_back')
         all_layers=layers
         select=False
         select_layer=[]
         for item in all_layers:
-            ret=Information.is_selected(job,step,item)
+            ret=Information.has_selected_features(job,step,item)
             if ret:
                 select=True 
                 select_layer.append(item)
 
         if select==True:
             all_layers=select_layer
         for item in all_layers:
             if select == False:
                 Selection.reverse_select(job,step,item)
             Layers.move2other_layer(job,step,[item],job,step,'line_back',False,0,0,0,0,0,0,0)
             Selection.set_featuretype_filter(True,True,True,True,True,False,False)
             Selection.select_features_by_filter(job,step,['line_back'])
-            deleteselect=Information.is_selected(job,step,'line_back')
+            deleteselect=Information.has_selected_features(job,step,'line_back')
             if deleteselect:
                 Layers.move2other_layer(job,step,['line_back'],job,step,item,False,0,0,0,0,0,0,0)
             Selection.reset_select_filter()
             Selection.set_featuretype_filter(True,True,False,False,False,False,True)
             Selection.select_features_by_filter(job,step,['line_back'])
-            padselect=Information.is_selected(job,step,'line_back')
+            padselect=Information.has_selected_features(job,step,'line_back')
             if padselect:
                 Layers.move2other_layer(job,step,['line_back'],job,step,'slotpad_back',False,0,0,0,0,0,0,0)
                 padinfo=Information.get_all_symbol_info(job,step,'slotpad_back')['pad_list']
                 ovallist=[]
                 for pad in padinfo:
                     if pad['symbolname'][0:4] =='oval':
                         ovallist.append(pad['symbolname'])
                 Selection.reset_select_filter()
                 Selection.set_include_symbol_filter(ovallist)
                 Selection.select_features_by_filter(job,step,['slotpad_back'])
                 Selection.reverse_select(job,step,'slotpad_back')
-                info=Information.is_selected(job,step,'slotpad_back')
+                info=Information.has_selected_features(job,step,'slotpad_back')
                 if info:
                     Layers.move2other_layer(job,step,['slotpad_back'],job,step,item,False,0,0,0,0,0,0,0)
             linesum=Information.get_layer_feature_count(job,step,'line_back')
             ovalsum=Information.get_layer_feature_count(job,step,'slotpad_back')
             if linesum==0 and ovalsum==0:
                 return False
             #对feature做处理
@@ -675,8 +676,133 @@
             del j['ix']
             del j['iy']
         return ret
     except Exception as e:
         print(e)
     return []
 
+def outline2surface(job:str, step:str, layers:list, to_pad:bool):
+    try:
+        BASE.outline2surface(job,step,layers,to_pad)
+    except Exception as e:
+        print(e)
+    return None
+
+#将指定料号指定层中选中的feature移动至目标料号下的目标层中，
+def move2other_layer(src_job:str, src_step:str, src_layers:list, dst_job:str, dst_step:str, dst_layer:str, invert:bool, offset_x:int, offset_y:int, mirror:int, resize:float, rotation:float, x_anchor:float, y_anchor:float)->None:
+    try:
+        BASE.sel_move_other(src_job, src_step, src_layers, dst_job, dst_step, dst_layer, invert, offset_x, offset_y, 
+                    mirror, resize, rotation, x_anchor, y_anchor)
+    except Exception as e:
+        print(e)
+
+def copy_usersymbol_to_other_job(job1:str, job2:str, symbol1:str, symbol2:str):
+    try:
+        BASE.copy_usersymbol_to_other_job(job1,job2,symbol1,symbol2)
+    except Exception as e:
+        print(e)
+
+def set_fill_grid_param(angle:int, dx:int, dy:int, linewidth:int, xoffset:int, yoffset:int):
+    try:
+        ret = Information.get_fill_param()
+        fillType = 2
+        patternParams = ret['patternParams']
+        solidParams = ret['solidParams']
+        gridParams = ret['gridParams']
+        gridParams['angle'] = angle
+        gridParams['dx'] = dx
+        gridParams['dy'] = dy
+        gridParams['lineWidth'] = linewidth
+        gridParams['xOffset'] = xoffset
+        gridParams['yOffset'] = yoffset
+        BASE.set_fill_param(fillType,gridParams,patternParams,solidParams)
+    except Exception as e:
+        print(e)
+
+def set_fill_pattern_param(symbolname:str, break_partial:bool, cut_primitive:bool, dx:int, dy:int, origin_point:bool, outline:bool, outline_invert:bool=False,outline_width:int=0,even_offset:int=0,odd_offset:int=0):
+    try:
+        ret = Information.get_fill_param()
+        fillType = 3
+        patternParams = ret['patternParams']
+        solidParams = ret['solidParams']
+        gridParams = ret['gridParams']
+        patternParams['breakPartial'] = break_partial
+        patternParams['cutPrimitive'] = cut_primitive
+        patternParams['dx'] = dx
+        patternParams['dy'] = dy
+        patternParams['evenOffset'] = even_offset
+        patternParams['oddOffset'] = odd_offset
+        patternParams['originPoint'] = origin_point
+        patternParams['outline'] = outline
+        patternParams['outlineInvert'] = outline_invert
+        patternParams['outlineWidth'] = outline_width
+        patternParams['symbolName'] = symbolname
+        BASE.set_fill_param(fillType,gridParams,patternParams,solidParams)
+    except Exception as e:
+        print(e)
+
+def set_fill_solid_param(solid_type:bool=True,min_brush:int=25400,use_arcs:bool=False):
+    try:
+        ret = Information.get_fill_param()
+        fillType = 0
+        patternParams = ret['patternParams']
+        solidParams = ret['solidParams']
+        gridParams = ret['gridParams']
+        solidParams['minBrush'] = min_brush
+        solidParams['solidType'] = solid_type
+        solidParams['useArcs'] = use_arcs
+        BASE.set_fill_param(fillType,gridParams,patternParams,solidParams)
+    except Exception as e:
+        print(e)
+
+def fill_contours(job:str,step:str,layer:str,type:int):
+    try:
+        ret = BASE.get_fill_param()
+        param = json.loads(ret)['paras']
+        if type == 0:
+            minBrush = param['solidParams']['minBrush']
+            useArcs = param['solidParams']['useArcs']
+            BASE.use_solid_fill_contours(job,step,[layer],True,minBrush,useArcs)
+        elif type == 1:
+            angle = param['gridParams']['angle']
+            dx = param['gridParams']['dx']
+            dy = param['gridParams']['dy']
+            lineWidth = param['gridParams']['lineWidth']
+            xOffset = param['gridParams']['xOffset']
+            yOffset = param['gridParams']['yOffset']
+            BASE.fill_select_feature_by_grid(job,step,layer,dx,dy,lineWidth,xOffset,yOffset,angle)
+        elif type == 2:
+            breakPartial = param['patternParams']['breakPartial']
+            cutPrimitive = param['patternParams']['cutPrimitive']
+            dx = param['patternParams']['dx']
+            dy = param['patternParams']['dy']
+            evenOffset = param['patternParams']['evenOffset']
+            oddOffset = param['patternParams']['oddOffset']
+            originPoint = param['patternParams']['originPoint']
+            outline = param['patternParams']['outline']
+            outlineInvert = param['patternParams']['outlineInvert']
+            outlineWidth = param['patternParams']['outlineWidth']
+            symbolName = param['patternParams']['symbolName']
+            BASE.use_pattern_fill_contours(job,step,layer,symbolName,dx,dy,breakPartial,cutPrimitive,originPoint,outline,outlineWidth,outlineInvert,oddOffset,evenOffset)
+    except Exception as e:
+        print(e)
+
+def use_solid_fill_contours(job:str, step:str, layers:list, min_brush:int, use_arcs:bool=False):
+    try:
+        BASE.use_solid_fill_contours(job,step,layers,True,min_brush,use_arcs)
+    except Exception as e:
+        print(e)
+
+def add_chain(job:str,step:str,layer:str,chain_number:int,first_index:int,comp:int,keep_direction:bool,
+              add_plunge:bool,toolsize:float,rout_flag:float = 0,feed:float = 0,speed:float = 0):
+    try:
+        if comp == 0:
+            comp = 'None'
+        elif comp == 1:
+            comp = 'Left'
+        elif comp == 2:
+            comp = 'Right'
+        BASE.add_chain(job,step,layer,chain_number,first_index,comp,keep_direction,add_plunge,toolsize,rout_flag,feed,speed)
+    except Exception as e:
+        print(e)
+
```

## epkernel/Edition/Matrix.py

```diff
@@ -1,49 +1,48 @@
 import os, sys, json
 from epkernel import BASE
 from epkernel.Edition import Layers
 from epkernel.Action import Selection, Information
 
+
 # 拷贝Layer
-# jobname, org_layer_index, dst_layer, poi_layer_index
-def copy_layer(jobname:str, old_layer_name:str):
+def copy_layer(job:str, old_layer_name:str) :
     try:
-        ret = BASE.get_matrix(jobname)
+        ret = BASE.get_matrix(job)
         data = json.loads(ret)
         layer_infos = data['paras']['info']
         src_layername=[]
-        src_layername= Information.get_layers(jobname)
+        src_layername= Information.get_layers(job)
         if old_layer_name in src_layername:
             for i in range(0, len(layer_infos)):         
                 if layer_infos[i]['name'] == old_layer_name:
                     old_layer_index = i + 1
         else:
             print('e')
             return 0
         dst_layer = ''
         # 新建空layer
-        create_layer(jobname, 'jbz')
-        ret2 = BASE.copy_layer(jobname, old_layer_index,
+        create_layer(job, 'jbz')
+        ret2 = BASE.copy_layer(job, old_layer_index,
                                dst_layer, len(layer_infos) + 1)
         data2 = json.loads(ret2)
         new_layer = data2['paras']['newname']
         # 删除新层
-        delete_layer(jobname, 'jbz')
+        delete_layer(job, 'jbz')
         return new_layer
     except Exception as e:
         print(e)
         print('123456')
     return ''
 
 # 创建layer
-def create_layer(job:str, layer:str):
+def create_layer(job:str, layer:str, row_index:int=-1):
     try:
-        index = -1  # 默认创建在末尾
         step = ''  # 在所有层创建
-        BASE.create_new_layer(job, step, layer, index)
+        BASE.create_new_layer(job, step, layer, row_index)
     except Exception as e:
         print(e)
 
 # 删除layer
 def delete_layer(job:str, layername:str):
     try:
         ret = BASE.get_matrix(job)
@@ -54,37 +53,22 @@
                 layer_index = i + 1
                 BASE.delete_layer(job, layer_index)
                 break
     except Exception as e:
         print(e)
     return 0
 
-def insert_row(job:str, row_index:int,row_name:str):
-    try:
-        BASE.create_new_layer(job, '', row_name, row_index)
-    except Exception as e:
-        print(e)
-    return 0
-
-def insert_column(job:str, col_index:int,col_name:str):
-    try:
-        BASE.create_step(job, col_name, col_index)
-    except Exception as e:
-        print(e)
-    return 0
-
 # 创建step
-def create_step(job:str, step:str):
+def create_step(job:str, step:str, col_index:int=-1):
     try:
-        index = -1  # 默认创建在末尾
-        BASE.create_step(job, step, index)
+        BASE.create_step(job, step, col_index)
     except Exception as e:
         print(e)
 
-def change_matrix_row(job:str, layer:str, context:str, type:str, layername:str, polarity = True):
+def change_matrix_row(job:str, layer:str, context:str, type:str, layername:str, polarity:bool = True):
     """
     #修改指定层别信息,若修改后信息与原层别一致，则此函数不执行
     :param     jobname:
     :param     layer:
     :param     context:
     :returns   :
     :raises    error:
@@ -106,43 +90,40 @@
                 layer_infos[i]['polarity'] = polarity
         BASE.change_matrix(job, -1, layer_index, '',
                            layer_infos[layer_index-1])
     except Exception as e:
         print(e)
     return 0
 
-
 def change_matrix_column(job:str, src_name:str, dst_name:str):
     try:
         ret = BASE.get_matrix(job)
         data = json.loads(ret)
         step_infos = data['paras']['steps']
         old_step_index = step_infos.index(src_name) + 1
         old_layer_index = -1
         new_layer_info = ''
         BASE.change_matrix(job, old_step_index,
                            old_layer_index, dst_name, new_layer_info)
     except Exception as e:
         print(e)
 
-
 def delete_step(job:str, step:str):
     try:
         ret = BASE.get_matrix(job)
         data = json.loads(ret)
         step_infos = data['paras']['steps']
         for i in range(0, len(step_infos)):
             if step_infos[i] == step:
                 step_index = i + 1
         BASE.delete_step(job, step_index)
     except Exception as e:
         print(e)
     return 0
 
-
 def copy_step(job:str, src_step_name:str)->str:
     try:
         ret = BASE.get_matrix(job)
         data = json.loads(ret)
         step_infos = data['paras']['steps']
         if src_step_name in step_infos:
             for i in range(0, len(step_infos)):
@@ -172,20 +153,132 @@
             if new_layer not in layer_list:
                 create_layer(job, new_layer)
             else:
                 BASE.clear_selected_features(job, step, new_layer)
                 Selection.reverse_select(job, step, new_layer) 
                 Layers.delete_feature(job, step, new_layer)  
                 BASE.clear_selected_features(job, step, new_layer)
-            Layers.copy_other(job, step, layer, new_layer, False, 0, 0, 0, 0, 0, 0, 0)
+            Layers.copy2other_layer(job, step, layer, new_layer, False, 0, 0, 0, 0, 0, 0, 0)
     except Exception as e:
         print(e)
         return None
-        
 
 def move_layer(job:str, org_layer_index:int, dst_layer_index:int):
     try:
         jobname = job
         BASE.move_layer(jobname, org_layer_index, dst_layer_index)
     except Exception as e:
         print(e)
-        return None
+        return None
+
+def set_layer_infos(job:str, layerInfos:list, oldList:list, newList:list)->bool:
+    try:
+        if not len(oldList) == len(newList):
+            return False
+        if not len(oldList) == len(layerInfos):
+            return False
+        if len(oldList) == 0:
+            return False
+        nameMap = []
+        for i in range(len(oldList)):
+            nameMap.append({oldList[i] : newList[i]})
+        ret = BASE.set_layer_infos(job, layerInfos, nameMap)
+        ret = json.loads(ret)
+        if 'status' in ret:
+            if ret['status'] == 'true':
+                return True
+            else:
+                return False
+        else:
+            return False
+    except Exception as e:
+        print(e)
+        return False
+
+def auto_matrix(job:str)->tuple:
+    try:
+        #获取所有层别名
+        nameList = Information.get_layers(job)
+        vv = BASE.auto_matrix(nameList)
+        nn = json.loads(vv)
+        ret = json.loads(nn['msg'])
+        if ret == '':
+            return ([], [], [])
+        #将匹配结果转为set_layer_infos需要的数据结构
+        bbb = BASE.matchLayers2LayerInfos(ret)
+        layerInfos = bbb[0]
+        oldList = bbb[1]
+        newList = bbb[2]
+
+        #加入将未匹配成功的层
+        for v in layerInfos:
+            nameList.remove(v["old_name"])
+        
+        vIndex = 1
+        for vv in nameList:
+            layerInfo = {}
+            layerInfo['type'] = 'document'
+            layerInfo['name'] = vv
+            layerInfo['context'] = 'misc'
+            layerInfo['polarity'] = 'positive'
+            layerInfo['start_name'] = ""
+            layerInfo['end_name'] = ""
+            layerInfo['old_name'] = vv
+            layerInfo['row'] = len(layerInfos) + vIndex
+            layerInfos.append(layerInfo)
+            #nameMap.append({vv : vv})
+            oldList.append(vv)
+            newList.append(vv)
+        return (layerInfos, oldList, newList)
+    except Exception as e:
+        print(e)
+        return ([], [], [])
+
+def create_flip(job:str, step:str)->bool:
+    try:
+        _ret = BASE.step_flip(job,step)
+        ret = json.loads(_ret)['paras']['result']
+        return ret
+    except Exception as e:
+        print(e)
+        return False
+
+def edit_step_attributes(job:str, step:str, edit_mode:int, edit_attr_name:str, edit_attr_value:str)->bool:
+    try:
+        _ret = BASE.edit_step_attributes(job,step,edit_mode,edit_attr_name,edit_attr_value)
+        ret = json.loads(_ret)['status']
+        if ret == 'true':
+            ret = True
+        else:
+            ret = False
+        return ret
+    except Exception as e:
+        print(e)
+        return False
+
+def edit_layer_attributes(job:str, step:str, layer:str, edit_mode:int, edit_attr_name:str, edit_attr_value:str)->bool:
+    try:
+        _ret = BASE.edit_layer_attributes(job,step,layer,edit_mode,edit_attr_name,edit_attr_value)
+        ret = json.loads(_ret)['status']
+        if ret == 'true':
+            ret = True
+        else:
+            ret = False
+        return ret
+    except Exception as e:
+        print(e)
+        return False
+
+def change_drill_cross(job:str, layer:str, start_name:str, end_name:str):
+    try:
+        ret = BASE.get_matrix(job)
+        data = json.loads(ret)
+        layer_infos = data['paras']['info']
+        for i in range(0, len(layer_infos)):
+                if layer_infos[i]['name'] == layer:
+                    layer_index = i + 1
+                    layer_infos[i]['start_name'] = start_name
+                    layer_infos[i]['end_name'] = end_name
+        BASE.change_matrix(job, -1, layer_index, '', layer_infos[layer_index-1])
+    except Exception as e:
+        print(e)
+    return 0
```

## Comparing `epkernel-1.1.7.dist-info/RECORD` & `epkernel-1.1.8.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-epkernel/Application.py,sha256=7B3vqPYVpIl-wmYyypc-XmKbfv3yt1izgkd0VgMBFD8,7130
-epkernel/BASE.py,sha256=_zHOLjBadj-p2UZ89F0j2CEp3zIEPqEqRSfu6J6JwAU,148519
-epkernel/Configuration.py,sha256=13BcGvRqM2YqPDtd2hx2xvtLi-zU82gpz316yRRhxII,597
+epkernel/Analysis.py,sha256=EHrEXUjN13tVPG5R-VjcXPaQkY_svfNWJC62Oy9cuWU,64
+epkernel/Application.py,sha256=9v5GKYbAHb6OF4Ami3bUXrkhBUOYZOFxqkb0rddzLLs,9662
+epkernel/BASE.py,sha256=XidC1gbIjbz-pYQIVpGVsZBoeBwZR2O-p51_H6nM2V8,161283
+epkernel/Configuration.py,sha256=JaAC93hYFnKGdixb6SxYbLQlhn-faj-p5dqUSwem2gc,1421
 epkernel/GUI.py,sha256=85_U95DnbVqH1FIY2oOZae3H7KnoHIspRcKUIWPiCaA,666
-epkernel/Input.py,sha256=gUnIYUcap-vmNgQIBkNDv6OkiyRg7sxkIaRmyZpujcY,1849
-epkernel/Output.py,sha256=OW-WpjOZu47ToyDPwcL-Z3KyortCBIxogX0CH8XIBK4,10667
+epkernel/Guide.py,sha256=U1S8vSSiFMW4UQgzgQlloyY7xewxqVuiV23tBipD-Ow,5625
+epkernel/Input.py,sha256=fmoeCG4uUs8bj4xrKmx4FTTKpgyg5LNYaRx5ZYi3BB0,1897
+epkernel/Optimization.py,sha256=rzje6N2_nFVGKQrL8HG7KrR0MSnmFMH4IgNGZvliKAA,58
+epkernel/Output.py,sha256=mVi7hu1M7_pvbizlC_CbteRiy4XwTf2GYVUjRFzEUBA,12016
 epkernel/__init__.py,sha256=lZHH04lPU2cmQ2j48ZMHK0WpbcNwiwnWtSGGhiPftJA,118
-epkernel/analysis.py,sha256=YXLp0PftLooN48OxSTNfOyaSmp2fjkqe-evXdyDXnxs,56
-epkernel/epcam.py,sha256=smbyQlTnvSP55Pbl56rQpMacBFUQo9D2l_Svyhq-3CU,2738
-epkernel/optimization.py,sha256=rzje6N2_nFVGKQrL8HG7KrR0MSnmFMH4IgNGZvliKAA,58
-epkernel/Action/Information.py,sha256=6Y536mZmaSVnhnmTkfUQRKXwyOhP19cQH_yCkrL8PpI,37677
-epkernel/Action/Selection.py,sha256=RIhrqI8eERNIHekr1iJwt611u6k4XWXt0hlkB_sRFTo,12051
-epkernel/Edition/Job.py,sha256=Cg4CT6WDg8cAZo7Zrx1qfDQ6HogbTZ-9vVIXoScmajw,1922
-epkernel/Edition/Layers.py,sha256=P1bfOIbiwHOQoDr68XwTMVT8lmd6zbpRg8eNBFIMDDg,30022
-epkernel/Edition/Matrix.py,sha256=K7Rte7oCS6QM1iFncXzhlML62EgMt0y2fq79FxcIbQ4,6296
+epkernel/epcam.py,sha256=TZvCGpoA0uOw4WpTuJlq3sXMs1AsOgXBkSPHrgGYMsg,4760
+epkernel/Action/Information.py,sha256=dsufpLHJSFnliAPg1o3NJ93-lupkWAqbT0IoZWip9dQ,42198
+epkernel/Action/Selection.py,sha256=52ObkOUQekVvC_3gWB4S46yVppK57c357PBiWPjmJB8,15089
+epkernel/Edition/Job.py,sha256=zAp1LgglCW5u-0jlIY4WDPfPjhDa4LL9wfR9oGKH9YA,2509
+epkernel/Edition/Layers.py,sha256=jTa6PyoawUcU3AcZidYiCKzP3eOnPmEFkbOGVa1l9WY,35969
+epkernel/Edition/Matrix.py,sha256=rmMWiI2vgBds9gaLAL6eqqdQi_Jgbwczp6c9Emm0ELI,9598
 epkernel/MI/stackup.py,sha256=9W9BimAp9ZWR1cniEo_pYw4gTQhGucUHhy-KV50WQCc,4708
-epkernel-1.1.7.dist-info/METADATA,sha256=ZKSC3GideIWK4FmhrG24ezYifzOzM5UqtYg3LFszKLk,251
-epkernel-1.1.7.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
-epkernel-1.1.7.dist-info/top_level.txt,sha256=ZuE7Ixa_gsE-hxrVTnAi1_dJLLrUD834POg9onk7F0U,9
-epkernel-1.1.7.dist-info/RECORD,,
+epkernel-1.1.8.dist-info/METADATA,sha256=AtxVGGGyB7W-6djjC1-b2f0V9m2kc_68xPIV5NwpVzY,251
+epkernel-1.1.8.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
+epkernel-1.1.8.dist-info/top_level.txt,sha256=ZuE7Ixa_gsE-hxrVTnAi1_dJLLrUD834POg9onk7F0U,9
+epkernel-1.1.8.dist-info/RECORD,,
```

