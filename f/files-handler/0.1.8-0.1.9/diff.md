# Comparing `tmp/files-handler-0.1.8.tar.gz` & `tmp/files-handler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "files-handler-0.1.8.tar", last modified: Fri Mar 17 14:34:14 2023, max compression
+gzip compressed data, was "files-handler-0.1.9.tar", last modified: Wed Apr 19 17:29:59 2023, max compression
```

## Comparing `files-handler-0.1.8.tar` & `files-handler-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 14:34:14.044716 files-handler-0.1.8/
--rw-rw-rw-   0        0        0     3712 2023-03-17 14:34:14.043710 files-handler-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2919 2023-02-24 14:24:34.000000 files-handler-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-17 14:34:14.012179 files-handler-0.1.8/files_handler/
--rw-rw-rw-   0        0        0      106 2023-02-24 14:24:15.000000 files-handler-0.1.8/files_handler/__init__.py
--rw-rw-rw-   0        0        0     1454 2023-03-17 14:33:39.000000 files-handler-0.1.8/files_handler/folders_handler.py
--rw-rw-rw-   0        0        0     5801 2023-03-17 14:33:39.000000 files-handler-0.1.8/files_handler/s3_handler.py
-drwxrwxrwx   0        0        0        0 2023-03-17 14:34:14.041710 files-handler-0.1.8/files_handler.egg-info/
--rw-rw-rw-   0        0        0     3712 2023-03-17 14:34:13.000000 files-handler-0.1.8/files_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-03-17 14:34:13.000000 files-handler-0.1.8/files_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 14:34:13.000000 files-handler-0.1.8/files_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-17 14:34:13.000000 files-handler-0.1.8/files_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-17 14:34:13.000000 files-handler-0.1.8/files_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 14:34:14.044716 files-handler-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-03-17 14:33:57.000000 files-handler-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:29:59.160026 files-handler-0.1.9/
+-rw-rw-rw-   0        0        0     3712 2023-04-19 17:29:59.158028 files-handler-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2919 2023-02-24 14:24:34.000000 files-handler-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 17:29:59.087229 files-handler-0.1.9/files_handler/
+-rw-rw-rw-   0        0        0      106 2023-02-24 14:24:15.000000 files-handler-0.1.9/files_handler/__init__.py
+-rw-rw-rw-   0        0        0     1454 2023-03-17 14:33:39.000000 files-handler-0.1.9/files_handler/folders_handler.py
+-rw-rw-rw-   0        0        0     5337 2023-04-19 17:29:03.000000 files-handler-0.1.9/files_handler/s3_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:29:59.153028 files-handler-0.1.9/files_handler.egg-info/
+-rw-rw-rw-   0        0        0     3712 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 17:29:58.000000 files-handler-0.1.9/files_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 17:29:59.160545 files-handler-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-04-19 17:29:43.000000 files-handler-0.1.9/setup.py
```

### Comparing `files-handler-0.1.8/PKG-INFO` & `files-handler-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: files-handler
-Version: 0.1.8
+Version: 0.1.9
 Summary: Files Handler Library
 Home-page: 
 Author: Bhryan Henderson
 Author-email: bhryan.perpetuo@concert.com.br
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `files-handler-0.1.8/README.md` & `files-handler-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `files-handler-0.1.8/files_handler/folders_handler.py` & `files-handler-0.1.9/files_handler/folders_handler.py`

 * *Files identical despite different names*

### Comparing `files-handler-0.1.8/files_handler/s3_handler.py` & `files-handler-0.1.9/files_handler/s3_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,15 @@
     :param bucket: The Bucket.
     :type bucket: string
     :param path_ref: Reference Path to manage the files and folders.
     :type path_ref: string
     """
 
     def __init__(self, bucket, path_ref, input_path='input', result_path='output'):
-        self.access_key_id = os.environ.get('AWS_ACCESS_KEY_ID')
-        self.secret_access_key = os.environ.get('AWS_SECRET_ACCESS_KEY')
-        self.region_name = os.environ.get('AWS_REGION_NAME')
+        self.session = boto3.Session(profile_name='default')
         self.bucket = bucket
         self.path_ref = path_ref
         self.path_to_predict_images = os.path.join(path_ref, input_path)
         self.s3_client = boto3.client('s3')
         self.folders_handler = folders_handler('')
 
     # Get image from s3 bucket 
@@ -49,15 +47,15 @@
 
             self.folders_handler.verify_and_create_folder(download_path, 'Creating input directory...')
 
             image_name = os.path.basename(s3_image_path)
             local_image_path = os.path.join(download_path, image_name).replace("\\", "/")
 
             print(f'Downloading file: {image_name} to {download_path} folder') 
-            s3 = boto3.resource('s3', aws_access_key_id=self.access_key_id,  aws_secret_access_key=self.secret_access_key, region_name=self.region_name)
+            s3 = self.session.resource('s3')
             bucket = s3.Bucket(self.bucket)
 
             if progress_bar:
                 meta_data = self.s3_client.head_object(Bucket=self.bucket, Key=s3_image_path)
                 total_length = int(meta_data.get('ContentLength', 0))
                 with tqdm.tqdm(total=total_length, unit="B", unit_scale=True, desc=s3_image_path) as pbar:
                     bucket.download_file(s3_image_path, local_image_path, Callback=lambda bytes_transferred: pbar.update(bytes_transferred))
@@ -86,15 +84,15 @@
         :type progress_bar: boolean
     
         :return: If the image was uploaded or not.
         :rtype: boolean
         """
         try:
             print(f'Uploading results to {s3_output_path}')
-            s3 = boto3.resource('s3', aws_access_key_id=self.access_key_id,  aws_secret_access_key=self.secret_access_key, region_name=self.region_name)
+            s3 = self.session.resource('s3')
             bucket = s3.Bucket(self.bucket)
 
             image_name = os.path.basename(local_image_path)
             s3_image_path = os.path.join(s3_output_path, image_name).replace("\\", "/")
             print(f'Complete path: {s3_image_path}')
 
             if progress_bar:
@@ -118,15 +116,15 @@
         :param s3_path: the path of the file on S3
         :type s3_path: string
     
         :return: If the file exists or not.
         :rtype: boolean
         """
         try:
-            s3 = boto3.resource('s3', aws_access_key_id=self.access_key_id,  aws_secret_access_key=self.secret_access_key, region_name=self.region_name)
+            s3 = self.session.resource('s3')
             try:
                 s3.Object(self.bucket, os.path.join(s3_path, file_name).replace("\\", "/")).load()
                 return True
             except botocore.exceptions.ClientError as e:
                 if e.response['Error']['Code'] == "404":
                     # The object does not exist.
                     return False
```

### Comparing `files-handler-0.1.8/files_handler.egg-info/PKG-INFO` & `files-handler-0.1.9/files_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: files-handler
-Version: 0.1.8
+Version: 0.1.9
 Summary: Files Handler Library
 Home-page: 
 Author: Bhryan Henderson
 Author-email: bhryan.perpetuo@concert.com.br
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `files-handler-0.1.8/setup.py` & `files-handler-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="files-handler",
-    version="0.1.8",
+    version="0.1.9",
     description="Files Handler Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Bhryan Henderson",
     author_email="bhryan.perpetuo@concert.com.br",
     license="MIT",
```

