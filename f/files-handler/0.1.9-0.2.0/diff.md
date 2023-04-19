# Comparing `tmp/files-handler-0.1.9.tar.gz` & `tmp/files-handler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "files-handler-0.1.9.tar", last modified: Wed Apr 19 17:29:59 2023, max compression
+gzip compressed data, was "files-handler-0.2.0.tar", last modified: Wed Apr 19 17:47:30 2023, max compression
```

## Comparing `files-handler-0.1.9.tar` & `files-handler-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 17:29:59.160026 files-handler-0.1.9/
--rw-rw-rw-   0        0        0     3712 2023-04-19 17:29:59.158028 files-handler-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2919 2023-02-24 14:24:34.000000 files-handler-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 17:29:59.087229 files-handler-0.1.9/files_handler/
--rw-rw-rw-   0        0        0      106 2023-02-24 14:24:15.000000 files-handler-0.1.9/files_handler/__init__.py
--rw-rw-rw-   0        0        0     1454 2023-03-17 14:33:39.000000 files-handler-0.1.9/files_handler/folders_handler.py
--rw-rw-rw-   0        0        0     5337 2023-04-19 17:29:03.000000 files-handler-0.1.9/files_handler/s3_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:29:59.153028 files-handler-0.1.9/files_handler.egg-info/
--rw-rw-rw-   0        0        0     3712 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 17:29:59.160545 files-handler-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-04-19 17:29:43.000000 files-handler-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:47:30.573364 files-handler-0.2.0/
+-rw-rw-rw-   0        0        0     3343 2023-04-19 17:47:30.569367 files-handler-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2558 2023-04-19 17:34:33.000000 files-handler-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 17:47:30.513810 files-handler-0.2.0/files_handler/
+-rw-rw-rw-   0        0        0      106 2023-02-24 14:24:15.000000 files-handler-0.2.0/files_handler/__init__.py
+-rw-rw-rw-   0        0        0     1454 2023-03-17 14:33:39.000000 files-handler-0.2.0/files_handler/folders_handler.py
+-rw-rw-rw-   0        0        0     5315 2023-04-19 17:45:42.000000 files-handler-0.2.0/files_handler/s3_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:47:30.566367 files-handler-0.2.0/files_handler.egg-info/
+-rw-rw-rw-   0        0        0     3343 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 17:47:30.574365 files-handler-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-04-19 17:47:20.000000 files-handler-0.2.0/setup.py
```

### Comparing `files-handler-0.1.9/PKG-INFO` & `files-handler-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: files-handler
-Version: 0.1.9
+Version: 0.2.0
 Summary: Files Handler Library
 Home-page: 
 Author: Bhryan Henderson
 Author-email: bhryan.perpetuo@concert.com.br
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,22 +18,14 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ## Instalação da biblioteca
 
 - Para instalar a biblioteca basta chamar no console "pip install files-handler"
 
-## Variáveis de ambiente
-
-- Para o correto funcionamento da biblioteca é preciso ter configurado na aplicação que irá chamar a biblioteca três variáveis de ambiente, sendo elas:
-
-  AWS_ACCESS_KEY_ID = Access key do usuário na AWS
-  AWS_SECRET_ACCESS_KEY = Secret Access key do usuário na AWS
-  AWS_REGION_NAME' = Região que está o bucket S3
-
 ## Inicialização da biblioteca
 
 - Para iniciar a biblioteca, basta importar as duas classes, ou apenas a de interesse com o "from files_handler import s3_handler, folders_handler"
 - O próximo passo é instanciar a classe respectiva:
 
   s3_handler_class = s3_handler(bucket, path_ref)
   Para essa classe é preciso passar no construtor, o bucket do S3 e também um diretorio de referência local para obter e salvar os arquivos
```

### Comparing `files-handler-0.1.9/README.md` & `files-handler-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 ## Instalação da biblioteca
 
 - Para instalar a biblioteca basta chamar no console "pip install files-handler"
 
-## Variáveis de ambiente
-
-- Para o correto funcionamento da biblioteca é preciso ter configurado na aplicação que irá chamar a biblioteca três variáveis de ambiente, sendo elas:
-
-  AWS_ACCESS_KEY_ID = Access key do usuário na AWS
-  AWS_SECRET_ACCESS_KEY = Secret Access key do usuário na AWS
-  AWS_REGION_NAME' = Região que está o bucket S3
-
 ## Inicialização da biblioteca
 
 - Para iniciar a biblioteca, basta importar as duas classes, ou apenas a de interesse com o "from files_handler import s3_handler, folders_handler"
 - O próximo passo é instanciar a classe respectiva:
 
   s3_handler_class = s3_handler(bucket, path_ref)
   Para essa classe é preciso passar no construtor, o bucket do S3 e também um diretorio de referência local para obter e salvar os arquivos
```

### Comparing `files-handler-0.1.9/files_handler/folders_handler.py` & `files-handler-0.2.0/files_handler/folders_handler.py`

 * *Files identical despite different names*

### Comparing `files-handler-0.1.9/files_handler/s3_handler.py` & `files-handler-0.2.0/files_handler/s3_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     :param bucket: The Bucket.
     :type bucket: string
     :param path_ref: Reference Path to manage the files and folders.
     :type path_ref: string
     """
 
     def __init__(self, bucket, path_ref, input_path='input', result_path='output'):
-        self.session = boto3.Session(profile_name='default')
+        self.session = boto3.Session()
         self.bucket = bucket
         self.path_ref = path_ref
         self.path_to_predict_images = os.path.join(path_ref, input_path)
         self.s3_client = boto3.client('s3')
         self.folders_handler = folders_handler('')
 
     # Get image from s3 bucket
```

### Comparing `files-handler-0.1.9/files_handler.egg-info/PKG-INFO` & `files-handler-0.2.0/files_handler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: files-handler
-Version: 0.1.9
+Version: 0.2.0
 Summary: Files Handler Library
 Home-page: 
 Author: Bhryan Henderson
 Author-email: bhryan.perpetuo@concert.com.br
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,22 +18,14 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ## Instalação da biblioteca
 
 - Para instalar a biblioteca basta chamar no console "pip install files-handler"
 
-## Variáveis de ambiente
-
-- Para o correto funcionamento da biblioteca é preciso ter configurado na aplicação que irá chamar a biblioteca três variáveis de ambiente, sendo elas:
-
-  AWS_ACCESS_KEY_ID = Access key do usuário na AWS
-  AWS_SECRET_ACCESS_KEY = Secret Access key do usuário na AWS
-  AWS_REGION_NAME' = Região que está o bucket S3
-
 ## Inicialização da biblioteca
 
 - Para iniciar a biblioteca, basta importar as duas classes, ou apenas a de interesse com o "from files_handler import s3_handler, folders_handler"
 - O próximo passo é instanciar a classe respectiva:
 
   s3_handler_class = s3_handler(bucket, path_ref)
   Para essa classe é preciso passar no construtor, o bucket do S3 e também um diretorio de referência local para obter e salvar os arquivos
```

### Comparing `files-handler-0.1.9/setup.py` & `files-handler-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="files-handler",
-    version="0.1.9",
+    version="0.2.0",
     description="Files Handler Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Bhryan Henderson",
     author_email="bhryan.perpetuo@concert.com.br",
     license="MIT",
```

