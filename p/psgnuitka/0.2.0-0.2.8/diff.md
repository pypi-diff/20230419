# Comparing `tmp/psgnuitka-0.2.0.tar.gz` & `tmp/psgnuitka-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgnuitka-0.2.0.tar", max compression
+gzip compressed data, was "psgnuitka-0.2.8.tar", max compression
```

## Comparing `psgnuitka-0.2.0.tar` & `psgnuitka-0.2.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1086 2023-04-12 00:26:22.121472 psgnuitka-0.2.0/LICENSE
--rw-r--r--   0        0        0    16453 2023-04-17 02:13:13.643372 psgnuitka-0.2.0/psgnuitka.py
--rw-r--r--   0        0        0      837 2023-04-17 01:54:36.809754 psgnuitka-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1622 2023-04-12 12:13:22.154596 psgnuitka-0.2.0/README.md
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 psgnuitka-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-12 00:26:22.121472 psgnuitka-0.2.8/LICENSE
+-rw-r--r--   0        0        0    16876 2023-04-19 04:58:38.296578 psgnuitka-0.2.8/psgnuitka.py
+-rw-r--r--   0        0        0      837 2023-04-19 04:58:38.297551 psgnuitka-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1622 2023-04-12 12:13:22.154596 psgnuitka-0.2.8/README.md
+-rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 psgnuitka-0.2.8/PKG-INFO
```

### Comparing `psgnuitka-0.2.0/LICENSE` & `psgnuitka-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psgnuitka-0.2.0/psgnuitka.py` & `psgnuitka-0.2.8/psgnuitka.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         sys_language = "zh_CN"
     info['sys_language'] = sys_language
     info['language_code'] = language_code
     return info
 
 
 def runbuildcommand(command: str, window: PySimpleGUI.Window = None, timeout: int = None, system_encode: str = None) -> tuple:
-    p = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+    p = subprocess.Popen(command, shell=True,
+                         stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     # if PySimpleGUI.running_windows():
     #     # command = shlex.split(command)
     #     p = subprocess.Popen(
     #         command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     # else:
     #     command = shlex.split(command)
     #     p = subprocess.Popen(
@@ -51,62 +52,70 @@
         "zh_CN": {
             "PYTHON-PATH": "使用的Python解释器位置",
             "FileBrowse-Button": "选择文件",
             "FolderBrowse-Button": "选择目录",
             "PY-PATH": "选择Python脚本文件",
         }
     }
