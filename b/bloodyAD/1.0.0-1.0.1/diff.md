# Comparing `tmp/bloodyAD-1.0.0.tar.gz` & `tmp/bloodyAD-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloodyAD-1.0.0.tar", last modified: Sun Apr 16 21:48:26 2023, max compression
+gzip compressed data, was "bloodyAD-1.0.1.tar", last modified: Wed Apr 19 12:34:00 2023, max compression
```

## Comparing `bloodyAD-1.0.0.tar` & `bloodyAD-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/
--rwxrwx---   0 silver    (1000) silver    (1001)     1068 2022-09-07 15:23:19.000000 bloodyAD-1.0.0/LICENSE
--rw-r--r--   0 silver    (1000) silver    (1001)     8342 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/PKG-INFO
--rw-r--r--   0 silver    (1000) silver    (1001)     7595 2023-03-27 18:43:52.000000 bloodyAD-1.0.0/README.md
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.772246 bloodyAD-1.0.0/bloodyAD/
--rw-r--r--   0 silver    (1000) silver    (1001)      108 2023-03-28 10:43:06.000000 bloodyAD-1.0.0/bloodyAD/__init__.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.772246 bloodyAD-1.0.0/bloodyAD/cli_modules/
--rw-r--r--   0 silver    (1000) silver    (1001)        0 2022-12-26 08:53:44.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/__init__.py
--rw-r--r--   0 silver    (1000) silver    (1001)    16094 2023-04-16 20:55:01.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/add.py
--rw-r--r--   0 silver    (1000) silver    (1001)    10343 2023-04-16 20:45:02.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/get.py
--rw-r--r--   0 silver    (1000) silver    (1001)     8942 2023-04-16 20:41:09.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/remove.py
--rw-r--r--   0 silver    (1000) silver    (1001)     3332 2023-04-16 20:41:09.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/set.py
--rw-r--r--   0 silver    (1000) silver    (1001)     1920 2023-03-18 13:00:15.000000 bloodyAD-1.0.0/bloodyAD/exceptions.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.772246 bloodyAD-1.0.0/bloodyAD/formatters/
--rw-r--r--   0 silver    (1000) silver    (1001)        0 2023-02-10 15:42:23.000000 bloodyAD-1.0.0/bloodyAD/formatters/__init__.py
--rw-r--r--   0 silver    (1000) silver    (1001)     5952 2023-04-12 13:41:14.000000 bloodyAD-1.0.0/bloodyAD/formatters/accesscontrol.py
--rw-r--r--   0 silver    (1000) silver    (1001)   118418 2023-04-16 20:41:10.000000 bloodyAD-1.0.0/bloodyAD/formatters/adschema.py
--rw-r--r--   0 silver    (1000) silver    (1001)     2594 2023-04-16 20:41:09.000000 bloodyAD-1.0.0/bloodyAD/formatters/common.py
--rw-r--r--   0 silver    (1000) silver    (1001)     5029 2023-02-08 15:06:03.000000 bloodyAD-1.0.0/bloodyAD/formatters/cryptography.py
--rw-r--r--   0 silver    (1000) silver    (1001)     8547 2023-04-16 20:24:41.000000 bloodyAD-1.0.0/bloodyAD/formatters/dns.py
--rw-r--r--   0 silver    (1000) silver    (1001)     1773 2023-04-16 20:46:39.000000 bloodyAD-1.0.0/bloodyAD/formatters/formatters.py
--rw-r--r--   0 silver    (1000) silver    (1001)     2016 2023-04-16 20:41:10.000000 bloodyAD-1.0.0/bloodyAD/formatters/helpers.py
--rw-r--r--   0 silver    (1000) silver    (1001)    16246 2023-03-18 13:05:44.000000 bloodyAD-1.0.0/bloodyAD/formatters/ldaptypes.py
--rw-r--r--   0 silver    (1000) silver    (1001)    23266 2023-01-16 17:02:26.000000 bloodyAD-1.0.0/bloodyAD/formatters/structure.py
--rwxrwx---   0 silver    (1000) silver    (1001)   486395 2023-03-18 13:06:07.000000 bloodyAD-1.0.0/bloodyAD/formatters/winerror.py
--rwxr-xr-x   0 silver    (1000) silver    (1001)     8007 2023-04-16 20:41:10.000000 bloodyAD-1.0.0/bloodyAD/main.py
--rw-r--r--   0 silver    (1000) silver    (1001)     3950 2023-02-08 15:01:35.000000 bloodyAD-1.0.0/bloodyAD/md4.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/bloodyAD/network/
--rw-r--r--   0 silver    (1000) silver    (1001)     2537 2023-03-18 13:00:15.000000 bloodyAD-1.0.0/bloodyAD/network/config.py
--rw-r--r--   0 silver    (1000) silver    (1001)     8680 2023-04-16 20:57:57.000000 bloodyAD-1.0.0/bloodyAD/network/ldap.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/bloodyAD/patch/
--rw-r--r--   0 silver    (1000) silver    (1001)    47840 2023-03-18 13:05:45.000000 bloodyAD-1.0.0/bloodyAD/patch/ldap3_patch.py
--rw-r--r--   0 silver    (1000) silver    (1001)    16697 2023-04-16 20:51:07.000000 bloodyAD-1.0.0/bloodyAD/utils.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.772246 bloodyAD-1.0.0/bloodyAD.egg-info/
--rw-r--r--   0 silver    (1000) silver    (1001)     8342 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/PKG-INFO
--rw-r--r--   0 silver    (1000) silver    (1001)      902 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/SOURCES.txt
--rw-r--r--   0 silver    (1000) silver    (1001)        1 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/dependency_links.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       48 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/entry_points.txt
--rw-r--r--   0 silver    (1000) silver    (1001)      190 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/requires.txt
--rw-r--r--   0 silver    (1000) silver    (1001)        9 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/top_level.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       38 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/setup.cfg
--rw-r--r--   0 silver    (1000) silver    (1001)     1365 2023-04-16 20:41:10.000000 bloodyAD-1.0.0/setup.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/
+-rwxrwx---   0 silver    (1000) silver    (1001)     1068 2022-09-07 15:23:19.000000 bloodyAD-1.0.1/LICENSE
+-rw-r--r--   0 silver    (1000) silver    (1001)     7763 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/PKG-INFO
+-rw-r--r--   0 silver    (1000) silver    (1001)     7016 2023-04-17 09:41:24.000000 bloodyAD-1.0.1/README.md
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/
+-rw-r--r--   0 silver    (1000) silver    (1001)      108 2023-03-28 10:43:06.000000 bloodyAD-1.0.1/bloodyAD/__init__.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/cli_modules/
+-rw-r--r--   0 silver    (1000) silver    (1001)        0 2022-12-26 08:53:44.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/__init__.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    16389 2023-04-19 11:41:32.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/add.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    10912 2023-04-19 11:40:41.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/get.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     9087 2023-04-19 11:40:41.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/remove.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     3332 2023-04-16 20:41:09.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/set.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     1920 2023-03-18 13:00:15.000000 bloodyAD-1.0.1/bloodyAD/exceptions.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/formatters/
+-rw-r--r--   0 silver    (1000) silver    (1001)        0 2023-02-10 15:42:23.000000 bloodyAD-1.0.1/bloodyAD/formatters/__init__.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     5952 2023-04-12 13:41:14.000000 bloodyAD-1.0.1/bloodyAD/formatters/accesscontrol.py
+-rw-r--r--   0 silver    (1000) silver    (1001)   118418 2023-04-16 20:41:10.000000 bloodyAD-1.0.1/bloodyAD/formatters/adschema.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     2594 2023-04-16 20:41:09.000000 bloodyAD-1.0.1/bloodyAD/formatters/common.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     5021 2023-04-19 11:40:41.000000 bloodyAD-1.0.1/bloodyAD/formatters/cryptography.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     8547 2023-04-16 20:24:41.000000 bloodyAD-1.0.1/bloodyAD/formatters/dns.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     1771 2023-04-17 09:30:32.000000 bloodyAD-1.0.1/bloodyAD/formatters/formatters.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     2016 2023-04-16 20:41:10.000000 bloodyAD-1.0.1/bloodyAD/formatters/helpers.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    16246 2023-03-18 13:05:44.000000 bloodyAD-1.0.1/bloodyAD/formatters/ldaptypes.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    23266 2023-01-16 17:02:26.000000 bloodyAD-1.0.1/bloodyAD/formatters/structure.py
+-rwxrwx---   0 silver    (1000) silver    (1001)   486395 2023-03-18 13:06:07.000000 bloodyAD-1.0.1/bloodyAD/formatters/winerror.py
+-rwxr-xr-x   0 silver    (1000) silver    (1001)     7019 2023-04-19 11:40:41.000000 bloodyAD-1.0.1/bloodyAD/main.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     3950 2023-02-08 15:01:35.000000 bloodyAD-1.0.1/bloodyAD/md4.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/network/
+-rw-r--r--   0 silver    (1000) silver    (1001)     2537 2023-03-18 13:00:15.000000 bloodyAD-1.0.1/bloodyAD/network/config.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     8680 2023-04-16 20:57:57.000000 bloodyAD-1.0.1/bloodyAD/network/ldap.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/patch/
+-rw-r--r--   0 silver    (1000) silver    (1001)    47840 2023-03-18 13:05:45.000000 bloodyAD-1.0.1/bloodyAD/patch/ldap3_patch.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    16673 2023-04-17 19:14:34.000000 bloodyAD-1.0.1/bloodyAD/utils.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD.egg-info/
+-rw-r--r--   0 silver    (1000) silver    (1001)     7763 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/PKG-INFO
+-rw-r--r--   0 silver    (1000) silver    (1001)      902 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/SOURCES.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)        1 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/dependency_links.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       48 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/entry_points.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)      190 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/requires.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)        9 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/top_level.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       38 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/setup.cfg
+-rw-r--r--   0 silver    (1000) silver    (1001)     1365 2023-04-19 11:40:34.000000 bloodyAD-1.0.1/setup.py
```

### Comparing `bloodyAD-1.0.0/LICENSE` & `bloodyAD-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/PKG-INFO` & `bloodyAD-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bloodyAD
-Version: 1.0.0
+Version: 1.0.1
 Summary: AD Privesc Swiss Army Knife
 Home-page: https://github.com/CravateRouge/bloodyAD
-Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.1.tar.gz
 Author: CravateRouge
 Author-email: baptiste.crepin@ntymail.com
 License: MIT
 Keywords: Active Directory,Privilege Escalation
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -81,17 +81,15 @@
 ```
 
 **Note:** You can find more examples on <https://cravaterouge.github.io/> and in the documentation folder of this project
 
 List of all available functions:
 
 ```ps1
-usage: bloodyAD.py [-h] [-d DOMAIN] [-u USERNAME] [-p PASSWORD] [-k] [-c CERTIFICATE] [-s] [--host HOST]
-                   {getObjectAttributes,setAttribute,addUser,addComputer,delObject,changePassword,addObjectToGroup,addForeignObjectToGroup,delObjectFromGroup,getChildObjects,search,setShadowCredentials,setGenericAll,setOwner,setRbcd,setDCSync,setUserAccountControl,add,get,remove}
-                   ...
+usage: bloodyAD.py [-h] [-d DOMAIN] [-u USERNAME] [-p PASSWORD] [-k] [-c CERTIFICATE] [-s] [--host HOST] [-v {QUIET,INFO,DEBUG}] {add,get,remove,set} ...
 
 AD Privesc Swiss Army Knife
 
 options:
   -h, --help            show this help message and exit
   -d DOMAIN, --domain DOMAIN
                         Domain used for NTLM authentication
