# Comparing `tmp/speech2speech-0.2.0.tar.gz` & `tmp/speech2speech-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech2speech-0.2.0.tar", last modified: Mon Apr 17 13:10:52 2023, max compression
+gzip compressed data, was "speech2speech-0.3.0.tar", last modified: Wed Apr 19 09:40:16 2023, max compression
```

## Comparing `speech2speech-0.2.0.tar` & `speech2speech-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-17 13:10:52.385020 speech2speech-0.2.0/
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     6413 2023-04-17 13:10:52.385020 speech2speech-0.2.0/PKG-INFO
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     5721 2023-04-17 12:46:20.000000 speech2speech-0.2.0/README.md
--rw-rw-r--   0 oem1      (1001) oem1      (1001)      612 2023-04-17 12:58:06.000000 speech2speech-0.2.0/pyproject.toml
--rw-rw-r--   0 oem1      (1001) oem1      (1001)       38 2023-04-17 13:10:52.385020 speech2speech-0.2.0/setup.cfg
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     8063 2023-04-17 13:08:30.000000 speech2speech-0.2.0/setup.py
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-17 13:10:52.385020 speech2speech-0.2.0/speech2speech/
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-17 13:10:52.385020 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     6413 2023-04-17 13:10:52.000000 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/PKG-INFO
--rw-rw-r--   0 oem1      (1001) oem1      (1001)      237 2023-04-17 13:10:52.000000 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/SOURCES.txt
--rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-17 13:10:52.000000 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/dependency_links.txt
--rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-17 13:10:52.000000 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/top_level.txt
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-19 09:40:16.110804 speech2speech-0.3.0/
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     5341 2023-04-19 09:40:16.110804 speech2speech-0.3.0/PKG-INFO
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     4649 2023-04-19 09:33:00.000000 speech2speech-0.3.0/README.md
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)      612 2023-04-19 09:39:07.000000 speech2speech-0.3.0/pyproject.toml
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)       38 2023-04-19 09:40:16.110804 speech2speech-0.3.0/setup.cfg
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     8063 2023-04-19 09:38:38.000000 speech2speech-0.3.0/setup.py
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-19 09:40:16.110804 speech2speech-0.3.0/speech2speech/
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-19 09:40:16.110804 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     5341 2023-04-19 09:40:16.000000 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/PKG-INFO
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)      237 2023-04-19 09:40:16.000000 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-19 09:40:16.000000 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-19 09:40:16.000000 speech2speech-0.3.0/speech2speech/speech2speech.egg-info/top_level.txt
```

### Comparing `speech2speech-0.2.0/README.md` & `speech2speech-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,63 @@
 # Speech2Speech
+<img src="speech2speech/imgs/speech2speech.png" alt="image of main screen" 
+height="762" width="723">
 
 The Speech2Speech Python package is a Streamlit Web application that **models 
 all phases of speech-to-speech translation**, including:
 - recording speech in the source language, 
 - converting the source language speech to source language text, 
 - translating the source language text to target language text, and 
 - converting the translated text to speech in the target language. 
 
+As a web application, it can be accessed through any web browser and is 
+**compatible with Linux, Mac, and Windows operating systems**.
+
 Speech2Speech is currently **configured to translate to and from 13 different 
 languages**. Although the quality of  translation may vary depending on the 
 target language, it is pretty good for popular languages such as English, 
 French, Portuguese, Spanish, German, Dutch and Italian. Speech2Speech **can be 
 configured for many more than just these languages** (specified in the config.
 ini file), as long as they are supported by Whisper AI, Chat-GPT and gtts, 
 the packages on which it depends.
 
-The package **automatically detects the source language used in speech**. The 
-user therefore is not asked to specify it.
 
 Speech2Speech is designed to be accessible to a **broad audience**. One of 
-the key advantages of Speech2Speech is that it's incredibly easy to use. 
-There is **no need to train the software or the user before actually using 
+the key advantages of Speech2Speech is that it's incredibly easy to use:
+- The package **automatically detects the source language used in speech**. The 
+user therefore is not asked to specify it.
+- There is **no need to train the software or the user before actually using 
 the product**. It works well straight out of the box with no further tuning 
-or configuration required. This makes it a highly accessible tool that anyone can use, regardless of their technical expertise or experience with speech recognition and machine translation technology.
+or configuration required. 
+This makes it a highly accessible tool that anyone can use, regardless of 
+their technical expertise or experience with speech recognition and machine 
+translation technology. 
+
+It is also hoped that this technology could be leveraged to develop 
+products specifically designed for **persons with visual impairments**. It 
+can empower them to have texts read aloud or dictate their texts 
+and listen to them being read out loud before forwarding them to their 
+intended recipients.
 
 Each phase of the workflow creates a file, whose name is defined in the 
 config.ini file. Advanced users can **start and/or interrupt the workflow 
