# Comparing `tmp/speech2speech-0.3.0.tar.gz` & `tmp/speech2speech-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech2speech-0.3.0.tar", last modified: Wed Apr 19 09:40:16 2023, max compression
+gzip compressed data, was "speech2speech-0.4.0.tar", last modified: Wed Apr 19 11:56:00 2023, max compression
```

## Comparing `speech2speech-0.3.0.tar` & `speech2speech-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-19 09:40:16.110804 speech2speech-0.3.0/
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     5341 2023-04-19 09:40:16.110804 speech2speech-0.3.0/PKG-INFO
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     4649 2023-04-19 09:33:00.000000 speech2speech-0.3.0/README.md
--rw-rw-r--   0 oem1      (1001) oem1      (1001)      612 2023-04-19 09:39:07.000000 speech2speech-0.3.0/pyproject.toml
--rw-rw-r--   0 oem1      (1001) oem1      (1001)       38 2023-04-19 09:40:16.110804 speech2speech-0.3.0/setup.cfg
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     8063 2023-04-19 09:38:38.000000 speech2speech-0.3.0/setup.py
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-19 09:40:16.110804 speech2speech-0.3.0/speech2speech/
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-19 09:40:16.110804 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     5341 2023-04-19 09:40:16.000000 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/PKG-INFO
--rw-rw-r--   0 oem1      (1001) oem1      (1001)      237 2023-04-19 09:40:16.000000 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/SOURCES.txt
--rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-19 09:40:16.000000 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/dependency_links.txt
--rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-19 09:40:16.000000 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/top_level.txt
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-19 11:56:00.616494 speech2speech-0.4.0/
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     6148 2023-04-19 11:56:00.616494 speech2speech-0.4.0/PKG-INFO
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     5456 2023-04-19 10:55:34.000000 speech2speech-0.4.0/README.md
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)      612 2023-04-19 11:55:31.000000 speech2speech-0.4.0/pyproject.toml
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)       38 2023-04-19 11:56:00.616494 speech2speech-0.4.0/setup.cfg
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     8063 2023-04-19 11:55:04.000000 speech2speech-0.4.0/setup.py
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-19 11:56:00.616494 speech2speech-0.4.0/speech2speech/
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-19 11:56:00.616494 speech2speech-0.4.0/speech2speech/speech2speech.egg-info/
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     6148 2023-04-19 11:56:00.000000 speech2speech-0.4.0/speech2speech/speech2speech.egg-info/PKG-INFO
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)      237 2023-04-19 11:56:00.000000 speech2speech-0.4.0/speech2speech/speech2speech.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-19 11:56:00.000000 speech2speech-0.4.0/speech2speech/speech2speech.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-19 11:56:00.000000 speech2speech-0.4.0/speech2speech/speech2speech.egg-info/top_level.txt
```

### Comparing `speech2speech-0.3.0/PKG-INFO` & `speech2speech-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speech2speech
-Version: 0.3.0
+Version: 0.4.0
 Summary: Source lang speech to machine translation to target lang speech
 Home-page: https://github.com/rcdalj/speech2speech
 Author: rcdalj
 Author-email: rcdalj1 <rcdalj1@gmail.com>
 Project-URL: Homepage, https://github.com/rcdalj/speech2speech
 Project-URL: Bug Tracker, https://github.com/rcdalj/speech2speech/issues
 Keywords: speech_recognition,machine_translation,text_to_speech,python-3,chat-gpt,whisper-ai,pyaudio,gtts
@@ -69,21 +69,43 @@
 
     pip install speech2speech
 
 In order to launch it locally follow these steps:
 
 1. Make sure the microphone and speakers of your device are on.
 
-2. Navigate to the directory where your Speech2Speech program is located 
-using the cd command.
-
-3. Type the following command in the terminal to launch Speech2Speech:
-
-
-   `streamlit run speech2speech.py`
+2. Enter the following URL in your browser to download the project as a zip 
+   file:
+- `https://github.com/rcdalj/speech2speech/archive/refs/heads/master.zip`
+3. Extract the contents of the zip file, thereby creating a local copy of 
+   the project directory
+4. In the terminal or command prompt, place yourself in the root of the 
+   local copy of the project directory (where you find, namely, the requirements.txt file)
+- `cd <full name of root of local project directory>`
+3. Create a virtual environment:
+
+3.1. On Mac and Linux:
+- `python3 -m pip install --user virtualenv`
+- `python3 -m venv venv`
+
+3.2. On Windows:
+- `py -m pip install --user virtualenv`
+- `py -m venv env`
+4. Activate the virtual environment:
+
+4.1. On Mac and Linux
+- `source venv/bin/activate`
+
+4.2. On Windows:
+- `.\env\Scripts\activate`
+5. Install project dependencies:
+- `pip install -r requirements.txt`
+6. Type the following commands in the terminal to launch Speech2Speech:
+- `cd speech2speech`
+- `streamlit run speech2speech.py`
 
 
 Workflow
 ----------
 Here's a step-by-step guide on how to use the full workflow of Speech2Speech:
 
 1. Copy your OpenAI API key and paste it into the text box below the label