@@ -100,20 +98,23 @@
   -p PASSWORD, --password PASSWORD
                         Cleartext password or LMHASH:NTHASH for NTLM authentication
   -k, --kerberos
   -c CERTIFICATE, --certificate CERTIFICATE
                         Certificate authentication, e.g: "path/to/key:path/to/cert"
   -s, --secure          Try to use LDAP over TLS aka LDAPS (default is LDAP)
   --host HOST           Hostname or IP of the DC (ex: my.dc.local or 172.16.1.3)
+  -v {QUIET,INFO,DEBUG}, --verbose {QUIET,INFO,DEBUG}
+                        Adjust output verbosity
 
 Commands:
-  {getObjectAttributes,setAttribute,addUser,addComputer,delObject,changePassword,addObjectToGroup,addForeignObjectToGroup,delObjectFromGroup,getChildObjects,search,setShadowCredentials,setGenericAll,setOwner,setRbcd,setDCSync,setUserAccountControl,add,get,remove}
+  {add,get,remove,set}
     add                 [ADD] function category
     get                 [GET] function category
     remove              [REMOVE] function category
+    set                 [SET] function category
 ```
 
 Help text to use a specific function:
 
 ```ps1
 [bloodyAD]$ bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 set password -h
 usage: bloodyAD.py set password [-h] [--oldpass OLDPASS] target newpass
@@ -125,15 +126,15 @@
 options:
   -h, --help         show this help message and exit
   --oldpass OLDPASS  old password of the target, mandatory if you don't have "change password" permission on the target (default: None)
   ```
 
 ## How it works
 
-bloodyAD communicates with a DC using mainly the LDAP protocol in order to get information or add/modify/delete AD objects. ~~A password cannot be updated with LDAP, it must be a secure connection that is LDAPS or SAMR. A DC doesn't have LDAPS activated by default because it must be configured (with a certificate) so SAMR is used in those cases.~~ Exchange of sensitive information such as passwords are now supported using cleartext LDAP.
+bloodyAD communicates with a DC using mainly the LDAP protocol in order to get information or add/modify/delete AD objects. Exchange of sensitive information such as passwords without LDAPS are now supported.
 
 ## Useful commands
 
 ```ps1
 # Get group members
 bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object Users --attr member
```

### Comparing `bloodyAD-1.0.0/README.md` & `bloodyAD-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,17 +61,15 @@
 ```
 
 **Note:** You can find more examples on <https://cravaterouge.github.io/> and in the documentation folder of this project
 
 List of all available functions:
 
 ```ps1
-usage: bloodyAD.py [-h] [-d DOMAIN] [-u USERNAME] [-p PASSWORD] [-k] [-c CERTIFICATE] [-s] [--host HOST]
-                   {getObjectAttributes,setAttribute,addUser,addComputer,delObject,changePassword,addObjectToGroup,addForeignObjectToGroup,delObjectFromGroup,getChildObjects,search,setShadowCredentials,setGenericAll,setOwner,setRbcd,setDCSync,setUserAccountControl,add,get,remove}
-                   ...
+usage: bloodyAD.py [-h] [-d DOMAIN] [-u USERNAME] [-p PASSWORD] [-k] [-c CERTIFICATE] [-s] [--host HOST] [-v {QUIET,INFO,DEBUG}] {add,get,remove,set} ...
 
 AD Privesc Swiss Army Knife
 
 options:
   -h, --help            show this help message and exit
   -d DOMAIN, --domain DOMAIN
                         Domain used for NTLM authentication
@@ -80,20 +78,23 @@
   -p PASSWORD, --password PASSWORD
                         Cleartext password or LMHASH:NTHASH for NTLM authentication
   -k, --kerberos
   -c CERTIFICATE, --certificate CERTIFICATE
                         Certificate authentication, e.g: "path/to/key:path/to/cert"
   -s, --secure          Try to use LDAP over TLS aka LDAPS (default is LDAP)
   --host HOST           Hostname or IP of the DC (ex: my.dc.local or 172.16.1.3)
+  -v {QUIET,INFO,DEBUG}, --verbose {QUIET,INFO,DEBUG}
+                        Adjust output verbosity
 
 Commands:
-  {getObjectAttributes,setAttribute,addUser,addComputer,delObject,changePassword,addObjectToGroup,addForeignObjectToGroup,delObjectFromGroup,getChildObjects,search,setShadowCredentials,setGenericAll,setOwner,setRbcd,setDCSync,setUserAccountControl,add,get,remove}
+  {add,get,remove,set}
     add                 [ADD] function category
     get                 [GET] function category
     remove              [REMOVE] function category
