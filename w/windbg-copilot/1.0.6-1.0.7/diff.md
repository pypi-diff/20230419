# Comparing `tmp/windbg_copilot-1.0.6.tar.gz` & `tmp/windbg_copilot-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windbg_copilot-1.0.6.tar", last modified: Tue Apr 18 06:20:00 2023, max compression
+gzip compressed data, was "windbg_copilot-1.0.7.tar", last modified: Wed Apr 19 06:19:33 2023, max compression
```

## Comparing `windbg_copilot-1.0.6.tar` & `windbg_copilot-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 06:20:00.621506 windbg_copilot-1.0.6/
--rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2947 2023-04-18 06:20:00.622470 windbg_copilot-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2023-04-18 06:19:04.000000 windbg_copilot-1.0.6/README.md
--rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      918 2023-04-18 06:20:00.624421 windbg_copilot-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:20:00.582300 windbg_copilot-1.0.6/windbg_copilot/
--rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.6/windbg_copilot/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-18 06:19:11.000000 windbg_copilot-1.0.6/windbg_copilot/version.py
--rw-rw-rw-   0        0        0     6699 2023-04-18 06:15:43.000000 windbg_copilot-1.0.6/windbg_copilot/windbg_copilot.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:20:00.619424 windbg_copilot-1.0.6/windbg_copilot.egg-info/
--rw-rw-rw-   0        0        0     2947 2023-04-18 06:19:59.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-18 06:20:00.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 06:19:59.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-18 06:20:00.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 06:20:00.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 06:19:33.662331 windbg_copilot-1.0.7/
+-rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2947 2023-04-19 06:19:33.662331 windbg_copilot-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2023-04-18 06:19:04.000000 windbg_copilot-1.0.7/README.md
+-rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      918 2023-04-19 06:19:33.662331 windbg_copilot-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:19:33.633989 windbg_copilot-1.0.7/windbg_copilot/
+-rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.7/windbg_copilot/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-19 06:19:11.000000 windbg_copilot-1.0.7/windbg_copilot/version.py
+-rw-rw-rw-   0        0        0     7043 2023-04-19 06:18:42.000000 windbg_copilot-1.0.7/windbg_copilot/windbg_copilot.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:19:33.662331 windbg_copilot-1.0.7/windbg_copilot.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-04-19 06:19:32.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-19 06:19:33.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 06:19:32.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-19 06:19:33.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 06:19:33.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/top_level.txt
```

### Comparing `windbg_copilot-1.0.6/LICENSE.txt` & `windbg_copilot-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.6/PKG-INFO` & `windbg_copilot-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg_copilot
-Version: 1.0.6
+Version: 1.0.7
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
```

### Comparing `windbg_copilot-1.0.6/README.md` & `windbg_copilot-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.6/setup.cfg` & `windbg_copilot-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.6/windbg_copilot/windbg_copilot.py` & `windbg_copilot-1.0.7/windbg_copilot/windbg_copilot.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,112 +91,113 @@
             else:
                 temp = self.output
         with self.buffer_lock:
             temp = self.output
             self.output = ""
         return temp
 
-print("Hello engineer, I am Windows debugger copilot, I'm here to assist you.")
-speak("Hello engineer, I am Windows debugger copilot, I'm here to assist you.")
+def windbg_copilot():
+    print("Hello, I am Windows debugger copilot, I'm here to assist you.")
+    speak("Hello, I am Windows debugger copilot, I'm here to assist you.")
+
+    print("\nThis software is used for Windows debugging learning purpose, do NOT load any customer data, all input and output will be sent to OpenAI API.")
+    speak("This software is used for Windows debugging learning purpose, do NOT load any customer data, all input and output will be sent to OpenAI API.")
+
+    print("\nFirst, please enter the memory dump file path.")
+    speak("First, please enter the memory dump file path.")
+
+    filename = input("Memory dump file path:")
+
+    while not os.path.exists(filename):
+        print("\nFile does not exist")
+        speak("File does not exist")
+        filename = input("Memory dump file path:")
+        
+    command = r'C:\Program Files (x86)\Windows Kits\10\Debuggers\x64\cdb.exe'
+    arguments = [command]
+    arguments.extend(['-y', "srv*C:\symbols*https://msdl.microsoft.com/download/symbols"])  # Symbol path, may use sys.argv[1]
+    # arguments.extend(['-i', sys.argv[2]])  # Image path
+    arguments.extend(['-z', filename])  # Dump file
+    arguments.extend(['-c', ".echo LOADING DONE"])
+    process = subprocess.Popen(arguments, stdout=subprocess.PIPE, stdin=subprocess.PIPE, universal_newlines=True)
+    reader = ReaderThread(process.stdout)
+    reader.start()
 
