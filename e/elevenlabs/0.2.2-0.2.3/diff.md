# Comparing `tmp/elevenlabs-0.2.2.tar.gz` & `tmp/elevenlabs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-0.2.2.tar", last modified: Tue Apr 18 20:35:23 2023, max compression
+gzip compressed data, was "elevenlabs-0.2.3.tar", last modified: Wed Apr 19 16:04:46 2023, max compression
```

## Comparing `elevenlabs-0.2.2.tar` & `elevenlabs-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/elevenlabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:04:46.622323 elevenlabs-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 16:04:46.618323 elevenlabs-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:04:46.618323 elevenlabs-0.2.3/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/elevenlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:04:46.618323 elevenlabs-0.2.3/elevenlabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/elevenlabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/elevenlabs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/elevenlabs/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/elevenlabs/api/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/elevenlabs/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/elevenlabs/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/elevenlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:04:46.618323 elevenlabs-0.2.3/elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 16:04:46.000000 elevenlabs-0.2.3/elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-19 16:04:46.000000 elevenlabs-0.2.3/elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:04:46.000000 elevenlabs-0.2.3/elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 16:04:46.000000 elevenlabs-0.2.3/elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 16:04:46.000000 elevenlabs-0.2.3/elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:04:46.622323 elevenlabs-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-19 16:04:34.000000 elevenlabs-0.2.3/setup.py
```

### Comparing `elevenlabs-0.2.2/PKG-INFO` & `elevenlabs-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.2
+Version: 0.2.3
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.2/elevenlabs/__init__.py` & `elevenlabs-0.2.3/elevenlabs/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import wave
 from collections.abc import Iterator
 from typing import List, Optional, Union
 
-from .api import TTS, Voice, Voices, VoiceSettings
+from .api import TTS, Voice, VoiceClone, Voices, VoiceSettings
 from .utils import *  # noqa F403
 
 
 def set_api_key(api_key: str) -> None:
     os.environ["ELEVEN_API_KEY"] = api_key
 
 
@@ -77,18 +77,22 @@
 def get_all_voices(api_key: Optional[str] = None) -> List[Voice]:
     if api_key:
         set_api_key(api_key)
     api_key = get_api_key()
     return Voices.from_api() if api_key else DEFAULT_VOICES
 
 
+def clone(**kwargs) -> Voice:
+    return Voice.from_clone(VoiceClone(**kwargs))
+
+
 def generate(
     text: str,
     api_key: Optional[str] = None,
-    voice: Union[str, Voice] = "Bella",
+    voice: Union[str, Voice] = DEFAULT_VOICES[2],  # Bella
     stream: bool = False,
     stream_chunk_size: int = 2048,
 ) -> Union[bytes, Iterator[bytes]]:
     if api_key:
         set_api_key(api_key)
 
     # Find first voice with matching name or id if string provided
```

### Comparing `elevenlabs-0.2.2/elevenlabs/api/base.py` & `elevenlabs-0.2.3/elevenlabs/api/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,48 +4,41 @@
 import requests  # type: ignore
 from pydantic import BaseModel
 
 api_base_url_v1 = "https://api.elevenlabs.io/v1"
 
 
 class API(BaseModel):
+    class Config:
+        # Parse enum to strings when converting to dict
+        use_enum_values = True
+        # Validate fields when setting manually
+        validate_assignment = True
+
     @staticmethod
-    def request(
-        url: str,
-        method: str,
-        data: Optional[dict] = None,
-        files=None,
-        api_key: Optional[str] = None,
-        stream: bool = False,
-    ):
-        headers = {
-            "Accept": "application/json",
-            "xi-api-key": api_key or os.environ.get("ELEVEN_API_KEY"),
-        }
+    def request(url: str, method: str, api_key: Optional[str] = None, **kwargs):
+        headers = {"xi-api-key": api_key or os.environ.get("ELEVEN_API_KEY")}
 
         if method == "get":
-            response = requests.get(
-                url, headers=headers, json=data, files=files, stream=stream
-            )
+            response = requests.get(url, headers=headers, **kwargs)
         elif method == "post":
-            response = requests.post(
-                url, headers=headers, json=data, files=files, stream=stream
-            )
+            response = requests.post(url, headers=headers, **kwargs)
         else:
             raise ValueError(f"Invalid request method {method}")
 