+    set                 [SET] function category
 ```
 
 Help text to use a specific function:
 
 ```ps1
 [bloodyAD]$ bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 set password -h
 usage: bloodyAD.py set password [-h] [--oldpass OLDPASS] target newpass
@@ -105,15 +106,15 @@
 options:
   -h, --help         show this help message and exit
   --oldpass OLDPASS  old password of the target, mandatory if you don't have "change password" permission on the target (default: None)
   ```
 
 ## How it works
 
-bloodyAD communicates with a DC using mainly the LDAP protocol in order to get information or add/modify/delete AD objects. ~~A password cannot be updated with LDAP, it must be a secure connection that is LDAPS or SAMR. A DC doesn't have LDAPS activated by default because it must be configured (with a certificate) so SAMR is used in those cases.~~ Exchange of sensitive information such as passwords are now supported using cleartext LDAP.
+bloodyAD communicates with a DC using mainly the LDAP protocol in order to get information or add/modify/delete AD objects. Exchange of sensitive information such as passwords without LDAPS are now supported.
 
 ## Useful commands
 
 ```ps1
 # Get group members
 bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object Users --attr member
```

### Comparing `bloodyAD-1.0.0/bloodyAD/cli_modules/add.py` & `bloodyAD-1.0.1/bloodyAD/cli_modules/add.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import binascii, datetime, random, string
 from typing import Literal
 from bloodyAD import utils
 from bloodyAD.utils import LOG
 from bloodyAD.formatters import accesscontrol, common, cryptography, dns
-from ldap3.core.exceptions import (
-    LDAPEntryAlreadyExistsResult,
-    LDAPAttributeOrValueExistsResult,
-)
 import ldap3
 from cryptography import x509
 from cryptography.x509.oid import NameOID
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from bloodyAD.exceptions import BloodyError
 
@@ -142,50 +138,61 @@
 
     # TODO: take into account custom ForestDnsZones and DomainDnsZones partition name ?
     if forest:
         zone_type = "ForestDnsZones"
     else:
         zone_type = "DomainDnsZones"
 
-    zone_dn = f",DC={zone},CN=MicrosoftDNS,DC={zone_type}{naming_context}"
-    record_dn = f"DC={name}{zone_dn}"
+    zone_dn = f"DC={zone},CN=MicrosoftDNS,DC={zone_type}{naming_context}"
+    record_dn = None
 
     serial = None
-    for dns_record in next(conn.ldap.bloodysearch(f"DC=@{zone_dn}", attr="dnsRecord"))[
-        "dnsRecord"
-    ]:
-        if dns_record.get("Type") == "SOA":
-            serial = dns_record["Data"]["SerialNo"]
-            break
+    new_dnsrecord_list = None
+    ldap_filter = f"(|(name=@)(name={name}))"
+    for entry in conn.ldap.bloodysearch(
+        zone_dn,
+        ldap_filter=ldap_filter,
+        search_scope=ldap3.SUBTREE,
+        attr=["name", "dnsRecord"],
+        raw=True,
+    ):
+        if entry["name"][0] == b"@":
+            for raw_record in entry["dnsRecord"]:
+                dns_record = dns.Record(raw_record).toDict()
+                if dns_record.get("Type") == "SOA":
+                    serial = dns_record["Data"]["SerialNo"]
+                    break
+        else:
+            record_dn = entry["distinguishedName"].decode()
+            new_dnsrecord_list = entry["dnsRecord"]
 