-    text=all_text[sys_info['sys_language']]
+    sys_info
+    text = all_text.get(sys_info['sys_language'], "zh_CN")
+    # text=all_text[sys_info['sys_language']]
 
     # 主体布局
     main_layout = [
         [
-            PySimpleGUI.Text(text["PYTHON-PATH"]
-                             ), PySimpleGUI.Input(key="PYTHON-PATH"),
-            PySimpleGUI.FileBrowse(button_text=text['FileBrowse-Button'], file_types=[("", "python.exe python")],
-                                   target="PYTHON-PATH"), PySimpleGUI.Text(text["PY-PATH"]),
+            PySimpleGUI.Text("使用的Python解释器位置"),
+            PySimpleGUI.Input(key="PYTHON-PATH"),
+            PySimpleGUI.FileBrowse(button_text="选择文件", file_types=[
+                                   ("", "python.exe python")], target="PYTHON-PATH"),
+            PySimpleGUI.Text("选择Python脚本文件"),
             PySimpleGUI.Input(key="PY-PATH"),
-            PySimpleGUI.FileBrowse(button_text=text['FileBrowse-Button'], file_types=[("", "*.py")], target="PY-PATH")],
+            PySimpleGUI.FileBrowse(button_text="选择文件", file_types=[("", "*.py")], target="PY-PATH")],
         [
         ],
         [
             PySimpleGUI.Text("构建生成目录"),
             PySimpleGUI.Input(key="OUTPUT-DIR"),
-            PySimpleGUI.FolderBrowse(button_text=text['FolderBrowse-Button'],
-                                     target="OUTPUT-DIR"),
+            PySimpleGUI.FolderBrowse(button_text="选择目录", target="OUTPUT-DIR"),
             PySimpleGUI.Text("可执行文件名"),
             PySimpleGUI.Input(key="OUTPUT-FILENAME"),
         ],
         [
-            PySimpleGUI.Frame("C编译器选择", layout=[[
-                PySimpleGUI.Radio(group_id="CCOMPILER",
-                                  text="MingW64", default=True, key="MINGW64"),
-                PySimpleGUI.Radio(group_id="CCOMPILER",
-                                  text="Clang", default=False, key="CLANG"),
-                PySimpleGUI.Radio(group_id="CCOMPILER",
-                                  text="MSVC", default=False, key="MSVC"),
-            ]]),
+            PySimpleGUI.Frame("C编译器选择", layout=[
+                [
+                    PySimpleGUI.Radio(group_id="CCOMPILER",
+                                      text="MingW64", default=True, key="MINGW64"),
+                    PySimpleGUI.Radio(group_id="CCOMPILER",
+                                      text="Clang", default=False, key="CLANG"),
+                    PySimpleGUI.Radio(group_id="CCOMPILER",
+                                      text="MSVC", default=False, key="MSVC"),
+                ]
+            ]),
             PySimpleGUI.Frame("单文件模式", layout=[[
                 PySimpleGUI.Checkbox(
                     text="onefile", default=False, key="ONEFILE")
             ]]),
-            PySimpleGUI.Frame("是否控制台可用", layout=[[
-                PySimpleGUI.Radio(group_id="CONSOLE", text="enable",
-                                  default=True, key="ENABLE-CONSOLE"),
-                PySimpleGUI.Radio(group_id="CONSOLE", text="disable",
-                                  default=False, key="DISABLE-CONSOLE"),
-            ]]),
-            PySimpleGUI.Frame("工具链来源选择", layout=[[
-                PySimpleGUI.Radio(group_id="TOOLCHAINFROM", text="使用系统环境路径", default=False,
-                                  key="SYSTEMTOOLCHAIN"),
-                PySimpleGUI.Radio(group_id="TOOLCHAINFROM", text="使用本工具自带版本", default=False,
-                                  key="LOCALTOOLCHAIN", disabled=True),
-                PySimpleGUI.Radio(group_id="TOOLCHAINFROM", text="由nuitka自动下载处理", default=True,
-                                  key="NUITKATOOLCHAIN"),
-            ]]),
+            PySimpleGUI.Frame("是否控制台可用", layout=[
+                [
+                    PySimpleGUI.Radio(
+                        group_id="CONSOLE", text="enable", default=True, key="ENABLE-CONSOLE"),
+                    PySimpleGUI.Radio(
+                        group_id="CONSOLE", text="disable", default=False, key="DISABLE-CONSOLE"),
+                ]
+            ]),
+            PySimpleGUI.Frame("工具链来源选择", layout=[
+                [
+                    PySimpleGUI.Radio(
+                        group_id="TOOLCHAINFROM", text="使用系统环境路径", default=False, key="SYSTEMTOOLCHAIN"),
+                    PySimpleGUI.Radio(group_id="TOOLCHAINFROM", text="使用本工具自带版本",
+                                      default=False, key="LOCALTOOLCHAIN", disabled=True),
+                    PySimpleGUI.Radio(
+                        group_id="TOOLCHAINFROM", text="由nuitka自动下载处理", default=True, key="NUITKATOOLCHAIN"),
+                ]
+            ]),
         ],
         [
             PySimpleGUI.Frame("额外插件", layout=[
                 [
                     PySimpleGUI.Checkbox(
                         text="eventlet", default=False, key="EVENTLET"),
                     PySimpleGUI.Checkbox(
@@ -161,27 +170,32 @@
                 [
 
                 ]
             ]),
         ],
         [
             PySimpleGUI.Frame("需要的数据文件", expand_x=True, layout=[
-                [PySimpleGUI.Table(values=[[]], headings=["添加列表"], key="DATA-TABLE",
-                                   expand_x=True, justification="left")],
-                [PySimpleGUI.Button("添加文件", key="ADD-DATA-FILE"),
-                 PySimpleGUI.Button("添加目录", key="ADD-DATA-DIR"),
-                 PySimpleGUI.Button("添加指定模块的所有数据文件", key="ADD-DATA-PACKAGE"),
-                 PySimpleGUI.Button("删除选中", key="DEL-DATA-TABLE")]
+                [
+                    PySimpleGUI.Table(values=[[]], headings=["添加列表"], key="DATA-TABLE",
+                                      expand_x=True, justification="left")],
+                [
+                    PySimpleGUI.Button("添加文件", key="ADD-DATA-FILE"),
+                    PySimpleGUI.Button("添加目录", key="ADD-DATA-DIR"),
+                    PySimpleGUI.Button(
+                        "添加指定模块的所有数据文件", key="ADD-DATA-PACKAGE"),
+                    PySimpleGUI.Button("删除选中", key="DEL-DATA-TABLE")]
             ]),
             PySimpleGUI.Frame("需要的模块", expand_x=True, layout=[
-                [PySimpleGUI.Table(values=[[]], headings=["添加列表"], key="MODULE-TABLE",
-                                   expand_x=True, justification="left")],
-                [PySimpleGUI.Button("指定需要导入的模块", key="ADD-MODULE-NAME"),
-                 PySimpleGUI.Button("指定不希望导入的模块", key="NO-MODULE-NAME"),
-                 PySimpleGUI.Button("删除选中", key="DEL-MODULE-TABLE")]
+                [
+                    PySimpleGUI.Table(values=[[]], headings=["添加列表"], key="MODULE-TABLE",
+                                      expand_x=True, justification="left")],
+                [
+                    PySimpleGUI.Button("指定需要导入的模块", key="ADD-MODULE-NAME"),
+                    PySimpleGUI.Button("指定不希望导入的模块", key="NO-MODULE-NAME"),
+                    PySimpleGUI.Button("删除选中", key="DEL-MODULE-TABLE")]
             ])
         ],
 
         [
             PySimpleGUI.Text("构建命令:")
         ],
         [
@@ -198,25 +212,25 @@
         ],
         [
             PySimpleGUI.Button(button_text="生成构建命令", key="GENERATE-CMD"),
             PySimpleGUI.Button(button_text="构建", key="BUILD"),
             PySimpleGUI.Button(button_text="退出", key="EXIT")
         ]
     ]
-    window = PySimpleGUI.Window(title="psgnuitka", layout=main_layout, font="_ 14", resizable=True,
+    window = PySimpleGUI.Window(title="psgnuitka", layout=main_layout, font=("", 14), resizable=True,
                                 auto_size_text=True, auto_size_buttons=True, scaling=1.0,)
 
     data_table = []
     module_table = []
     build_cmd = ""
     start_time = 0
     stop_time = 0
     i = 0
     while True:
-        event, values = window.read(timeout=10)
+        event, values = window.read(timeout=10, timeout_key="--TIMEOUT--")
         if event in [PySimpleGUI.WINDOW_CLOSED, "EXIT"]:
             break
         if event == "GENERATE-CMD":
             cmd = list()
             cmd.append(str(pathlib.Path(values['PYTHON-PATH']).absolute()))
             cmd.append('-m')
             cmd.append('nuitka')
@@ -254,74 +268,77 @@
             # cmd.append("--verbose")
             cmd.append(str(pathlib.Path(values['PY-PATH']).absolute()))
             build_cmd = " ".join(cmd)
             window['BUILD-CMD'].update(build_cmd)
             # print(os.environ.get("PYTHONHOME"), os.environ.get("PYTHONPATH"))
             # PySimpleGUI.popup_get_file(message="选择要添加的文件", no_window=True)
         if event == "ADD-DATA-FILE":
-            file_path = PySimpleGUI.popup_get_file(message="", no_window=True,keep_on_top=True)
+            file_path = PySimpleGUI.popup_get_file(
+                message="", no_window=True, keep_on_top=True)
             if file_path:
                 file_name = PySimpleGUI.popup_get_text(
-                    message="添加的文件名为", default_text=file_path.split("/")[-1], font="_ 14",keep_on_top=True)
+                    message="添加的文件名为", default_text=file_path.split("/")[-1], font="_ 14", keep_on_top=True)
                 data_table.append(
                     ["--include-data-files=" + str(pathlib.Path(file_path).absolute()) + "=" + file_name])
                 window["DATA-TABLE"].update(values=data_table)
             else:
                 continue
         if event == "ADD-DATA-DIR":
-            dir_path = PySimpleGUI.popup_get_folder(message="", no_window=True,keep_on_top=True)
+            dir_path = PySimpleGUI.popup_get_folder(
+                message="", no_window=True, keep_on_top=True)
             if dir_path:
                 dir_name = PySimpleGUI.popup_get_text(message="添加的目录名为",
-                                                      default_text=dir_path.split("/")[-1], font="_ 14",keep_on_top=True)
+                                                      default_text=dir_path.split("/")[-1], font="_ 14", keep_on_top=True)
                 data_table.append(
                     ["--include-data-dir=" + str(pathlib.Path(dir_path).absolute()) + "=" + dir_name])
                 window["DATA-TABLE"].update(values=data_table)
             else:
                 continue
         if event == "ADD-DATA-PACKAGE":
             package_name = PySimpleGUI.popup_get_text(
-                message="添加指定模块数据", font="_ 14",keep_on_top=True)
+                message="添加指定模块数据", font="_ 14", keep_on_top=True)
             if package_name:
                 data_table.append(["--include-package-data=" + package_name])
                 window["DATA-TABLE"].update(values=data_table)
             else:
                 continue
         if event == "DEL-DATA-TABLE":
             if values["DATA-TABLE"]:
                 if len(data_table) != 0:
                     data_table.pop(values["DATA-TABLE"][0])
                     window["DATA-TABLE"].update(values=data_table)
             else:
                 continue
         if event == "ADD-MODULE-NAME":
             module_name = PySimpleGUI.popup_get_text(
-                message="希望导入的模块", font="_ 14",keep_on_top=True)
+                message="希望导入的模块", font="_ 14", keep_on_top=True)
             if module_name:
                 module_table.append(["--follow-import-to=" + module_name])
                 window["MODULE-TABLE"].update(values=module_table)
             else:
                 continue
         if event == "NO-MODULE-NAME":
             module_name = PySimpleGUI.popup_get_text(
-                message="不希望导入的模块", font="_ 14",keep_on_top=True)
+                message="不希望导入的模块", font="_ 14", keep_on_top=True)
             if module_name:
                 module_table.append(["--nofollow-import-to=" + module_name])
                 window["MODULE-TABLE"].update(values=module_table)
             else:
                 continue
         if event == "DEL-MODULE-TABLE":
             if values["MODULE-TABLE"]:
                 if len(module_table) != 0:
                     module_table.pop(values["MODULE-TABLE"][0])
                     window["MODULE-TABLE"].update(values=module_table)
             else:
                 continue
         if event == "BUILD":
             if build_cmd == "":