-wherever they need** by inserting their own files in the speech2speech/data 
+wherever they need** by inserting their own files in the `speech2speech/data` 
 subdirectory and adapting the config.ini file to refer to them. 
 
 Prerequisites
 -----------------------------------------------------------------------------
-Before using Speech2Speech, you need to sign up for an OpenAI account, create an API key, and set up an environment variable. Here's how to do it:
-
-1. **Signup and Create an OpenAI Account**: Go to the OpenAI website and 
-   click on the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
-
-2. **Create an OpenAI API Key**: Click on Personal at the right upper corner  and on the "View API Keys" tab in the OpenAI dashboard. Click on the "Create new secret key" button. Give your API key a name and select the type of API key you want to create (restricted or full). Once you have created your API key, copy it to your clipboard. Make sure to keep your API key secure, as it provides access to powerful computing resources and data.
-
-3. **Create an Environment Variable to Load Your OpenAI API Key**:
-
-   A. **Ubuntu (tested) and Mac (not yet tested)**
-   
-   Open your terminal. Type the following command to open your shell profile file:
-      
-         nano ~/.bashrc
-      
-   Scroll to the bottom of the file and add the following line:
-   
-         export OPENAI_API_KEY=<YOUR_API_KEY>
-      
-   Replace <YOUR_API_KEY> with the API key you created in the previous section. Save and close the file by pressing Ctrl + X, then Y, and then Enter. Type the following command to apply the changes:
-         
-         source ~/.bashrc
-         
-B. **Windows (not yet tested)**
-   
-   Right-click on the "Start" button and select "System".
-   
-   Click on "Advanced system settings".
-   
-   Click on "Environment Variables".
-   
-   Under "User variables", click on "New".
-   
-   Enter "OPENAI_API_KEY" in the "Variable name" field.
-   
-   Enter your API key in the "Variable value" field.
-   
-   Click on "OK" to save the changes.
-   
+You need to [get an OpenAI API key](https://www.howtogeek.com/885918/how-to-get-an-openai-api-key/#autotoc_anchor_0) in order to use this app.
    
-Speech2Speech installation
+Speech2Speech local installation
 --------------------------
-To install Speech2Speech, open your terminal and run the following command:
+Run the following command:
 
     pip install speech2speech
 
-Launch Speech2Speech
-------------------------------------
-To launch Speech2Speech, follow these steps:
+In order to launch it locally follow these steps:
 
 1. Make sure the microphone and speakers of your device are on.
 
 2. Navigate to the directory where your Speech2Speech program is located 
 using the cd command.
 
 3. Type the following command in the terminal to launch Speech2Speech:
@@ -92,21 +66,24 @@
    `streamlit run speech2speech.py`
 
 
 Workflow
 ----------
 Here's a step-by-step guide on how to use the full workflow of Speech2Speech:
 
-1. Click the "Record Audio" button to start recording.
-2. Begin speaking or reading aloud. As long as it supports it, Chat-GPT can 
+1. Copy your OpenAI API key and paste it into the text box below the label 
+   "OpenAI API Key". The API key you enter will not be visible on 
+   the screen by default.
+2. Click the "Record Audio" button to start recording.
+3. Begin speaking or reading aloud. When your dictation is finished, press 
+   CTRL+E to stop recording it. Chat-GPT can 
    automatically detect the 
-   language you're speaking, so there's no need to specify it.
-3. Click the "Stop Recording" button to end the recording.
-4. Click the "Transcribe" button to convert your speech into text. The 
-   transcription will appear on a green background after a few seconds.
+   language you're speaking (as long as it also supports it), so there's no 
+   need to specify it.
+4. Click the "Transcribe" button to convert your dictation into text.
 5. Select your desired target language from the dropdown menu under "Target 
    Language".
 6. Click the "Translate" button to translate the transcription into your 
    chosen target language. The translated text will appear on a blue 
    background after a few seconds.
 7. Click the "Read Translation" button to listen to the translated text.
 8. If you want to repeat the process with a new dictation, click the "Refresh 
@@ -114,8 +91,9 @@
    
 As indicated above, you can also use just parts of this full workflow by specifying the name(s) of the file(s) you want to use in the config.ini file and by clicking the relevant button of the user interface.
 
 What to do if you encounter issues
 -------------------------------
 
 If Chat-GPT or Speech2Speech get stuck or you encounter any issues, simply 
-refresh the browser page.
+refresh the browser page. ChatGPT may, however, have lots of users at certain times 
+of the day and be poorly responsive for a while.
```

### Comparing `speech2speech-0.2.0/pyproject.toml` & `speech2speech-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "speech2speech"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="rcdalj1", email="rcdalj1@gmail.com" },
 ]
 description = "Source lang speech to machine translation to target lang speech"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `speech2speech-0.2.0/setup.py` & `speech2speech-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="speech2speech",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.2.0",  # Required
+    version="0.3.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Speech2Speech is a Python package that performs speech  "
                 "recognition of your voice, followed by translation to a "
                 "target language  of your choice, which is then read out "
                 "aloud by a high-quality voice.",  # Optional
```