-    dns_record = dns.Record()
-    dns_record.fromDict(
+    if not serial:
+        raise BloodyError(f"No '@' entry found in '{zone_dn}' with '{ldap_filter}'")
+    new_dnsrecord = dns.Record()
+    new_dnsrecord.fromDict(
         data, dnstype, ttl, rank, serial, preference, port, priority, weight
     )
-    record_attr = {
-        "objectClass": ["top", "dnsNode"],
-        "dnsRecord": dns_record.getData(),
-        "dNSTombstoned": False,
-    }
 
-    try:
+    if not record_dn:
+        record_dn = f"DC={name},{zone_dn}"
+        record_attr = {
+            "objectClass": ["top", "dnsNode"],
+            "dnsRecord": new_dnsrecord.getData(),
+            "dNSTombstoned": False,
+        }
         conn.ldap.bloodyadd(record_dn, attributes=record_attr)
-        success_log = f"[+] {name} has been successfully added"
-    except LDAPEntryAlreadyExistsResult:
-        try:
-            conn.ldap.bloodymodify(
-                record_dn, {"dnsRecord": [ldap3.MODIFY_ADD, record_attr["dnsRecord"]]}
-            )
-            success_log = f"[+] {name} has been successfully updated"
-        except LDAPAttributeOrValueExistsResult:
-            LOG.warning(f"[!] {name} has already a record of this type")
-            LOG.warning("[!] Record not updated")
-            return
+        LOG.info(f"[+] {name} has been successfully added")
+        return
 
-    LOG.info(success_log)
+    new_dnsrecord_list.append(new_dnsrecord.getData())
+    print(new_dnsrecord_list)
+    conn.ldap.bloodymodify(
+        record_dn, {"dnsRecord": [ldap3.MODIFY_REPLACE, new_dnsrecord_list]}
+    )
+    LOG.info(f"[+] {name} has been successfully updated")
 
 
 def genericAll(conn, target: str, trustee: str):
     """
     Gives full control to trustee on target (you must own the object or have WriteDacl)
 
     :param target: sAMAccountName, DN, GUID or SID of the target
```

### Comparing `bloodyAD-1.0.0/bloodyAD/cli_modules/get.py` & `bloodyAD-1.0.1/bloodyAD/cli_modules/get.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,45 +74,46 @@
 
             if domain_name == "@":  # @ is for dnsZone info
                 domain_name = domain_suffix
 
             yield_entry = {"domain": domain_name}
             for record in entry["dnsRecord"]:
                 try:
+                    if record["Type"] not in yield_entry:
+                        yield_entry[record["Type"]] = []
                     if record["Type"] in ["A", "AAAA", "NS", "CNAME", "PTR", "TXT"]:
-                        yield_entry[record["Type"]] = record["Data"]
+                        yield_entry[record["Type"]].append(record["Data"])
                     elif record["Type"] == "MX":
-                        yield_entry[record["Type"]] = record["Data"]["Name"]
+                        yield_entry[record["Type"]].append(record["Data"]["Name"])
                     elif record["Type"] == "SRV":
-                        yield_entry[record["Type"]] = (
+                        yield_entry[record["Type"]].append(
                             f"{record['Data']['Target']}:{record['Data']['Port']}"
                         )
                     elif record["Type"] == "SOA":
-                        yield_entry[record["Type"]] = [
-                            record["Data"]["PrimaryServer"],
-                            record["Data"]["zoneAdminEmail"].replace(".", "@", 1),
-                        ]
+                        yield_entry[record["Type"]].append(
+                            {
+                                "PrimaryServer": record["Data"]["PrimaryServer"],
+                                "zoneAdminEmail": record["Data"][
+                                    "zoneAdminEmail"
+                                ].replace(".", "@", 1),
+                            }
+                        )
                 except KeyError:
                     LOG.error("[-] KeyError for record: " + record)
                     continue
             yield yield_entry
 
 
 def membership(conn, target: str, no_recurse: bool = False):
     """
     Retrieves SID and SAM Account Names of all groups a target belongs to
 
     :param target: sAMAccountName, DN, GUID or SID of the target
     :param no_recurse: if set, doesn't retrieve groups where target isn't a direct member
     """
-    # We fetch primaryGroupID, since this group is not reflected in memberOf
-    # Additionally we get objectSid to have the domain sid
-    # it is helpful to resolve the primary group RID to a DN
-    # Finally we add the special identity groups: Authenticated Users and Everyone
-
     filter = ""
     if no_recurse:
         entries = conn.ldap.bloodysearch(target, attr=["objectSid", "memberOf"])
         for entry in entries:
             for group in entry["memberOf"]:
                 filter += f"(distinguishedName={group})"
         if not filter:
@@ -146,15 +147,15 @@
     conn, target: str, attr: str = "*", resolve_sd: bool = False, raw: bool = False
 ):
     """
     Retrieves LDAP attributes for the target object provided, binary data will be outputed in base64
 
     :param target: sAMAccountName, DN, GUID or SID of the target
     :param attr: name of the attribute to retrieve, retrieves all the attributes by default
-    :param resolve_sd: if set, permissions linked to a security descriptor will be resolved !!resolving can take some time!!
+    :param resolve_sd: if set, permissions linked to a security descriptor will be resolved (see documentation/accesscontrol.md for more information)
     :param raw: if set, will return attributes as sent by the server without any formatting, binary data will be outputed in base64
     """
     entries = conn.ldap.bloodysearch(target, attr=attr, raw=raw)
     rendered_entries = utils.renderSearchResult(entries)
     if resolve_sd and not raw:
         for entry in rendered_entries:
             if "nTSecurityDescriptor" in entry:
@@ -167,34 +168,44 @@
 
 
 def search(
     conn,
     searchbase: str,
     filter: str = "(objectClass=*)",
     attr: str = "*",
+    resolve_sd: bool = False,
     raw: bool = False,
 ):
     """
     Searches in LDAP database, binary data will be outputed in base64
 
     :param searchbase: DN of the parent object
     :param filter: filter to apply to the LDAP search (see Microsoft LDAP filter syntax)
     :param attr: attributes to retrieve separated by a comma
+    :param resolve_sd: if set, permissions linked to a security descriptor will be resolved (see documentation/accesscontrol.md for more information)
     :param raw: if set, will return attributes as sent by the server without any formatting, binary data will be outputed in base64
     """
     entries = conn.ldap.bloodysearch(
         searchbase,
         filter,
         search_scope=ldap3.SUBTREE,
         attr=attr.split(","),
         raw=raw,
         generator=True,
     )
-
-    return utils.renderSearchResult(entries)
+    rendered_entries = utils.renderSearchResult(entries)
+    if resolve_sd and not raw:
+        for entry in rendered_entries:
+            if "nTSecurityDescriptor" in entry:
+                entry["nTSecurityDescriptor"] = utils.renderSD(
+                    entry["nTSecurityDescriptor"], conn
+                )
+            yield entry
+    else:
+        yield from rendered_entries
 
 
 # TODO: Search writable for application partitions too?
 def writable(
     conn,
     otype: Literal["ALL", "OU", "USER", "COMPUTER", "GROUP", "DOMAIN", "GPO"] = "ALL",
     right: Literal["ALL", "WRITE", "CHILD"] = "ALL",
```

### Comparing `bloodyAD-1.0.0/bloodyAD/cli_modules/remove.py` & `bloodyAD-1.0.1/bloodyAD/cli_modules/remove.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,18 +81,20 @@
     else:
         zone_type = "DomainDnsZones"
 
     zone_dn = f",DC={zone},CN=MicrosoftDNS,DC={zone_type}{naming_context}"
     record_dn = f"DC={name}{zone_dn}"
 
     record_to_remove = None
-    for raw_record in next(
-        conn.ldap.bloodysearch(record_dn, attr="dnsRecord", raw=True)
-    )["dnsRecord"]:
+    dns_list = next(conn.ldap.bloodysearch(record_dn, attr="dnsRecord", raw=True))[
+        "dnsRecord"
+    ]
+    for raw_record in dns_list:
         record = dns.Record(raw_record)
+        print(record.toDict())
         tmp_record = dns.Record()
 
         if not ttl:
             ttl = record["TtlSeconds"]
         tmp_record.fromDict(
             data,
             dnstype,
@@ -108,17 +110,20 @@
             record_to_remove = raw_record
             break
 
     if not record_to_remove:
         LOG.warning("[!] Record not found")
         return
 
-    conn.ldap.bloodymodify(
-        record_dn, {"dnsRecord": (ldap3.MODIFY_DELETE, record_to_remove)}
-    )
+    if len(dns_list) > 1:
+        conn.ldap.bloodymodify(
+            record_dn, {"dnsRecord": (ldap3.MODIFY_DELETE, record_to_remove)}
+        )
+    else:
+        conn.ldap.bloodydelete(record_dn)
 
     LOG.info(f"[-] Given record has been successfully removed from {name}")
 
 
 def genericAll(conn, target: str, trustee: str):
     """
     Removes full control of trustee on target
```

### Comparing `bloodyAD-1.0.0/bloodyAD/cli_modules/set.py` & `bloodyAD-1.0.1/bloodyAD/cli_modules/set.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/exceptions.py` & `bloodyAD-1.0.1/bloodyAD/exceptions.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/accesscontrol.py` & `bloodyAD-1.0.1/bloodyAD/formatters/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/adschema.py` & `bloodyAD-1.0.1/bloodyAD/formatters/adschema.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/common.py` & `bloodyAD-1.0.1/bloodyAD/formatters/common.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/cryptography.py` & `bloodyAD-1.0.1/bloodyAD/formatters/cryptography.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,34 +49,34 @@
 
     def __init__(self, data=None, identifier=None, **kwargs):
         super().__init__(data, **kwargs)
 
         if identifier:
             self["Identifier"] = self.identifiers[identifier]
 
-    def toString(self):
-        identifier = {
+    def toDict(self):
+        identifier = [
             i for i in self.identifiers if self.identifiers[i] == self["Identifier"]
-        }
-        return f"{identifier}:{self['Value']}"
+        ][0]
+        return {identifier: self["Value"].hex()}
 
 
 class KEYCREDENTIALLINK_BLOB(Structure):
     """
     KEYCREDENTIALLINK_BLOB - [MS-ADTS] section 2.2.20.2
     """
 
     KEY_CREDENTIAL_LINK_VERSION_2 = 0x200
 
     commonHdr = (("Version", "<I=self.KEY_CREDENTIAL_LINK_VERSION_2"),)
     structure = (("KEYCREDENTIALLINK_ENTRY_LIST", "*:", KEYCREDENTIALLINK_ENTRY),)
 
     # Structure class doesn't handle correctly unpacking variable size array with custom format
     # so we have to do it ourselves. First we take it as raw data and then we're unpacking it
-    # using the underlying entry structure with length header
+    # using the underlying entry structure with header length
     def __init__(self, data=None, **kwargs):
         if data:
             self.structure = (("KEYCREDENTIALLINK_ENTRY_LIST", ":"),)
             super().__init__(data, **kwargs)
             raw_blob = self["KEYCREDENTIALLINK_ENTRY_LIST"]
             entries = []
             while raw_blob:
@@ -104,19 +104,20 @@
         )
 
         key_id = KEYCREDENTIALLINK_ENTRY(identifier="KeyID")
         key_id["Value"] = hashlib.sha256(key_material["Value"]).digest()
 
         self["KEYCREDENTIALLINK_ENTRY_LIST"] = [key_id, key_material]
 