-                PySimpleGUI.PopupError(f"出错了，请先生成构建命令", font="_ 14",keep_on_top=True)
+                PySimpleGUI.PopupError(
+                    f"出错了，请先生成构建命令", font="_ 14", keep_on_top=True)
                 continue
             if PySimpleGUI.running_windows():
                 os.environ["PYTHONPATH"] = str(pathlib.Path(
                     values['PYTHON-PATH']).absolute().parent)
                 os.environ["PYTHONHOME"] = str(pathlib.Path(
                     values['PYTHON-PATH']).absolute().parent)
             start_time = time.perf_counter()
@@ -336,12 +353,13 @@
         if event == "BUILD-DONE":
             stop_time = time.perf_counter()
             use_time = round(stop_time - start_time, 2)
             # PySimpleGUI.PopupOK(f"处理完毕，用时{use_time}s", font="_ 14")
             window['BUILD'].update(disabled=False)
             # print(values["BUILD-DONE"])
             if values["BUILD-DONE"][0] == 0:
-                PySimpleGUI.popup_ok(f"处理完毕，用时{use_time}s", font="_ 14",keep_on_top=True)
+                PySimpleGUI.popup_ok(
+                    f"处理完毕，用时{use_time}s", font="_ 14", keep_on_top=True)
             else:
                 PySimpleGUI.popup_error(
-                    f"出错了，请对照输出检查信息，用时{use_time}s", font="_ 14",keep_on_top=True)
+                    f"出错了，请对照输出检查信息，用时{use_time}s", font="_ 14", keep_on_top=True)
     window.close()
```

### Comparing `psgnuitka-0.2.0/pyproject.toml` & `psgnuitka-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psgnuitka"
-version = "0.2.0"
+version = "0.2.8"
 description = "A graphical tool to facilitate the generation of Python executables using Nuitka"
 authors = ["boulderh <boulderh@163.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/BoulderH/psgnuitka"
 repository = "https://github.com/BoulderH/psgnuitka"
 keywords = ["nuitka","PySimpleGUI","psgnuitka"]
```

### Comparing `psgnuitka-0.2.0/README.md` & `psgnuitka-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `psgnuitka-0.2.0/PKG-INFO` & `psgnuitka-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psgnuitka
-Version: 0.2.0
+Version: 0.2.8
 Summary: A graphical tool to facilitate the generation of Python executables using Nuitka
 Home-page: https://github.com/BoulderH/psgnuitka
 License: MIT
 Keywords: nuitka,PySimpleGUI,psgnuitka
 Author: boulderh
 Author-email: boulderh@163.com
 Requires-Python: >=3.8,<4.0
```
