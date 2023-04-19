# Comparing `tmp/zood-0.6.6.tar.gz` & `tmp/zood-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zood-0.6.6.tar", max compression
+gzip compressed data, was "zood-0.6.7.tar", max compression
```

## Comparing `zood-0.6.6.tar` & `zood-0.6.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      550 2023-04-02 00:15:02.205669 zood-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.6.6/README.md
--rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.6.6/zood/__init__.py
--rw-r--r--   0        0        0     5924 2023-04-01 23:48:51.709845 zood-0.6.6/zood/config/_config.yml
--rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.6.6/zood/config/img/after_copy.png
--rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.6.6/zood/config/img/before_copy.png
--rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.6.6/zood/config/img/enter.png
--rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.6.6/zood/config/img/enter.svg
--rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.6.6/zood/config/img/moon.png
--rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.6.6/zood/config/img/search.svg
--rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.6.6/zood/config/img/sun.png
--rw-r--r--   0        0        0    17456 2023-04-02 00:14:32.929281 zood-0.6.6/zood/config/index.css
--rw-r--r--   0        0        0     3547 2023-02-19 10:19:17.056632 zood-0.6.6/zood/config/js/change_mode.js
--rw-r--r--   0        0        0      955 2023-04-02 00:07:20.610243 zood-0.6.6/zood/config/js/check_box.js
--rw-r--r--   0        0        0     1064 2023-03-05 08:47:36.973322 zood-0.6.6/zood/config/js/copy_code.js
--rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.6.6/zood/config/js/next_front.js
--rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.6.6/zood/config/js/picture_preview.js
--rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.6.6/zood/config/js/picture_title.js
--rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.6.6/zood/config/js/prismjs/prism.css
--rw-r--r--   0        0        0    52330 2023-03-23 13:29:38.926084 zood-0.6.6/zood/config/js/prismjs/prism.js
--rw-r--r--   0        0        0     5911 2023-02-19 10:17:58.103017 zood-0.6.6/zood/config/js/search.js
--rw-r--r--   0        0        0      980 2023-02-24 16:17:35.264950 zood-0.6.6/zood/config/template.html
--rw-r--r--   0        0        0     4224 2023-01-17 16:20:04.563105 zood-0.6.6/zood/main.py
--rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.6.6/zood/md_parser.py
--rw-r--r--   0        0        0     4290 2023-02-19 08:16:38.877522 zood-0.6.6/zood/util.py
--rw-r--r--   0        0        0     8017 2023-03-08 03:42:01.835849 zood-0.6.6/zood/zood.py
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.6.6/setup.py
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-04-19 13:14:12.551676 zood-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.6.7/README.md
+-rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.6.7/zood/__init__.py
+-rw-r--r--   0        0        0     5924 2023-04-01 23:48:51.709845 zood-0.6.7/zood/config/_config.yml
+-rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.6.7/zood/config/img/after_copy.png
+-rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.6.7/zood/config/img/before_copy.png
+-rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.6.7/zood/config/img/enter.png
+-rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.6.7/zood/config/img/enter.svg
+-rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.6.7/zood/config/img/moon.png
+-rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.6.7/zood/config/img/search.svg
+-rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.6.7/zood/config/img/sun.png
+-rw-r--r--   0        0        0    17324 2023-04-19 11:34:46.154555 zood-0.6.7/zood/config/index.css
+-rw-r--r--   0        0        0     3547 2023-02-19 10:19:17.056632 zood-0.6.7/zood/config/js/change_mode.js
+-rw-r--r--   0        0        0      955 2023-04-02 00:07:20.610243 zood-0.6.7/zood/config/js/check_box.js
+-rw-r--r--   0        0        0     1282 2023-04-19 11:38:57.244766 zood-0.6.7/zood/config/js/copy_code.js
+-rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.6.7/zood/config/js/next_front.js
+-rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.6.7/zood/config/js/picture_preview.js
+-rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.6.7/zood/config/js/picture_title.js
+-rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.6.7/zood/config/js/prismjs/prism.css
+-rw-r--r--   0        0        0    52330 2023-03-23 13:29:38.926084 zood-0.6.7/zood/config/js/prismjs/prism.js
+-rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.6.7/zood/config/js/search.js
+-rw-r--r--   0        0        0      980 2023-02-24 16:17:35.264950 zood-0.6.7/zood/config/template.html
+-rw-r--r--   0        0        0     4224 2023-04-03 14:22:34.682079 zood-0.6.7/zood/main.py
+-rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.6.7/zood/md_parser.py
+-rw-r--r--   0        0        0     4290 2023-04-03 14:22:32.130915 zood-0.6.7/zood/util.py
+-rw-r--r--   0        0        0     8017 2023-03-08 03:42:01.835849 zood-0.6.7/zood/zood.py
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.6.7/setup.py
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.6.7/PKG-INFO
```

### Comparing `zood-0.6.6/pyproject.toml` & `zood-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zood"
-version = "0.6.6"
+version = "0.6.7"
 description = "web page documentation & comment generation documentation"
 license = "MIT"
 authors = ["kamilu <luzhixing12345@163.com>"]
 readme = "README.md"
 repository = "https://github.com/luzhixing12345/zood"
 documentation = "https://luzhixing12345.github.io/zood/"