-    def toString(self):
-        entries_str = ""
-        for entry in self["KEYCREDENTIALLINK_ENTRY_LIST"]:
-            entries_str += entry.toString() + "\n"
-        return entries_str
+    def toDict(self):
+        return {
+            k: v
+            for entry in self["KEYCREDENTIALLINK_ENTRY_LIST"]
+            for k, v in entry.toDict().items()
+        }
 
     def getKeyID(self):
         return [
             entry["Value"]
             for entry in self["KEYCREDENTIALLINK_ENTRY_LIST"]
             if entry["Identifier"] == entry.identifiers["KeyID"]
         ][0]
```

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/dns.py` & `bloodyAD-1.0.1/bloodyAD/formatters/dns.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/formatters.py` & `bloodyAD-1.0.1/bloodyAD/formatters/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,8 +58,8 @@
         dn_binary.binary_value = common.WELLKNOWN_GUID[dn_binary.binary_value]
     return dn_binary
 
 
 def formatKeyCredentialLink(key_dnbinary):
     return cryptography.KEYCREDENTIALLINK_BLOB(
         common.DNBinary(key_dnbinary).value
-    ).toString()
+    ).toDict()
```

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/helpers.py` & `bloodyAD-1.0.1/bloodyAD/formatters/helpers.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/ldaptypes.py` & `bloodyAD-1.0.1/bloodyAD/formatters/ldaptypes.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/structure.py` & `bloodyAD-1.0.1/bloodyAD/formatters/structure.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/formatters/winerror.py` & `bloodyAD-1.0.1/bloodyAD/formatters/winerror.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/main.py` & `bloodyAD-1.0.1/bloodyAD/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
-from bloodyAD import cli_modules
-from bloodyAD import ConnectionHandler
+from bloodyAD import cli_modules, ConnectionHandler, utils
 import sys, argparse, types
 
 # For dynamic argparse
 from inspect import getmembers, isfunction, signature
 from pkgutil import iter_modules
 
 
