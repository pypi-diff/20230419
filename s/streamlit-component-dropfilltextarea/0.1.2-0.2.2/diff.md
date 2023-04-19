# Comparing `tmp/streamlit-component-dropfilltextarea-0.1.2.tar.gz` & `tmp/streamlit-component-dropfilltextarea-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-component-dropfilltextarea-0.1.2.tar", last modified: Tue Apr 18 11:45:40 2023, max compression
+gzip compressed data, was "streamlit-component-dropfilltextarea-0.2.2.tar", last modified: Wed Apr 19 18:45:40 2023, max compression
```

## Comparing `streamlit-component-dropfilltextarea-0.1.2.tar` & `streamlit-component-dropfilltextarea-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 11:45:40.810479 streamlit-component-dropfilltextarea-0.1.2/
--rwxr-xr-x   0 runner    (1000) runner    (1000)     1069 2023-04-18 10:38:05.000000 streamlit-component-dropfilltextarea-0.1.2/LICENSE
--rwxr-xr-x   0 runner    (1000) runner    (1000)       93 2023-04-18 11:35:11.000000 streamlit-component-dropfilltextarea-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     1342 2023-04-18 11:45:40.810479 streamlit-component-dropfilltextarea-0.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1000) runner    (1000)      833 2023-04-18 10:38:05.000000 streamlit-component-dropfilltextarea-0.1.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-18 11:45:40.810479 streamlit-component-dropfilltextarea-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1000) runner    (1000)      904 2023-04-18 11:44:12.000000 streamlit-component-dropfilltextarea-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 11:45:40.766479 streamlit-component-dropfilltextarea-0.1.2/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 11:45:40.770479 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/
--rwxr-xr-x   0 runner    (1000) runner    (1000)     2514 2023-04-18 10:38:05.000000 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 11:45:40.766479 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 11:45:40.770479 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 11:45:40.770479 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/css/
--rw-r--r--   0 runner    (1000) runner    (1000)      600 2023-04-18 11:45:28.000000 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/css/app.a458ce97.css
--rw-r--r--   0 runner    (1000) runner    (1000)      725 2023-04-18 11:45:28.000000 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/index.html
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 11:45:40.782479 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/js/
--rw-r--r--   0 runner    (1000) runner    (1000)     7676 2023-04-18 11:45:28.000000 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/js/app.087221f4.js
--rw-r--r--   0 runner    (1000) runner    (1000)    28746 2023-04-18 11:45:28.000000 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/js/app.087221f4.js.map
--rw-r--r--   0 runner    (1000) runner    (1000)   865876 2023-04-18 11:45:28.000000 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js
--rw-r--r--   0 runner    (1000) runner    (1000)  3348860 2023-04-18 11:45:28.000000 streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 11:45:40.810479 streamlit-component-dropfilltextarea-0.1.2/src/streamlit_component_dropfilltextarea.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1342 2023-04-18 11:45:40.000000 streamlit-component-dropfilltextarea-0.1.2/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      764 2023-04-18 11:45:40.000000 streamlit-component-dropfilltextarea-0.1.2/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-18 11:45:40.000000 streamlit-component-dropfilltextarea-0.1.2/src/streamlit_component_dropfilltextarea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-04-18 11:45:40.000000 streamlit-component-dropfilltextarea-0.1.2/src/streamlit_component_dropfilltextarea.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2023-04-18 11:45:40.000000 streamlit-component-dropfilltextarea-0.1.2/src/streamlit_component_dropfilltextarea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.533434 streamlit-component-dropfilltextarea-0.2.2/
+-rwxr-xr-x   0 runner    (1000) runner    (1000)     1069 2023-04-18 10:38:05.000000 streamlit-component-dropfilltextarea-0.2.2/LICENSE
+-rwxr-xr-x   0 runner    (1000) runner    (1000)       93 2023-04-18 11:35:11.000000 streamlit-component-dropfilltextarea-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     2570 2023-04-19 18:45:40.529434 streamlit-component-dropfilltextarea-0.2.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1000) runner    (1000)     2061 2023-04-19 18:44:44.000000 streamlit-component-dropfilltextarea-0.2.2/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-19 18:45:40.533434 streamlit-component-dropfilltextarea-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1000) runner    (1000)      904 2023-04-19 18:44:44.000000 streamlit-component-dropfilltextarea-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.517434 streamlit-component-dropfilltextarea-0.2.2/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.521434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/
+-rwxr-xr-x   0 runner    (1000) runner    (1000)     3111 2023-04-19 18:44:44.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.517434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.521434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.521434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/css/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1135 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/css/app.153d1a1e.css
+-rw-r--r--   0 runner    (1000) runner    (1000)      725 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/index.html
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.525434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/
+-rw-r--r--   0 runner    (1000) runner    (1000)     8229 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js
+-rw-r--r--   0 runner    (1000) runner    (1000)    31077 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js.map
+-rw-r--r--   0 runner    (1000) runner    (1000)   865876 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js
+-rw-r--r--   0 runner    (1000) runner    (1000)  3348860 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.529434 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2570 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      764 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/top_level.txt
```

### Comparing `streamlit-component-dropfilltextarea-0.1.2/LICENSE` & `streamlit-component-dropfilltextarea-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.1.2/setup.py` & `streamlit-component-dropfilltextarea-0.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-component-dropfilltextarea",
-    version="0.1.2",
+    version="0.2.2",
     author="Jiayi Chen",
     author_email="chenjiayi_344@hotmail.com",
     description="Streamlit's DropFillTextarea lets users drag and drop files onto a text area, filling in text quickly. It populates text areas with pre-existing files, reducing manual input, while offering layout customization. Ideal for simplifying workflows for both developers and users.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/__init__.py` & `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
 
 
 def st_dropfill_textarea(label, value,
                          placeholder="",
                          layout="column",
+                         labelWidth=None,
                          height=200,
                          key=None):
     component_value = _component_func(
         label=label,
         value=value,
+        labelWidth=labelWidth,
         placeholder=placeholder,
         layout=layout,
         height=height,
         key=key,
         default=value)
     return component_value
 
@@ -55,14 +57,25 @@
     text = ''
     returnText = st_dropfill_textarea(label, text,
                                       placeholder="Type at here",
                                       height=200)
     st.write(f"Returned text: {returnText}")
 
     st.subheader("Component with row layout")