```

### Comparing `zood-0.6.6/zood/config/_config.yml` & `zood-0.6.7/zood/config/_config.yml`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/config/img/enter.png` & `zood-0.6.7/zood/config/img/enter.png`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/config/index.css` & `zood-0.6.7/zood/config/index.css`

 * *Files 1% similar despite different names*

```diff
@@ -180,16 +180,15 @@
   word-break: normal;
   white-space: pre;
   background: transparent;
   border: 0;
 }
 
 .markdown-body pre code {
-  display: inline;
-  max-width: auto;
+  max-width: 100%;
   padding: 0;
   margin: 0;
   overflow: visible;
   line-height: inherit;
   word-wrap: normal;
   background-color: initial;
   border: 0;
@@ -339,33 +338,27 @@
   position: absolute;
   right: 10px;
   top: 50%;
   margin-top: -16px;
   padding: 3px;
   opacity: 0.9;
   border: 1px solid rgba(149, 157, 165, 0.2);
-  transition: all 0.5s;
   border-radius: 5px;
 }
 
 .markdown-light pre #code_copy {
   background-color: rgb(196, 196, 196);
 }
 
 .markdown-body pre #code_copy:hover {
-  transition: all 0.5s;
   background-color: #ffffff;
   box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
   border-radius: 5px;
 }
 
-.markdown-body pre #code_copy:active {
-  padding: 2px;
-}
-
 .markdown-light :not(pre) > code[class*="language-"],
 .markdown-light pre[class*="language-"] {
   background: "<%markdown_code_bg_color%>";
 }
 
 .markdown-dark :not(pre) > code[class*="language-"],
 .markdown-dark pre[class*="language-"] {
```

### Comparing `zood-0.6.6/zood/config/js/change_mode.js` & `zood-0.6.7/zood/config/js/change_mode.js`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/config/js/check_box.js` & `zood-0.6.7/zood/config/js/check_box.js`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/config/js/copy_code.js` & `zood-0.6.7/zood/config/js/copy_code.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -3,14 +3,19 @@
 
 function add(block) {
     var clip_board = document.createElement('img');
     clip_board.id = 'code_copy';
     clip_board.src = global_before_copy_url;
     clip_board.onclick = function() {
         clip_board.src = global_after_copy_url;
+        var range = document.createRange();
+        range.selectNodeContents(block.firstChild);
+        var selection = window.getSelection();
+        selection.removeAllRanges();
+        selection.addRange(range);
         navigator.clipboard.writeText(block.firstChild.innerText);
     }
     block.appendChild(clip_board)
 }
 
 function remove(block) {
     var clip_board = document.getElementById('code_copy')
```

### Comparing `zood-0.6.6/zood/config/js/next_front.js` & `zood-0.6.7/zood/config/js/next_front.js`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/config/js/picture_preview.js` & `zood-0.6.7/zood/config/js/picture_preview.js`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/config/js/prismjs/prism.css` & `zood-0.6.7/zood/config/js/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/config/js/prismjs/prism.js` & `zood-0.6.7/zood/config/js/prismjs/prism.js`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/config/js/search.js` & `zood-0.6.7/zood/config/js/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -103,15 +103,18 @@
         items[i].lastChild.src = ''
     }
 }
 
 
 function activeSelectedItem() {
 
-    if (searched_result_length == 0) return;
+    if (searched_result_length == 0) {
+        selected_item_index = -1;
+        return;
+    }
 
     center_search_input.blur();
     selected_item_index = (selected_item_index + searched_result_length) % searched_result_length;
     // console.log(selected_item_index,searched_result_length)
     var selected_item = document.getElementsByClassName('search-result-item')[selected_item_index];
     selected_item.classList.add('search-selected');
     selected_item.lastChild.src = enter_img_src;
@@ -152,20 +155,22 @@
     // event.preventDefault();
     var ev = window.event || e;
     if (ev.key === 'k' && ev.ctrlKey) {
         displayCenterSearch()
         ev.preventDefault()
     }
     if (ev.keyCode == 27) {
+        // ESC
         closeCenterSearch()
         ev.preventDefault()
     }
     if (ev.which === 13) {
+        // enter
         var word = center_search_input.value.trim();
-        if (word == '') {
+        if (word === '') {
             closeCenterSearch()
             return;
         }
         if (selected_item_index == -1) {
             // 没有开始选择
             startSearch(word)
         } else {
```

### Comparing `zood-0.6.6/zood/config/template.html` & `zood-0.6.7/zood/config/template.html`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/main.py` & `zood-0.6.7/zood/main.py`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/md_parser.py` & `zood-0.6.7/zood/md_parser.py`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/util.py` & `zood-0.6.7/zood/util.py`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/zood/zood.py` & `zood-0.6.7/zood/zood.py`

 * *Files identical despite different names*

### Comparing `zood-0.6.6/setup.py` & `zood-0.6.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ['MarkdownParser', 'PyYAML>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['zood = zood.main:main']}
 
 setup_kwargs = {
     'name': 'zood',
-    'version': '0.6.6',
+    'version': '0.6.7',
     'description': 'web page documentation & comment generation documentation',
     'long_description': '# zood\n\nzood 是一个辅助文档生成的Python库, zood的页面风格更倾向于纯文档内容而非博客\n\n## 主题预览\n\n[![20230101121438](https://raw.githubusercontent.com/learner-lu/picbed/master/20230101121438.png)](https://luzhixing12345.github.io/zood/)\n\n## 安装与使用\n\n```bash\npip install zood\n```\n\n参见 [用户使用文档](https://luzhixing12345.github.io/zood/)\n\n## 参考\n\n- [UI](https://remixicon.com/)',
     'author': 'kamilu',
     'author_email': 'luzhixing12345@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/luzhixing12345/zood',
```

### Comparing `zood-0.6.6/PKG-INFO` & `zood-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zood
-Version: 0.6.6
+Version: 0.6.7
 Summary: web page documentation & comment generation documentation
 Home-page: https://github.com/luzhixing12345/zood
 License: MIT
 Author: kamilu
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

