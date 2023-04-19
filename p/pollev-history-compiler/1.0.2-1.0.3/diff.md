# Comparing `tmp/pollev-history-compiler-1.0.2.tar.gz` & `tmp/pollev-history-compiler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollev-history-compiler-1.0.2.tar", last modified: Tue Apr 18 17:18:49 2023, max compression
+gzip compressed data, was "pollev-history-compiler-1.0.3.tar", last modified: Wed Apr 19 06:26:30 2023, max compression
```

## Comparing `pollev-history-compiler-1.0.2.tar` & `pollev-history-compiler-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 17:18:49.933287 pollev-history-compiler-1.0.2/
--rw-rw-rw-   0        0        0     1898 2023-04-18 17:18:49.933287 pollev-history-compiler-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1244 2023-04-18 17:02:41.000000 pollev-history-compiler-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 17:18:49.923589 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/
--rw-rw-rw-   0        0        0     1898 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 17:18:49.929186 pollev-history-compiler-1.0.2/pollev_tools/
--rw-rw-rw-   0        0        0        0 2023-04-18 17:02:41.000000 pollev-history-compiler-1.0.2/pollev_tools/__init__.py
--rw-rw-rw-   0        0        0    27958 2023-04-18 17:14:01.000000 pollev-history-compiler-1.0.2/pollev_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:18:49.933287 pollev-history-compiler-1.0.2/resources/
--rw-rw-rw-   0        0        0      567 2023-04-18 17:02:41.000000 pollev-history-compiler-1.0.2/resources/config.ini
--rw-rw-rw-   0        0        0      424 2023-04-18 17:02:41.000000 pollev-history-compiler-1.0.2/resources/html-styles.css
--rw-rw-rw-   0        0        0       42 2023-04-18 17:18:49.933287 pollev-history-compiler-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-04-18 17:14:40.000000 pollev-history-compiler-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:26:30.134873 pollev-history-compiler-1.0.3/
+-rw-rw-rw-   0        0        0     2657 2023-04-19 06:26:30.133873 pollev-history-compiler-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-04-19 06:26:09.000000 pollev-history-compiler-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 06:26:30.130854 pollev-history-compiler-1.0.3/pollev_history_compiler.egg-info/
+-rw-rw-rw-   0        0        0     2657 2023-04-19 06:26:30.000000 pollev-history-compiler-1.0.3/pollev_history_compiler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-19 06:26:30.000000 pollev-history-compiler-1.0.3/pollev_history_compiler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 06:26:30.000000 pollev-history-compiler-1.0.3/pollev_history_compiler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-19 06:26:30.000000 pollev-history-compiler-1.0.3/pollev_history_compiler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-04-19 06:26:30.000000 pollev-history-compiler-1.0.3/pollev_history_compiler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-19 06:26:30.000000 pollev-history-compiler-1.0.3/pollev_history_compiler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 06:26:30.131864 pollev-history-compiler-1.0.3/pollev_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-17 22:46:25.000000 pollev-history-compiler-1.0.3/pollev_tools/__init__.py
+-rw-rw-rw-   0        0        0    29902 2023-04-19 06:26:09.000000 pollev-history-compiler-1.0.3/pollev_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:26:30.132871 pollev-history-compiler-1.0.3/resources/
+-rw-rw-rw-   0        0        0      567 2023-04-16 17:02:01.000000 pollev-history-compiler-1.0.3/resources/config.ini
+-rw-rw-rw-   0        0        0     1244 2023-04-19 06:26:09.000000 pollev-history-compiler-1.0.3/resources/html-styles.css
+-rw-rw-rw-   0        0        0       42 2023-04-19 06:26:30.134873 pollev-history-compiler-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-04-19 06:26:09.000000 pollev-history-compiler-1.0.3/setup.py
```

### Comparing `pollev-history-compiler-1.0.2/PKG-INFO` & `pollev-history-compiler-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollev-history-compiler
-Version: 1.0.2
+Version: 1.0.3
 Summary: A script for the compilation of PollEverywhere history CSV files into more usable forms.
 Home-page: https://github.com/tony-zeidan/PollEvHistoryCompiler
 Author: Tony Abou Zeidan
 Author-email: tony.azp25@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -45,11 +45,30 @@
 Good options include presenter name:
 ```
 pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --presenter <NAME> <OPTIONS>
 ```
 
 Remove hidden questions from the result:
 ```
-pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --rhidden
+pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --remove_hidden
 ```
 