-    label = 'row layout: '
-    text = ''
-    returnText = st_dropfill_textarea(label, text,
-                                      placeholder="Type at here",
+    label = 'short row: '
+    text_short = ''
+    text_short = st_dropfill_textarea(label, text_short,
+                                      placeholder="",
                                       layout="row",
+                                      labelWidth=120,
                                       height=200)
-    st.write(f"Returned text: {returnText}")
+    label = 'looooong row:'
+    text_long = ''
+    text_long = st_dropfill_textarea(label, text_long,
+                                     layout="row",
+                                     labelWidth=120,
+                                     height=200)
+    text_default = ""
+    text_default = st.text_area("streamlit textarea", text_default, height=200)
+    st.write(f"Returned short row: {text_short}")
+    st.write(f"Returned long row: {text_long}")
+    st.write(f"Returned streamlit textarea: {text_default}")
```

### Comparing `streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/index.html` & `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang=en><head><meta charset=utf-8><meta http-equiv=X-UA-Compatible content="IE=edge"><meta name=viewport content="width=device-width,initial-scale=1"><title>streamlit_component_template</title><link href=css/app.a458ce97.css rel=preload as=style><link href=js/app.087221f4.js rel=preload as=script><link href=js/chunk-vendors.e7772cca.js rel=preload as=script><link href=css/app.a458ce97.css rel=stylesheet></head><body><noscript><strong>We're sorry but streamlit_component_template doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id=app></div><script src=js/chunk-vendors.e7772cca.js></script><script src=js/app.087221f4.js></script></body></html>
+<!DOCTYPE html><html lang=en><head><meta charset=utf-8><meta http-equiv=X-UA-Compatible content="IE=edge"><meta name=viewport content="width=device-width,initial-scale=1"><title>streamlit_component_template</title><link href=css/app.153d1a1e.css rel=preload as=style><link href=js/app.fd804a62.js rel=preload as=script><link href=js/chunk-vendors.e7772cca.js rel=preload as=script><link href=css/app.153d1a1e.css rel=stylesheet></head><body><noscript><strong>We're sorry but streamlit_component_template doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id=app></div><script src=js/chunk-vendors.e7772cca.js></script><script src=js/app.fd804a62.js></script></body></html>
```

### Comparing `streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/js/app.087221f4.js` & `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (function(e) {
     function t(t) {
-        for (var r, i, c = t[0], l = t[1], u = t[2], f = 0, d = []; f < c.length; f++) i = c[f], Object.prototype.hasOwnProperty.call(a, i) && a[i] && d.push(a[i][0]), a[i] = 0;
+        for (var r, i, c = t[0], l = t[1], u = t[2], d = 0, f = []; d < c.length; d++) i = c[d], Object.prototype.hasOwnProperty.call(a, i) && a[i] && f.push(a[i][0]), a[i] = 0;
         for (r in l) Object.prototype.hasOwnProperty.call(l, r) && (e[r] = l[r]);
         s && s(t);
-        while (d.length) d.shift()();
+        while (f.length) f.shift()();
         return o.push.apply(o, u || []), n()
     }
 
     function n() {
         for (var e, t = 0; t < o.length; t++) {
             for (var n = o[t], r = !0, c = 1; c < n.length; c++) {
                 var l = n[c];
@@ -83,18 +83,19 @@
         n("1eca")
     },
     "4b1c": function(e, t, n) {
         "use strict";
         n("5084")
     },
     5084: function(e, t, n) {},
-    "9c23": function(e, t, n) {
+    "96e9": function(e, t, n) {
         "use strict";
-        n("f619")
+        n("b380")
     },
+    b380: function(e, t, n) {},
     cd49: function(e, t, n) {
         "use strict";
         n.r(t);
         n("e260"), n("e6cf"), n("cca6"), n("a79d");
         var r = n("830f"),
             a = n("5c40"),
             o = {
@@ -111,47 +112,54 @@
                         args: t
                     }, null, 8, ["args"])]
                 })),
                 _: 1
             })])
         }
         var c = n("9ff4"),
-            l = Object(a["C"])("data-v-b293b72e"),
-            u = l((function(e, t, n, o, i, l) {
+            l = Object(a["C"])("data-v-61db93e8");
+        Object(a["s"])("data-v-61db93e8");
+        var u = {
+            class: "textarea-container",
+            ref: "textarea-container"
+        };
+        Object(a["r"])();
+        var s = l((function(e, t, n, o, i, l) {
                 return Object(a["q"])(), Object(a["d"])("div", {
                     class: "container",
                     style: e.cssProps,
                     ref: "container"
                 }, [Object(a["h"])("div", {
                     class: "label",
                     ref: "label"
-                }, Object(c["F"])(e.label), 513), Object(a["B"])(Object(a["h"])("textarea", {
+                }, Object(c["F"])(e.label), 513), Object(a["h"])("div", u, [Object(a["B"])(Object(a["h"])("textarea", {
                     ref: "textarea",
                     "onUpdate:modelValue": t[1] || (t[1] = function(t) {
                         return e.value = t
                     }),
+                    placeholder: e.args.placeholder,
                     onChange: t[2] || (t[2] = function() {
                         return e.handlesChange.apply(e, arguments)
                     }),
                     onDrop: t[3] || (t[3] = function() {
                         return e.handleDrop.apply(e, arguments)
                     })
-                }, null, 544), [
+                }, null, 40, ["placeholder"]), [
                     [r["b"], e.value]
-                ])], 4)
+                ])], 512)], 4)
             })),
-            s = (n("4de4"), n("a15b"), n("ac1f"), n("5319"), n("498a"), n("b85c")),
+            d = (n("4de4"), n("a15b"), n("ac1f"), n("5319"), n("498a"), n("b85c")),
             f = n("a1e9"),
-            d = n("d092");
+            h = n("d092");
 
         function p() {
             Object(a["n"])((function() {
-                d["a"].setFrameHeight()
+                h["a"].setFrameHeight()
             })), Object(a["p"])((function() {
-                d["a"].setFrameHeight()
+                h["a"].setFrameHeight()
             }))
         }
         /**
          * @license
          * Copyright 2018-2020 Streamlit Inc.
          *
          * Licensed under the Apache License, Version 2.0 (the "License");
@@ -162,15 +170,15 @@
          *
          * Unless required by applicable law or agreed to in writing, software
          * distributed under the License is distributed on an "AS IS" BASIS,
          * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
          * See the License for the specific language governing permissions and
          * limitations under the License.
          */
