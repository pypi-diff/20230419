# Comparing `tmp/buge-0.0.4.tar.gz` & `tmp/buge-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buge-0.0.4.tar", last modified: Wed Apr 19 01:19:38 2023, max compression
+gzip compressed data, was "buge-0.0.5.tar", last modified: Wed Apr 19 20:01:48 2023, max compression
```

## Comparing `buge-0.0.4.tar` & `buge-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 01:19:38.121640 buge-0.0.4/
--rw-r--r--   0 damonpickett   (501) staff       (20)     1073 2023-04-14 22:43:18.000000 buge-0.0.4/LICENSE
--rw-r--r--   0 damonpickett   (501) staff       (20)       25 2023-04-14 22:43:29.000000 buge-0.0.4/MANIFEST.in
--rw-r--r--   0 damonpickett   (501) staff       (20)     3863 2023-04-19 01:19:38.121690 buge-0.0.4/PKG-INFO
--rw-r--r--   0 damonpickett   (501) staff       (20)     3224 2023-04-19 01:18:42.000000 buge-0.0.4/README.md
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 01:19:38.120695 buge-0.0.4/buge/
--rw-r--r--   0 damonpickett   (501) staff       (20)     2988 2023-04-19 01:18:42.000000 buge-0.0.4/buge/main.py
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 01:19:38.121510 buge-0.0.4/buge.egg-info/
--rw-r--r--   0 damonpickett   (501) staff       (20)     3863 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/PKG-INFO
--rw-r--r--   0 damonpickett   (501) staff       (20)      246 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/SOURCES.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)        1 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/dependency_links.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)       40 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/entry_points.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)       26 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/requires.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)        5 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/top_level.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)      644 2023-04-19 01:19:09.000000 buge-0.0.4/pyproject.toml
--rw-r--r--   0 damonpickett   (501) staff       (20)      784 2023-04-19 01:19:38.121931 buge-0.0.4/setup.cfg
--rw-r--r--   0 damonpickett   (501) staff       (20)       37 2023-04-13 22:46:26.000000 buge-0.0.4/setup.py
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 20:01:48.004632 buge-0.0.5/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     1073 2023-04-14 22:43:18.000000 buge-0.0.5/LICENSE
+-rw-r--r--   0 damonpickett   (501) staff       (20)       25 2023-04-14 22:43:29.000000 buge-0.0.5/MANIFEST.in
+-rw-r--r--   0 damonpickett   (501) staff       (20)     5346 2023-04-19 20:01:48.004694 buge-0.0.5/PKG-INFO
+-rw-r--r--   0 damonpickett   (501) staff       (20)     4707 2023-04-19 20:01:30.000000 buge-0.0.5/README.md
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 20:01:48.003736 buge-0.0.5/buge/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     2734 2023-04-19 20:01:30.000000 buge-0.0.5/buge/main.py
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 20:01:48.004534 buge-0.0.5/buge.egg-info/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     5346 2023-04-19 20:01:47.000000 buge-0.0.5/buge.egg-info/PKG-INFO
+-rw-r--r--   0 damonpickett   (501) staff       (20)      246 2023-04-19 20:01:48.000000 buge-0.0.5/buge.egg-info/SOURCES.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)        1 2023-04-19 20:01:47.000000 buge-0.0.5/buge.egg-info/dependency_links.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)       40 2023-04-19 20:01:48.000000 buge-0.0.5/buge.egg-info/entry_points.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)       26 2023-04-19 20:01:48.000000 buge-0.0.5/buge.egg-info/requires.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)        5 2023-04-19 20:01:48.000000 buge-0.0.5/buge.egg-info/top_level.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)      644 2023-04-19 20:01:30.000000 buge-0.0.5/pyproject.toml
+-rw-r--r--   0 damonpickett   (501) staff       (20)      784 2023-04-19 20:01:48.004934 buge-0.0.5/setup.cfg
+-rw-r--r--   0 damonpickett   (501) staff       (20)       37 2023-04-13 22:46:26.000000 buge-0.0.5/setup.py
```

### Comparing `buge-0.0.4/LICENSE` & `buge-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `buge-0.0.4/PKG-INFO` & `buge-0.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buge
-Version: 0.0.4
+Version: 0.0.5
 Summary: buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 Home-page: https://github.com/damonpickett/buge
 Author: Damon Pickett
 Author-email: Damon Pickett <damon.pickett@gmail.com>
 Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3
@@ -15,25 +15,35 @@
 License-File: LICENSE
 
 # buge
 *Think BUG-E, except I pronounce it 'booj'*
 
 ## Table of Contents
 
-- [Project Title](#macta)
 - [Description](#description)
-- [Tech Stack](#tech-stack)
-- [Installation](#installation)
-- [Usage](#usage)
+- [Instructions](#instructions)
+- [Dependencies](#dependencies)
+- [How buge Works](#how-buge-works)
 - [Contributing](#contributing)
 - [License](#license)
+- [Disclaimer](#disclaimer)
 
 ## Description
 
-BUGE is a command-line application that helps developers understand and troubleshoot common error messages by generating explanations and solutions using the OpenAI GPT-3 language model.
+buge is a command-line application that helps developers understand and troubleshoot common error messages by generating explanations and solutions using the OpenAI GPT-3 language model. Here's buge in action:
+
+![BUGE Demo](./assets/buge-demo-gif-2.gif)
+
+## Instructions
+
+1. Install buge by entering `pip3 install buge` in your terminal.
+2. Call buge from anywhere in your terminal by entering `buge`.
+3. If it's your first time calling buge, you will be prompted for you OpenAI API key. You'll only need to do this once.
+4. You'll then be prompted for your error code. Paste you error code into your terminal and hit 'enter'.
+5. buge makes an API call and then returns the the meaning of the error code, possible causes, and possible solutions.
 
 This program is free to use. However, if you would like to <a href="https://www.buymeacoffee.com/damonpickett" target="_blank">buy me a coffee</a>, you can do so here:
 
 <p align="center">
   <a href="https://www.buymeacoffee.com/damonpickett" target="_blank">
     <img src="./assets/bmc-button300x84.png" alt="Buy me a cofee button">
   </a>
@@ -41,23 +51,25 @@
 
 ## Dependencies
 
 - [OpenAI](https://pypi.org/project/openai/): A cloud-based platform that allows users to build various artificial intelligence models, including natural language processing models that can generate text.
 - [python-dotenv](https://pypi.org/project/python-dotenv/): Python-dotenv reads key-value pairs from a .env file and can set them as environment variables. It helps in the development of applications following the [12-factor](https://12factor.net/) principles.
 - [rich package](https://pypi.org/project/rich): Rich is a Python library for rich text and beautiful formatting in the terminal.
 
-## Installation
+## How buge Works
 
-## Usage
+1. Upon running the program, buge first checks your OpenAI API key in your `.env` file. If this file does not exist, buge prompts the user for their key, creates the file, and writes the key to the file. The .env file is then saved in the package folder.
+2. buge then prompts the user for their error code.
+3. buge takes the user's error code and passes it to the `get_error_explanation()` function as a parameter. This function makes three API calls based on the user's error code. It asks `text-davinci-003` for the meaning of the error code, possible causes for the error code, and possible solutions. It then prints the results to the user's console. I chose to use three seperate API calls as opposed to asking for everything at once to ensure that everything being asked for would be given its proper due by GPT-3. Bunching everything together in one prompt would have caused mixed results for users.
 
 ## Contributing
 
 Contributions to BUGE are welcome! If you encounter any issues, have suggestions for improvements, or want to add new features, feel free to submit a pull request or open an issue in the GitHub repository.
 
-## Licence
+## License
 
 Copyright (c) 2018 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

#### html2text {}

```diff
@@ -1,39 +1,58 @@
-Metadata-Version: 2.1 Name: buge Version: 0.0.4 Summary: buge is a command-line
+Metadata-Version: 2.1 Name: buge Version: 0.0.5 Summary: buge is a command-line
 application that uses the OpenAI API to diagnose bugs when programming. Home-
 page: https://github.com/damonpickett/buge Author: Damon Pickett Author-email:
 Damon Pickett
 pickett@gmail.com> Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # buge *Think BUG-E, except I pronounce it 'booj'* ## Table of Contents