+Remove image-related questions from the result:
+```
+pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --remove_images
+```
+
+Markdown format is now supported! 
+```
+pollev-compiler <INPUT CSV> markdown
+```
+This process uses `markdownify` to turn the pre-existing HTML functionality into a markdown file.
+
+You can now use the `--quiz_mode` option in the `html` transform to turn the output to a interactable quiz that highlights your guesses,
+and your score on the quiz (correct over total). You can do this like:
+```
+pollev-compiler <INPUT CSV> html --quiz_mode
+```
+The output consists of a JavaScript file, CSS file, and HTML file. Without quiz mode, the JavaScript file isn't added.
+
+
 ## Documentation
```

### Comparing `pollev-history-compiler-1.0.2/README.md` & `pollev-history-compiler-1.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -29,11 +29,30 @@
 Good options include presenter name:
 ```
 pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --presenter <NAME> <OPTIONS>
 ```
 
 Remove hidden questions from the result:
 ```
-pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --rhidden
+pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --remove_hidden
 ```
 
+Remove image-related questions from the result:
+```
+pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --remove_images
+```
+
+Markdown format is now supported! 
+```
+pollev-compiler <INPUT CSV> markdown
+```
+This process uses `markdownify` to turn the pre-existing HTML functionality into a markdown file.
+
+You can now use the `--quiz_mode` option in the `html` transform to turn the output to a interactable quiz that highlights your guesses,
+and your score on the quiz (correct over total). You can do this like:
+```
+pollev-compiler <INPUT CSV> html --quiz_mode
+```
+The output consists of a JavaScript file, CSS file, and HTML file. Without quiz mode, the JavaScript file isn't added.
+
+
 ## Documentation
```

### Comparing `pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/PKG-INFO` & `pollev-history-compiler-1.0.3/pollev_history_compiler.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollev-history-compiler
-Version: 1.0.2
+Version: 1.0.3
 Summary: A script for the compilation of PollEverywhere history CSV files into more usable forms.
 Home-page: https://github.com/tony-zeidan/PollEvHistoryCompiler
 Author: Tony Abou Zeidan
 Author-email: tony.azp25@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -45,11 +45,30 @@
 Good options include presenter name:
 ```
 pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --presenter <NAME> <OPTIONS>
 ```
 
 Remove hidden questions from the result:
 ```
-pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --rhidden
+pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --remove_hidden
 ```
 
+Remove image-related questions from the result:
+```
+pollev-compiler <INPUT CSV> <TRANSFORM (json, yaml, toml, etc.)>  --output-file <OUTPUT PATH (dir)> --remove_images
+```
+
+Markdown format is now supported! 
+```
+pollev-compiler <INPUT CSV> markdown
+```
+This process uses `markdownify` to turn the pre-existing HTML functionality into a markdown file.
+
+You can now use the `--quiz_mode` option in the `html` transform to turn the output to a interactable quiz that highlights your guesses,
+and your score on the quiz (correct over total). You can do this like:
+```
+pollev-compiler <INPUT CSV> html --quiz_mode
+```
+The output consists of a JavaScript file, CSS file, and HTML file. Without quiz mode, the JavaScript file isn't added.
+
+
 ## Documentation
```

### Comparing `pollev-history-compiler-1.0.2/pollev_tools/reader.py` & `pollev-history-compiler-1.0.3/pollev_tools/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pandas as pd
 import yaml
 import json
 import random
 import configparser
 import shutil
 from collections import OrderedDict
