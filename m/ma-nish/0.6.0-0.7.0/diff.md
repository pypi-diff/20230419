# Comparing `tmp/ma-nish-0.6.0.tar.gz` & `tmp/ma-nish-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma-nish-0.6.0.tar", last modified: Sun Apr 16 15:26:55 2023, max compression
+gzip compressed data, was "ma-nish-0.7.0.tar", last modified: Wed Apr 19 21:19:43 2023, max compression
```

## Comparing `ma-nish-0.6.0.tar` & `ma-nish-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:26:55.386890 ma-nish-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-16 15:26:41.000000 ma-nish-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-16 15:26:55.386890 ma-nish-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-16 15:26:41.000000 ma-nish-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:26:55.386890 ma-nish-0.6.0/ma_nish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:26:55.386890 ma-nish-0.6.0/manish/
--rw-r--r--   0 runner    (1001) docker     (123)    37823 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/template.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:26:55.386890 ma-nish-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-16 15:26:41.000000 ma-nish-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:19:43.247946 ma-nish-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 21:19:32.000000 ma-nish-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-19 21:19:43.247946 ma-nish-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-19 21:19:32.000000 ma-nish-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:19:43.247946 ma-nish-0.7.0/ma_nish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-19 21:19:43.000000 ma-nish-0.7.0/ma_nish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 21:19:43.000000 ma-nish-0.7.0/ma_nish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:19:43.000000 ma-nish-0.7.0/ma_nish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 21:19:43.000000 ma-nish-0.7.0/ma_nish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 21:19:43.000000 ma-nish-0.7.0/ma_nish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:19:43.247946 ma-nish-0.7.0/manish/
+-rw-r--r--   0 runner    (1001) docker     (123)    38717 2023-04-19 21:19:32.000000 ma-nish-0.7.0/manish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-19 21:19:32.000000 ma-nish-0.7.0/manish/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-19 21:19:32.000000 ma-nish-0.7.0/manish/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-19 21:19:32.000000 ma-nish-0.7.0/manish/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-19 21:19:32.000000 ma-nish-0.7.0/manish/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-19 21:19:32.000000 ma-nish-0.7.0/manish/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 21:19:43.247946 ma-nish-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-19 21:19:32.000000 ma-nish-0.7.0/setup.py
```

### Comparing `ma-nish-0.6.0/LICENSE` & `ma-nish-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ma-nish-0.6.0/PKG-INFO` & `ma-nish-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma-nish
-Version: 0.6.0
+Version: 0.7.0
 Summary: manish is an unofficial python wrapper for Whatsapp cloud api
 Home-page: https://github.com/t0mer/ma-nish
 Download-URL: https://pypi.org/project/ma-nish/
 Author: Tomer Klein
 Author-email: tomer.klein@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/t0mer/ma-nish
```

### Comparing `ma-nish-0.6.0/README.md` & `ma-nish-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ma-nish-0.6.0/ma_nish.egg-info/PKG-INFO` & `ma-nish-0.7.0/ma_nish.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma-nish
-Version: 0.6.0
+Version: 0.7.0
 Summary: manish is an unofficial python wrapper for Whatsapp cloud api
 Home-page: https://github.com/t0mer/ma-nish
 Download-URL: https://pypi.org/project/ma-nish/
 Author: Tomer Klein
 Author-email: tomer.klein@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/t0mer/ma-nish
```

### Comparing `ma-nish-0.6.0/manish/__init__.py` & `ma-nish-0.7.0/manish/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,43 @@
             self.headers = {
                 "Content-Type": "application/json",
                 "Authorization": "Bearer {}".format(self.token),
             }
         except Exception as e:
             logger.error("Error initializing MaNish: " + str(e))
 
+
+    def set_status(self, message_id):
+        """
+        Change the status of a message.
+        Args:
+            message_id[str]: The id of the message
+        Example:
+            ```python
+            >>> from manish import MaNish
+            >>> manish = MaNish(token, phone_number_id)
+            >>> manish.set_status(message_id)
+
+        """
+        try:
+            data = {
+                "messaging_product": "whatsapp",
+                "status": "read",
+                "message_id": message_id
+            }
+            r = requests.post(f"{self.url}", headers=self.headers, json=data)
+            if r.status_code == 200:
+                logger.info(f"Message ID {message_id} marked as read")
+                return r.json()
+        except Exception as e:
+            logger.error("aw snap something went wrong: " + str(e))
+            return '{"error":"' + str(e)  + '"}'
+
+
+
     def send_message(self, message, recipient_id, recipient_type="individual", preview_url=True):
         """
          Sends a text message to a WhatsApp user
          Args:
                 message[str]: Message to be sent to the user
                 recipient_id[str]: Phone number of the user with country code wihout +
                 recipient_type[str]: Type of the recipient, either individual or group
@@ -664,15 +693,15 @@
 
     def get_message_id(self, data):
         """
         Extracts the message id of the sender from the data received from the webhook.
         Args:
             data[dict]: The data received from the webhook
         Returns:
-            str: The message id of the sender
+            str: The message id of the message
         Example:
             >>> from manish import MaNish
             >>> manish = MaNish(token, phone_number_id)
             >>> message_id = manish.get_message_id(data)
         """
         try:
             data = self.preprocess(data)
```

### Comparing `ma-nish-0.6.0/manish/button.py` & `ma-nish-0.7.0/manish/button.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.6.0/manish/contact.py` & `ma-nish-0.7.0/manish/contact.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.6.0/manish/helpers.py` & `ma-nish-0.7.0/manish/helpers.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.6.0/manish/location.py` & `ma-nish-0.7.0/manish/location.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.6.0/manish/template.py` & `ma-nish-0.7.0/manish/template.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.6.0/setup.py` & `ma-nish-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="UTF-8") as f:
      readme = f.read()
 
 
 setup_args = dict(
     name='ma-nish',
-    version='0.6.0',
+    version='0.7.0',
     description='manish is an unofficial python wrapper for Whatsapp cloud api',
     long_description_content_type="text/markdown",
     long_description=readme,
     license='MIT',
     packages=find_packages(),
     author='Tomer Klein',
     author_email='tomer.klein@gmail.com',
```