-- [Project Title](#macta) - [Description](#description) - [Tech Stack](#tech-
-stack) - [Installation](#installation) - [Usage](#usage) - [Contributing]
-(#contributing) - [License](#license) ## Description BUGE is a command-line
-application that helps developers understand and troubleshoot common error
-messages by generating explanations and solutions using the OpenAI GPT-
-3 language model. This program is free to use. However, if you would like to
-buy_me_a_coffee, you can do so here:
+- [Description](#description) - [Instructions](#instructions) - [Dependencies]
+(#dependencies) - [How buge Works](#how-buge-works) - [Contributing]
+(#contributing) - [License](#license) - [Disclaimer](#disclaimer) ##
+Description buge is a command-line application that helps developers understand
+and troubleshoot common error messages by generating explanations and solutions
+using the OpenAI GPT-3 language model. Here's buge in action: ![BUGE Demo](./
+assets/buge-demo-gif-2.gif) ## Instructions 1. Install buge by entering `pip3
+install buge` in your terminal. 2. Call buge from anywhere in your terminal by
+entering `buge`. 3. If it's your first time calling buge, you will be prompted
+for you OpenAI API key. You'll only need to do this once. 4. You'll then be
+prompted for your error code. Paste you error code into your terminal and hit
+'enter'. 5. buge makes an API call and then returns the the meaning of the
+error code, possible causes, and possible solutions. This program is free to
+use. However, if you would like to buy_me_a_coffee, you can do so here:
                             [Buy_me_a_cofee_button]
 ## Dependencies - [OpenAI](https://pypi.org/project/openai/): A cloud-based
 platform that allows users to build various artificial intelligence models,
 including natural language processing models that can generate text. - [python-
 dotenv](https://pypi.org/project/python-dotenv/): Python-dotenv reads key-value
 pairs from a .env file and can set them as environment variables. It helps in
 the development of applications following the [12-factor](https://12factor.net/
 ) principles. - [rich package](https://pypi.org/project/rich): Rich is a Python
-library for rich text and beautiful formatting in the terminal. ## Installation
-## Usage ## Contributing Contributions to BUGE are welcome! If you encounter
-any issues, have suggestions for improvements, or want to add new features,
-feel free to submit a pull request or open an issue in the GitHub repository.
-## Licence Copyright (c) 2018 The Python Packaging Authority Permission is
-hereby granted, free of charge, to any person obtaining a copy of this software
-and associated documentation files (the "Software"), to deal in the Software
+library for rich text and beautiful formatting in the terminal. ## How buge
+Works 1. Upon running the program, buge first checks your OpenAI API key in
+your `.env` file. If this file does not exist, buge prompts the user for their
+key, creates the file, and writes the key to the file. The .env file is then
+saved in the package folder. 2. buge then prompts the user for their error
+code. 3. buge takes the user's error code and passes it to the
+`get_error_explanation()` function as a parameter. This function makes three
+API calls based on the user's error code. It asks `text-davinci-003` for the
+meaning of the error code, possible causes for the error code, and possible
+solutions. It then prints the results to the user's console. I chose to use
+three seperate API calls as opposed to asking for everything at once to ensure
+that everything being asked for would be given its proper due by GPT-3.
+Bunching everything together in one prompt would have caused mixed results for
+users. ## Contributing Contributions to BUGE are welcome! If you encounter any
+issues, have suggestions for improvements, or want to add new features, feel
+free to submit a pull request or open an issue in the GitHub repository. ##
+License Copyright (c) 2018 The Python Packaging Authority Permission is hereby
+granted, free of charge, to any person obtaining a copy of this software and
+associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
```

### Comparing `buge-0.0.4/buge/main.py` & `buge-0.0.5/buge/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,22 +23,14 @@
 
     openai.api_key = os.getenv("OPENAI_API_KEY")
 
     error_message = input("Please paste your error code here: ")
 
     console = Console()
 
-    if sys.version_info < (3, 7):
-        console.print("[bold red]Error:[/bold red] BUGE requires Python 3.7 or higher to run.")
-        console.print("Please update to a newer version of Python.\n")
-        console.print("[bold]Suggestions:[/bold]")
-        console.print("- Install the latest version of Python 3 from the official Python website (https://www.python.org/downloads/).")
-        console.print("- Use a Python version manager like pyenv to easily switch between multiple versions of Python.\n")
-        sys.exit(1)
-
     def get_error_explanation(error_message):
         base_prompt = (f"Explain the following error code in simple terms: `{error_message}`")
         base_response = openai.Completion.create(
             engine="text-davinci-003",
             prompt=base_prompt,
             max_tokens=1024,
             n=1,
@@ -67,24 +59,26 @@
             max_tokens=1024,
             n=1,
             stop=None,
             temperature=0.7,
         )
         third_response_text = third_response.choices[0].text.strip()
 
-        print('----------')
         print("")
-        print("Meaning:")
-        print(base_response_text)
+        console.print('[bold]--------------------[/bold]')
+        print("")
+        console.print("[bold cyan]Meaning:[/bold cyan]")
+        console.print(f"[green]`{base_response_text}`[green]")
+        print("")
+        console.print("[bold cyan]Possible Causes:[/bold cyan]")
+        console.print(f"[green]`{secondary_response_text}`[green]")
         print("")
-        print("Possible Causes:")
-        print(secondary_response_text)
+        console.print("[bold cyan]Possible Solutions:[/bold cyan]")
+        console.print(f"[green]`{third_response_text}`[green]")
         print("")
-        print("Possible Solutions:")
-        print(third_response_text)
+        console.print('[bold]--------------------[/bold]')
         print("")
-        print('----------')
 
     get_error_explanation(error_message)
 
 if __name__ == '__main__':
     main()
```

### Comparing `buge-0.0.4/buge.egg-info/PKG-INFO` & `buge-0.0.5/buge.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buge
-Version: 0.0.4
+Version: 0.0.5
 Summary: buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 Home-page: https://github.com/damonpickett/buge
 Author: Damon Pickett
 Author-email: Damon Pickett <damon.pickett@gmail.com>
 Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3
@@ -15,25 +15,35 @@
 License-File: LICENSE
 
 # buge
 *Think BUG-E, except I pronounce it 'booj'*
 
 ## Table of Contents
 
-- [Project Title](#macta)
 - [Description](#description)
-- [Tech Stack](#tech-stack)
-- [Installation](#installation)
-- [Usage](#usage)
+- [Instructions](#instructions)
+- [Dependencies](#dependencies)
+- [How buge Works](#how-buge-works)
 - [Contributing](#contributing)
 - [License](#license)
+- [Disclaimer](#disclaimer)
 
 ## Description
 
-BUGE is a command-line application that helps developers understand and troubleshoot common error messages by generating explanations and solutions using the OpenAI GPT-3 language model.
+buge is a command-line application that helps developers understand and troubleshoot common error messages by generating explanations and solutions using the OpenAI GPT-3 language model. Here's buge in action:
+
+![BUGE Demo](./assets/buge-demo-gif-2.gif)
+
+## Instructions
+
+1. Install buge by entering `pip3 install buge` in your terminal.
+2. Call buge from anywhere in your terminal by entering `buge`.
+3. If it's your first time calling buge, you will be prompted for you OpenAI API key. You'll only need to do this once.
+4. You'll then be prompted for your error code. Paste you error code into your terminal and hit 'enter'.
+5. buge makes an API call and then returns the the meaning of the error code, possible causes, and possible solutions.
 
 This program is free to use. However, if you would like to <a href="https://www.buymeacoffee.com/damonpickett" target="_blank">buy me a coffee</a>, you can do so here:
 
 <p align="center">
   <a href="https://www.buymeacoffee.com/damonpickett" target="_blank">
     <img src="./assets/bmc-button300x84.png" alt="Buy me a cofee button">
   </a>
@@ -41,23 +51,25 @@
 
 ## Dependencies
 
 - [OpenAI](https://pypi.org/project/openai/): A cloud-based platform that allows users to build various artificial intelligence models, including natural language processing models that can generate text.
 - [python-dotenv](https://pypi.org/project/python-dotenv/): Python-dotenv reads key-value pairs from a .env file and can set them as environment variables. It helps in the development of applications following the [12-factor](https://12factor.net/) principles.
 - [rich package](https://pypi.org/project/rich): Rich is a Python library for rich text and beautiful formatting in the terminal.
 
-## Installation
+## How buge Works
 
-## Usage
+1. Upon running the program, buge first checks your OpenAI API key in your `.env` file. If this file does not exist, buge prompts the user for their key, creates the file, and writes the key to the file. The .env file is then saved in the package folder.
+2. buge then prompts the user for their error code.
+3. buge takes the user's error code and passes it to the `get_error_explanation()` function as a parameter. This function makes three API calls based on the user's error code. It asks `text-davinci-003` for the meaning of the error code, possible causes for the error code, and possible solutions. It then prints the results to the user's console. I chose to use three seperate API calls as opposed to asking for everything at once to ensure that everything being asked for would be given its proper due by GPT-3. Bunching everything together in one prompt would have caused mixed results for users.
 
 ## Contributing
 
 Contributions to BUGE are welcome! If you encounter any issues, have suggestions for improvements, or want to add new features, feel free to submit a pull request or open an issue in the GitHub repository.
 
-## Licence
+## License
 
 Copyright (c) 2018 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

#### html2text {}

```diff
@@ -1,39 +1,58 @@
-Metadata-Version: 2.1 Name: buge Version: 0.0.4 Summary: buge is a command-line
+Metadata-Version: 2.1 Name: buge Version: 0.0.5 Summary: buge is a command-line
 application that uses the OpenAI API to diagnose bugs when programming. Home-
 page: https://github.com/damonpickett/buge Author: Damon Pickett Author-email:
 Damon Pickett
 pickett@gmail.com> Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # buge *Think BUG-E, except I pronounce it 'booj'* ## Table of Contents
-- [Project Title](#macta) - [Description](#description) - [Tech Stack](#tech-
-stack) - [Installation](#installation) - [Usage](#usage) - [Contributing]
-(#contributing) - [License](#license) ## Description BUGE is a command-line
-application that helps developers understand and troubleshoot common error
-messages by generating explanations and solutions using the OpenAI GPT-
-3 language model. This program is free to use. However, if you would like to
-buy_me_a_coffee, you can do so here:
+- [Description](#description) - [Instructions](#instructions) - [Dependencies]
+(#dependencies) - [How buge Works](#how-buge-works) - [Contributing]
+(#contributing) - [License](#license) - [Disclaimer](#disclaimer) ##
+Description buge is a command-line application that helps developers understand
+and troubleshoot common error messages by generating explanations and solutions
+using the OpenAI GPT-3 language model. Here's buge in action: ![BUGE Demo](./
+assets/buge-demo-gif-2.gif) ## Instructions 1. Install buge by entering `pip3
+install buge` in your terminal. 2. Call buge from anywhere in your terminal by
+entering `buge`. 3. If it's your first time calling buge, you will be prompted
+for you OpenAI API key. You'll only need to do this once. 4. You'll then be
+prompted for your error code. Paste you error code into your terminal and hit
+'enter'. 5. buge makes an API call and then returns the the meaning of the
+error code, possible causes, and possible solutions. This program is free to
+use. However, if you would like to buy_me_a_coffee, you can do so here:
                             [Buy_me_a_cofee_button]
 ## Dependencies - [OpenAI](https://pypi.org/project/openai/): A cloud-based
 platform that allows users to build various artificial intelligence models,
 including natural language processing models that can generate text. - [python-
 dotenv](https://pypi.org/project/python-dotenv/): Python-dotenv reads key-value
 pairs from a .env file and can set them as environment variables. It helps in
 the development of applications following the [12-factor](https://12factor.net/
 ) principles. - [rich package](https://pypi.org/project/rich): Rich is a Python
-library for rich text and beautiful formatting in the terminal. ## Installation
-## Usage ## Contributing Contributions to BUGE are welcome! If you encounter
-any issues, have suggestions for improvements, or want to add new features,
-feel free to submit a pull request or open an issue in the GitHub repository.
-## Licence Copyright (c) 2018 The Python Packaging Authority Permission is
-hereby granted, free of charge, to any person obtaining a copy of this software
-and associated documentation files (the "Software"), to deal in the Software
+library for rich text and beautiful formatting in the terminal. ## How buge
+Works 1. Upon running the program, buge first checks your OpenAI API key in
+your `.env` file. If this file does not exist, buge prompts the user for their
+key, creates the file, and writes the key to the file. The .env file is then
+saved in the package folder. 2. buge then prompts the user for their error
+code. 3. buge takes the user's error code and passes it to the
+`get_error_explanation()` function as a parameter. This function makes three
+API calls based on the user's error code. It asks `text-davinci-003` for the
+meaning of the error code, possible causes for the error code, and possible
+solutions. It then prints the results to the user's console. I chose to use
+three seperate API calls as opposed to asking for everything at once to ensure
+that everything being asked for would be given its proper due by GPT-3.
+Bunching everything together in one prompt would have caused mixed results for
+users. ## Contributing Contributions to BUGE are welcome! If you encounter any
+issues, have suggestions for improvements, or want to add new features, feel
+free to submit a pull request or open an issue in the GitHub repository. ##
+License Copyright (c) 2018 The Python Packaging Authority Permission is hereby
+granted, free of charge, to any person obtaining a copy of this software and
+associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
```

### Comparing `buge-0.0.4/pyproject.toml` & `buge-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "buge"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Damon Pickett", email="damon.pickett@gmail.com" },
 ]
 description = "buge is a command-line application that uses the OpenAI API to diagnose bugs when programming."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `buge-0.0.4/setup.cfg` & `buge-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = buge
-version = 0.0.4
+version = 0.0.5
 author = Damon Pickett
 author_email = damon.pickett@gmail.com
 description = buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/damonpickett/buge
 classifiers =
```