+import uuid
 
 TEX_CHARS_ESCAPE = ['%']
 QUESTION_START_CHARS = [')', '.', ']', '&']
 
 def remove_question_start(s: str, max_len: int):
     """
     Removes the start of a question. 
@@ -264,16 +265,20 @@
     except KeyError:
         raise ValueError("Column couldn't be found, can't continue.")
     
 
 def html_helper(
         row,
         title_col: str = 'Activity title',
+        response_options_class: str = 'options',
         correct_class: str = 'correct',
         incorrect_class: str = 'incorrect',
+        question_class: str = 'question-title',
+        group_class: str = 'question-responses',
+        tab_start: int = 2,
         show_correct: bool = True,
         **kwargs
     ) -> str:
     """
     Converts the current row into a HTML block.
 
     :param correct_class: Classname (HTML) for the correct answers
@@ -285,67 +290,88 @@
     """
 
     strbuilder = []
 
     title = row[title_col]
     title = change_tex_chars(title)
 
-    strbuilder.append(rf'<li>{title}</li>')
+    question_ID = str(uuid.uuid4())
 
-    strbuilder.append('\t<ol type="a">')
+    tabs = lambda c: "\t"*c
+
+    strbuilder.append(rf'{tabs(tab_start)}<div class="{group_class}">')
+    strbuilder.append(f'{tabs(tab_start+1)}<p class="{question_class}" data-linked-id="{question_ID}">{title}</p>')
+    strbuilder.append(f'{tabs(tab_start+1)}<ol type="a" class="{response_options_class}" data-linked-id="{question_ID}">')
     for resp in row['split_responses']:
         resp_new = resp
         if resp in row['split_correct_responses']:
             if show_correct:
-                strbuilder.append(f"\t\t<li class={correct_class}>{resp_new}</li>")
+                strbuilder.append(f'{tabs(tab_start+2)}<li class="{correct_class}">{resp_new}</li>')
             else:
-                strbuilder.append(f"\t\t<li>{resp_new}</li>")
+                strbuilder.append(f'{tabs(tab_start+2)}<li>{resp_new}</li>')
         else:
-            strbuilder.append(f"\t\t<li class={incorrect_class}>{resp_new}</li>")
+            strbuilder.append(f'{tabs(tab_start+2)}<li class="{incorrect_class}">{resp_new}</li>')
 
-    strbuilder.append('\t</ol>\n')
+    strbuilder.append(f'{tabs(tab_start+1)}</ol>')
+    strbuilder.append(f'{tabs(tab_start)}</div>\n')
 
     return "\n".join(strbuilder)
 
-def to_html_report(data_df: pd.DataFrame, output_file: str, show_correct: bool = True, encoding: str = None):
+def to_html_report(data_df: pd.DataFrame, output_file: str, show_correct: bool = True, quiz_mode: bool = False, encoding: str = None):
     """
     Converts the CSV dataframe into a LaTeX exam report.
 
     :param data_df: The dataframe
     :param output_file: The file to output to (.TeX)
     :param encoding: The encoding to use when outputting
     """
 
     try: 
-        name, _ = os.path.splitext(output_file)
+        quiz_mode_script = ''
+        page_title = 'Extracted Polls'
+        page_heading = 'Polls Report'
+        page_bar = ''
+        if quiz_mode:
+            quiz_mode_script = "<script type='text/javascript' src='html-js.js'></script>"
+            page_title = 'Polls Quiz'
+            page_heading = 'Polls Quiz'
+            html_lst_values = data_df.apply(lambda x: html_helper(x, show_correct=show_correct), axis=1)
+            page_bar = f'''<div class='counter-bar'>
+            <p id='counter' data-maximum="{len(html_lst_values)}" data-curr="0">0/{len(html_lst_values)}</p>
+            <button class='reset'>Reset</button>
+        </div>'''
 
-        html_lst =  '\n'.join(data_df.apply(lambda x: html_helper(x, show_correct=show_correct), axis=1))
+        else:
+            html_lst_values = data_df.apply(lambda x: html_helper(x, show_correct=show_correct, correct_class='correct-quiz-selected'), axis=1)
+        html_lst = '\n'.join(html_lst_values)
 
         html_gen = f'''
 <!DOCTYPE html>
 <html lang="en">
 <head>
-    <script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha384-KyZXEAg3QhqLMpG8r+Knujsl5/1zwaQ7wxt2NN9138DhxUeK5l/5Vp1+XWlFm_tv" crossorigin="anonymous"></script>
+    {quiz_mode_script}
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway&display=swap" />
     <link rel="stylesheet" href="html-styles.css">
-    <title>{name}</title>
+    <title>{page_title}</title>
 </head> 
 <body>
     <div class='center-container'>
+        {page_bar}
         <div class='center-div'>
-            <h1>PollEverywhere Report</h1>
+            <h1>{page_heading}</h1>
         </div>          
-        {html_lst}
+{html_lst}
+        <div>
+            <button class='reset' id='bottom-reset'>Reset Quiz</button>
+        </div>
     </div>
 </body>
 </html>
         '''
 
-        
-
         with open(output_file, 'w', encoding=encoding) as out_file:
             out_file.write(html_gen)
 
     except KeyError:
         raise ValueError("Column couldn't be found, can't continue.")
     
 def to_markdown_report(data_df: pd.DataFrame, output_file: str, show_correct: bool = True, encoding: str = None):
@@ -372,15 +398,15 @@
     <title>{name}</title>
 </head> 
 <body>
     <div class='center-container'>
         <div class='center-div'>
             <h1>PollEverywhere Report</h1>
         </div>          
-        {html_lst}
+{html_lst}
     </div>
 </body>
 </html>
         '''
 
     md_str = markdownify.markdownify(html_gen)
     with open(output_file, 'w', encoding=encoding) as out_file:
@@ -530,14 +556,15 @@
     Main script executable.
     """
 
     base_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
     res_path = config_path = os.path.join(base_dir, "resources") 
     config_path = os.path.join(res_path, "config.ini") 
     styles_path = os.path.join(res_path, "html-styles.css")
