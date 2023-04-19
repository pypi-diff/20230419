# Comparing `tmp/ExpdFtpService-0.7.0.tar.gz` & `tmp/ExpdFtpService-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ExpdFtpService-0.7.0.tar", last modified: Tue Apr 18 05:36:32 2023, max compression
+gzip compressed data, was "dist\ExpdFtpService-0.8.0.tar", last modified: Wed Apr 19 01:22:14 2023, max compression
```

## Comparing `ExpdFtpService-0.7.0.tar` & `ExpdFtpService-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/
--rw-rw-rw-   0        0        0      305 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-04-07 09:01:05.000000 ExpdFtpService-0.7.0/README.md
--rw-rw-rw-   0        0        0      115 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-04-18 04:32:03.000000 ExpdFtpService-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService/
--rw-rw-rw-   0        0        0     4339 2023-04-18 05:35:54.000000 ExpdFtpService-0.7.0/src/ExpdFtpService/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/
--rw-rw-rw-   0        0        0      305 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/
+-rw-rw-rw-   0        0        0      305 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-04-18 05:39:20.000000 ExpdFtpService-0.8.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      441 2023-04-19 01:16:48.000000 ExpdFtpService-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService/
+-rw-rw-rw-   0        0        0     4512 2023-04-19 01:21:54.000000 ExpdFtpService-0.8.0/src/ExpdFtpService/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/
+-rw-rw-rw-   0        0        0      305 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/top_level.txt
```

### Comparing `ExpdFtpService-0.7.0/README.md` & `ExpdFtpService-0.8.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 How to install:
 
     pip install ExpdFtpService
 
 
 How to use with download methods:
 
-    from ExpdFtpService.download import ExpdDownloadFtpServerFile
+    from ExpdFtpService import ExpdDownloadFtpServerFile
     ExpdDownloadFtpServerFile(hostname, username, password, destfolder, savefolder, fstartwith).download(numbers=10)
     
 
 How to use with upload methods:
 
-    from ExpdFtpService.upload import ExpdUploadFtpServerFile
+    from ExpdFtpService import ExpdUploadFtpServerFile
     ExpdUploadFtpServerFile(hostname, username, password, destfolder).upload_file_to_serve(r"D:\Solutions\2431295471_PIE_E433593539.pdf")
```

### Comparing `ExpdFtpService-0.7.0/src/ExpdFtpService/__init__.py` & `ExpdFtpService-0.8.0/src/ExpdFtpService/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.ftp.cwd(self.destfolder)
         if self.fstartwith is not None:
             files = [x for x in self.ftp.nlst() if x.startswith(self.fstartwith)]
         elif self.filendwith is not None:
             files = [x for x in self.ftp.nlst() if x.endswith(self.filendwith)]
         else:
             files = [x for x in self.ftp.nlst() if str(x).lower() != 'history']
-        logger.debug(f"server total files: [{len(files)}]")
+        logger.debug(f"Ftp server {self.servercode} total files: [{len(files)}]")
         return files
     
     def archive(self, from_file, to_path, to_file):
         history = self.ftp.nlst(to_path)
         if to_file not in history:
             self.ftp.rename(f"{from_file}", f"{to_path}\{to_file}")
         else:
@@ -53,15 +53,15 @@
     def download(self, numbers):
         try:
             for count, file in enumerate(self.files, 1):
                 if count <= numbers:
                     with open(path.join(self.savefolder, f"{file}"), 'wb') as rd:
                         self.ftp.retrbinary('RETR %s' % file, rd.write)
                     self.archive(file, "History", file)
-                    logger.debug(f"NO.{count}: file {file} download from {self.servercode} successfully")
+                    logger.debug(f"NO.{count}: file {file} download from {self.servercode} successfully.")
         finally:
             self.ftp.quit()
     
 
 class ExpdUploadFtpServerFile(ConnFtpServer):
     """Class is used for connecting to a FTP Server and upload files.
         The constructor accepts the following parameters with the indicated types:
@@ -84,15 +84,17 @@
     
     @logger.catch(reraise=True)
     def upload_file_to_server(self, local_file):
         try:
             with open(local_file,'rb') as f:  
                 self.ftp.cwd(self.destfolder)          
                 self.ftp.storbinary(f'STOR {path.basename(local_file)}', f)
-                logger.debug(f"{local_file} uploaded to {self.servercode} successfully")
+                logger.debug(f"{path.basename(local_file)} uploaded to {self.servercode} successfully.")
+        except Exception as e:  
+            logger.error(f"{path.basename(local_file)} uploaded to {self.servercode} failed: {e}")
         finally:
             self.ftp.quit()
     
 
 if __name__ == '__main__':
     ExpdUploadFtpServerFile(
         hostname="xxx",
```