@@ -33,14 +32,21 @@
         action="store_true",
         default=False,
     )
     parser.add_argument(
         "--host",
         help="Hostname or IP of the DC (ex: my.dc.local or 172.16.1.3)",
     )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        help="Adjust output verbosity",
+        choices=["QUIET", "INFO", "DEBUG"],
+        default="INFO",
+    )
 
     subparsers = parser.add_subparsers(title="Commands")
     # Iterates all submodules in module package and creates one parser per submodule
     for importer, submodname, ispkg in iter_modules(cli_modules.__path__):
         subparser = subparsers.add_parser(
             submodname, help=f"[{submodname.upper()}] function category"
         )
@@ -112,14 +118,16 @@
         parser.print_help(sys.stderr)
         sys.exit(1)
 
     # Get the list of parameters to provide to the command
     param_names = args.func.__code__.co_varnames[1 : args.func.__code__.co_argcount]
     params = {param_name: vars(args)[param_name] for param_name in param_names}
 
+    LOGGING_LEVELS = {"QUIET": 50, "INFO": 20, "DEBUG": 10}
+    utils.LOG.setLevel(LOGGING_LEVELS[args.verbose])
     # Launch the command
     conn = ConnectionHandler(args=args)
     output = args.func(conn, **params)
 
     # Prints output, will print it directly if it's not an iterable
     # Output is expected to be of type [{name:[members]},{...}...]
     # If it's not, will print it raw
@@ -133,40 +141,14 @@
 
     for entry in output:
         print()
         for attr_name, attr_val in entry.items():
             entry_str = print_entry(attr_name, attr_val)
             if entry_str:
                 print(f"{attr_name}: {entry_str}")
-            # attr = entry[attr_name]
-            # if type(attr) not in [list, types.GeneratorType]:
-            #     print(f"{attr_name}: {attr}")
-            # else:
-            #     i = 0
-            #     dict_entries = ""
-            #     simple_entries = f"{attr_name}: "
-            #     isSimple = False
-            #     for attr_member in attr:
-            #         if type(attr_member) == dict:
-            #             for k,v in attr_member.items():
-            #                 if type(v) in [list, set]:
-            #                     rendered_v = ', '.join([str(item) for item in v])
-            #                 else:
-            #                     rendered_v = str(v)
-            #                 dict_entries += f"{attr_name}.{i}.{k}: {rendered_v}\n"
-            #             i += 1
-            #         else:
-            #             isSimple = True
-            #             simple_entries += f"{attr_member}, "
-            #     rendered_entries = dict_entries
-            #     if isSimple:
-            #         # Replaces last ", " with newline
-            #         simple_entries = simple_entries[:-2] + "\n"
-            #         rendered_entries += simple_entries
-            #     print(rendered_entries, end='')
 
 
 # Gets unparsed doc and returns a tuple of two values
 # first is function description (starts at the beginning of the string and ends before two newlines)
 # second is a list of parameter descriptions
 # (other part of the string, one parameter description per line, starting with :param param_name:)
 def doc_parser(doc):
```

### Comparing `bloodyAD-1.0.0/bloodyAD/md4.py` & `bloodyAD-1.0.1/bloodyAD/md4.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/network/config.py` & `bloodyAD-1.0.1/bloodyAD/network/config.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/network/ldap.py` & `bloodyAD-1.0.1/bloodyAD/network/ldap.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/patch/ldap3_patch.py` & `bloodyAD-1.0.1/bloodyAD/patch/ldap3_patch.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/bloodyAD/utils.py` & `bloodyAD-1.0.1/bloodyAD/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,25 +425,23 @@
 
     def __str__(self):
         return global_lazy_adschema.getsid(self.sid)
 
 
 def aceFactory(k, a):
     if k == "Trustee":
-        return {k: LazySid(a)}
+        return LazySid(a)
     elif k == "Right":
-        return {k: Right(a)}
-    elif k == "ObjectType":
-        return {k: LazyGuid(a)}
-    elif k == "InheritedObjectType":
-        return {k: LazyGuid(a)}
+        return Right(a)
+    elif k in ("ObjectType", "InheritedObjectType"):
+        return LazyGuid(a)
     elif k == "Flags":
-        return {k: AceFlag(a)}
+        return AceFlag(a)
     else:
-        return {k: a}
+        return a
 
 
 def renderSD(sddl, conn):
     global_lazy_adschema.conn = conn
     sd = SECURITY_DESCRIPTOR.from_sddl(sddl)
     # We don't print Revision because it's always 1,
     # Group isn't used in ADDS