```

### Comparing `speech2speech-0.3.0/README.md` & `speech2speech-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,21 +53,43 @@
 
     pip install speech2speech
 
 In order to launch it locally follow these steps:
 
 1. Make sure the microphone and speakers of your device are on.
 
-2. Navigate to the directory where your Speech2Speech program is located 
-using the cd command.
-
-3. Type the following command in the terminal to launch Speech2Speech:
-
-
-   `streamlit run speech2speech.py`
+2. Enter the following URL in your browser to download the project as a zip 
+   file:
+- `https://github.com/rcdalj/speech2speech/archive/refs/heads/master.zip`
+3. Extract the contents of the zip file, thereby creating a local copy of 
+   the project directory
+4. In the terminal or command prompt, place yourself in the root of the 
+   local copy of the project directory (where you find, namely, the requirements.txt file)
+- `cd <full name of root of local project directory>`
+3. Create a virtual environment:
+
+3.1. On Mac and Linux:
+- `python3 -m pip install --user virtualenv`
+- `python3 -m venv venv`
+
+3.2. On Windows:
+- `py -m pip install --user virtualenv`
+- `py -m venv env`
+4. Activate the virtual environment:
+
+4.1. On Mac and Linux
+- `source venv/bin/activate`
+
+4.2. On Windows:
+- `.\env\Scripts\activate`
+5. Install project dependencies:
+- `pip install -r requirements.txt`
+6. Type the following commands in the terminal to launch Speech2Speech:
+- `cd speech2speech`
+- `streamlit run speech2speech.py`
 
 
 Workflow
 ----------
 Here's a step-by-step guide on how to use the full workflow of Speech2Speech:
 
 1. Copy your OpenAI API key and paste it into the text box below the label
```

### Comparing `speech2speech-0.3.0/pyproject.toml` & `speech2speech-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "speech2speech"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="rcdalj1", email="rcdalj1@gmail.com" },
 ]
 description = "Source lang speech to machine translation to target lang speech"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `speech2speech-0.3.0/setup.py` & `speech2speech-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="speech2speech",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.3.0",  # Required
+    version="0.4.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Speech2Speech is a Python package that performs speech  "
                 "recognition of your voice, followed by translation to a "
                 "target language  of your choice, which is then read out "
                 "aloud by a high-quality voice.",  # Optional
```

### Comparing `speech2speech-0.3.0/speech2speech/speech2speech.egg-info/PKG-INFO` & `speech2speech-0.4.0/speech2speech/speech2speech.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speech2speech
-Version: 0.3.0
+Version: 0.4.0
 Summary: Source lang speech to machine translation to target lang speech
 Home-page: https://github.com/rcdalj/speech2speech
 Author: rcdalj
 Author-email: rcdalj1 <rcdalj1@gmail.com>
 Project-URL: Homepage, https://github.com/rcdalj/speech2speech
 Project-URL: Bug Tracker, https://github.com/rcdalj/speech2speech/issues
 Keywords: speech_recognition,machine_translation,text_to_speech,python-3,chat-gpt,whisper-ai,pyaudio,gtts
@@ -69,21 +69,43 @@
 
     pip install speech2speech
 
 In order to launch it locally follow these steps:
 
 1. Make sure the microphone and speakers of your device are on.
 
-2. Navigate to the directory where your Speech2Speech program is located 
-using the cd command.
-
-3. Type the following command in the terminal to launch Speech2Speech:
-
-
-   `streamlit run speech2speech.py`
+2. Enter the following URL in your browser to download the project as a zip 
+   file:
+- `https://github.com/rcdalj/speech2speech/archive/refs/heads/master.zip`
+3. Extract the contents of the zip file, thereby creating a local copy of 
+   the project directory
+4. In the terminal or command prompt, place yourself in the root of the 
+   local copy of the project directory (where you find, namely, the requirements.txt file)
+- `cd <full name of root of local project directory>`
+3. Create a virtual environment:
+
+3.1. On Mac and Linux:
+- `python3 -m pip install --user virtualenv`
+- `python3 -m venv venv`
+
+3.2. On Windows:
+- `py -m pip install --user virtualenv`
+- `py -m venv env`
+4. Activate the virtual environment:
+
+4.1. On Mac and Linux
+- `source venv/bin/activate`
+
+4.2. On Windows:
+- `.\env\Scripts\activate`
+5. Install project dependencies:
+- `pip install -r requirements.txt`
+6. Type the following commands in the terminal to launch Speech2Speech:
+- `cd speech2speech`
+- `streamlit run speech2speech.py`
 
 
 Workflow
 ----------
 Here's a step-by-step guide on how to use the full workflow of Speech2Speech:
 
 1. Copy your OpenAI API key and paste it into the text box below the label
```