-print("\nThis software is used for Windows debugging learning purpose, do NOT load any customer data, all input and output will be sent to OpenAI API.")
-speak("This software is used for Windows debugging learning purpose, do NOT load any customer data, all input and output will be sent to OpenAI API.")
-
-print("\nFirst, Where is the memory dump?")
-speak("First, Where is the memory dump?")
-
-filename = input("Memory dump file location:")
-
-while not os.path.exists(filename):
-    print("\nFile does not exist")
-    speak("File does not exist")
-    filename = input("Memory dump file location:")
-    
-command = r'C:\Program Files (x86)\Windows Kits\10\Debuggers\x64\cdb.exe'
-arguments = [command]
-arguments.extend(['-y', "srv*C:\debug\symbols*https://msdl.microsoft.com/download/symbols"])  # Symbol path, may use sys.argv[1]
-# arguments.extend(['-i', sys.argv[2]])  # Image path
-arguments.extend(['-z', filename])  # Dump file
-arguments.extend(['-c', ".echo LOADING DONE"])
-process = subprocess.Popen(arguments, stdout=subprocess.PIPE, stdin=subprocess.PIPE, universal_newlines=True)
-reader = ReaderThread(process.stdout)
-reader.start()
-
-result = ""
-while not re.search("LOADING DONE", result):
-    result = reader.getoutput()  # ignore initial output
-
-def dbg(command):
-    process.stdin.write(command+"\r\n")
-    process.stdin.flush()
     result = ""
-    while result == "":
-        result = reader.getoutput(timeout=2)
-    return result
-
-dump_type = ""
-
-result = dbg("||")
-print(result)
-speak(result)
-if "user mini" in result:
-    dump_type="User"
-    print("Yay, it's a User mode dump")
-    speak("Yay, it's a User mode dump")
-elif "kernel" in result:
-    dump_type="Kernel"
-    print("Yay, it's a Kernel mode dump")
-    speak("Yay, it's a Kernel mode dump")
-    
-# result = dbg("!analyze -v")
-# print(result)
-# chat(result,"explain")
-# chat(result,"suggest")
-
-conversation=""
-while True:
-    # Prompt the user for input
-    
-    speak("I am your Windows debugger copilot, please enter your input.")
-    user_input = input("\n"+'kd> ')
-    
-    speak("your input is "+user_input)
-    if user_input.startswith("!chat"):
-        text=chat(user_input,"chat")
-        speak(text)
-    elif user_input.startswith("!explain"):
-        # Print the output of cdb.exe
-        text=chat(conversation,"explain")
-        speak(text)
-    elif user_input.startswith("!suggest"):
-        # Print the output of cdb.exe
-        text=chat(conversation,"suggest")
-        speak(text)
-    elif user_input.startswith("!ask"):
-        # Print the output of cdb.exe
-        question = conversation + "\n" + user_input[4:]
-        text=chat(question,"ask")
-        speak(text)
-    elif user_input.startswith("!q"):
-        # Print the output of cdb.exe
-        text=chat("Goodbye Windows debugger copilot, please quit","chat")
-        speak(text)
-        dbg("q")
-        break
-    elif user_input.startswith("!help"):
-        help_msg = '''
-        !chat <you may ask anything related to debugging>
-        !ask <ask any question for the above output>
-        !explain: explain the last output
-        !suggest: suggest how to do next
-        !q: quit
-        '''
-        print(help_msg)
-        speak(help_msg)
-    else:
-        # Send the user input to cdb.exe
-        result = dbg(user_input)
-        conversation += "\n"+result
-        print("\n"+result)
+    while not re.search("LOADING DONE", result):
+        result = reader.getoutput()  # ignore initial output
+
+    def dbg(command):
+        process.stdin.write(command+"\r\n")
+        process.stdin.flush()
+        result = ""
+        while result == "":
+            result = reader.getoutput(0.2)
+        return result
+
+    # dump_type = ""
+
+    result = dbg("||")
+    print(result)
+    # speak(result)
+    if "user mini" in result:
+        # dump_type="User"
+        print("Yay, it's a User mode dump")
+        # speak("Yay, it's a User mode dump")
+    elif "kernel" in result:
+        # dump_type="Kernel"
+        print("Yay, it's a Kernel mode dump")
+        # speak("Yay, it's a Kernel mode dump")
+        
+    # result = dbg("!analyze -v")
+    # print(result)
+    # chat(result,"explain")
+    # chat(result,"suggest")
+
+    conversation=""
+    while True:
+        # Prompt the user for input
+        
+        speak("Please enter your input.")
+        user_input = input("\n"+'kd> ')
+        
+        speak(user_input)
+        if user_input.startswith("!chat"):
+            text=chat(user_input,"chat")
+            speak(text)
+        elif user_input.startswith("!explain"):
+            # Print the output of cdb.exe
+            text=chat(conversation,"explain")
+            speak(text)
+        elif user_input.startswith("!suggest"):
+            # Print the output of cdb.exe
+            text=chat(conversation,"suggest")
+            speak(text)
+        elif user_input.startswith("!ask"):
+            # Print the output of cdb.exe
+            question = conversation + "\n" + user_input[4:]
+            text=chat(question,"ask")
+            speak(text)
+        elif user_input.startswith("!q"):
+            # Print the output of cdb.exe
+            text=chat("Goodbye Windows debugger copilot, please quit","chat")
+            speak(text)
+            dbg("q")
+            break
+        elif user_input.startswith("!help"):
+            help_msg = '''
+            !chat <you may ask anything related to debugging>
+            !ask <ask any question for the above output>
+            !explain: explain the last output
+            !suggest: suggest how to do next
+            !q: quit
+            '''
+            print(help_msg)
+            speak(help_msg)
+        else:
+            # Send the user input to cdb.exe
+            result = dbg(user_input)
+            conversation += "\n"+result
+            print("\n"+result)
```

### Comparing `windbg_copilot-1.0.6/windbg_copilot.egg-info/PKG-INFO` & `windbg_copilot-1.0.7/windbg_copilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg-copilot
-Version: 1.0.6
+Version: 1.0.7
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
```