@@ -481,20 +479,22 @@
     typed_aces = []
     for ace in grouped_aces:
         typed_ace = {}
         for k, v in ace.items():
             if not v:
                 continue
             try:
+                typed_ace[k] = []
                 for a in v:  # If it's a set of guids/sids
-                    typed_ace |= aceFactory(k, a)
+                    typed_ace[k].append(aceFactory(k, a))
             except TypeError:  # If it's a mask
-                typed_ace |= aceFactory(k, v)
+                typed_ace[k] = aceFactory(k, v)
 
         typed_aces.append(typed_ace)
+
     renderedSD["ACL"] = typed_aces
 
     return renderedSD
 
 
 def renderSearchResult(entries):
     """
```

### Comparing `bloodyAD-1.0.0/bloodyAD.egg-info/PKG-INFO` & `bloodyAD-1.0.1/bloodyAD.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bloodyAD
-Version: 1.0.0
+Version: 1.0.1
 Summary: AD Privesc Swiss Army Knife
 Home-page: https://github.com/CravateRouge/bloodyAD
-Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.1.tar.gz
 Author: CravateRouge
 Author-email: baptiste.crepin@ntymail.com
 License: MIT
 Keywords: Active Directory,Privilege Escalation
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -81,17 +81,15 @@
 ```
 
 **Note:** You can find more examples on <https://cravaterouge.github.io/> and in the documentation folder of this project
 
 List of all available functions:
 
 ```ps1
-usage: bloodyAD.py [-h] [-d DOMAIN] [-u USERNAME] [-p PASSWORD] [-k] [-c CERTIFICATE] [-s] [--host HOST]
-                   {getObjectAttributes,setAttribute,addUser,addComputer,delObject,changePassword,addObjectToGroup,addForeignObjectToGroup,delObjectFromGroup,getChildObjects,search,setShadowCredentials,setGenericAll,setOwner,setRbcd,setDCSync,setUserAccountControl,add,get,remove}
-                   ...
+usage: bloodyAD.py [-h] [-d DOMAIN] [-u USERNAME] [-p PASSWORD] [-k] [-c CERTIFICATE] [-s] [--host HOST] [-v {QUIET,INFO,DEBUG}] {add,get,remove,set} ...
 
 AD Privesc Swiss Army Knife
 
 options:
   -h, --help            show this help message and exit
   -d DOMAIN, --domain DOMAIN
                         Domain used for NTLM authentication
@@ -100,20 +98,23 @@
   -p PASSWORD, --password PASSWORD
                         Cleartext password or LMHASH:NTHASH for NTLM authentication
   -k, --kerberos
   -c CERTIFICATE, --certificate CERTIFICATE
                         Certificate authentication, e.g: "path/to/key:path/to/cert"
   -s, --secure          Try to use LDAP over TLS aka LDAPS (default is LDAP)
   --host HOST           Hostname or IP of the DC (ex: my.dc.local or 172.16.1.3)
+  -v {QUIET,INFO,DEBUG}, --verbose {QUIET,INFO,DEBUG}
+                        Adjust output verbosity
 
 Commands:
-  {getObjectAttributes,setAttribute,addUser,addComputer,delObject,changePassword,addObjectToGroup,addForeignObjectToGroup,delObjectFromGroup,getChildObjects,search,setShadowCredentials,setGenericAll,setOwner,setRbcd,setDCSync,setUserAccountControl,add,get,remove}
+  {add,get,remove,set}
     add                 [ADD] function category
     get                 [GET] function category
     remove              [REMOVE] function category
+    set                 [SET] function category
 ```
 
 Help text to use a specific function:
 
 ```ps1
 [bloodyAD]$ bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 set password -h
 usage: bloodyAD.py set password [-h] [--oldpass OLDPASS] target newpass
@@ -125,15 +126,15 @@
 options:
   -h, --help         show this help message and exit
   --oldpass OLDPASS  old password of the target, mandatory if you don't have "change password" permission on the target (default: None)
   ```
 
 ## How it works
 
-bloodyAD communicates with a DC using mainly the LDAP protocol in order to get information or add/modify/delete AD objects. ~~A password cannot be updated with LDAP, it must be a secure connection that is LDAPS or SAMR. A DC doesn't have LDAPS activated by default because it must be configured (with a certificate) so SAMR is used in those cases.~~ Exchange of sensitive information such as passwords are now supported using cleartext LDAP.
+bloodyAD communicates with a DC using mainly the LDAP protocol in order to get information or add/modify/delete AD objects. Exchange of sensitive information such as passwords without LDAPS are now supported.
 
 ## Useful commands
 
 ```ps1
 # Get group members
 bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object Users --attr member
```

### Comparing `bloodyAD-1.0.0/bloodyAD.egg-info/SOURCES.txt` & `bloodyAD-1.0.1/bloodyAD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.0/setup.py` & `bloodyAD-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="bloodyAD",
-    version="1.0.0",
+    version="1.0.1",
     description="AD Privesc Swiss Army Knife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="CravateRouge",
     author_email="baptiste.crepin@ntymail.com",
     url="https://github.com/CravateRouge/bloodyAD",
     download_url=(
-        "https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.0.tar.gz"
+        "https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.1.tar.gz"
     ),
     license="MIT",
     install_requires=[
         "cryptography>=37.0.2",
         "ldap3>=2.9.1",
         "winacl>=0.1.7",
         'gssapi>=1.8.1 ; platform_system=="Linux" or platform_system=="Darwin"',
```