+    js_path = os.path.join(res_path, "html-js.js")
 
     # define default values
     default_io_opts = dict(
         output_path = os.getcwd(),
         encoding = 'utf-8',
         transform = 'csv',
         remove_start_len = 5,
@@ -554,15 +581,15 @@
         resp_opt_block_type = 'choice',
         resp_opt_correct_block_type = 'CorrectChoice',
         end_spacing = 4,
         end_spacing_metric = 'pt'
     )
 
     default_html_opts = dict(
-
+        quiz_mode = False
     )
 
     default_json_opts = dict(
         root_name = 'questions'
     )
 
     default_yaml_opts = dict(
@@ -577,14 +604,18 @@
         
     )
 
     default_text_opts = dict(
         
     )
 
+    default_md_opts = dict(
+        
+    )
+
 
 
     config_parser = argparse.ArgumentParser(add_help=False)
     config_parser.add_argument('--config_path', type=str, help='Path to the configuration file (optional)', default=default_io_opts['config'])
     config_args, remaining_argv = config_parser.parse_known_args()
     default_io_opts['config'] = config_args.config_path
 
@@ -608,19 +639,22 @@
         elif default_io_opts['transform'] == 'json' and 'pollev_transforms.json' in config:
             default_json_opts.update(update_defaults_config(default_json_opts, config, 'pollev_transforms.json'))
 
         elif default_io_opts['transform'] == 'csv' and 'pollev_transforms.csv' in config:
             default_csv_opts.update(update_defaults_config(default_csv_opts, config, 'pollev_transforms.csv'))
 
         elif default_io_opts['transform'] == 'toml' and 'pollev_transforms.toml' in config:
-            default_toml_opts.update(update_defaults_config(default_csv_opts, config, 'pollev_transforms.toml'))
+            default_toml_opts.update(update_defaults_config(default_toml_opts, config, 'pollev_transforms.toml'))
 
         elif default_io_opts['transform'] == 'txt' and 'pollev_transforms.txt' in config:
-            default_toml_opts.update(update_defaults_config(default_csv_opts, config, 'pollev_transforms.txt'))
+            default_text_opts.update(update_defaults_config(default_text_opts, config, 'pollev_transforms.txt'))
     
