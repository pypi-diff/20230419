# Comparing `tmp/one_block-0.1.1.tar.gz` & `tmp/one_block-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one_block-0.1.1.tar", max compression
+gzip compressed data, was "one_block-0.1.2.tar", max compression
```

## Comparing `one_block-0.1.1.tar` & `one_block-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1074 2023-04-03 15:08:01.927054 one_block-0.1.1/LICENSE
--rw-r--r--   0        0        0     1312 2023-04-03 15:08:01.927054 one_block-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/__init__.py
--rw-r--r--   0        0        0      196 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/accessory/__init__.py
--rw-r--r--   0        0        0       90 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/accessory/accessory.py
--rw-r--r--   0        0        0     1120 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/accessory/button.py
--rw-r--r--   0        0        0      400 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/accessory/checkbox.py
--rw-r--r--   0        0        0      717 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/accessory/option.py
--rw-r--r--   0        0        0      415 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/accessory/overflow.py
--rw-r--r--   0        0        0     1329 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/accessory/picker.py
--rw-r--r--   0        0        0      454 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/accessory/radio.py
--rw-r--r--   0        0        0     2648 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/accessory/selects.py
--rw-r--r--   0        0        0       23 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/actions/__init__.py
--rw-r--r--   0        0        0      353 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/actions/actions.py
--rw-r--r--   0        0        0      647 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/base.py
--rw-r--r--   0        0        0       29 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/context/__init__.py
--rw-r--r--   0        0        0      301 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/context/context.py
--rw-r--r--   0        0        0       27 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/divider/__init__.py
--rw-r--r--   0        0        0      132 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/divider/plain.py
--rw-r--r--   0        0        0       22 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/header/__init__.py
--rw-r--r--   0        0        0      254 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/header/header.py
--rw-r--r--   0        0        0       21 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/image/__init__.py
--rw-r--r--   0        0        0      587 2023-04-03 15:08:01.927054 one_block-0.1.1/one_block/image/image.py
--rw-r--r--   0        0        0       49 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/input_blocks/__init__.py
--rw-r--r--   0        0        0      574 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/input_blocks/plain_text_input.py
--rw-r--r--   0        0        0      444 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/input_blocks/selects.py
--rw-r--r--   0        0        0      703 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/input_blocks/text_input.py
--rw-r--r--   0        0        0      143 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/__init__.py
--rw-r--r--   0        0        0      856 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/button.py
--rw-r--r--   0        0        0      419 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/checkbox.py
--rw-r--r--   0        0        0      436 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/image.py
--rw-r--r--   0        0        0      255 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/markdown.py
--rw-r--r--   0        0        0      397 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/overflow.py
--rw-r--r--   0        0        0      860 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/picker.py
--rw-r--r--   0        0        0      277 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/plain_text.py
--rw-r--r--   0        0        0      427 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/radio_buttons.py
--rw-r--r--   0        0        0     2008 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/selects.py
--rw-r--r--   0        0        0      327 2023-04-03 15:08:01.931054 one_block-0.1.1/one_block/section/text_fields.py
--rw-r--r--   0        0        0     1007 2023-04-03 15:08:01.931054 one_block-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 one_block-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-18 22:22:40.858196 one_block-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1306 2023-04-18 22:22:40.858196 one_block-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 22:22:40.858196 one_block-0.1.2/one_block/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-18 22:22:40.858196 one_block-0.1.2/one_block/accessory/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-18 22:22:40.858196 one_block-0.1.2/one_block/accessory/accessory.py
+-rw-r--r--   0        0        0      903 2023-04-18 22:22:40.858196 one_block-0.1.2/one_block/accessory/button.py
+-rw-r--r--   0        0        0      500 2023-04-18 22:22:40.858196 one_block-0.1.2/one_block/accessory/checkbox.py
+-rw-r--r--   0        0        0      611 2023-04-18 22:22:40.858196 one_block-0.1.2/one_block/accessory/option.py
+-rw-r--r--   0        0        0      415 2023-04-18 22:22:40.858196 one_block-0.1.2/one_block/accessory/overflow.py
+-rw-r--r--   0        0        0     1314 2023-04-18 22:22:40.858196 one_block-0.1.2/one_block/accessory/picker.py
+-rw-r--r--   0        0        0      454 2023-04-18 22:22:40.858196 one_block-0.1.2/one_block/accessory/radio.py
+-rw-r--r--   0        0        0     2660 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/accessory/selects.py
+-rw-r--r--   0        0        0       23 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/actions/__init__.py
+-rw-r--r--   0        0        0      353 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/actions/actions.py
+-rw-r--r--   0        0        0      641 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/base.py
+-rw-r--r--   0        0        0       29 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/context/__init__.py
+-rw-r--r--   0        0        0      301 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/context/context.py
+-rw-r--r--   0        0        0       27 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/divider/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/divider/plain.py
+-rw-r--r--   0        0        0       22 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/header/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/header/header.py
+-rw-r--r--   0        0        0       21 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/image/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/image/image.py
+-rw-r--r--   0        0        0       49 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/input_blocks/__init__.py
+-rw-r--r--   0        0        0      574 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/input_blocks/plain_text_input.py
+-rw-r--r--   0        0        0      434 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/input_blocks/selects.py
+-rw-r--r--   0        0        0      693 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/input_blocks/text_input.py
+-rw-r--r--   0        0        0      143 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/__init__.py
+-rw-r--r--   0        0        0      549 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/button.py
+-rw-r--r--   0        0        0      426 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/checkbox.py
+-rw-r--r--   0        0        0      420 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/image.py
+-rw-r--r--   0        0        0      262 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/markdown.py
+-rw-r--r--   0        0        0      426 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/overflow.py
+-rw-r--r--   0        0        0      878 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/picker.py
+-rw-r--r--   0        0        0      267 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/plain_text.py
+-rw-r--r--   0        0        0      434 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/radio_buttons.py
+-rw-r--r--   0        0        0     2059 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/selects.py
+-rw-r--r--   0        0        0      327 2023-04-18 22:22:40.862196 one_block-0.1.2/one_block/section/text_fields.py
+-rw-r--r--   0        0        0     1007 2023-04-18 22:22:40.862196 one_block-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 one_block-0.1.2/PKG-INFO
```

### Comparing `one_block-0.1.1/LICENSE` & `one_block-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `one_block-0.1.1/README.md` & `one_block-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# slack-blocks
+# one-block
 
-`slack-blocks` has started as I needed to start using [Slack's Block Kit](https://api.slack.com/block-kit) for the
+`one-block` has started as I needed to start using [Slack's Block Kit](https://api.slack.com/block-kit) for the
 design of my application. While there are [a few Python packages available](#alternative-python-implementations)
 already, they were either using a license I was uncomfortable with, or have simply not been kept up-to-date.
 
 > Note, this is still a pre-release version, and as such, features might change or go away entirely.
 
 ## Available features
```