-        try:
-            response.raise_for_status()
-            return response
-        except requests.exceptions.HTTPError:
-            if response.status_code == 401:
-                raise requests.exceptions.RequestException(
-                    "Your quota is exceeded or your API key is invalid, please set a"
-                    " valid key: ELEVEN_API_KEY"
-                )
+        # print(response.status_code, response.reason, response.text)
+
+        if response.status_code == 401:
+            raise SystemExit(
+                "Your quota is exceeded or your API key is invalid, please set a"
+                " valid key: ELEVEN_API_KEY"
+            )
+
+        response.raise_for_status()
+        return response
 
     @staticmethod
     def get(url: str, *args, **kwargs):
         return API.request(url, method="get", *args, **kwargs)  # type: ignore
 
     @staticmethod
     def post(url: str, *args, **kwargs):
```

### Comparing `elevenlabs-0.2.2/elevenlabs/api/history.py` & `elevenlabs-0.2.3/elevenlabs/api/history.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     character_count_change_to: int
     character_count_change: Optional[int]
     content_type: str
     settings: Optional[VoiceSettings]
     feedback: Optional[str]
 
     @root_validator
-    def computed(cls, values) -> int:
+    def computed(cls, values):
         # Compute character count field
         change_from = values["character_count_change_from"]
         change_to = values["character_count_change_to"]
         values["character_count_change"] = change_to - change_from
         # Compute datetime field
         values["date"] = datetime.utcfromtimestamp(values["date_unix"])
         return values
```

### Comparing `elevenlabs-0.2.2/elevenlabs/api/tts.py` & `elevenlabs-0.2.3/elevenlabs/api/tts.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 
 class TTS(API):
     @staticmethod
     def generate(text: str, voice: Voice) -> bytes:
         url = f"{api_base_url_v1}/text-to-speech/{voice.voice_id}"
         data = dict(text=text, voice_settings=voice.settings.dict())  # type: ignore
-        response = API.post(url, data=data)
+        response = API.post(url, json=data)
         return response.content
 
     @staticmethod
     def generate_stream(
         text: str, voice: Voice, stream_chunk_size: int = 2048
     ) -> Iterator[bytes]:
         url = f"{api_base_url_v1}/text-to-speech/{voice.voice_id}/stream"
         data = dict(text=text, voice_settings=voice.settings.dict())  # type: ignore
-        response = API.post(url, data=data, stream=True)
+        response = API.post(url, json=data, stream=True)
         for chunk in response.iter_content(chunk_size=stream_chunk_size):
             if chunk:
                 yield chunk
```

### Comparing `elevenlabs-0.2.2/elevenlabs/utils.py` & `elevenlabs-0.2.3/elevenlabs/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 import wave
 from collections.abc import Iterator
 from pathlib import Path
 
 from IPython.display import Audio, display
 
 
+def is_installed(lib_name: str) -> bool:
+    lib = shutil.which(lib_name)
+    if lib is None:
+        return False
+    global_path = Path(lib)
+    # else check if path is valid and has the correct access rights
+    return global_path.exists() and os.access(global_path, os.X_OK)
+
+
 def play(audio: bytes, notebook: bool = False) -> None:
     if notebook:
         display(Audio(audio, rate=44100, autoplay=True))
     else:
         if not is_installed("ffplay"):
             raise ValueError("ffplay from ffmpeg not found, necessary to play audio.")
         args = ["ffplay", "-autoexit", "-", "-nodisp"]
@@ -29,23 +38,14 @@
     with wave.open(filename, "w") as f:
         f.setnchannels(2)
         f.setsampwidth(2)
         f.setframerate(44100)
         f.writeframes(audio)
 
 
-def is_installed(lib_name: str) -> bool:
-    lib = shutil.which(lib_name)
-    if lib is None:
-        return False
-    global_path = Path(lib)
-    # else check if path is valid and has the correct access rights
-    return global_path.exists() and os.access(global_path, os.X_OK)
-
-
 def stream(audio_stream: Iterator[bytes]) -> None:
     if not is_installed("mpv"):
         raise ValueError("mpv not found, necessary to stream audio.")
 
     mpv_command = ["mpv", "--no-cache", "--no-terminal", "--", "fd://0"]
     mpv_process = subprocess.Popen(
         mpv_command,
```

### Comparing `elevenlabs-0.2.2/elevenlabs.egg-info/PKG-INFO` & `elevenlabs-0.2.3/elevenlabs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.2
+Version: 0.2.3
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.2/setup.py` & `elevenlabs-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elevenlabs",
     packages=find_packages(exclude=[]),
-    version="0.2.2",
+    version="0.2.3",
     description="The official elevenlabs python package.",
     long_description_content_type="text/markdown",
     author="Elevenlabs",
     url="https://github.com/elevenlabs/elevenlabs-python",
     keywords=["artificial intelligence", "deep learning"],
     install_requires=["pydantic>=1.10", "ipython>=8.0"],
     classifiers=[
```