+        elif default_io_opts['transform'] == 'markdown' and 'pollev_transforms.md' in config:
+            default_md_opts.update(update_defaults_config(default_csv_opts, config, 'pollev_transforms.md'))
+
     except FileNotFoundError:
         parser.set_defaults(transform=default_io_opts['transform'])
         args, _ = parser.parse_known_args(remaining_argv)
         pass
 
     global_parser = argparse.ArgumentParser(description='Read CSV file with optional screen name filter', add_help=False)
     global_parser.add_argument('--config_path', type=str, help='Path to the configuration file (optional)', default=default_io_opts['config'])
@@ -647,15 +681,16 @@
     parser_tex.add_argument('--resp_opt_block_type', type=str, help='LaTeX block used for a single response (if not correct)', default=default_tex_opts['resp_opt_block_type'])
     parser_tex.add_argument('--resp_opt_correct_block_type', type=str, help='LaTeX block used for a single response (if correct)', default=default_tex_opts['resp_opt_correct_block_type'])
     parser_tex.add_argument('--end_spacing', type=int, help='The amount of space to add after each response option', default=default_tex_opts['end_spacing'])
     parser_tex.add_argument('--end_spacing_metric', type=str, help='The metric for end_spacing', default=default_tex_opts['end_spacing_metric'])
     
     # HTML transform
     parser_html = transform_parser.add_parser('html', help='Convert to HTML', parents=[global_parser], add_help=True)
-
+    parser_html.add_argument('--quiz_mode', help='Change the HTML into an interactable quiz!', default=default_html_opts['quiz_mode'], action='store_true')
+    
     # Markdown transform
     parser_markdown = transform_parser.add_parser('markdown', help='Convert to MARKDOWN', parents=[global_parser], add_help=True)
 
     # YAML transform
     parser_yaml = transform_parser.add_parser('yaml', help='Convert to YAML', parents=[global_parser], add_help=True)
     parser_yaml.add_argument('--root_name', type=str, help='Root name of YAML', default=default_yaml_opts['root_name'])
 
@@ -699,17 +734,21 @@
         try:
             os.mkdir(html_path)
         except Exception:
             pass
         
         to_html_report(data_df, os.path.join(html_path, f'{name}.html'), encoding=args.encoding, show_correct=show_correct, **update_defaults(args, default_html_opts))
         
-        # copy over the CSS file
+        # copy over the CSS and JS file
         try:
             shutil.copyfile(styles_path, os.path.join(html_path, f'html-styles.css'))
+
+            # only copy js if quiz mode
+            if args.quiz_mode:
+                shutil.copyfile(js_path, os.path.join(html_path, f'html-js.js'))
         except Exception:
             pass
     elif args.transform == 'toml':
         to_toml_report(data_df, os.path.join(args.output_path, f'{name}.toml'), encoding=args.encoding, show_correct=show_correct, **update_defaults(args, default_toml_opts))
     elif args.transform == 'markdown':
         to_markdown_report(data_df, os.path.join(args.output_path, f'{name}.md'), encoding=args.encoding, show_correct=show_correct, **update_defaults(args, default_toml_opts))
     elif args.transform == 'txt':
```

### Comparing `pollev-history-compiler-1.0.2/resources/config.ini` & `pollev-history-compiler-1.0.3/resources/config.ini`

 * *Files identical despite different names*

### Comparing `pollev-history-compiler-1.0.2/setup.py` & `pollev-history-compiler-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pollev-history-compiler",
-    version="1.0.2",
+    version="1.0.3",
     author="Tony Abou Zeidan",
     author_email="tony.azp25@gmail.com",
     description="A script for the compilation of PollEverywhere history CSV files into more usable forms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tony-zeidan/PollEvHistoryCompiler",
     packages=find_packages(),
@@ -20,15 +20,16 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     python_requires=">=3.6",
     install_requires=[
         'pandas',
-        'markdownify'
+        'markdownify',
+        'toml'
     ],
     package_data={
         "pollev_tools": [
             "../resources/html-styles.css",
             "../resources/config.ini",
 
         ],
```