### Comparing `one_block-0.1.1/one_block/accessory/picker.py` & `one_block-0.1.2/one_block/accessory/picker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from one_block.accessory import Accessory
-from one_block.base import BasePlainText
+from one_block.base import BaseText
 
 
 class DatePicker(Accessory):
     def __init__(self, action_id, initial_date=None, placeholder=None):
         self.action_id = action_id
         self.initial_date = initial_date
         if placeholder:
-            self.placeholder = BasePlainText(placeholder)
+            self.placeholder = BaseText(placeholder)
         else:
             self.placeholder = None
 
     def json(self):
         base = {
             'type': 'datepicker',
             'action_id': self.action_id
@@ -24,15 +24,15 @@
 
 
 class TimePicker(Accessory):
     def __init__(self, action_id, initial_time=None, placeholder=None):
         self.action_id = action_id
         self.initial_time = initial_time
         if placeholder:
-            self.placeholder = BasePlainText(placeholder)
+            self.placeholder = BaseText(placeholder)
         else:
             self.placeholder = None
 
     def json(self):
         base = {
             'type': 'timepicker',
             'action_id': self.action_id
```

### Comparing `one_block-0.1.1/one_block/accessory/selects.py` & `one_block-0.1.2/one_block/accessory/selects.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from one_block import base
 from one_block.accessory import Accessory, Option
 
 
 class UserSelect(Accessory):
     def __init__(self, placeholder, action_id, initial=None, multi=False):
-        self.placeholder = base.BaseMarkdown(placeholder)
+        self.placeholder = base.BaseText(placeholder, markdown=True)
         self.action_id = action_id
         self.initial = initial
         self.multi = multi
 
     def json(self):
         select_type = 'users_select' if not self.multi else 'multi_users_select'
         base = {
@@ -21,15 +21,15 @@
         if self.initial:
             base['initial_user'] = self.initial
         return base
 
 
 class StaticSelect(Accessory):
     def __init__(self, placeholder, action_id, options: List[Option], initial=None, multi=False):
-        self.placeholder = base.BasePlainText(placeholder)
+        self.placeholder = base.BaseText(placeholder)
         self.action_id = action_id
         self.options = options
         self.initial = initial
         self.multi = multi
 
     def json(self):
         select_type = 'static_select' if not self.multi else 'multi_static_select'
@@ -42,15 +42,15 @@
             ]
         }
         return base
 
 
 class ConversationSelect(Accessory):
     def __init__(self, placeholder, action_id, initial=None, multi=False):
-        self.placeholder = base.BaseMarkdown(placeholder)
+        self.placeholder = base.BaseText(placeholder, markdown=True)
         self.action_id = action_id
         self.initial = initial
         self.multi = multi
 
     def json(self):
         select_type = 'conversations_select' if not self.multi else 'multi_conversations_select'
         base = {
@@ -61,15 +61,15 @@
         if self.initial:
             base['initial_conversation'] = self.initial
         return base
 
 
 class ChannelSelect(Accessory):
     def __init__(self, placeholder, action_id, initial=None, multi=False):
-        self.placeholder = base.BasePlainText(placeholder)
+        self.placeholder = base.BaseText(placeholder)
         self.action_id = action_id
         self.initial = initial
         self.multi = multi
 
     def json(self):
         select_type = 'channels_select' if not self.multi else 'multi_channels_select'
         base = {
```

### Comparing `one_block-0.1.1/one_block/image/image.py` & `one_block-0.1.2/one_block/image/image.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from one_block.accessory import Accessory
-from one_block.base import BasePlainText
+from one_block.base import BaseText
 
 
 class Image(Accessory):
     def __init__(self, image_url, alt_text, title=None):
         self.image_url = image_url
         self.alt_text = alt_text
         if title:
-            self.title = BasePlainText(title)
+            self.title = BaseText(title)
         else:
             self.title = None
 
     def json(self):
         base = {
             'type': 'image',
             'image_url': self.image_url,
```

### Comparing `one_block-0.1.1/one_block/input_blocks/plain_text_input.py` & `one_block-0.1.2/one_block/input_blocks/plain_text_input.py`

 * *Files identical despite different names*

### Comparing `one_block-0.1.1/one_block/input_blocks/text_input.py` & `one_block-0.1.2/one_block/input_blocks/text_input.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from one_block.base import Base, BasePlainText
+from one_block.base import Base, BaseText
 from one_block.input_blocks.plain_text_input import PlainTextInput
 
 
 class TextInput(Base):
     def __init__(self, label, action_id, block_id, dispatch=False, multiline=False, custom_triggers=None):
-        self.label = BasePlainText(label)
+        self.label = BaseText(label)
         self.dispatch = dispatch
         self.block_id = block_id
         self.element = PlainTextInput(action_id, multiline=multiline, custom_triggers=custom_triggers)
 
     def json(self):
         return {
             'dispatch_action': self.dispatch,
```

### Comparing `one_block-0.1.1/one_block/section/picker.py` & `one_block-0.1.2/one_block/section/picker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from one_block import accessory
-from one_block.base import Base, BaseMarkdown
+from one_block.base import Base, BaseText
 
 
 class DatePicker(Base):
     def __init__(self, text, action_id, initial_date=None, placeholder=None):
-        self.text = BaseMarkdown(text)
+        self.text = BaseText(text, markdown=True)
         self.accessory = accessory.DatePicker(action_id, initial_date, placeholder)
 
     def json(self):
         return {
             'type': 'section',
             'text': self.text.json(),
             'accessory': self.accessory.json()
         }
 
 
 class TimePicker(Base):
     def __init__(self, text, action_id, initial_time=None, placeholder=None):
-        self.text = BaseMarkdown(text)
+        self.text = BaseText(text, markdown=True)
         self.accessory = accessory.DatePicker(action_id, initial_time, placeholder)
 
     def json(self):
         return {
             'type': 'section',
             'text': self.text.json(),
             'accessory': self.accessory.json()
```

### Comparing `one_block-0.1.1/pyproject.toml` & `one_block-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "one-block"
-version = "0.1.1"
+version = "0.1.2"
 description = "An easy-to-use, opinionated slack blockkit implementation"
 authors = ["Dragos Dumitrache <dragos@afterburner.dev>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "one_block"}]
```

### Comparing `one_block-0.1.1/PKG-INFO` & `one_block-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: one-block
-Version: 0.1.1
+Version: 0.1.2
 Summary: An easy-to-use, opinionated slack blockkit implementation
 License: MIT
 Author: Dragos Dumitrache
 Author-email: dragos@afterburner.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-# slack-blocks
+# one-block
 
-`slack-blocks` has started as I needed to start using [Slack's Block Kit](https://api.slack.com/block-kit) for the
+`one-block` has started as I needed to start using [Slack's Block Kit](https://api.slack.com/block-kit) for the
 design of my application. While there are [a few Python packages available](#alternative-python-implementations)
 already, they were either using a license I was uncomfortable with, or have simply not been kept up-to-date.
 
 > Note, this is still a pre-release version, and as such, features might change or go away entirely.
 
 ## Available features
```