-        var h = n("c343"),
+        var b = n("c343"),
             v = {
                 name: "DropfillTextarea",
                 props: {
                     args: Object
                 },
                 setup: function() {
                     p()
@@ -190,55 +198,60 @@
                     },
                     cssProps: function() {
                         var e = {
                             "--flex-direction": "column",
                             "--margin-right": "0px",
                             "--container-height": 1.15 * this.args.height + "px",
                             "--textarea-height": this.args.height + "px",
-                            "--align-items": "left"
+                            "--align-items": "left",
+                            "--background-color": "#f0f2f6"
                         };
                         return "column" !== this.args.layout && (e["--flex-direction"] = "row", e["--margin-right"] = "4px", e["--align-items"] = "center"), e
                     }
                 },
                 methods: {
                     renderColumn: function() {
                         var e = this;
                         setTimeout((function() {
                             var t = e.$refs["container"],
                                 n = e.$refs["label"],
                                 r = e.$refs["textarea"],
                                 a = n.clientHeight + r.clientHeight,
-                                o = t.clientWidth - 32 - 2;
-                            t.style.height = a + "px", r.style.width = o + "px"
-                        }), 500)
+                                o = t.clientWidth - 32 - 4;
+                            t.style.height = a + "px", r.style.width = o + "px", r.style.height = e.args.height - 16 + "px"
+                        }), 100)
                     },
                     renderRow: function() {
                         var e = this;
                         setTimeout((function() {
-                            var t = e.$refs["container"],
-                                n = e.$refs["textarea"],
-                                r = 1.1 * n.clientHeight;
-                            t.style.height = r + "px"
-                        }), 500)
+                            var t, n = e.$refs["container"],
+                                r = e.$refs["label"],
+                                a = e.$refs["textarea-container"],
+                                o = e.$refs["textarea"],
+                                i = e.args.labelWidth;
+                            null !== i ? (r.style.width = i + "px", t = n.clientWidth - i - 32 - 8) : t = n.clientWidth - r.clientWidth - 32 - 8;
+                            var c = a.clientHeight;
+                            n.style.height = c + "px", a.style.width = t + "px", a.style.height = e.args.height + "px", o.style.height = e.args.height - 32 + "px"
+                        }), 100)
                     },
                     rerender: function() {
                         "column" === this.args.layout ? this.renderColumn() : this.renderRow()
                     },
                     handlesChange: function() {
-                        d["a"].setComponentValue(this.value)
+                        h["a"].setComponentValue(this.value)
                     },
                     updateValue: function(e) {
                         this.value = e, this.handlesChange()
                     },
                     getTextFromNode: function(e) {
                         var t = "";
                         if (e.nodeType === Node.TEXT_NODE) t += e.textContent.trim();
                         else {
                             var n, r = [],
-                                a = Object(s["a"])(e.childNodes);
+                                a = Object(d["a"])(e.childNodes);
                             try {
                                 for (a.s(); !(n = a.n()).done;) {
                                     var o = n.value;
                                     r.push(this.getTextFromNode(o))
                                 }
                             } catch (i) {
                                 a.e(i)
@@ -252,34 +265,34 @@
                         return t
                     },
                     convertToJson: function(e) {
                         var t, n = new DOMParser,
                             r = n.parseFromString(e, "text/html"),
                             a = r.getElementsByTagName("body")[0],
                             o = [],
-                            i = Object(s["a"])(a.childNodes);
+                            i = Object(d["a"])(a.childNodes);
                         try {
                             for (i.s(); !(t = i.n()).done;) {
                                 var c = t.value,
                                     l = this.getTextFromNode(c);
                                 o.push(l)
                             }
-                        } catch (f) {
-                            i.e(f)
+                        } catch (s) {
+                            i.e(s)
                         } finally {
                             i.f()
                         }
                         var u = o.join("\n");
                         u = u.replace(/(\r\n|\r|\n){2,}/g, "$1\n"), this.updateValue(u)
                     },
                     handleDocx: function(e) {
                         var t = this,
                             n = new FileReader;
                         n.onload = function() {
-                            Object(h["convertToHtml"])({
+                            Object(b["convertToHtml"])({
                                 arrayBuffer: n.result
                             }).then((function(e) {
                                 t.convertToJson(e.value)
                             }))
                         }, n.readAsArrayBuffer(e)
                     },
                     handleHtml: function(e) {
@@ -296,82 +309,82 @@
                             t.updateValue(n.result)
                         }, n.readAsText(e)
                     },
                     fileHandler: function(e) {
                         var t = {
                             "application/vnd.openxmlformats-officedocument.wordprocessingml.document": this.handleDocx,
                             "text/html": this.handleHtml,
-                            "text/plain": this.handlPlainText
+                            "text/plain": this.handlPlainText,
+                            "application/json": this.handlPlainText
                         };
                         return t[e.type]
                     },
                     handleDrop: function(e) {
                         e.preventDefault(), e.stopPropagation();
                         var t = e.dataTransfer.files[0],
                             n = this.fileHandler(t);
                         void 0 !== n ? n(t) : this.updateValue("Dropped file type not supported")
                     }
                 }
             };
-        n("9c23");
-        v.render = u, v.__scopeId = "data-v-b293b72e";
-        var b = v,
-            g = Object(a["C"])("data-v-bef81972");
+        n("96e9");
+        v.render = s, v.__scopeId = "data-v-61db93e8";
+        var g = v,
+            O = Object(a["C"])("data-v-bef81972");
         Object(a["s"])("data-v-bef81972");
-        var m = {
+        var j = {
                 key: 0
             },
-            O = Object(a["h"])("h1", {
+            m = Object(a["h"])("h1", {
                 class: "err__title"
             }, "Component Error", -1),
-            j = {
+            x = {
                 class: "err__msg"
             };
         Object(a["r"])();
-        var y = g((function(e, t, n, r, o, i) {
-                return Object(a["q"])(), Object(a["d"])("div", null, ["" != e.componentError ? (Object(a["q"])(), Object(a["d"])("div", m, [O, Object(a["h"])("div", j, "Message: " + Object(c["F"])(e.componentError), 1)])) : null != e.renderData ? Object(a["t"])(e.$slots, "default", {
+        var y = O((function(e, t, n, r, o, i) {
+                return Object(a["q"])(), Object(a["d"])("div", null, ["" != e.componentError ? (Object(a["q"])(), Object(a["d"])("div", j, [m, Object(a["h"])("div", x, "Message: " + Object(c["F"])(e.componentError), 1)])) : null != e.renderData ? Object(a["t"])(e.$slots, "default", {
                     key: 1,
                     args: e.renderData.args,
                     disabled: e.renderData.disabled
                 }) : Object(a["e"])("", !0)])
             })),
-            x = Object(a["i"])({
+            T = Object(a["i"])({
                 name: "WithStreamlitConnection",
                 setup: function() {
                     var e = Object(f["i"])(void 0),
                         t = Object(f["i"])(""),
                         n = function(n) {
                             var r = n;
                             e.value = r.detail, t.value = ""
                         };
                     return Object(a["n"])((function() {
-                        d["a"].events.addEventListener(d["a"].RENDER_EVENT, n), d["a"].setComponentReady()
+                        h["a"].events.addEventListener(h["a"].RENDER_EVENT, n), h["a"].setComponentReady()
                     })), Object(a["p"])((function() {
-                        "" != t.value && d["a"].setFrameHeight()
+                        "" != t.value && h["a"].setFrameHeight()
                     })), Object(a["o"])((function() {
-                        d["a"].events.removeEventListener(d["a"].RENDER_EVENT, n)
+                        h["a"].events.removeEventListener(h["a"].RENDER_EVENT, n)
                     })), Object(a["m"])((function(e) {
                         t.value = String(e)
                     })), {
                         renderData: e,
                         componentError: t
                     }
                 }
             });
         n("44dc");
-        x.render = y, x.__scopeId = "data-v-bef81972";
-        var T = x,
-            w = Object(a["i"])({
+        T.render = y, T.__scopeId = "data-v-bef81972";
+        var w = T,
+            D = Object(a["i"])({
                 name: "App",
                 components: {
-                    DropfillTextarea: b,
-                    WithStreamlitConnection: T
+                    DropfillTextarea: g,
+                    WithStreamlitConnection: w
                 }
             });
         n("4b1c");
-        w.render = i;
-        var D = w;
-        Object(r["a"])(D).mount("#app")
-    },
-    f619: function(e, t, n) {}
+        D.render = i;
+        var _ = D;
+        Object(r["a"])(_).mount("#app")
+    }
 });
-//# sourceMappingURL=app.087221f4.js.map
+//# sourceMappingURL=app.fd804a62.js.map
```

### Comparing `streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/js/app.087221f4.js.map` & `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8202179031121651%*

 * *Differences: {"'file'": "'js/app.fd804a62.js'",*

 * * "'mappings'": "'aACE,SAASA,EAAqBC,GAQ7B,IAPA,IAMIC,EAAUC,EANVC,EAAWH,EAAK,GAChBI,EAAcJ,EAAK,GACnBK,EAAiBL,EAAK,GAIHM,EAAI,EAAGC,EAAW,GACpCD,EAAIH,EAASK,OAAQF,IACzBJ,EAAUC,EAASG,GAChBG,OAAOC,UAAUC,eAAeC,KAAKC,EAAiBX,IAAYW,EAAgBX,IACpFK,EAASO,KAAKD,EAAgBX,GAAS,IAExCW,EAAgBX,GAAW,EAE5B,IAAID,KAAYG,EACZK,OAAOC,UAAUC,eAAeC,KAAKR,EAAaH,KACpDc,EAAQd,GAAYG,EAAYH,IAG/Be,GAAqBA,EAAoBhB,GAE5C,MAAMO,EAASC,OACdD,EAASU,OAATV,GAOD,OAHAW,EAAgBJ,KAAKK,MAAMD,EAAiBb,GAAkB,IAGvDe,IAER,SAASA, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "js/app.087221f4.js",
-    "mappings": "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",
+    "file": "js/app.fd804a62.js",
+    "mappings": "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",
     "names": [
         "webpackJsonpCallback",
         "data",
         "moduleId",
         "chunkId",
         "chunkIds",
         "moreModules",
@@ -63,18 +63,19 @@
         "jsonpArray",
         "window",
         "oldJsonpFunction",
         "slice",
         "id",
         "args",
         "class",
+        "ref",
         "style",
         "cssProps",
-        "ref",
         "label",
+        "placeholder",
         "handlesChange",
         "handleDrop",
         "useStreamlit",
         "setFrameHeight",
         "props",
         "setup",
         "mounted",
@@ -91,14 +92,16 @@
         "$refs",
         "labelRef",
         "textareaRef",
         "clientHeight",
         "width",
         "clientWidth",
         "renderRow",
+        "textareaContainerRef",
+        "labelWidth",
         "setComponentValue",
         "updateValue",
         "newValue",
         "getTextFromNode",
         "node",
         "text",
         "nodeType",
@@ -163,15 +166,15 @@
         "mount"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///webpack/bootstrap",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue?196c",
         "webpack:///./src/App.vue?3a46",
-        "webpack:///./src/DropfillTextarea.vue?1051",
+        "webpack:///./src/DropfillTextarea.vue?4bbd",
         "webpack:///./src/App.vue",
         "webpack:///./src/DropfillTextarea.vue",
         "webpack:///./src/streamlit/StreamlitVue.ts",
         "webpack:///./src/DropfillTextarea.vue?8ae3",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue?69f8",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue?07d5",
@@ -179,19 +182,19 @@
         "webpack:///./src/App.vue?97f5",
         "webpack:///./src/main.ts"
     ],
     "sourcesContent": [
         " \t// install a JSONP callback for chunk loading\n \tfunction webpackJsonpCallback(data) {\n \t\tvar chunkIds = data[0];\n \t\tvar moreModules = data[1];\n \t\tvar executeModules = data[2];\n\n \t\t// add \"moreModules\" to the modules object,\n \t\t// then flag all \"chunkIds\" as loaded and fire callback\n \t\tvar moduleId, chunkId, i = 0, resolves = [];\n \t\tfor(;i < chunkIds.length; i++) {\n \t\t\tchunkId = chunkIds[i];\n \t\t\tif(Object.prototype.hasOwnProperty.call(installedChunks, chunkId) && installedChunks[chunkId]) {\n \t\t\t\tresolves.push(installedChunks[chunkId][0]);\n \t\t\t}\n \t\t\tinstalledChunks[chunkId] = 0;\n \t\t}\n \t\tfor(moduleId in moreModules) {\n \t\t\tif(Object.prototype.hasOwnProperty.call(moreModules, moduleId)) {\n \t\t\t\tmodules[moduleId] = moreModules[moduleId];\n \t\t\t}\n \t\t}\n \t\tif(parentJsonpFunction) parentJsonpFunction(data);\n\n \t\twhile(resolves.length) {\n \t\t\tresolves.shift()();\n \t\t}\n\n \t\t// add entry modules from loaded chunk to deferred list\n \t\tdeferredModules.push.apply(deferredModules, executeModules || []);\n\n \t\t// run deferred modules when all chunks ready\n \t\treturn checkDeferredModules();\n \t};\n \tfunction checkDeferredModules() {\n \t\tvar result;\n \t\tfor(var i = 0; i < deferredModules.length; i++) {\n \t\t\tvar deferredModule = deferredModules[i];\n \t\t\tvar fulfilled = true;\n \t\t\tfor(var j = 1; j < deferredModule.length; j++) {\n \t\t\t\tvar depId = deferredModule[j];\n \t\t\t\tif(installedChunks[depId] !== 0) fulfilled = false;\n \t\t\t}\n \t\t\tif(fulfilled) {\n \t\t\t\tdeferredModules.splice(i--, 1);\n \t\t\t\tresult = __webpack_require__(__webpack_require__.s = deferredModule[0]);\n \t\t\t}\n \t\t}\n\n \t\treturn result;\n \t}\n\n \t// The module cache\n \tvar installedModules = {};\n\n \t// object to store loaded and loading chunks\n \t// undefined = chunk not loaded, null = chunk preloaded/prefetched\n \t// Promise = chunk loading, 0 = chunk loaded\n \tvar installedChunks = {\n \t\t\"app\": 0\n \t};\n\n \tvar deferredModules = [];\n\n \t// The require function\n \tfunction __webpack_require__(moduleId) {\n\n \t\t// Check if module is in cache\n \t\tif(installedModules[moduleId]) {\n \t\t\treturn installedModules[moduleId].exports;\n \t\t}\n \t\t// Create a new module (and put it into the cache)\n \t\tvar module = installedModules[moduleId] = {\n \t\t\ti: moduleId,\n \t\t\tl: false,\n \t\t\texports: {}\n \t\t};\n\n \t\t// Execute the module function\n \t\tmodules[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n \t\t// Flag the module as loaded\n \t\tmodule.l = true;\n\n \t\t// Return the exports of the module\n \t\treturn module.exports;\n \t}\n\n\n \t// expose the modules object (__webpack_modules__)\n \t__webpack_require__.m = modules;\n\n \t// expose the module cache\n \t__webpack_require__.c = installedModules;\n\n \t// define getter function for harmony exports\n \t__webpack_require__.d = function(exports, name, getter) {\n \t\tif(!__webpack_require__.o(exports, name)) {\n \t\t\tObject.defineProperty(exports, name, { enumerable: true, get: getter });\n \t\t}\n \t};\n\n \t// define __esModule on exports\n \t__webpack_require__.r = function(exports) {\n \t\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n \t\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n \t\t}\n \t\tObject.defineProperty(exports, '__esModule', { value: true });\n \t};\n\n \t// create a fake namespace object\n \t// mode & 1: value is a module id, require it\n \t// mode & 2: merge all properties of value into the ns\n \t// mode & 4: return value when already ns object\n \t// mode & 8|1: behave like require\n \t__webpack_require__.t = function(value, mode) {\n \t\tif(mode & 1) value = __webpack_require__(value);\n \t\tif(mode & 8) return value;\n \t\tif((mode & 4) && typeof value === 'object' && value && value.__esModule) return value;\n \t\tvar ns = Object.create(null);\n \t\t__webpack_require__.r(ns);\n \t\tObject.defineProperty(ns, 'default', { enumerable: true, value: value });\n \t\tif(mode & 2 && typeof value != 'string') for(var key in value) __webpack_require__.d(ns, key, function(key) { return value[key]; }.bind(null, key));\n \t\treturn ns;\n \t};\n\n \t// getDefaultExport function for compatibility with non-harmony modules\n \t__webpack_require__.n = function(module) {\n \t\tvar getter = module && module.__esModule ?\n \t\t\tfunction getDefault() { return module['default']; } :\n \t\t\tfunction getModuleExports() { return module; };\n \t\t__webpack_require__.d(getter, 'a', getter);\n \t\treturn getter;\n \t};\n\n \t// Object.prototype.hasOwnProperty.call\n \t__webpack_require__.o = function(object, property) { return Object.prototype.hasOwnProperty.call(object, property); };\n\n \t// __webpack_public_path__\n \t__webpack_require__.p = \"\";\n\n \tvar jsonpArray = window[\"webpackJsonp\"] = window[\"webpackJsonp\"] || [];\n \tvar oldJsonpFunction = jsonpArray.push.bind(jsonpArray);\n \tjsonpArray.push = webpackJsonpCallback;\n \tjsonpArray = jsonpArray.slice();\n \tfor(var i = 0; i < jsonpArray.length; i++) webpackJsonpCallback(jsonpArray[i]);\n \tvar parentJsonpFunction = oldJsonpFunction;\n\n\n \t// add entry module to deferred list\n \tdeferredModules.push([0,\"chunk-vendors\"]);\n \t// run deferred modules when ready\n \treturn checkDeferredModules();\n",
         "export * from \"-!../../node_modules/mini-css-extract-plugin/dist/loader.js??ref--6-oneOf-1-0!../../node_modules/css-loader/dist/cjs.js??ref--6-oneOf-1-1!../../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/stylePostLoader.js!../../node_modules/postcss-loader/src/index.js??ref--6-oneOf-1-2!../../node_modules/cache-loader/dist/cjs.js??ref--0-0!../../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/index.js??ref--0-1!./WithStreamlitConnection.vue?vue&type=style&index=0&id=bef81972&scoped=true&lang=css\"",
         "export * from \"-!../node_modules/mini-css-extract-plugin/dist/loader.js??ref--6-oneOf-1-0!../node_modules/css-loader/dist/cjs.js??ref--6-oneOf-1-1!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/stylePostLoader.js!../node_modules/postcss-loader/src/index.js??ref--6-oneOf-1-2!../node_modules/cache-loader/dist/cjs.js??ref--0-0!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/index.js??ref--0-1!./App.vue?vue&type=style&index=0&id=9d77823c&lang=css\"",
-        "export * from \"-!../node_modules/mini-css-extract-plugin/dist/loader.js??ref--6-oneOf-1-0!../node_modules/css-loader/dist/cjs.js??ref--6-oneOf-1-1!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/stylePostLoader.js!../node_modules/postcss-loader/src/index.js??ref--6-oneOf-1-2!../node_modules/cache-loader/dist/cjs.js??ref--0-0!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/index.js??ref--0-1!./DropfillTextarea.vue?vue&type=style&index=0&id=b293b72e&scoped=true&lang=css\"",
+        "export * from \"-!../node_modules/mini-css-extract-plugin/dist/loader.js??ref--6-oneOf-1-0!../node_modules/css-loader/dist/cjs.js??ref--6-oneOf-1-1!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/stylePostLoader.js!../node_modules/postcss-loader/src/index.js??ref--6-oneOf-1-2!../node_modules/cache-loader/dist/cjs.js??ref--0-0!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/index.js??ref--0-1!./DropfillTextarea.vue?vue&type=style&index=0&id=61db93e8&scoped=true&lang=css\"",
         "<!-- \n  We bootstrap our Component to Streamlit with our scoped slot in the top-level App.\n  This is where scoped slot passes Streamlit `args` data from itself to children MyComponent.\n  You should not have to edit this, but are free to do so :)\n-->\n<template>\n  <div id=\"app\">\n    <WithStreamlitConnection v-slot=\"{ args }\">\n      <DropfillTextarea :args=\"args\" />\n    </WithStreamlitConnection>\n  </div>\n</template>\n\n<script lang=\"ts\">\nimport { defineComponent } from \"vue\"\nimport DropfillTextarea from \"./DropfillTextarea.vue\"\n\n// \"withStreamlitConnection\" is a scoped slot. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nimport WithStreamlitConnection from \"./streamlit/WithStreamlitConnection.vue\"\n\nexport default defineComponent({\n  name: \"App\",\n  components: {\n    DropfillTextarea,\n    WithStreamlitConnection,\n  },\n})\n</script>\n\n<style>\nbody {\n  margin: 0;\n}\n#app {\n  font-family: Avenir, Helvetica, Arial, sans-serif;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n  color: #2c3e50;\n}\n</style>\n",
-        "<template>\n  <div class=\"container\" :style=\"cssProps\" ref=\"container\">\n    <div class=\"label\" ref=\"label\">\n      {{ label }}\n    </div>\n    <textarea\n      ref=\"textarea\"\n      v-model=\"value\"\n      @change=\"handlesChange\"\n      @drop=\"handleDrop\"\n    />\n  </div>\n</template>\n\n<script>\n  import { ref } from \"vue\";\n  import { Streamlit } from \"streamlit-component-lib\";\n  import { useStreamlit } from \"./streamlit\";\n  import { convertToHtml } from \"mammoth\";\n\n  export default {\n    name: \"DropfillTextarea\",\n    props: {\n      args: Object,\n    }, // Arguments that are passed to the plugin in Python are accessible in prop \"args\"\n    setup() {\n      useStreamlit(); // lifecycle hooks for automatic Streamlit resize\n    },\n\n    data() {\n      const value = ref(\"\");\n      return {\n        value,\n      };\n    },\n\n    mounted() {\n      this.value = ref(this.args.value);\n      this.rerender();\n    },\n\n    computed: {\n      label() {\n        return this.args.label;\n      },\n      cssProps() {\n        const propObj = {\n          \"--flex-direction\": \"column\",\n          \"--margin-right\": \"0px\",\n          \"--container-height\": this.args.height * 1.15 + \"px\",\n          \"--textarea-height\": this.args.height + \"px\",\n          \"--align-items\": \"left\",\n        };\n        if (this.args.layout !== \"column\") {\n          propObj[\"--flex-direction\"] = \"row\";\n          propObj[\"--margin-right\"] = \"4px\";\n          propObj[\"--align-items\"] = \"center\";\n        }\n        return propObj;\n      },\n    },\n\n    methods: {\n      renderColumn() {\n        setTimeout(() => {\n          const containerRef = this.$refs[\"container\"];\n          const labelRef = this.$refs[\"label\"];\n          const textareaRef = this.$refs[\"textarea\"];\n          const height = labelRef.clientHeight + textareaRef.clientHeight;\n          const width = containerRef.clientWidth - 16 * 2 - 2;\n          containerRef.style.height = height + \"px\";\n          textareaRef.style.width = width + \"px\";\n        }, 500);\n      },\n      renderRow() {\n        setTimeout(() => {\n          const containerRef = this.$refs[\"container\"];\n          const textareaRef = this.$refs[\"textarea\"];\n          const height = textareaRef.clientHeight * 1.1;\n          containerRef.style.height = height + \"px\";\n        }, 500);\n      },\n\n      rerender() {\n        if (this.args.layout === \"column\") {\n          this.renderColumn();\n        } else {\n          this.renderRow();\n        }\n      },\n      handlesChange() {\n        Streamlit.setComponentValue(this.value);\n      },\n\n      updateValue(newValue) {\n        this.value = newValue;\n        this.handlesChange();\n      },\n\n      getTextFromNode(node) {\n        let text = \"\";\n        if (node.nodeType === Node.TEXT_NODE) {\n          text += node.textContent.trim();\n        } else {\n          let children = [];\n          for (const child of node.childNodes) {\n            children.push(this.getTextFromNode(child));\n          }\n          children = children.filter((child) => child.length > 0);\n          text += children.join(\"\") + \"\\n\";\n        }\n        return text;\n      },\n\n      convertToJson(html) {\n        const parser = new DOMParser();\n        const dom = parser.parseFromString(html, \"text/html\");\n        const body = dom.getElementsByTagName(\"body\")[0];\n        const content = [];\n        for (const node of body.childNodes) {\n          const text = this.getTextFromNode(node);\n          content.push(text);\n        }\n        let text = content.join(\"\\n\");\n        text = text.replace(/(\\r\\n|\\r|\\n){2,}/g, \"$1\\n\");\n        this.updateValue(text);\n      },\n\n      handleDocx(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          convertToHtml({ arrayBuffer: reader.result }).then((result) => {\n            this.convertToJson(result.value);\n          });\n        };\n\n        reader.readAsArrayBuffer(file);\n      },\n\n      handleHtml(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          this.convertToJson(reader.result);\n        };\n\n        reader.readAsText(file);\n      },\n\n      handlPlainText(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          this.updateValue(reader.result);\n        };\n\n        reader.readAsText(file);\n      },\n\n      fileHandler(file) {\n        const files = {\n          \"application/vnd.openxmlformats-officedocument.wordprocessingml.document\": this\n            .handleDocx,\n          \"text/html\": this.handleHtml,\n          \"text/plain\": this.handlPlainText,\n        };\n        return files[file.type];\n      },\n\n      handleDrop(event) {\n        event.preventDefault();\n        event.stopPropagation(); // stops the browser from redirecting.\n        const file = event.dataTransfer.files[0];\n        const handle = this.fileHandler(file);\n        if (handle !== undefined) handle(file);\n        else this.updateValue(\"Dropped file type not supported\");\n      },\n    },\n  };\n</script>\n\n<style scoped>\n  .container {\n    display: flex;\n    flex-direction: var(--flex-direction);\n    align-items: var(--align-items);\n    height: var(--container-height);\n  }\n  .label {\n    margin-right: var(--margin-right);\n    font: var(--font);\n  }\n  textarea {\n    width: 98%;\n    height: var(--textarea-height);\n    resize: none;\n    padding: 16px;\n    color: var(--text-color);\n    background-color: var(--background-color);\n    font: var(--font);\n  }\n</style>\n",
+        "<template>\n  <div class=\"container\" :style=\"cssProps\" ref=\"container\">\n    <div class=\"label\" ref=\"label\">\n      {{ label }}\n    </div>\n    <div class=\"textarea-container\" ref=\"textarea-container\">\n      <textarea\n        ref=\"textarea\"\n        v-model=\"value\"\n        :placeholder=\"args.placeholder\"\n        @change=\"handlesChange\"\n        @drop=\"handleDrop\"\n      />\n    </div>\n  </div>\n</template>\n\n<script>\n  import { ref } from \"vue\";\n  import { Streamlit } from \"streamlit-component-lib\";\n  import { useStreamlit } from \"./streamlit\";\n  import { convertToHtml } from \"mammoth\";\n\n  export default {\n    name: \"DropfillTextarea\",\n    props: {\n      args: Object,\n    }, // Arguments that are passed to the plugin in Python are accessible in prop \"args\"\n    setup() {\n      useStreamlit(); // lifecycle hooks for automatic Streamlit resize\n    },\n\n    data() {\n      const value = ref(\"\");\n      return {\n        value,\n      };\n    },\n\n    mounted() {\n      this.value = ref(this.args.value);\n      this.rerender();\n    },\n\n    computed: {\n      label() {\n        return this.args.label;\n      },\n      cssProps() {\n        const propObj = {\n          \"--flex-direction\": \"column\",\n          \"--margin-right\": \"0px\",\n          \"--container-height\": this.args.height * 1.15 + \"px\",\n          \"--textarea-height\": this.args.height + \"px\",\n          \"--align-items\": \"left\",\n          \"--background-color\": \"#f0f2f6\",\n        };\n        if (this.args.layout !== \"column\") {\n          propObj[\"--flex-direction\"] = \"row\";\n          propObj[\"--margin-right\"] = \"4px\";\n          propObj[\"--align-items\"] = \"center\";\n        }\n        return propObj;\n      },\n    },\n\n    methods: {\n      renderColumn() {\n        setTimeout(() => {\n          const containerRef = this.$refs[\"container\"];\n          const labelRef = this.$refs[\"label\"];\n          const textareaRef = this.$refs[\"textarea\"];\n          const height = labelRef.clientHeight + textareaRef.clientHeight;\n          const width = containerRef.clientWidth - 16 * 2 - 4;\n          containerRef.style.height = height + \"px\";\n          textareaRef.style.width = width + \"px\";\n          textareaRef.style.height = this.args.height - 16 + \"px\";\n        }, 100);\n      },\n      renderRow() {\n        setTimeout(() => {\n          const containerRef = this.$refs[\"container\"];\n          const labelRef = this.$refs[\"label\"];\n          const textareaContainerRef = this.$refs[\"textarea-container\"];\n          const textareaRef = this.$refs[\"textarea\"];\n          const labelWidth = this.args.labelWidth;\n          let width;\n          if (labelWidth !== null) {\n            labelRef.style.width = labelWidth + \"px\";\n            width = containerRef.clientWidth - labelWidth - 16 * 2 - 8;\n          } else {\n            width =\n              containerRef.clientWidth - labelRef.clientWidth - 16 * 2 - 8;\n          }\n          const height = textareaContainerRef.clientHeight;\n\n          containerRef.style.height = height + \"px\";\n          textareaContainerRef.style.width = width + \"px\";\n          textareaContainerRef.style.height = this.args.height + \"px\";\n          textareaRef.style.height = this.args.height - 16 * 2 + \"px\";\n        }, 100);\n      },\n\n      rerender() {\n        if (this.args.layout === \"column\") {\n          this.renderColumn();\n        } else {\n          this.renderRow();\n        }\n      },\n      handlesChange() {\n        Streamlit.setComponentValue(this.value);\n      },\n\n      updateValue(newValue) {\n        this.value = newValue;\n        this.handlesChange();\n      },\n\n      getTextFromNode(node) {\n        let text = \"\";\n        if (node.nodeType === Node.TEXT_NODE) {\n          text += node.textContent.trim();\n        } else {\n          let children = [];\n          for (const child of node.childNodes) {\n            children.push(this.getTextFromNode(child));\n          }\n          children = children.filter((child) => child.length > 0);\n          text += children.join(\"\") + \"\\n\";\n        }\n        return text;\n      },\n\n      convertToJson(html) {\n        const parser = new DOMParser();\n        const dom = parser.parseFromString(html, \"text/html\");\n        const body = dom.getElementsByTagName(\"body\")[0];\n        const content = [];\n        for (const node of body.childNodes) {\n          const text = this.getTextFromNode(node);\n          content.push(text);\n        }\n        let text = content.join(\"\\n\");\n        text = text.replace(/(\\r\\n|\\r|\\n){2,}/g, \"$1\\n\");\n        this.updateValue(text);\n      },\n\n      handleDocx(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          convertToHtml({ arrayBuffer: reader.result }).then((result) => {\n            this.convertToJson(result.value);\n          });\n        };\n\n        reader.readAsArrayBuffer(file);\n      },\n\n      handleHtml(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          this.convertToJson(reader.result);\n        };\n\n        reader.readAsText(file);\n      },\n\n      handlPlainText(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          this.updateValue(reader.result);\n        };\n\n        reader.readAsText(file);\n      },\n\n      fileHandler(file) {\n        const files = {\n          \"application/vnd.openxmlformats-officedocument.wordprocessingml.document\": this\n            .handleDocx,\n          \"text/html\": this.handleHtml,\n          \"text/plain\": this.handlPlainText,\n          \"application/json\": this.handlPlainText,\n        };\n        return files[file.type];\n      },\n\n      handleDrop(event) {\n        event.preventDefault();\n        event.stopPropagation(); // stops the browser from redirecting.\n        const file = event.dataTransfer.files[0];\n        const handle = this.fileHandler(file);\n        if (handle !== undefined) handle(file);\n        else this.updateValue(\"Dropped file type not supported\");\n      },\n    },\n  };\n</script>\n\n<style scoped>\n  .container {\n    display: flex;\n    flex-direction: var(--flex-direction);\n    align-items: var(--align-items);\n    height: var(--container-height);\n  }\n  .label {\n    margin-right: var(--margin-right);\n    font: var(--font);\n    white-space: pre;\n  }\n\n  .textarea-container {\n    width: 100%;\n    display: flex;\n    justify-content: center;\n  }\n  textarea {\n    width: 100%;\n    height: var(--textarea-height);\n    resize: none;\n    padding: 16px;\n    border: none;\n    border-radius: 6px;\n    color: var(--text-color);\n    background-color: var(--background-color);\n    font: var(--font);\n    scrollbar-width: none; /* hide the scrollbar when out of focus */\n    overflow: hidden; /* hide the overflow when out of focus */\n  }\n  textarea:focus {\n    outline: 1px solid red;\n  }\n\n  textarea:hover {\n    scrollbar-width: auto; /* show the scrollbar when in focus */\n    overflow: auto; /* show the overflow when in focus */\n  }\n\n  textarea::-webkit-scrollbar {\n    width: 6px;\n    height: 6px;\n  }\n\n  textarea::-webkit-scrollbar-thumb {\n    border-radius: 100px;\n    background-color: rgba(143, 141, 141, 0.8);\n  }\n\n  textarea::-webkit-scrollbar-track {\n    border-radius: 100px;\n  }\n</style>\n",
         "/**\n * Vue.js specific composables\n */\nimport { onMounted, onUpdated } from \"vue\"\nimport { Streamlit } from \"streamlit-component-lib\"\n\nexport function useStreamlit() {\n  /**\n   * Optional Streamlit Vue-based setup.\n   *\n   * You are not required call this function on your Streamlit\n   * component. If you decide not to call it, you should implement the\n   * `onMounted` and `onUpdated` functions in your own component,\n   * so that your plugin properly resizes.\n   */\n\n  onMounted((): void => {\n    // After we're rendered for the first time, tell Streamlit that our height\n    // has changed.\n    Streamlit.setFrameHeight()\n  })\n\n  onUpdated((): void => {\n    // After we're updated, tell Streamlit that our height may have changed.\n    Streamlit.setFrameHeight()\n  })\n}\n",
-        "import { render } from \"./DropfillTextarea.vue?vue&type=template&id=b293b72e&scoped=true\"\nimport script from \"./DropfillTextarea.vue?vue&type=script&lang=js\"\nexport * from \"./DropfillTextarea.vue?vue&type=script&lang=js\"\n\nimport \"./DropfillTextarea.vue?vue&type=style&index=0&id=b293b72e&scoped=true&lang=css\"\nscript.render = render\nscript.__scopeId = \"data-v-b293b72e\"\n\nexport default script",
+        "import { render } from \"./DropfillTextarea.vue?vue&type=template&id=61db93e8&scoped=true\"\nimport script from \"./DropfillTextarea.vue?vue&type=script&lang=js\"\nexport * from \"./DropfillTextarea.vue?vue&type=script&lang=js\"\n\nimport \"./DropfillTextarea.vue?vue&type=style&index=0&id=61db93e8&scoped=true&lang=css\"\nscript.render = render\nscript.__scopeId = \"data-v-61db93e8\"\n\nexport default script",
         "<template>\n  <div>\n    <!--  Error boundary. If our wrapped component threw an error, display it. -->\n    <div v-if=\"componentError != ''\">\n      <h1 class=\"err__title\">Component Error</h1>\n      <div class=\"err__msg\">Message: {{ componentError }}</div>\n    </div>\n    <!-- \n      Else render the component slot and pass Streamlit event data in `args` props to it.\n      Don't render until we've gotten our first RENDER_EVENT from Streamlit.\n      All components get disabled while the app is being re-run, and become re-enabled when the re-run has finished.\n    -->\n    <slot\n      v-else-if=\"renderData != null\"\n      :args=\"renderData.args\"\n      :disabled=\"renderData.disabled\"\n    ></slot>\n  </div>\n</template>\n\n<script lang=\"ts\">\nimport {\n  ref,\n  defineComponent,\n  onMounted,\n  onUpdated,\n  onUnmounted,\n  onErrorCaptured,\n} from \"vue\"\nimport { Streamlit, RenderData } from \"streamlit-component-lib\"\n\nexport default defineComponent({\n  name: \"WithStreamlitConnection\",\n  setup() {\n    const renderData = ref<RenderData>((undefined as unknown) as RenderData)\n    const componentError = ref(\"\")\n\n    const onRenderEvent = (event: Event): void => {\n      const renderEvent = event as CustomEvent<RenderData>\n      renderData.value = renderEvent.detail\n      componentError.value = \"\"\n    }\n\n    // Set up event listeners, and signal to Streamlit that we're ready.\n    // We won't render the component until we receive the first RENDER_EVENT.\n    onMounted(() => {\n      Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRenderEvent)\n      Streamlit.setComponentReady()\n    })\n    onUpdated(() => {\n      // If our slot threw an error, we display it in render(). In this\n      // case, the slot won't be mounted and therefore won't call\n      // `setFrameHeight` on its own. We do it here so that the rendered\n      // error will be visible.\n      if (componentError.value != \"\") {\n        Streamlit.setFrameHeight()\n      }\n    })\n    onUnmounted(() => {\n      Streamlit.events.removeEventListener(\n        Streamlit.RENDER_EVENT,\n        onRenderEvent\n      )\n    })\n    onErrorCaptured(err => {\n      componentError.value = String(err)\n    })\n\n    return {\n      renderData,\n      componentError,\n    }\n  },\n})\n</script>\n\n<style scoped>\n.err__title,\n.err__msg {\n  margin: 0;\n}\n</style>\n",
         "\nimport {\n  ref,\n  defineComponent,\n  onMounted,\n  onUpdated,\n  onUnmounted,\n  onErrorCaptured,\n} from \"vue\"\nimport { Streamlit, RenderData } from \"streamlit-component-lib\"\n\nexport default defineComponent({\n  name: \"WithStreamlitConnection\",\n  setup() {\n    const renderData = ref<RenderData>((undefined as unknown) as RenderData)\n    const componentError = ref(\"\")\n\n    const onRenderEvent = (event: Event): void => {\n      const renderEvent = event as CustomEvent<RenderData>\n      renderData.value = renderEvent.detail\n      componentError.value = \"\"\n    }\n\n    // Set up event listeners, and signal to Streamlit that we're ready.\n    // We won't render the component until we receive the first RENDER_EVENT.\n    onMounted(() => {\n      Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRenderEvent)\n      Streamlit.setComponentReady()\n    })\n    onUpdated(() => {\n      // If our slot threw an error, we display it in render(). In this\n      // case, the slot won't be mounted and therefore won't call\n      // `setFrameHeight` on its own. We do it here so that the rendered\n      // error will be visible.\n      if (componentError.value != \"\") {\n        Streamlit.setFrameHeight()\n      }\n    })\n    onUnmounted(() => {\n      Streamlit.events.removeEventListener(\n        Streamlit.RENDER_EVENT,\n        onRenderEvent\n      )\n    })\n    onErrorCaptured(err => {\n      componentError.value = String(err)\n    })\n\n    return {\n      renderData,\n      componentError,\n    }\n  },\n})\n",
         "import { render } from \"./WithStreamlitConnection.vue?vue&type=template&id=bef81972&scoped=true\"\nimport script from \"./WithStreamlitConnection.vue?vue&type=script&lang=ts\"\nexport * from \"./WithStreamlitConnection.vue?vue&type=script&lang=ts\"\n\nimport \"./WithStreamlitConnection.vue?vue&type=style&index=0&id=bef81972&scoped=true&lang=css\"\nscript.render = render\nscript.__scopeId = \"data-v-bef81972\"\n\nexport default script",
         "\nimport { defineComponent } from \"vue\"\nimport DropfillTextarea from \"./DropfillTextarea.vue\"\n\n// \"withStreamlitConnection\" is a scoped slot. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nimport WithStreamlitConnection from \"./streamlit/WithStreamlitConnection.vue\"\n\nexport default defineComponent({\n  name: \"App\",\n  components: {\n    DropfillTextarea,\n    WithStreamlitConnection,\n  },\n})\n",
         "import { render } from \"./App.vue?vue&type=template&id=9d77823c\"\nimport script from \"./App.vue?vue&type=script&lang=ts\"\nexport * from \"./App.vue?vue&type=script&lang=ts\"\n\nimport \"./App.vue?vue&type=style&index=0&id=9d77823c&lang=css\"\nscript.render = render\n\nexport default script",
         "import { createApp } from 'vue'\nimport App from './App.vue'\n\ncreateApp(App).mount('#app')\n"
     ],
```

### Comparing `streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js` & `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.1.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map` & `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.1.2/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt` & `streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/st_dropfill_textarea/__init__.py
 src/st_dropfill_textarea/frontend/dist/index.html
-src/st_dropfill_textarea/frontend/dist/css/app.a458ce97.css
-src/st_dropfill_textarea/frontend/dist/js/app.087221f4.js
-src/st_dropfill_textarea/frontend/dist/js/app.087221f4.js.map
+src/st_dropfill_textarea/frontend/dist/css/app.153d1a1e.css
+src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js
+src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js.map
 src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js
 src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map
 src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO
 src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt
 src/streamlit_component_dropfilltextarea.egg-info/dependency_links.txt
 src/streamlit_component_dropfilltextarea.egg-info/requires.txt
 src/streamlit_component_dropfilltextarea.egg-info/top_level.txt
```

